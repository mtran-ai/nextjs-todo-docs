---
storyId: "4.1"
storyKey: "4-1-implement-task-filtering-by-completion-status"
epicId: "4"
epicTitle: "Task Organization & Efficient Discovery"
projectName: "nextjs-todo-docs"
userName: "Minh"
date: "2026-04-06"
status: "ready-for-dev"
priority: "high"
---

# Story 4.1: Implement Task Filtering by Completion Status

## Story Statement

**As a** daily user (Jordan)  
**I want to** filter tasks by status (all, active, completed)  
**So that** I can focus on what needs attention

---

## Acceptance Criteria

- [ ] Filter buttons: "All" (default), "Active", "Completed"
- [ ] Clicking filter updates list immediately
- [ ] Active filter visually indicated (e.g., bold, different background, underline)
- [ ] Task count updates (e.g., "3 of 8 tasks") when filter changes
- [ ] Empty state: "No active tasks" if no matches for selected filter
- [ ] Design: modern UI with design tokens (colors, spacing, typography)
- [ ] Accessibility: buttons are semantic, focus visible, screen reader announces current filter state

---

## Dev Notes

### Context & Background

**Epic 4** covers task organization and discovery. Story 4.1 is the **first story in this epic** and adds the most fundamental filtering capability: filtering by completion status (all/active/completed). This is a high-priority feature because:

1. **Users manage 20-30 tasks daily** (Jordan persona) and need quick filtering to focus
2. **Filters work independently and together** — story 4.2 adds search, 4.3 adds sorting
3. **Foundation for discovery workflow** — filtering should feel instant and satisfying
4. **Design consistency matters** — filter controls set the pattern for other controls (sort, search)

**Related Work:**
- Story 4.2 (search) is independent but shares the same UI space
- Story 4.3 (sort) is independent but works with filtering
- Story 4.4 (polish) refines all three together for responsive design

### Implementation Strategy

**Architecture Patterns (from existing codebase):**
- **State Management:** React Context + useReducer for filter state (matches existing pattern)
- **Data Filtering:** Client-side filtering in component (tasks already fetched via Server Action)
- **Styling:** Tailwind CSS tokens for design consistency
- **Forms:** Semantic button elements (not links or divs)
- **Accessibility:** Standard button semantics with ARIA labels where needed

**Key Technical Decisions:**

1. **Filter State Location:** Keep in React Context (not URL params for MVP)
   - Simpler for first implementation
   - Can be moved to URL params later for bookmarkable state
   
2. **Filtering Logic:** Client-side filtering
   - Tasks already fetched via Server Action on page load
   - Filter in useEffect or directly in render logic
   - No additional server calls needed for filtering
   
3. **UI Pattern:** Button group (semantic)
   - Three buttons: "All", "Active", "Completed"
   - Active button visually indicated with design tokens
   - Focus ring on keyboard navigation

4. **Task Counting:** Dynamic counter
   - Show "X of Y tasks" pattern
   - Update immediately as filter changes

### Design System Integration

**Color Tokens:** Use existing Tailwind tokens
- **Active button:** Primary color (`primary` token) with white text
- **Inactive buttons:** Secondary appearance (muted background, gray text)
- **Focus ring:** Standard ring color with visible indicator (44px+ touch target on mobile)

**Typography:** Use existing type scale
- **Button text:** Semibold (600 weight), same size as other UI elements
- **Count text:** Regular (400 weight), muted color

**Spacing:** Follow existing 4px base unit
- **Button group:** 8px gap between buttons (2 units)
- **Button padding:** 8px horizontal, 6px vertical (consistent with other buttons)
- **Below filter:** 16px gap to task list

### Performance Considerations

- **Filtering should be instant:** <50ms for up to 100 tasks (in-memory filtering)
- **No re-fetch:** Use already-loaded task data, don't make new API calls
- **Memoization:** Consider useMemo if filter logic becomes complex (unlikely for v1)

### Accessibility Requirements (WCAG AA)

- **Semantic HTML:** Use `<button>` elements with proper nesting
- **ARIA Labels:** Add aria-current="page" or aria-selected="true" to active filter
- **Keyboard Navigation:** Tab through all buttons, Space/Enter to activate
- **Focus Indicators:** Visible 2px focus ring on all buttons
- **Screen Reader:** "3 of 8 tasks filtered - Active" should be announced
- **Color Contrast:** Active button must meet 4.5:1 contrast ratio (test with existing theme)

### Component Architecture

**New/Modified Components:**
1. **TaskFilterBar** (new) — Container for filter buttons + task count
   - Props: `activeFilter`, `onFilterChange`, `totalTasks`, `filteredTasks`
   - Returns: Filter UI with semantic buttons

2. **TaskList** (existing, will be modified) — Accept filter state
   - May need to accept a `filter` prop
   - Responsibility: render filtered tasks (filtering logic handled in parent or context)

**Hooks/Context Changes:**
- **useTaskFilter** (new) — Custom hook for filter state management
  - State: `activeFilter` ("all" | "active" | "completed")
  - Handler: `setFilter(newFilter)`
  - Could be used from Context or local state

**Placement in Page:**
- Task filter controls appear above the task list
- Below page heading but above search bar (if search exists)
- Visual separation via spacing/border

### Testing Requirements

**Unit Tests:**
- Filter state transitions (all → active → completed)
- Filtered task count calculations
- Empty state rendering when no matching tasks
- Accessibility: button focus, keyboard navigation

**Integration Tests:**
- Filter button click updates task display
- Task count updates correctly
- Filtering works correctly with existing task data
- Active filter state persists while browsing (context preservation)

**E2E Tests (Playwright):**
- User clicks "Active" filter → sees only incomplete tasks
- User clicks "Completed" filter → sees only completed tasks
- User clicks "All" → sees all tasks
- Task count displays correctly for each filter state

### Previous Story Intelligence

**Story 3.7** (Task Management Responsive Design & Accessibility) completed the core task management features. Key learnings:
- Task list component exists and works
- Tasks have `done` boolean property
- Task count and display logic is in place
- Design tokens are configured and applied

**Story 4.2** (Search) will add another filter UI element — coordinate on placement and styling so both look cohesive.

### Git Intelligence

Recent commits show:
- `c0a58ea` Epic design and user story breakdown complete
- Architecture and UX design finalized, no code implementation started yet

This is a **fresh implementation** — no existing filter code in the codebase to leverage or refactor.

### Code Examples from Architecture

**Server Action Pattern** (already established):
```typescript
const getTasks = action(
  z.object({ userId: z.string() }),
  async ({ userId }, { userId: actualUserId }) => {
    const tasks = await db.task.findMany({
      where: { userId: actualUserId }
    })
    return tasks
  }
)
```

**Context Usage Pattern** (for filter state):
```typescript
interface TaskFilterContext {
  filter: "all" | "active" | "completed"
  setFilter: (f: "all" | "active" | "completed") => void
}

export const TaskFilterContext = createContext<TaskFilterContext>(...)
```

---

## Tasks/Subtasks

### Subtask 1: Create TaskFilterBar component with filter buttons
- [ ] Create `src/components/task-filter-bar.tsx`
- [ ] Define component props: `activeFilter`, `onFilterChange`, `totalTasks`, `filteredTasks`
- [ ] Render three buttons: "All", "Active", "Completed"
- [ ] Apply design tokens for styling (colors, spacing, typography)
- [ ] Add aria labels for accessibility
- [ ] Test button click handlers and state changes

### Subtask 2: Create useTaskFilter hook for state management
- [ ] Create `src/lib/hooks/use-task-filter.ts`
- [ ] Initialize filter state ("all" by default)
- [ ] Implement `setFilter` handler
- [ ] Export hook for use in components
- [ ] Test state transitions between filters

### Subtask 3: Add filter context if needed
- [ ] Determine if Context is needed (depends on page structure)
- [ ] Create TaskFilterProvider in layout if required
- [ ] Wrap relevant components with provider
- [ ] Ensure filter state persists across re-renders

### Subtask 4: Implement filtering logic in TaskList
- [ ] Update TaskList to accept/read filter state
- [ ] Filter tasks based on `done` property:
  - `all` → show all tasks
  - `active` → show only tasks where `done === false`
  - `completed` → show only tasks where `done === true`
- [ ] Calculate filtered task count
- [ ] Render empty state when no tasks match filter

### Subtask 5: Implement empty state for filtered results
- [ ] Create empty state message: "No active tasks" (for active filter)
- [ ] Create empty state message: "No completed tasks" (for completed filter)
- [ ] Apply consistent empty state styling/spacing
- [ ] Ensure message is semantically clear to screen readers

### Subtask 6: Keyboard accessibility and focus management
- [ ] Verify Tab navigation through all filter buttons
- [ ] Verify Space/Enter activates button
- [ ] Verify visible focus ring on button focus
- [ ] Test with keyboard only (no mouse)
- [ ] Ensure focus ring meets design requirements (visible, ~2px)

### Subtask 7: Write comprehensive tests
- [ ] Unit tests: filter state transitions, task counting
- [ ] Integration tests: filter click updates display
- [ ] E2E tests: user filtering workflow
- [ ] Accessibility tests: screen reader, keyboard navigation
- [ ] Verify Lighthouse accessibility score > 90

### Subtask 8: Validate acceptance criteria
- [ ] All ACs met: buttons, immediate update, visual indication, count, empty state, design, accessibility
- [ ] No regressions in existing task list functionality
- [ ] Code review ready: clean, documented, tested

---

## File List

### New Files
- `src/components/task-filter-bar.tsx` — Filter button component
- `src/lib/hooks/use-task-filter.ts` — Filter state hook
- `src/__tests__/task-filter-bar.test.tsx` — Component tests
- `src/__tests__/use-task-filter.test.ts` — Hook tests

### Modified Files
- `src/components/task-list.tsx` — Add filter support
- `src/app/[username]/page.tsx` — Integrate filter state, pass to TaskList
- `src/lib/contexts/task-context.ts` — Add filter context (if needed)

---

## Dev Agent Record

### Implementation Plan
- [x] Understand acceptance criteria and design requirements
- [x] Load architecture patterns and existing code structure
- [x] Plan component hierarchy and state management
- [ ] **Next:** Implement TaskFilterBar component
- [ ] Implement useTaskFilter hook
- [ ] Add filtering logic to TaskList
- [ ] Implement empty states
- [ ] Write tests
- [ ] Validate all ACs
- [ ] Code review

### Debug Log
- 2026-04-06: Story created with comprehensive context. Ready for development.

### Completion Notes
_(Will be updated as work progresses)_

---

## Change Log

- 2026-04-06: Story 4.1 created with full context (epic requirements, architecture patterns, design guidelines, testing strategy)

---

## Status

**Current:** ready-for-dev  
**Last Updated:** 2026-04-06  
**Owner:** (Dev Agent)

---

## Success Criteria

This story is **complete** when:
1. ✅ All acceptance criteria satisfied
2. ✅ All subtasks completed and checked
3. ✅ Filter buttons work (all/active/completed)
4. ✅ Task count updates correctly
5. ✅ Empty states display appropriately
6. ✅ Keyboard navigation works (Tab, Space, Enter)
7. ✅ Focus rings visible and accessible
8. ✅ Screen reader announces filter state
9. ✅ All tests pass (unit, integration, e2e)
10. ✅ No regressions in existing functionality
11. ✅ Code ready for review
