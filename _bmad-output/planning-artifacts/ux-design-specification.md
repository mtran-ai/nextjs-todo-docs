---
stepsCompleted:
  - step-01-init
  - step-02-discovery
  - step-03-core-experience
  - step-04-emotional-response
  - step-05-inspiration
  - step-06-design-system
  - step-07-defining-experience
  - step-08-visual-foundation
  - step-09-design-directions
  - step-10-user-journeys
  - step-11-component-strategy
  - step-12-ux-patterns
  - step-13-responsive-accessibility
workflowStatus: complete
completedDate: 2026-04-05
lastStep: 14
inputDocuments:
  - prd.md
workflowStatus: in-progress
date: 2026-04-05
---

# UX Design Specification NextJS Todo Redesign

**Author:** Minh  
**Date:** 2026-04-05

---

## Executive Summary

### Project Vision

NextJS Todo is undergoing a visual and UX modernization to transform a functionally complete but visually dated application into a contemporary, polished productivity tool. The redesign applies modern design principles—refined visual language, smooth interactions, improved information hierarchy, and professional aesthetics—while preserving all existing functionality, data models, and architecture. This is a brownfield modernization project serving as a training vehicle to validate AI-assisted design-to-code workflows.

### Target Users

The redesign serves four distinct user personas representing the full product usage spectrum:

1. **Alex (New User/Onboarding)** - First-time user seeking a welcoming, modern experience that builds confidence in the product's quality and professionalism
2. **Jordan (Daily Power User)** - Primary user managing 20-30 tasks daily, needs polished interfaces that support efficient task scanning, filtering, and interaction
3. **Casey (Collaborator)** - User who shares tasks with teammates, needs discoverable sharing mechanisms and professional-looking shared views
4. **Morgan (Developer/GitHub User)** - Technical user linking GitHub repos to tasks, needs clean metadata display and professional presentation of technical information

### Key Design Challenges

1. **Modernization without disruption** - Apply contemporary design without changing how users interact with the core product
2. **Visual polish across complexity** - Create refined, cohesive aesthetics across diverse features (auth, task management, collaboration, GitHub integration)
3. **Information hierarchy** - Present task details, metadata, and interactions with clarity and visual guidance
4. **Micro-interaction satisfaction** - Design smooth, responsive interactions that feel intentional and rewarding

### Design Opportunities

1. **Visual language as differentiator** - Modern typography, color palette, and spacing can elevate perceived quality and professionalism
2. **Interaction polish** - Smooth animations and transitions create delight without complexity
3. **Information design** - Clear visual hierarchy and spacing improve scannability and reduce cognitive load
4. **Consistency** - Unified design system across all features strengthens the perception of a complete, thoughtful product

## Core User Experience

### Defining Experience

The core experience is **task lifecycle efficiency with visual satisfaction**. Users engage in a repeating cycle: scan their task list, understand what needs attention, take action (create, complete, filter), and see clear feedback. The redesign elevates this core loop by making every interaction feel responsive, intentional, and polished. Task completion should feel satisfying—not just functionally complete, but emotionally rewarding. The interface should support Jordan's daily 20-30 task management without friction, while welcoming Alex into the product with confidence.

### Platform Strategy

**Primary Platform:** Web application with standard mouse/keyboard interaction model
- Web-first design, responsive but not mobile-optimized in this phase
- Desktop-centric interaction patterns (click, hover, keyboard shortcuts where applicable)
- Modern browser capabilities (smooth transitions, CSS animations)
- No offline functionality required—assume reliable network connectivity

### Effortless Interactions

The following interactions should require zero cognitive friction:

1. **Task Completion** - Marking a task done should be a single click with immediate visual feedback. The action feels smooth and satisfying, not clunky.
2. **Task Creation** - Adding a new task should be discoverable and quick (2-3 fields max for basic task). Form layout should guide the user naturally.
3. **List Scanning** - Jordan should be able to quickly scan 20-30 tasks and understand status at a glance. Visual hierarchy and spacing should guide the eye naturally.
4. **Filtering/Search** - Finding tasks by status or keywords should feel responsive and intuitive, not buried or technical.

### Critical Success Moments

1. **First Impression (Alex)** - Landing on the sign-up page should immediately communicate "this is a professional, modern tool." Clean, spacious design with clear typography builds trust.
2. **First Task Creation** - Alex creates their first task within 2 minutes. The form is simple, labeling is clear, and interaction feels smooth.
3. **Daily Efficiency (Jordan)** - Opening the app each morning, Jordan scans their list, marks done/incomplete tasks, filters to today's work. All interactions feel snappy and responsive.
4. **Task Completion Satisfaction** - Marking a task done has micro-interaction feedback (checkmark animation, subtle color change) that creates a small moment of accomplishment.

### Experience Principles

1. **Polish through clarity** - Modern design comes from clear information hierarchy and generous spacing, not from complexity or visual clutter
2. **Interaction feedback matters** - Every user action should have immediate, satisfying visual feedback (smooth animations, clear state changes)
3. **Efficiency without friction** - Frequent actions (mark complete, add task, filter) should require minimal cognitive load and clicks
4. **Consistency builds confidence** - Unified visual language and interaction patterns across all features make the product feel intentional and complete

## Desired Emotional Response

### Primary Emotional Goals

Users should feel **accomplished, confident, and in control**. The redesigned interface communicates professionalism and quality—making users trust the tool and want to return to it. Each interaction should create a small moment of satisfaction, building momentum through the day. The primary emotional goal is to make task management feel effortless and rewarding, not obligatory.

### Emotional Journey Mapping

- **First Visit (Alex):** Feels welcomed and impressed by modern design; confidence that this is a professional tool they can trust
- **Task Creation:** Sense of ease and clarity—the form guides them naturally without overwhelming options
- **Daily Use (Jordan):** Enters a productive, focused state; scanning the list feels satisfying and clear
- **Task Completion:** Micro-satisfaction from smooth interaction and visual feedback; accomplishment builds with each completed item
- **End of Session:** Sense of progress and control; wanting to return because using it feels good
- **Daily Habit:** Looking forward to opening the app; efficiency and completion create positive reinforcement

### Micro-Emotions

The redesign should emphasize:

1. **Confidence** - Modern, clear design signals quality and trustworthiness (not confusion or skepticism)
2. **Accomplishment** - Task completion should feel earned and satisfying (not indifferent or hollow)
3. **Control** - Users feel they're managing their work, not overwhelmed by the tool (not anxiety or helplessness)
4. **Calm Focus** - Clean layout and clear hierarchy support concentration without visual noise (not overwhelm or distraction)
5. **Delight** - Smooth interactions and thoughtful details create small moments of joy (not just functional)

### Design Implications

To achieve these emotional goals, UX decisions must support:

- **Confidence through Design:** Clear typography, generous spacing, professional color choices, and consistent patterns build trust from first impression
- **Accomplishment through Feedback:** Smooth animations on task completion, clear state changes, and satisfying visual feedback reinforce progress
- **Control through Clarity:** Information hierarchy, scannable layouts, and predictable interactions make users feel in command of their work
- **Calm through Simplicity:** Eliminate unnecessary elements, use whitespace effectively, focus the interface on core actions
- **Delight through Attention to Detail:** Smooth transitions, thoughtful micro-interactions, and refined visual elements create moments of pleasure

### Emotional Design Principles

1. **Modern design builds trust** - Contemporary aesthetics (clean typography, refined spacing, professional color) communicate quality and competence
2. **Smooth interactions create satisfaction** - Every action should feel responsive and polished, reinforcing user agency
3. **Clarity reduces anxiety** - Clear visual hierarchy and predictable patterns eliminate confusion and build confidence
4. **Completion should feel earned** - Task interactions should provide satisfying feedback that acknowledges user accomplishment
5. **Refinement signals care** - Attention to details (spacing, typography, micro-animations) shows the product was thoughtfully designed

## UX Pattern Analysis & Inspiration

### Inspiring Products Analysis

Well-designed task management applications demonstrate proven patterns for modern productivity UX. Analysis of leading examples (Todoist, Things 3, Microsoft To Do, Linear) reveals consistent success patterns:

**Core Strengths Across Leaders:**
- **Clean list views** with clear visual hierarchy and generous spacing
- **Instant visual feedback** on task completion (satisfying animations, color changes)
- **Minimal friction onboarding** that gets users to their first task quickly
- **Flexible filtering/views** that don't overwhelm with options
- **Modern typography and color** that feels contemporary and professional
- **Smooth interactions** throughout (transitions, hover states, micro-animations)
- **Clear information hierarchy** that lets users scan quickly
- **Consistent interaction patterns** across all features

### Transferable UX Patterns

**Patterns We'll Adopt for NextJS Todo:**

1. **Task Completion Animation** - Todoist and Things 3 excel here. When marking a task done, smooth animation (checkmark appear, subtle color shift to muted, or line-through fade) creates satisfying feedback. This directly supports our accomplishment emotional goal.

2. **Scannable Task List** - Linear's task list demonstrates excellent information hierarchy. Title/description prioritized, metadata (due date, tags) positioned consistently below, supporting Jordan's ability to scan 20-30 tasks quickly.

3. **Subtle Hover States** - Modern task apps use hover states effectively (background shift, action buttons appear) without being distracting. This guides user attention and makes interactions discoverable.

4. **Quick Add Pattern** - Todoist's floating action button and Things 3's quick-add at the top both solve the "create task" flow elegantly. Minimal friction, clear focus, gets users to content entry instantly.

5. **Color Coding/Status Indicators** - Visual status indicators (completion, priority, due date) communicate task state at a glance without text overload.

6. **Clear Form Design** - Modern productivity apps strip forms down to essentials. Required fields clearly labeled, optional fields don't clutter the view, submit/cancel actions unambiguous.

7. **Whitespace and Breathing Room** - All successful modern task apps use generous spacing. This reduces cognitive load and communicates sophistication.

### Anti-Patterns to Avoid

1. **Overwhelming Filter Options** - Too many filtering/sorting options create analysis paralysis. Keep filtering simple and discoverable.

2. **Busy Visual Design** - Dated task apps over-decorate. Avoid unnecessary colors, gradients, shadows, or visual effects. Restraint = modern.

3. **Sluggish Interactions** - Animations that feel slow or laggy frustrate users. Keep animations quick (200-300ms) and purposeful.

4. **Hidden Functionality** - Required actions (delete, share, comment) shouldn't be hidden behind menus. Make common actions discoverable.

5. **Poor Empty States** - Empty task lists should guide users, not demoralize them. Use empty states to educate and invite action.

6. **Inconsistent Interactions** - If task creation works one way, don't make editing work differently. Consistency builds confidence.

### Design Inspiration Strategy

**What to Adopt:**
- Task completion animations that provide satisfying visual feedback
- Clean, scannable list layouts with clear information hierarchy
- Subtle hover states that guide interaction discovery
- Quick-add patterns that minimize friction for task creation
- Modern typography (clear, open sans-serif) and spacious layouts
- Consistent interaction patterns across all features

**What to Adapt:**
- Color coding/status indicators (adapted for our visual language)
- Form design patterns (simplified for our core task features)
- Navigation approaches (adapted to our authentication + task management model)
- Empty state messaging (tailored to our onboarding journey)

**What to Avoid:**
- Overdecoration, visual clutter, trendy effects that date quickly
- Complex filtering systems that confuse users
- Sluggish or unresponsive interactions
- Inconsistent UI patterns that break user confidence
- Hidden or unclear actions

This strategy ensures NextJS Todo benefits from proven patterns while maintaining its own identity and focus on modernized task management.

## Design System Foundation

### Design System Choice

**Recommendation: Tailwind CSS + Custom Component Library**

For NextJS Todo, we recommend a **Tailwind CSS foundation with custom-built components**. This approach balances speed (Tailwind's utility-first system) with visual control and consistency.

### Rationale for Selection

1. **Perfect for Single Developer + AI** - Tailwind's utility-first approach makes it easy for AI tools to generate and modify components consistently. The developer can quickly review and iterate.

2. **Brownfield Integration** - If NextJS Todo already uses React and standard tooling, Tailwind integrates smoothly without replacing existing code. This is safer than adopting a full component library that might conflict with current patterns.

3. **Visual Control** - Unlike Material Design or Ant Design (which carry opinionated aesthetics), Tailwind gives complete freedom to create a modern, custom visual identity that feels unique to NextJS Todo.

4. **Fast Component Development** - Custom components built with Tailwind are quick to create and modify. Combined with AI assistance, this accelerates the design-to-code workflow.

5. **Consistency via Design Tokens** - Tailwind's configuration (colors, spacing, typography, shadows) acts as our design system. All components use the same tokens, ensuring consistency automatically.

6. **NextJS Native** - Tailwind works seamlessly with NextJS. No additional configuration complexity.

### Implementation Approach

**Phase 1: Design Token System**
- Define core design tokens in Tailwind config: color palette, typography scale, spacing scale, shadow system, border radius, transitions
- These tokens become the source of truth for visual consistency

**Phase 2: Component Library**
- Build ~12-15 core components: Button, Input, Card, Modal, Toast, Dropdown, Checkbox, Radio, Textarea, Select, Badge, Spinner
- Each component uses Tailwind utilities + design tokens
- Keep components simple and composable

**Phase 3: Feature Components**
- Combine core components into feature-specific components: TaskCard, TaskForm, TaskList, AuthForm, CommentThread, etc.
- These are built in the actual app during implementation

**Phase 4: Iteration**
- As designs are implemented, refine tokens and components based on real usage
- AI-assisted generation makes iteration fast

### Customization Strategy

**Visual Identity Through Design Tokens:**
- Modern color palette (likely a clean primary color + complementary accent, neutral grays for backgrounds/text)
- Contemporary typography (open sans-serif like Inter, Poppins, or Geist)
- Generous spacing (16px base unit with 1.5x scale: 4, 8, 12, 16, 24, 32, 48, 64)
- Subtle shadows (not overdone, supporting depth and hierarchy)
- Smooth transitions (200-300ms for interactions, supporting our emotional goals)

**Component Customization:**
- Buttons: Modern, minimal design with clear states (default, hover, active, disabled)
- Inputs: Clean borders, clear focus states, good padding
- Cards: Subtle shadow and spacing, room to breathe
- Status indicators: Color-coded with clear semantics (done=muted/strikethrough, todo=bold, overdue=warning-color)
- Micro-interactions: Smooth checkmark animation on task completion, subtle hover states, responsive feedback

## Core Experience Definition

### The Defining Experience: Task Completion

**The interaction that makes NextJS Todo special is marking tasks complete.** This is the moment where users experience accomplishment and momentum. If we nail this one interaction—making it smooth, responsive, and satisfying—everything else follows. Jordan uses this action 30+ times a day. Perfecting it is perfecting the product.

### User Mental Model

Users think about task completion naturally:
- **Mental model:** "I did this thing. It's done. Move it off my plate."
- **Expectation:** One-click completion with clear visual feedback that it worked
- **What users love in existing tools:** Smooth animations, instant feedback, small moments of delight (Todoist's satisfying checkmark, Things 3's smooth transitions)
- **What frustrates:** Sluggish interactions, unclear whether action registered, completion feeling hollow (no reward)

Current users who've tried good task apps (Todoist, Things 3, Apple Reminders) expect completion to be:
- **Instant:** No loading, no delay. Click and it's done.
- **Visual:** Clear state change (checkmark appears, strikethrough fades in, or muted color)
- **Satisfying:** A micro-interaction that feels rewarding, not just functional

### Success Criteria for Core Experience

Task completion succeeds when:

1. **Speed & Responsiveness** - Click registers instantly. Zero perceptible delay. User never thinks "is it working?"
2. **Visual Feedback** - Immediate visual change shows completion (animated checkmark, color shift, strikethrough, or combination)
3. **Satisfaction** - The interaction creates a small moment of pleasure. Users want to mark more tasks done.
4. **Clarity** - No ambiguity about state. User knows at a glance whether tasks are done or pending
5. **Undo-ability** - Users can revert if they marked something done by mistake. Undo is discoverable or automatic (e.g., brief undo toast)
6. **Momentum** - Each completion builds psychological momentum. Users feel progress.

### Established UX Pattern: Checkbox Toggle

Task completion uses an **established, proven pattern: the checkbox toggle.** Users already understand this from email (Gmail), productivity (Todoist), and everyday interfaces. We don't need to innovate on the interaction itself—we innovate on the **delight and responsiveness.**

**Why not innovate:**
- Users bring expectations from other tools
- Checkbox is instantly recognizable
- Trying a novel interaction risks confusion

**How we innovate within this pattern:**
- Smooth, polished animation on the checkbox itself (SVG animation, Lottie, or CSS)
- The entire task row responds to completion (color fade, strikethrough, subtle movement)
- Optional: Undo toast appears briefly below the completed task
- Combined effect: Familiar pattern + delight through execution

### Experience Mechanics: Mark Task Complete

Breaking down the step-by-step flow:

**1. Initiation**
- User hovers over a task in their list
- Checkbox becomes more prominent (slight scale increase or color change on hover)
- Visual cue: "I can interact with this"

**2. Interaction**
- User clicks the checkbox (or hits a keyboard shortcut like Cmd+Enter)
- System registers the action immediately (optimistic update - UI changes instantly)
- Zero waiting for server response

**3. Feedback - Primary**
- **Checkbox animation:** SVG checkmark draws itself smoothly (200-300ms animation)
- **Task row response:** Entire row transitions to "done" state:
  - Text color fades to muted gray (not full white, not black—a lighter gray showing it's backgrounded)
  - Optional strikethrough text fades in
  - Row maintains position (doesn't disappear, doesn't move—consistency matters)
  
**4. Feedback - Secondary (Optional)**
- **Undo toast:** Brief toast appears below the completed task: "Task marked done. Undo?"
- Toast disappears after 3 seconds or when user closes it
- If user clicks undo: Task reverts to pending state with smooth reverse animation

**5. Completion**
- Task is now visually marked complete in the interface
- Data syncs to server in background (user doesn't wait for this)
- If server sync fails, user gets a subtle notification (banner or inline message)
- User's list updates to show their progress (e.g., "3 of 8 complete" counter increments)

### Interaction Details

**Timing:**
- Checkbox animation: 200-300ms (fast, snappy)
- Row color transition: 300-400ms (smooth fade, feels polished)
- Undo toast timing: Appears instantly, shows for 3 seconds
- Overall flow: 400-500ms from click to complete rest state

**States:**
- **Unchecked/Active:** Bold text, full color, prominent
- **Checked/Done:** Muted gray text, strikethrough (optional), subtle appearance
- **Hover (unchecked):** Checkbox highlights, row background subtly lightens
- **Hover (checked):** Checkbox highlights (for potential undo), row maintains muted appearance
- **Keyboard focus:** Clear focus ring around checkbox for accessibility

**Accessibility:**
- Checkbox is a semantic HTML input with proper ARIA labels
- Keyboard users can tab to checkbox and press Enter/Space to toggle
- Screen readers announce task completion
- High contrast maintained between all states

### Why This Matters

If task completion feels perfect—responsive, satisfying, clear—users will:
- Want to use the app daily (momentum-building interaction)
- Trust the interface (instant feedback builds confidence)
- Perceive the entire product as polished (details matter)
- Recommend it to others ("This app feels so good to use")

This single interaction, executed well, transforms the entire perception of NextJS Todo from "a functional task app" to "a delightful productivity tool."

## Visual Design Foundation

### Color System

**Philosophy:** Modern, minimal color palette that communicates professionalism while remaining warm and approachable. Color should guide attention, not distract. The palette supports our emotional goals: confidence (clear, consistent), accomplishment (satisfying feedback), and calm (restrained, not overwhelming).

**Core Color Palette:**

**Primary Color: Modern Blue (Confidence)**
- Primary: `#2563eb` (vibrant, trustworthy blue)
- Primary Light: `#3b82f6` (lighter for hover states)
- Primary Dark: `#1d4ed8` (darker for active states)
- Use for: Primary buttons, links, important interactive elements, task due date indicators

**Accent Color: Warm Teal (Accomplishment)**
- Accent: `#0d9488` (completed tasks, success states)
- Accent Light: `#14b8a6` (hover states)
- Use for: Task completion checkmarks, success notifications, positive feedback

**Neutral Base (Calm & Clarity)**
- White: `#ffffff` (backgrounds)
- Gray-50: `#f9fafb` (secondary backgrounds, subtle containers)
- Gray-100: `#f3f4f6` (tertiary backgrounds, hover states)
- Gray-200: `#e5e7eb` (borders, dividers)
- Gray-400: `#9ca3af` (secondary text, meta information)
- Gray-600: `#4b5563` (primary text)
- Gray-900: `#111827` (headings, strong emphasis)

**Semantic Colors:**
- **Success:** `#10b981` (completion, positive actions)
- **Warning:** `#f59e0b` (overdue tasks, caution)
- **Error:** `#ef4444` (destructive actions, errors)
- **Info:** `#2563eb` (secondary information, tooltips)

**Completed Task State:**
- Text: Gray-400 (muted, showing it's backgrounded)
- Strikethrough: Applied to text (optional, for clarity)
- Background: Unchanged (task stays in list, doesn't disappear)

**Accessibility:**
- All text meets WCAG AA contrast requirements (4.5:1 for body text, 3:1 for UI components)
- Color is never the only indicator of status (checkmarks, icons, text also communicate state)
- Focus states use visible rings, not just color changes

### Typography System

**Philosophy:** Clear, modern sans-serif that supports readability and hierarchy. Typography should guide users' eyes naturally through information, with generous sizing that communicates importance.

**Primary Typeface: Inter** (modern, open, highly readable)
- Fallback: `system-ui, -apple-system, sans-serif`
- Used for all body text, buttons, forms, and UI

**Secondary Typeface: Inter (same)** - Unified typeface for consistency
- Some designs use a serif for headings; we keep Inter throughout for cohesion

**Type Scale** (Tailwind-based):
- `text-xs`: 12px, line-height 1.5 (labels, meta text)
- `text-sm`: 14px, line-height 1.5 (secondary text, captions)
- `text-base`: 16px, line-height 1.5 (body text, standard)
- `text-lg`: 18px, line-height 1.5 (secondary headings, emphasis)
- `text-xl`: 20px, line-height 1.5 (section headings)
- `text-2xl`: 24px, line-height 1.3 (page headings)
- `text-3xl`: 30px, line-height 1.2 (main titles)

**Font Weights:**
- Regular (400): Body text, primary content
- Medium (500): Button text, labels, secondary headings
- Semibold (600): Strong emphasis, section headings
- Bold (700): Page titles, strong callouts

**Line Heights:**
- Headings: 1.2 (tighter, feels structured)
- Body: 1.5 (generous, improves readability)
- Input fields: 1.5 (comfortable for text entry)

**Example Hierarchy:**
- Page Title: 30px, Bold, Color gray-900
- Section Heading: 20px, Semibold, Color gray-900
- Card Title/Task Title: 16px, Medium, Color gray-900
- Body Text: 16px, Regular, Color gray-600
- Meta Text (date, tags): 12px, Regular, Color gray-400
- Button Text: 14px, Medium, Color (varies by button type)

### Spacing & Layout Foundation

**Philosophy:** Generous whitespace creates calm and clarity. Spacing follows a consistent scale, making the interface feel structured and intentional. Density supports scanning without overwhelming.

**Spacing Scale** (Tailwind 4px base unit):
- `4px` (1 unit): Tight spacing between related elements
- `8px` (2 units): Standard element padding
- `12px` (3 units): Spacing between form fields, small sections
- `16px` (4 units): Component padding, standard spacing
- `24px` (6 units): Section spacing, between major containers
- `32px` (8 units): Large section spacing
- `48px` (12 units): Page-level spacing

**Layout Grid:**
- 12-column responsive grid
- Desktop: Full width with side margins (24px left/right minimum)
- Tablet: Adjusted column span
- Responsive breakpoints align with Tailwind defaults

**Component Spacing:**
- **Buttons:** 16px padding (12px vertical, 16px horizontal)
- **Form inputs:** 8px top/bottom, 12px left/right padding
- **Cards:** 24px padding, 8px border-radius, subtle shadow
- **Lists:** 12px spacing between items
- **Sections:** 32-48px spacing between major sections

**Whitespace Strategy:**
- Use whitespace actively to group related elements
- Breathing room around interactive elements (buttons, inputs)
- Generous margins between unrelated sections
- Avoid wall-of-text layouts—break content with whitespace

**Task List Density:**
- Each task card: 16px padding
- Spacing between tasks: 8px
- Supports Jordan's 20-30 task scanning while maintaining clarity
- Tasks feel separate but cohesive as a list

### Accessibility Considerations

**Color & Contrast:**
- All text meets WCAG AA standards (4.5:1 for body, 3:1 for UI)
- Status communicated through multiple cues (not color alone)
- High contrast between interactive elements and backgrounds

**Typography:**
- Minimum 16px font size for body text (improves mobile readability)
- Line height 1.5+ supports dyslexia and visual processing
- Sufficient spacing between lines and letters

**Spacing:**
- Touch targets (buttons, checkboxes): 44px minimum height/width
- Click areas sufficiently spaced (8px minimum between interactive elements)
- Generous padding reduces accidental misclicks

**Interactive Elements:**
- Clear focus states (visible focus ring, not just color)
- Keyboard navigation supported throughout
- Semantic HTML (buttons, inputs, labels) for screen reader compatibility

**Dark Mode Consideration:**
- Design foundation works with light mode; dark mode can be supported via Tailwind dark: variants
- Would invert colors appropriately: white → dark gray, dark gray → light gray
- Same contrast ratios maintained in dark mode

## Design Direction Exploration

### Design Directions Generated

Eight comprehensive design direction mockups have been created and are available in `ux-design-directions.html`. These mockups explore different visual approaches while maintaining our core design system:

1. **Minimal/Clean** - Maximum whitespace, line separators, zen aesthetic
2. **Contemporary/Gradient** - Gradient backgrounds, colored left borders, subtle motion
3. **Cards & Depth** - Card-based layout with shadows and clear separation
4. **Flat/Bold** - Bold color bars, heavy typography, energetic feel
5. **Compact/Efficient** - Information-dense layout, maximum task visibility
6. **Elegant/Refined** - Sophisticated aesthetic with premium feel
7. **Dark/Modern** - Dark theme with blue accents, modern aesthetic
8. **Colorful/Personality** - Teal accents, friendly tone, more personality

Each mockup demonstrates task list interactions, completion states, and visual hierarchy in the context of the defining experience (marking tasks complete).

### Design Direction Strategy

The design directions serve multiple purposes:

- **Visual Exploration:** Exploring how our design tokens (colors, typography, spacing) can be applied in different ways
- **Aesthetic Alignment:** Testing which visual approach best supports our emotional goals (confidence, accomplishment, calm)
- **Implementation Reference:** Each direction shows proven patterns and component arrangements ready for implementation
- **Direction Flexibility:** Multiple options allow selection or combination of elements based on preference and feedback

The selected direction will guide component design, layout decisions, and visual styling throughout the remainder of the project.

## User Journey Flows

### Journey 1: Alex - New User Onboarding

**Goal:** First-time user creates account and completes first task within 2 minutes, feeling confident and impressed.

**Entry Point:** User lands on NextJS Todo homepage (cold visitor or shared link)

**Flow Steps:**

1. **Landing Page Moment**
   - User sees modern, clean homepage with clear value proposition
   - CTA: "Sign Up for Free" button prominent
   - Visual: Professional hero section with example task list (shows what the app does)
   - Emotional goal: "This looks professional and trustworthy"

2. **Sign Up Form**
   - Form asks for: Email, Password (required), Name (optional)
   - Form layout: Vertical stacking, generous spacing, clear labels
   - Submit button: "Create Account" in primary blue
   - Support text: "Takes 30 seconds"
   - Password strength indicator shown in real-time
   - Error handling: Clear inline errors if validation fails
   - Emotional goal: "This is simple and I can do this"

3. **Account Created - Empty State**
   - Success! User sees empty task list
   - Empty state design: Welcoming illustration, headline "Your tasks await"
   - Primary CTA: Large "Create Your First Task" button
   - Support text: "Add your first task to get started"
   - Optional secondary action: "See example tasks" (guides exploration)
   - Emotional goal: "I know exactly what to do next"

4. **Task Creation - Simplified Form**
   - User clicks "Create Your First Task"
   - Minimal form appears with 3 fields:
     - Task Title (required, auto-focused)
     - Description (optional, larger textarea)
     - Due Date (optional, date picker)
   - Submit button: "Create Task"
   - Form has natural flow: user types title → can add details → create
   - Validation: Only title required, feedback appears as user types
   - Emotional goal: "This is easy and feels responsive"

5. **Task Created - First Success**
   - Task appears in list (animated entrance)
   - Empty state disappears
   - Task shown with modern styling from chosen design direction
   - Small confirmation: Subtle success notification "Task created!"
   - Next CTA appears: "Create another task" or "View your task"
   - Emotional goal: "I did it! And it looks great!"

6. **Momentum Building**
   - User is now in the main app with one task
   - See filtering options, can mark complete, can add more tasks
   - If user marks task complete: Smooth completion animation reinforces accomplishment
   - If user creates another task: Form reappears, momentum continues

**Success Indicators:** Account created, at least 1 task created, user has experienced task completion animation

**Error Recovery:**
- If form validation fails: Inline error message, field highlights, form stays visible
- If network error on submit: Retry button appears, user can resubmit
- If password too weak: Suggestion shows requirements, user can adjust

**Optimization Principles:**
- Minimize information at each step (only essentials shown)
- Clear visual progression (empty → one task → task list)
- Celebrate small wins (success animations, confirmations)
- Remove friction (auto-focus, smart defaults, fast validation)

---

### Journey 2: Jordan - Daily Task Manager

**Goal:** Open app each morning, quickly scan tasks, prioritize work, mark done throughout day. Feel productive and in control.

**Entry Point:** User opens app (authenticated, morning routine)

**Flow Steps:**

1. **App Opened - Dashboard View**
   - User lands on main task list
   - Immediate visual hierarchy: shows tasks grouped by status
   - Counter visible: "X of Y tasks complete"
   - Tasks shown with: Title, due date, priority indicator, status
   - Navigation options visible: Filter, Search, Add task
   - Emotional goal: "I can see what matters at a glance"

2. **Quick Scan**
   - User reads task titles and due dates without clicking
   - Visual design supports quick scanning:
     - Overdue tasks: Warning color (orange), highlighted
     - Due today: Primary color (blue), emphasized
     - Due later: Neutral gray
   - Icons/badges show task status clearly
   - List ordered by due date by default
   - Emotional goal: "I understand my priorities instantly"

3. **Filtering for Focus**
   - User wants to focus on today's tasks
   - Click filter button or quick filter chip: "Today"
   - List instantly filters to show only today's tasks
   - Filter persists (if user navigates and returns, filter still active)
   - Easy to reset: Clear filter button always visible
   - Multiple filter options available: Today, This week, By status (done/not done), By priority
   - Emotional goal: "I can find what I need in seconds"

4. **Task Completion - Core Interaction**
   - User marks a task complete
   - Click on checkbox (or spacebar with keyboard)
   - Instant visual feedback:
     - Checkbox fills with green checkmark (animated)
     - Task text fades to gray (muted appearance)
     - Strikethrough appears (optional, based on design direction)
     - Task stays in list (doesn't disappear)
   - Brief undo notification appears: "Task marked done. Undo?" (3 sec auto-dismiss)
   - Counter updates: "X of Y" increments
   - Emotional goal: "That felt satisfying. I'm making progress."

5. **Task Details Access**
   - User needs to see/edit task details
   - Click task title or click expand button
   - Details view slides in or opens:
     - Full task title and description
     - Due date (editable)
     - Status (complete/incomplete toggle)
     - Comments thread (if collaboration enabled)
     - GitHub repo link (if linked)
   - Edit button allows quick inline editing of title/description
   - Back button or close returns to list
   - Emotional goal: "I can see everything about this task quickly"

6. **Quick Search**
   - User wants to find specific task
   - Click search icon in header
   - Search box appears with placeholder: "Search tasks..."
   - Type task name, description, or tag
   - Results filter in real-time (debounced)
   - Shows matching tasks highlighted
   - Clear search button to reset
   - Emotional goal: "Finding things is effortless"

7. **Adding New Tasks During Day**
   - User wants to capture a new task mid-day
   - Click "Add Task" button (always visible in header or footer)
   - Quick add modal appears:
     - Single input field: "What needs to be done?"
     - Optional details: click to expand and add due date
   - Submit: Task created and added to list
   - Modal closes, user back to list
   - Emotional goal: "Capturing tasks is instant, doesn't interrupt flow"

8. **End of Day Review**
   - User reviews completed tasks
   - See completed counter: "8 of 12 tasks complete"
   - Optional: Review what they accomplished
   - All interactions remain smooth and responsive
   - Emotional goal: "I can see what I accomplished. Great day!"

**Success Indicators:** Multiple tasks scanned, filtered view used, at least 3 tasks marked complete, no friction in core interactions

**Error Recovery:**
- Accidental completion: Undo toast appears automatically, click to revert
- Network issue on completion: Retry notification appears, can resubmit
- Form validation error: Inline message, field focuses, user corrects

**Optimization Principles:**
- Task completion is single-click (checkbox primary interaction)
- List stays visible while interacting (modals for details, not page navigation)
- Filtering is instant and discoverable
- Progress indicators visible throughout (counter, visual status)
- Keyboard shortcuts available for power users (space to complete, cmd+enter to create)

---

### Journey 3: Casey - Collaborator Sharing Tasks

**Goal:** Share a task with teammate, colleague sees details and comments. Both can collaborate asynchronously.

**Entry Point:** User is viewing a task they want to share

**Flow Steps:**

1. **Locate Task to Share**
   - User opens main task list
   - Finds task they want to share with teammate
   - Clicks task to view details
   - Emotional goal: "Task is visible and I know how to access it"

2. **Share Action Discovery**
   - In task details view, "Share" button is visible and accessible
   - Button is clearly labeled: "Share Task" or "Copy Share Link"
   - Located in header or action menu (consistent placement)
   - Visual treatment: Clear, clickable, discoverable at a glance
   - Emotional goal: "I can immediately see how to share this"

3. **Generate Share Link**
   - User clicks "Share Task" button
   - System generates unique, secure share link
   - Link copied to clipboard automatically (or user clicks copy button)
   - Confirmation toast appears: "Link copied to clipboard"
   - User can customize sharing (optional):
     - Allow comments? (yes/no toggle)
     - Allow editing? (no by default)
     - Expiration date? (optional, defaults to no expiration)
   - Link shown in modal with copy button, share to email/slack (if available)
   - Emotional goal: "Sharing is one click and I'm done"

4. **Teammate Receives Link**
   - Teammate opens shared link (email, Slack, or direct paste)
   - Shared task view loads
   - No login required (if sharing allows public access)
   - If login required: Simple sign-up/login flow before viewing
   - Emotional goal: "The link works and I can see the task immediately"

5. **Shared Task View**
   - Task displayed in clean, read-only format (or editable if permissions allow)
   - Shows:
     - Task title and full description
     - Due date
     - Status (complete/incomplete)
     - Comments thread
     - Related GitHub repo (if linked)
   - Comments are central to the experience (below details)
   - Emotional goal: "This looks professional and complete"

6. **Adding Comments**
   - Teammate clicks in comment input: "Add a comment..."
   - Types comment with formatting (optional: bold, lists)
   - Can mention other users with @mentions
   - Submit comment or Cmd+Enter
   - Comment appears immediately in thread
   - Original user (Casey) gets notification: "New comment on shared task"
   - Emotional goal: "Commenting is natural and collaborative"

7. **Real-time Collaboration**
   - Comments appear in real-time for both users
   - Task status updates reflected instantly (if teammate can edit)
   - Both can see conversation thread growing
   - Easy to follow conversation (nested replies, user avatars)
   - Emotional goal: "We're working together seamlessly"

8. **Returning to Shared Task**
   - Teammate can bookmark/favorite shared task
   - Returns via saved link later
   - Comments history visible (full conversation preserved)
   - Can continue collaboration asynchronously
   - Emotional goal: "Our collaboration is persistent and easy to find"

**Success Indicators:** Share link generated, teammate accessed shared task, comment added and visible, no login friction for teammate

**Error Recovery:**
- Link invalid: Clear error message, option to request new link
- Permission denied: Clear message, option to contact creator
- Comment submission failed: Retry button, notification of retry

**Optimization Principles:**
- Sharing is one-click (generate and copy link)
- Shared view is clean and professional (no clutter)
- Comments are threaded and easy to follow
- Permissions are clear (who can do what)
- Notifications alert collaborators of activity

---

### Journey 4: Morgan - Power User with GitHub Integration

**Goal:** Link GitHub repo to task, see repo metadata, track work-in-progress against code changes.

**Entry Point:** User creating a task related to code work

**Flow Steps:**

1. **Task Creation with GitHub Intent**
   - User creates new task (normal flow)
   - Fills in task title: "Implement user authentication"
   - In task details view, sees "Link Repository" action
   - Or in task form, optional section: "Link to GitHub"
   - Emotional goal: "GitHub integration is discoverable but optional"

2. **Repository Search & Linking**
   - User clicks "Link Repository"
   - Modal appears: "Search GitHub repositories"
   - Authenticated via GitHub OAuth (one-time setup)
   - User searches: types repo name or owner/repo
   - Results show matching repos with:
     - Repo name and owner
     - Description
     - Language/tech stack
     - Star count (relevance indicator)
   - User clicks repo to link
   - Emotional goal: "Finding and linking repos is simple"

3. **Metadata Sync**
   - System fetches repo metadata from GitHub API:
     - Repo name, description, URL
     - Open issues count
     - Recent commits
     - Language/tech stack
     - Collaborators
   - Data displayed in task details
   - Metadata updates periodically (hourly or on-demand refresh)
   - Link to repo is clickable (opens in new tab)
   - Emotional goal: "I have all the context I need in one place"

4. **Dedicated GitHub View**
   - User can click "View Repository" link
   - Navigates to dedicated GitHub repository view
   - Shows:
     - Repo name, description, link
     - Stats: Stars, Forks, Open Issues
     - Recent commits (last 5-10, with messages and authors)
     - Linked tasks count: "2 tasks linked to this repo"
     - Open issues (if public repo)
     - Related tasks (all tasks linked to this repo)
   - Professional, information-rich layout
   - Easy to switch between task view and repo view
   - Emotional goal: "I can see everything about this repo's status"

5. **Task-to-Issue Tracking**
   - Advanced: Link task to specific GitHub issue
   - In task details: "Link to GitHub Issue"
   - Search issues in repo: "Search open issues"
   - User selects issue
   - Task now shows linked issue:
     - Issue number and title
     - Issue status, labels, assignee
     - Link to issue on GitHub
   - Task status can sync with issue status (optional)
   - Emotional goal: "My task management syncs with our code workflow"

6. **Notification & Status Sync**
   - If issue status changes on GitHub: Notification in app
   - If task is marked complete: Optional notification to team
   - Webhook integration (if supported) keeps data fresh
   - User can manually refresh to sync latest data
   - Emotional goal: "No manual updates needed, everything stays in sync"

7. **Repository List View**
   - User can view all linked repositories
   - Shows which repos have active tasks
   - Quick filter: "Show repos with active tasks"
   - Useful for tracking multiple projects
   - Emotional goal: "All my code projects are visible and tracked"

**Success Indicators:** Repo successfully linked, metadata displayed, dedicated repo view accessed, task-to-issue relationship functional

**Error Recovery:**
- Repository not found: Search suggestions, helpful error message
- GitHub auth fails: Clear re-auth prompt, docs link
- Metadata sync fails: Retry button, manual refresh option
- Issue link broken: Clear notification, option to relink

**Optimization Principles:**
- GitHub integration is optional (doesn't block core workflow)
- Metadata is displayed naturally (not overwhelming)
- Linking is discoverable but non-intrusive
- Data stays fresh (periodic syncs or webhooks)
- Professional presentation of technical information

---

### Journey Patterns & Reusable Components

**Common Patterns Across All Journeys:**

1. **Modal/Detail Patterns**
   - Task details slide in from side or open as modal
   - Consistent close behavior (X button, click outside, Esc key)
   - Always show breadcrumb or back button to return to list

2. **Form Patterns**
   - Consistent form layout: vertical stacking, generous spacing
   - Required fields marked clearly
   - Real-time validation feedback
   - Submit and cancel buttons always visible
   - Auto-focus first field on open

3. **Feedback Patterns**
   - Toast notifications for quick actions (3 second auto-dismiss)
   - Inline errors for validation (red text, highlights)
   - Success animations for core interactions
   - Progress indicators for longer operations

4. **Navigation Patterns**
   - Primary list always accessible (back button or menu)
   - Quick actions (add, search, filter) always in header
   - Consistent icon usage and placement
   - Breadcrumbs show current context

5. **Data Persistence**
   - Form state auto-saves (drafts for unsaved comments)
   - Filter and sort preferences remembered
   - Recent searches available
   - User can navigate away without losing data

6. **Accessibility Patterns**
   - All actions have keyboard shortcuts (listed in help)
   - Tab order logical throughout
   - Focus states visible on all interactive elements
   - Screen reader friendly (semantic HTML, ARIA labels)

### Flow Optimization Principles

1. **Minimize Steps to Value**
   - Alex gets to first task in 2 minutes (onboarding)
   - Jordan marks complete with single click
   - Casey shares task in 3 clicks
   - Morgan links repo in less than 1 minute

2. **Provide Progressive Disclosure**
   - Basic view shows essentials
   - Click/expand to see details
   - Don't overwhelm with options upfront

3. **Create Satisfying Feedback**
   - Completion animations make actions feel rewarding
   - Success toasts confirm actions completed
   - Progress indicators show momentum building

4. **Handle Errors Gracefully**
   - Errors are clear and actionable
   - Recovery paths always visible (retry, undo, try again)
   - Errors never block user from trying alternative approach

5. **Support Power User Workflows**
   - Keyboard shortcuts for frequent actions
   - Batch operations where relevant
   - Advanced options available without overwhelming basics

6. **Maintain Consistency**
   - Same interaction pattern used throughout
   - Visual design consistent across all flows
   - Navigation structure predictable
   - Terminology consistent across UI

## Component Strategy

### Design System Components (Tailwind + Headless UI)

The following components are provided by Tailwind CSS and Headless UI, requiring minimal customization:

- **Button:** All variants (primary blue, secondary gray, danger red, sizes sm/md/lg)
- **Text Input:** Standard form input with focus states and validation
- **Textarea:** Multi-line text input with auto-expand option
- **Checkbox:** Standard checkbox with checked/unchecked states
- **Radio Button:** Single-select radio input
- **Select/Dropdown:** Native or custom dropdown component
- **Modal/Dialog:** Generic modal container with backdrop and close
- **Popover:** Tooltip and popover positioning
- **Toast/Notification:** Position-based notifications that auto-dismiss

### Custom Components

Custom components designed specifically for NextJS Todo task management experience:

#### 1. TaskCard

**Purpose:** Display a single task in list view. Central to the core experience (marking tasks complete).

**States:**
- **Pending (default):** White background, title in dark text, due date in gray
- **Pending (hover):** Subtle background color shift, checkbox becomes more prominent
- **Pending (focus):** Focus ring visible on checkbox
- **Completed:** Text fades to gray, strikethrough applied, checkbox shows checkmark (animated)
- **Completed (hover):** Still shows completion state
- **Overdue:** Warning color (orange) accent, "Overdue" label
- **Today:** Primary color (blue) accent, "Today" label

**Anatomy:**
- Checkbox (left): 20x20px, clickable
- Content (center): Title, description snippet, metadata (due date, tags)
- Actions (right, on hover): Edit, more menu (optional details)

**Interaction:**
- Click checkbox to toggle complete state
- Click task title/content to open details
- Completion state has smooth animation (200-300ms)

**Variants:**
- **Compact:** Title only, minimal metadata (for efficiency view)
- **Detailed:** Title, description, metadata, and action hints

**Accessibility:**
- Semantic checkbox input
- `aria-label` on task title
- Keyboard accessible (Tab to focus, Enter/Space to complete)

**CSS (Tailwind):**
```
base: flex gap-3 p-4 border-b hover:bg-gray-50 transition-colors
pending: text-gray-900
completed: text-gray-400 line-through
overdue: border-l-4 border-orange-400
```

---

#### 2. TaskList

**Purpose:** Container for multiple tasks. Supports scrolling, filtering, and density.

**Features:**
- Displays multiple TaskCard components
- Supports scrolling (max height with overflow)
- Shows empty state when no tasks
- Displays task count/progress ("X of Y complete")
- Compact spacing (8px between tasks)

**States:**
- **Loading:** Skeleton loaders for each task card
- **Empty:** Shows EmptyState component
- **With Data:** Renders all task cards with animations on entry
- **Filtered:** Shows subset of tasks based on filter criteria

**Interaction:**
- Infinite scroll or pagination (depends on volume)
- Visual feedback on scroll (sticky count at top)
- Animations on task entry/exit

**Accessibility:**
- List semantic HTML (`<ul>` with `<li>` items)
- `aria-label` for the list
- Keyboard navigation (arrow keys between tasks)

---

#### 3. TaskForm

**Purpose:** Create or edit tasks. Used in onboarding, quick-add, and detailed editing.

**Fields:**
- **Title** (required): Text input, auto-focused, placeholder "What needs to be done?"
- **Description** (optional): Textarea with auto-expand
- **Due Date** (optional): Date picker
- **Status** (optional): Toggle complete/incomplete
- **Tags** (optional): Multi-select tags

**States:**
- **Create Mode:** Empty form with "Create Task" submit button
- **Edit Mode:** Pre-populated with existing data, "Save Changes" button
- **Loading:** Submit button disabled during submission
- **Error:** Validation errors shown inline (red text, field highlight)

**Interaction:**
- Tab order flows naturally: Title → Description → Due Date → Submit
- Cmd+Enter submits form (power user feature)
- Escape closes form (if in modal)
- Auto-save drafts (optional, for collaboration)

**Variants:**
- **Quick-Add:** Minimal (title only, expand for details)
- **Full Form:** All fields visible
- **Inline Edit:** Edit title/description directly in task card

**Accessibility:**
- Label associated with each input
- Required fields marked clearly
- Error messages linked to fields via `aria-describedby`
- Clear focus states

---

#### 4. TaskDetails

**Purpose:** Show complete task information in modal or sidebar. Display title, description, metadata, comments, GitHub link.

**Sections:**
- **Header:** Task title, status toggle, due date
- **Description:** Full task description
- **Metadata:** Due date, tags, GitHub repo (if linked), assigned to
- **Comments:** Full comment thread
- **Actions:** Edit, share, delete, link repository

**States:**
- **Loading:** Skeleton content placeholders
- **View Mode:** Display task info, comments, read-only metadata
- **Edit Mode:** Allow editing title, description, due date

**Interaction:**
- Click "Edit" to enable editing
- Comments have reply functionality
- Share button opens ShareModal
- GitHub link opens dedicated repo view

**Accessibility:**
- Heading hierarchy clear (task title is h2)
- Comments have semantic structure
- Close button always available (X, Escape, click backdrop)

---

#### 5. CommentThread

**Purpose:** Display and allow adding comments to tasks. Shows author, timestamp, comment text, and replies.

**Features:**
- Displays comments in chronological order
- Shows author avatar, name, timestamp
- Support for mentions (@user)
- Optional basic formatting (bold, code blocks)
- Reply functionality (nested comments)
- Edit/delete for own comments

**States:**
- **Display:** Showing existing comments
- **Adding:** Input field visible for new comment
- **Submitting:** Loading state during submission
- **Error:** Error message if submission fails

**Interaction:**
- Click "Reply" to nest response under comment
- @mention opens user picker
- Submit with button or Cmd+Enter
- Edit/delete options in comment menu

**Accessibility:**
- Comments have `article` semantic element
- Author name associated with comment
- Timestamp shown accessibly
- Reply button clearly labeled

---

#### 6. ShareModal

**Purpose:** Generate and share task link. Set permissions, copy link, share to email/Slack.

**Features:**
- Generates unique share link (secure token-based)
- Copy button to clipboard
- Confirmation toast: "Copied to clipboard"
- Permission toggles: Allow comments, allow editing, set expiration
- Share options: Email, Slack (if integrated)

**States:**
- **Initial:** Link generated, copy button ready
- **Copied:** Confirmation message ("Copied!")
- **Configuring:** Permission toggles visible
- **Sharing:** Loading state when sharing to email/Slack

**Interaction:**
- Copy button copies link to clipboard
- Permission toggles update in real-time
- Email/Slack share opens native share dialogs or creates link

**Accessibility:**
- Clear "Copy Link" button label
- Confirmation message announces success
- Permission toggles have labels
- Modal has accessible close button

---

#### 7. GitHubRepo

**Purpose:** Display linked GitHub repository information. Shows repo name, description, stats, and link.

**Content:**
- Repo name and owner
- Description
- Primary language (badge)
- Stats: Stars, Forks, Open Issues
- Link to repo on GitHub
- Option to unlink

**States:**
- **Linked:** Full repo info displayed
- **Linking:** Loading state while linking
- **Error:** Error message if link fails

**Interaction:**
- Click repo name to navigate to GitHub
- Click "View Full Repository" to go to dedicated repo view
- Click unlink button to remove repo link

**Accessibility:**
- Repo name is a link with `target="_blank"`
- Stats have clear labels (not just numbers)
- Unlink button is clearly labeled and confirmable

---

#### 8. EmptyState

**Purpose:** Welcoming, motivating state when task list is empty. Used for new users and after completing all tasks.

**Variants:**
- **New User:** "Your tasks await" with "Create Your First Task" button
- **All Complete:** "Great job!" with encouragement to create more tasks
- **No Results:** "No tasks match your filter" with clear filter option

**Content:**
- Headline message
- Supporting text
- Primary CTA button
- Optional secondary CTA

**Visual:**
- Centered content
- Light background (gray-50)
- Illustration or icon (optional)
- Generous vertical spacing

**Accessibility:**
- Heading clearly states what's happening
- Buttons have clear labels
- No important content hidden in icons

---

#### 9. FilterSearchBar

**Purpose:** Quick filtering and searching tasks. Includes filter buttons and search input.

**Features:**
- Search input: Real-time search across title and description
- Quick filter chips: "Today", "This Week", "Done", "Not Done"
- Advanced filters: Priority, due date, tags (optional)
- Clear filters button

**States:**
- **Default:** Empty search, no filters applied
- **Searching:** Results updating in real-time
- **Filtered:** Active filter chips shown (with X to clear)
- **No Results:** Show empty state

**Interaction:**
- Type in search input (debounced 300ms)
- Click filter chips to toggle
- Click X on chip to remove filter
- Click "Clear All" to reset

**Accessibility:**
- Search input has label/placeholder
- Filter chips are buttons with aria-pressed state
- Results announce via aria-live (for screen readers)

---

#### 10. StatusIndicator

**Purpose:** Visual badge showing task status. Used on task cards and in details.

**Variants:**
- **Overdue:** Warning orange, "Overdue"
- **Today:** Primary blue, "Today"
- **This Week:** Secondary color, "This Week"
- **Complete:** Success green, checkmark icon
- **Priority High:** Red/urgent color

**Visual:**
- Compact badge (8px padding, 12px text)
- Icon + text or icon-only
- Consistent positioning

**Accessibility:**
- Badge has `aria-label` describing status
- Color not the only indicator (icon/text also present)

---

#### 11. UndoToast

**Purpose:** Notification appearing after task completion, allowing undo.

**Content:**
- Message: "Task marked done. Undo?"
- Undo button
- Auto-dismiss after 3 seconds

**States:**
- **Visible:** Toast slides up from bottom
- **Hovered:** Undo button highlights
- **After Undo:** Toast closes, task reverts to pending

**Interaction:**
- Click "Undo" to revert completion
- Toast auto-dismisses after 3 seconds
- Click anywhere else doesn't dismiss (user focused on task)

**Accessibility:**
- Toast announces via `aria-live="polite"`
- Undo button has clear label
- Toast is not intrusive (positioned at bottom)

---

#### 12. UserAvatar

**Purpose:** Display user profile picture or initials. Used in comments, shared views, and assignees.

**Variants:**
- **With Image:** Circular profile picture
- **With Initials:** Circle with user's initials (when no image)
- **Sizes:** sm (24px), md (32px), lg (48px)

**Features:**
- Circular shape (border-radius: 50%)
- Initials fallback (first letter of first and last name)
- Hover tooltip with user name (optional)
- Link to user profile (optional)

**Content:**
- Image: User profile photo
- Fallback: User initials on background color

**Accessibility:**
- Alt text on image: "[User Name]'s avatar"
- If initials shown, aria-label explains initials

---

### Component Implementation Strategy

**Foundation Approach:**
- All components built with Tailwind CSS utilities
- Use design tokens from step 8 (color palette, spacing, typography)
- Consistent state management (React hooks or state library)
- Full keyboard accessibility from the start
- TypeScript for type safety (if applicable)

**Component Library Location:**
- `/components/` directory in NextJS app
- Subdirectories: `/components/tasks/`, `/components/forms/`, `/components/ui/`

**Design Token Usage:**
- Colors reference Tailwind config (e.g., `bg-blue-600`, `text-gray-400`)
- Spacing uses Tailwind scale (e.g., `p-4`, `gap-3`, `mb-8`)
- Typography uses Tailwind classes (e.g., `text-base`, `font-medium`)

**Interaction Animations:**
- Task completion: 200-300ms checkmark animation (SVG or CSS)
- Hover states: Instant (0ms) or subtle 100ms transition
- Modal/toast entrance: 200ms slide-in animation
- Transitions on layout shift: 300ms smooth transition

**State Management:**
- Local component state for UI states (loading, error, focused)
- Global state for: current user, filtered tasks, selected filters
- Server state management via React Query or SWR (if needed)

### Implementation Roadmap

**Phase 1: Core Components (MVP - Essential for All Journeys)**
Priority: Needed immediately to launch redesigned UI

1. **TaskCard** - Central to Jordan's journey (daily task management)
2. **TaskList** - Container for main UI
3. **TaskForm** - Needed for Alex's onboarding and task creation
4. **TaskDetails** - Complete task view
5. **EmptyState** - Welcome new users like Alex
6. **FilterSearchBar** - Support Jordan's filtering needs
7. **UndoToast** - Satisfaction on task completion (core experience)

**Timeline:** 1-2 weeks of development

**Phase 2: Supporting Components (Enable Full Workflows)**
Priority: Needed for collaborators and power users

1. **CommentThread** - Enable Casey's collaboration journey
2. **ShareModal** - Enable task sharing for Casey
3. **GitHubRepo** - Enable Morgan's GitHub integration journey
4. **StatusIndicator** - Enhance task visibility

**Timeline:** 1 week additional development

**Phase 3: Polish & Refinement (Enhancement)**
Priority: Improve overall experience and consistency

1. **UserAvatar** - Display in comments and shared views
2. **Advanced filtering** - Tag-based and priority-based filtering
3. **Keyboard shortcuts** - Spacebar to complete, Cmd+K for command palette
4. **Dark mode variants** - Support light and dark modes

**Timeline:** 1 week refinement

**Total Estimated Timeline:** 3 weeks for complete component library

## UX Consistency Patterns

Consistency patterns ensure users learn interaction patterns once and apply them everywhere. These patterns are the "rules of engagement" for NextJS Todo.

### Button Hierarchy & States

**Primary Buttons** (Main actions: Create task, Submit form, Complete major flow)
- **Appearance:** Background blue-600, white text, 14px medium weight, 12px vertical × 16px horizontal padding
- **States:**
  - Default: `bg-blue-600 text-white`
  - Hover: `bg-blue-700` (slightly darker, indicates clickability)
  - Active/Pressed: `bg-blue-800` (even darker, feedback of press)
  - Disabled: `bg-gray-300 text-gray-500 cursor-not-allowed` (grayed out, clearly disabled)
  - Loading: Spinner appears inside button, text fades, button disables
- **Usage:** "Create Task", "Save", "Submit", "Confirm", "Sign Up"
- **Transitions:** 100ms smooth color transition

**Secondary Buttons** (Alternative actions: Cancel, Reset, Explore)
- **Appearance:** Background transparent, border 2px gray-200, text gray-600, 14px medium
- **States:**
  - Default: `border-gray-300 text-gray-600`
  - Hover: `bg-gray-50 border-gray-400` (subtle background, enhanced border)
  - Active: `bg-gray-100 border-gray-500`
  - Disabled: `border-gray-200 text-gray-300`
- **Usage:** "Cancel", "Clear Filters", "Skip", "View More"
- **Transitions:** 100ms smooth transition

**Danger Buttons** (Destructive actions: Delete task, Clear all)
- **Appearance:** Background red-600, white text, 14px medium
- **States:**
  - Default: `bg-red-600 text-white`
  - Hover: `bg-red-700` (darker, increases perceived danger)
  - Active: `bg-red-800`
  - Disabled: `bg-gray-300 text-gray-500`
- **Usage:** "Delete Task", "Clear All", "Remove"
- **Note:** Danger actions often require confirmation dialog first
- **Transitions:** 100ms smooth color transition

**Icon Buttons** (Compact actions: Edit, Delete, More menu)
- **Appearance:** Square or rounded, icon centered, subtle background
- **States:**
  - Default: `p-2 hover:bg-gray-100 rounded-md` (32×32px touch target)
  - Hover: Light gray background
  - Active: Slightly darker background
- **Usage:** Quick actions on task cards, header navigation
- **Icon Size:** 20×20px, color gray-600

**Button Groups** (Related actions: Filter chips, status toggles)
- **Appearance:** Multiple buttons in row, consistent styling, no gap between
- **Active Chip:** Primary blue background, white text
- **Inactive Chip:** Gray background, gray text
- **Usage:** Filter "Today", "This Week", "Done" | Status toggles
- **Spacing:** No gap (borders touch), or 8px gap depending on design

---

### Feedback Patterns

**Success Pattern** (Task created, saved, deleted successfully)
- **Toast Notification:**
  - Position: Bottom-right corner, 16px from edges
  - Content: "✓ Task created!" (icon + message)
  - Background: `bg-green-50` with `border-l-4 border-green-600`
  - Text: Green-900
  - Duration: Auto-dismiss after 3 seconds
  - Animation: Slide up from bottom (200ms ease-out)
- **Action:** Click to close, or auto-dismiss
- **Accessibility:** `aria-live="polite"` announces to screen readers

**Error Pattern** (Form validation failed, network error, delete failed)
- **Inline Errors (Form):**
  - Position: Below the input field that has error
  - Content: "Email is required" (clear, specific, actionable)
  - Styling: `text-red-600 text-sm mt-1`
  - Field highlight: Red border: `border-red-500` on input
  - Accessibility: `aria-describedby="field-error"` links error to field
- **Toast Errors (Major operations):**
  - Position: Bottom-right, but higher than success (more prominent)
  - Content: "✕ Task could not be saved. Try again?" (icon + message + action)
  - Background: `bg-red-50` with `border-l-4 border-red-600`
  - Action: "Retry" button inside toast
  - Duration: Stays visible until user acts (no auto-dismiss)
  - Animation: Slide up, might have shake animation to grab attention

**Warning Pattern** (Overdue task, unsaved changes, deprecation)
- **Badge on Task:** "Overdue" label in orange
- **Toast Warning:** (for less critical warnings)
  - Position: Bottom-right
  - Content: "⚠ You have overdue tasks"
  - Background: `bg-amber-50` with `border-l-4 border-amber-600`
  - Text: Amber-900
  - Duration: Auto-dismiss after 5 seconds
  - Action: Click to navigate to overdue tasks
- **Visual Indicator:** Warm color (orange/amber), warning icon

**Info Pattern** (Helpful hints, onboarding tips, feature discovery)
- **Inline Help Text:**
  - Position: Below form field
  - Content: "Tasks without due dates appear at the bottom of your list"
  - Styling: `text-gray-500 text-sm mt-2`
- **Help Tooltips:** (On hover)
  - Position: Below element, with small arrow pointing up
  - Content: One-line explanation
  - Styling: Dark background (gray-800), white text, 12px
  - Appearance: Fade in on hover (100ms), fade out on leave
  - Accessibility: Not essential (only supplementary info)

**Task Completion Pattern** (Core experience - satisfying feedback)
- **Checkbox Animation:**
  - Checkbox fills with green: 200ms animation
  - Checkmark draws itself: SVG animation, 150ms
  - Combined effect feels smooth and rewarding
- **Task Row Response:**
  - Text color: gray-600 (muted from gray-900)
  - Strikethrough: fades in (100ms transition)
  - Overall opacity: Stays at 100% (task visible, just muted)
- **Counter Update:**
  - "8 of 12 tasks complete" updates immediately
  - Counter animates +1 briefly
- **Undo Toast:**
  - Appears below task: "Task marked done. Undo?"
  - Auto-dismisses after 3 seconds
  - Click "Undo" to revert immediately with reverse animation

---

### Form Patterns

**Form Layout**
- **Stack:** Vertical stacking, never horizontal (better mobile)
- **Spacing:** 16px between each field
- **Full Width:** Form inputs stretch to 100% of container width
- **Focus State:** 2px blue border on focused input
- **Label:** Above input, 14px medium weight, gray-900, associated via `<label for>`

**Required Field Indicator**
- **Marking:** Red asterisk `*` after label: "Task Title *"
- **Position:** Immediately after label text
- **Alternative:** "(optional)" text for optional fields instead

**Input States**
- **Default:** `border border-gray-300 rounded-md p-3 focus:border-blue-500 focus:ring-2 focus:ring-blue-200`
- **Error:** `border-red-500 bg-red-50` when field has validation error
- **Disabled:** `bg-gray-100 text-gray-500 cursor-not-allowed` when field can't be edited
- **Loading/Processing:** Spinner appears inside input (right side)

**Validation Approach**
- **Live Validation:** Errors appear as user types (debounced 500ms)
- **Clear Error State:** When user fixes error, error message disappears immediately
- **Form Submit:** Only enabled when all required fields have values and no errors
- **Error Summary:** If multiple errors, show brief summary at top of form

**Required vs. Optional**
- **Required Fields:** Marked with `*`, validation blocks form submission
- **Optional Fields:** Marked "(optional)", can be left empty
- **Smart Defaults:** Pre-fill common values (today's date, current user) where relevant

**Button Placement in Forms**
- **Submit Button:** Primary button, aligned left in form or right-aligned (convention varies)
- **Cancel Button:** Secondary button, always next to submit
- **Spacing:** 16px horizontal gap between submit and cancel
- **Disabled Submit:** Disabled if form invalid or submitting

**Textarea Auto-expand**
- **Initial Size:** 3-4 lines visible
- **Expand:** Grows as user types, up to max height (8 lines)
- **Max Height:** Beyond max, scrolls internally
- **Behavior:** Feels responsive and infinite (writing flows naturally)

---

### Navigation Patterns

**Primary Navigation**
- **Location:** Top header, sticky when scrolling
- **Components:** App name/logo (left), task count (center), user menu (right)
- **Actions Available:** Search, add task, filters, user profile, settings
- **Mobile:** Hamburger menu collapses navigation to sidebar on small screens

**Secondary Navigation (Context-specific)**
- **In Task Details:** Breadcrumb "← Back to Tasks" at top, or back button
- **In Shared View:** "← Back to Home" or "← Back to Dashboard"
- **Clear Path Home:** Always possible to return to main task list with one action

**URL/Route Strategy**
- **Main:** `/tasks` - Task list view
- **Detail:** `/tasks/[id]` - Individual task detail
- **GitHub:** `/repos/[id]` - Repository detail view
- **Share:** `/shared/[token]` - Public shared task view (no auth required)
- **Clarity:** URL reflects current location, can be bookmarked/shared

**Filter/View State**
- **URL Params:** Filters persist in URL: `/tasks?filter=today&status=incomplete`
- **Back Button Behavior:** Returns to previous view state (filters, scroll position)
- **Deep Linking:** Sharing a URL with filters loads the same filtered view

**Mobile Navigation**
- **Drawer Menu:** Slides in from left on burger menu click
- **Bottom Actions:** Critical actions (add task) available at bottom on mobile
- **Gestures:** Swipe right to open menu, swipe left to close
- **Touch Targets:** All buttons ≥44px height for easy touch

---

### Confirmation Patterns

**Destructive Actions Require Confirmation** (Delete task, clear all tasks)
- **Pattern:** Don't delete immediately; show modal first
- **Modal Content:**
  - Clear headline: "Delete task?" (not just "Confirm")
  - Reminder of what's happening: "Task 'Finish project' will be deleted permanently"
  - Two buttons: "Delete" (danger red) and "Cancel" (secondary)
  - Optional: Undo after delete for 3 seconds
- **Keyboard:** Escape cancels, Enter deletes (dangerous but power-user feature)
- **Accessibility:** Focus moves to modal, reads full warning

**Irreversible Action Warning**
- **Pattern:** Before performing major action (delete all, clear cache), confirm
- **Modal:** "Are you sure?" with clear consequences
- **Undo Option:** If possible, offer undo for 5-10 seconds after action

**Sharing Confirmation** (optional)
- **Pattern:** After share link generated, "Link copied to clipboard" appears
- **Confirmation:** Toast shows, auto-dismisses after 3 seconds
- **Accessibility:** Toast announces to screen readers

---

### Loading & Empty States

**Loading States**
- **Skeleton Loaders:** While fetching task list, show 3-4 skeleton task cards
  - Pulse animation: opacity 0.5 → 1 → 0.5 every 1.5 seconds
  - Shape matches real content (task card shape with placeholder text)
  - Color: Gray-200 (light gray)
- **Spinner:** For smaller operations (submitting form), show inline spinner
  - Spinner replaces button text, button disables
  - Location: Center of button or input
  - Animation: Rotate 360° every 1 second
- **Progress Indicator:** For longer operations, show progress bar or percentage
  - Position: Top of modal or page
  - Animation: Smooth linear progression

**Empty Task List State**
- **New User:** "Your tasks await" with illustration, primary CTA "Create Your First Task"
- **After Filters:** "No tasks match your filter" with clear button to remove filter
- **All Complete:** "Great job! All tasks done." with CTA "Create a new task"
- **Styling:** Large heading, supporting text, generous vertical spacing, illustration

**Empty Search Results**
- **Content:** "No tasks match 'xyz'" with search term shown
- **Suggestions:** "Try different keywords or clear your search"
- **Visual:** Smaller empty state than full empty list, positioned center of results area

**Error State** (Failed to load tasks)
- **Content:** "We couldn't load your tasks. Try again?" with retry button
- **Visual:** Clear error icon, prominent text
- **Recovery:** Retry button attempts to reload

---

### Modal & Overlay Patterns

**Modal Behavior**
- **Backdrop:** Semi-transparent dark background (opacity 50%), covers entire screen
- **Modal Box:** Centered, with shadow, background white, border-radius 12px
- **Size:** 90% of screen width on mobile, 600px max width on desktop
- **Close:** X button in top-right corner, click backdrop to close, Escape key to close
- **Focus:** Focus moves to modal when opened, returns to trigger on close

**Task Details Modal**
- **Width:** 600px max on desktop, 100vw - 32px on mobile
- **Height:** 80vh max, scroll internally if needed
- **Content:** Sections (title, description, metadata, comments, actions)
- **Scrolling:** Only content scrolls, header stays fixed
- **Interaction:** Click outside to close (non-disruptive)
- **Animation:** Slide in from right on desktop, slide up from bottom on mobile (300ms)

**Confirmation Modal** (Delete, clear, major action)
- **Size:** Smaller, 400px max width
- **Focus:** Danger button gets focus, not cancel (intentional friction)
- **Buttons:** "Delete" (danger) on left, "Cancel" (secondary) on right
- **Spacing:** 16px between buttons
- **No Dismiss on Backdrop:** User must choose action (safety feature)

**Share Modal**
- **Size:** 500px max width
- **Sections:** Link display, copy button, permission toggles
- **Initial Focus:** Copy button (primary action)
- **Dismiss:** Click outside closes without issue (non-destructive)

---

### Search & Filter Patterns

**Search Input**
- **Position:** Header, prominent and always visible
- **Placeholder:** "Search tasks..." (hints at functionality)
- **Icon:** Magnifying glass icon on left side
- **Clear Button:** X icon appears when search has text
- **Behavior:** Real-time results (debounced 300ms), no enter required
- **Keyboard:** Cmd+K opens search (power user shortcut)

**Search Results**
- **Display:** Results update inline in task list
- **Highlighting:** Matching text highlighted in yellow/soft background
- **Empty Results:** Show "No tasks match 'xyz'"
- **Scope:** Searches title and description, not metadata

**Filter Chips** (Quick filters at top of list)
- **Appearance:** Rounded pill-shaped buttons
- **Style:**
  - Inactive: `bg-gray-100 text-gray-700` with hover `bg-gray-200`
  - Active: `bg-blue-600 text-white` with hover `bg-blue-700`
- **Chips:** "Today", "This Week", "Done", "Not Done", or other categories
- **Behavior:** Clicking toggles active state, filters list immediately
- **Multiple:** Can combine filters (e.g., "Today" + "Not Done")
- **Clear:** "Clear All Filters" button appears when filters active

**Advanced Filters** (Optional: Priority, tags, assigned to)
- **Location:** Behind "Filters" button or collapsed section
- **Options:** Checkboxes for each filter type
- **Behavior:** Each selection narrows results
- **Persistence:** Filter state saved in URL, survives navigation

**Filter Interaction**
- **Immediate:** Results filter instantly on chip click (no submit button)
- **Visual Feedback:** Active chips highlighted, task count updates
- **Clarity:** Always show which filters are active (via highlighted chips)
- **Recovery:** Clear filter button always visible to reset

---

### Accessibility Patterns (Applied Across All Above)

**Keyboard Navigation**
- **Tab Order:** Logical flow (top to bottom, left to right)
- **Focus Visible:** Clear blue ring (`outline outline-2 outline-blue-500`) on focused elements
- **Shortcuts:** Common actions have keyboard shortcuts (space to complete, cmd+k for search)
- **Menus:** Arrow keys navigate, Enter to select, Escape to close

**Screen Reader Support**
- **Semantic HTML:** Use `<button>`, `<input>`, `<label>`, `<nav>` not divs
- **ARIA Labels:** Every interactive element has accessible name
- **Live Regions:** Task completion count updates announced via `aria-live="polite"`
- **Form Errors:** Errors linked to fields via `aria-describedby`

**Color Contrast**
- **Text:** All text meets 4.5:1 contrast ratio (WCAG AA)
- **UI Components:** 3:1 contrast on component borders and icons
- **Not Color Alone:** Status never indicated by color alone (also use icons, text)

**Mobile & Touch**
- **Touch Targets:** All buttons/clickables ≥44px (WCAG AAA)
- **Spacing:** 8px minimum gap between touch targets
- **Gestures:** Swipe, tap, double-tap all work intuitively

---

### Summary: Consistency Rules

1. **Every interaction has consistent styling** (primary buttons always blue, always same padding)
2. **Feedback is always immediate** (task completion animates, form errors appear, success toasts show)
3. **Navigation is always clear** (breadcrumbs, back buttons, URL reflects state)
4. **Errors are recoverable** (retry buttons, undo, clear error messages)
5. **Accessibility is built-in** (keyboard nav, screen readers, contrast from day one)
6. **Mobile works as well as desktop** (touch targets, responsive layouts, gesture support)

## Responsive Design & Accessibility Strategy

### Responsive Design Strategy

NextJS Todo is **web-first** but fully responsive across all device sizes. Design adapts gracefully while maintaining visual consistency and interaction patterns.

#### Desktop Strategy (1024px and above)

**Layout Approach:**
- Full-width task list with comfortable spacing (24px margins)
- Optional: Side-by-side layout (task list + detail panel)
- Navigation: Full header with all actions visible (search, filters, add task, user menu)
- Horizontal space used for information density (task cards wider, more metadata visible)

**Features Available:**
- Hover states fully functional (task cards show action hints)
- Keyboard shortcuts and power-user features (Cmd+K for search, Space to complete)
- Advanced filters visible (by default or in discoverable menu)
- Multiple columns/panels visible simultaneously

**Visual Density:**
- Comfortable padding: 24px left/right margins, 16px between items
- Easy to scan: Generous line heights, clear visual hierarchy
- Not cramped: Whitespace used effectively to reduce cognitive load

#### Tablet Strategy (768px - 1023px)

**Layout Approach:**
- Single-column layout (task list full width)
- Navigation adapts: Hamburger menu if header too crowded, or collapsible sections
- Task cards touch-optimized (larger buttons, more padding)
- Modals scale appropriately (90% of screen width, max 600px)

**Touch Optimization:**
- Interactive elements: Minimum 44px height (WCAG AAA standard)
- Spacing between buttons: At least 8px gap (prevents accidental touches)
- Hover states replaced with active/pressed states
- Swipe gestures: Swipe right for navigation menu, swipe left to close

**Features Available:**
- All core features work (task creation, completion, sharing, filtering)
- Modals work smoothly (full-height or large overlay)
- Touch-friendly navigation (larger tap targets, clear visual feedback)
- Gestures supported (swipe to navigate, pinch to zoom not needed)

#### Mobile Strategy (320px - 767px)

**Layout Approach:**
- Mobile-first, single-column layouts
- Navigation: Hamburger menu with slide-out drawer (left side)
- Bottom navigation bar for critical actions (optional alternative to top menu)
- Task cards simplified but still scannable (essential info only)
- Full-width modals (or nearly full-width with small margins)

**Touch Optimization:**
- All buttons minimum 44px height and width
- Minimum 8px spacing between all touch targets
- Checkboxes: 24px size (not 20px like desktop), plenty of padding
- Button text clear and large (14px or larger)
- Form inputs: Full width, tall (48px minimum)

**Simplified Features:**
- Modals stack full-screen (not floating in center)
- Forms: One conceptual section at a time (task creation, comment, share)
- Search/filter: Slide-out panels or full-screen overlays (not dropdown menus)
- Navigation hidden by default (reveal via hamburger)

**Orientation Support:**
- Portrait (320px - 600px): Optimal mobile layout
- Landscape (600px - 1023px): Tablet-like layout or mobile stretched
- No horizontal scrolling required (except within scrollable content)

#### Responsive Breakpoints & Media Queries

**Tailwind Breakpoints:**
- `sm`: 640px (small phones landscape, small tablets)
- `md`: 768px (tablets, transition point)
- `lg`: 1024px (desktops, large tablets)
- `xl`: 1280px (large desktops, wide screens)

**Mobile-First Development:**
- Base styles for mobile (320px)
- `sm:` for enhanced mobile (640px)
- `md:` for tablets (768px)
- `lg:` for desktops (1024px)
- `xl:` for large desktops (1280px+)

**Critical Breakpoints:**
- **768px (md):** Shift from hamburger to full navigation
- **1024px (lg):** Expand margins, consider side-by-side layouts
- **1280px (xl):** Consider three-column layouts or expanded content

#### Responsive Layout Examples

**Task List:**
- Mobile: Full-width task cards, no margins (safe area considered)
- Tablet: 90% width with centered margins
- Desktop: 1000px max width, full margins 24px

**Task Details Modal:**
- Mobile: Full-screen (100vh, 100vw with small padding)
- Tablet: 90vw width, 80vh height, centered
- Desktop: 600px width, 80vh height, centered

**Forms:**
- Mobile: Full-width form fields, 48px minimum height
- Tablet: 90% width, 40px minimum height
- Desktop: 400px width (enough for 2-column if needed)

#### Performance Optimization

**Image & Asset Optimization:**
- Responsive images: `srcset` for different screen sizes
- Lazy loading: Images load on-demand
- Format optimization: WEBP with fallbacks
- Asset delivery: CDN-optimized for different regions

**Mobile Performance:**
- Minimal JavaScript on mobile (code splitting)
- Service worker for offline support (future enhancement)
- Efficient network requests (batching, caching)
- Fast Time to Interactive (< 3 seconds on 4G)

---

### Accessibility Strategy

**Accessibility Level: WCAG 2.1 AA (Industry Standard)**

This level ensures:
- Accessible to users with various disabilities
- Legal compliance in most jurisdictions
- Industry best practices for professional applications
- Balance between accessibility and feature richness

#### Color & Contrast

**Text Contrast Requirements:**
- **Normal text:** 4.5:1 ratio (black text on white = 21:1 ✓)
- **Large text (18pt+):** 3:1 ratio minimum
- **UI Components (buttons, borders):** 3:1 ratio minimum

**Color Palette Compliance:**
- Primary Blue (#2563eb) on white: ~8.5:1 ✓ (well above 4.5:1)
- Gray-600 text on white: ~7:1 ✓ (well above 4.5:1)
- Gray-400 on white: ~4.5:1 (meets minimum)
- Overdue/warning colors (orange #f59e0b) always paired with text or icon

**Non-Color-Dependent Communication:**
- Status never indicated by color alone
- Task completion uses: checkmark icon + color change + strikethrough
- Warnings use: icon + color + text
- Errors use: icon + border + text (not just red)

**Dark Mode Consideration:**
- Same contrast ratios maintained
- Colors inverted appropriately
- No images that rely on specific background color

#### Keyboard Navigation & Focus Management

**Keyboard Support:**
- All interactive elements (buttons, inputs, links) accessible via Tab key
- Tab order logical (top to bottom, left to right)
- Tab wraps from last element to first
- Escape closes modals, menus, dropdowns
- Enter/Space activates buttons and checkboxes
- Arrow keys navigate menus and lists

**Power User Keyboard Shortcuts:**
- **Space:** Mark task complete/incomplete (when focused)
- **Cmd/Ctrl+K:** Open search
- **Cmd/Ctrl+Enter:** Submit form (from any field)
- **Escape:** Close modal/menu, cancel operation
- **?:** Show keyboard shortcut help modal
- **Arrow Keys:** Navigate between tasks in list

**Focus Indicators:**
- Visible focus ring: 2px blue outline (`outline outline-2 outline-blue-500`)
- No removal of default focus styles
- Custom focus styles never disappear
- Focus ring visible on all elements (not just obvious ones like buttons)
- High contrast focus indicators (blue on white is 8.5:1)

**Skip Links:**
- "Skip to main content" link (hidden, visible on focus)
- Location: First focusable element in page
- Functionality: Jump past navigation directly to task list

#### Screen Reader Support

**Semantic HTML:**
- Use `<button>` for buttons (not divs with click handlers)
- Use `<input>` for form inputs (not custom controls)
- Use `<label>` associated with inputs
- Use `<nav>` for navigation
- Use `<main>` for main content
- Use `<article>` for tasks (semantic grouping)
- Use `<h1>`, `<h2>`, etc. for headings (proper hierarchy)

**ARIA Labels & Roles:**
- Every button has accessible name (label or aria-label)
- Form inputs have associated labels
- Icons use `aria-label` (e.g., "Delete task")
- Modals use `role="dialog"` with `aria-labelledby`
- Tabs use `role="tablist"`, `role="tab"`, `role="tabpanel"`
- Live regions use `aria-live="polite"` for updates

**Content Announcements:**
- Task completion count updates announced: "8 of 12 tasks complete"
- Form errors announced when appearing
- Toast notifications announced via `aria-live`
- Loading states communicated (not just visual)

**Navigation Structure:**
- Logical heading hierarchy (no skipped levels)
- Page title distinct (e.g., "Your Tasks - NextJS Todo")
- Breadcrumbs help orientation
- List landmarks used for task lists

#### Touch & Mobile Accessibility

**Touch Target Sizes:**
- Minimum 44×44px (WCAG AAA standard)
- Buttons: 44px height × 48px width preferred
- Checkboxes: 24×24px with padding (8px around = 40px total touch area)
- Form inputs: 48px height minimum
- Links: 44px minimum in interactive areas

**Spacing Between Targets:**
- 8px minimum gap between all touch targets
- Prevents accidental adjacent taps
- Especially important for delete buttons (don't place next to save)

**Mobile Form Considerations:**
- Large tap targets (48px for mobile, 40px for tablet)
- Clear labels (no tiny placeholder-only labels)
- Autocomplete enabled (name, email, etc.)
- Numeric keyboard for number inputs
- Date picker for date fields (not typing)

**Orientation & Responsive:**
- Works in both portrait and landscape
- Content reflows (not zoomed/scaled)
- Essential features available in both orientations
- Gestures have keyboard alternatives

#### Motion & Animation Accessibility

**Animation Principles:**
- Animations serve a purpose (not purely decorative)
- Animations are brief (< 500ms preferred, < 2s maximum)
- No flashing or blinking (could trigger photosensitive epilepsy)
- Animations respect `prefers-reduced-motion` setting

**CSS Support:**
```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
  }
}
```

**Animations to Include:**
- Task completion checkmark: Smooth 200ms draw (meaningful)
- Task row fade: 100ms opacity change (meaningful)
- Modal entrance: 200ms slide (indicates appearance)

**Animations to Avoid:**
- Purely decorative movements
- Auto-playing videos
- Parallax scrolling (disorienting)
- Constant blinking/pulsing elements

#### Form & Input Accessibility

**Form Structure:**
- Every input has associated `<label>`
- Labels not hidden or removed via CSS
- Required fields marked: `*` symbol + `aria-required="true"`
- Instructions clear and near inputs

**Input Validation:**
- Error messages linked via `aria-describedby`
- Errors appear near the field (not at top of form)
- Errors announced to screen readers automatically
- Clear error messages (not codes): "Please enter a valid email"
- Positive feedback also communicated ("Email looks good!")

**Input Types:**
- Email inputs: `type="email"` (enables email keyboards)
- Date inputs: `type="date"` (enables date pickers)
- Number inputs: `type="number"` (not text)
- Autocomplete attributes: `autocomplete="name"`, `autocomplete="email"`
- Passwords: `type="password"` (not visible by default)

#### Color Blindness & Vision Considerations

**Testing for Color Blindness:**
- Deuteranopia (red-green, 1% of population)
- Protanopia (red-green, 1% of population)
- Tritanopia (blue-yellow, 0.1% of population)
- Achromatopsia (complete color blindness, rare)

**Design Implications:**
- Never use red/green alone to indicate status (use icons too)
- Test with color blindness simulators (Coblis, Vischeck)
- Contrast maintained for all color combinations
- Icons always accompany color coding

**Overdue Task Example:**
- Color: Orange (#f59e0b) on white (5.5:1 contrast ✓)
- Icon: Warning/alert icon (visible indication)
- Text: "Overdue" label (textual indication)
- Result: Three cues, not just color

#### Testing Strategy

**Automated Testing:**
- axe DevTools (browser extension): Accessibility scanning
- Lighthouse (Chrome DevTools): Accessibility audit
- WAVE (WebAIM): Browser-based accessibility evaluation
- Color contrast checkers (WebAIM, Contrast Ratio)

**Manual Testing:**
- Keyboard-only navigation (don't use mouse)
- Screen reader testing:
  - NVDA (Windows, free)
  - JAWS (Windows, commercial)
  - VoiceOver (Mac/iOS, built-in)
  - TalkBack (Android, built-in)
- Color blindness simulation (Coblis)
- Mobile/touch testing on real devices

**User Testing:**
- Include testers with disabilities
- Test with assistive technology users
- Validate with diverse devices/browsers
- Collect feedback on accessibility features

**Continuous Testing:**
- Accessibility checks in CI/CD pipeline
- Accessibility regression tests (automatic)
- Manual testing before each release
- User feedback loop (accessibility issues reported, fixed)

#### Implementation Checklist

**Before Launch:**
- [ ] All text meets 4.5:1 contrast ratio
- [ ] All buttons/inputs have keyboard access
- [ ] All images have alt text (if meaningful)
- [ ] Form inputs have labels
- [ ] Focus indicators visible on all interactive elements
- [ ] Keyboard shortcuts documented
- [ ] Modal focus management implemented
- [ ] Color blindness testing completed
- [ ] Screen reader testing (at least one) completed
- [ ] Mobile touch targets tested (44px minimum)
- [ ] Motion/animation respects prefers-reduced-motion
- [ ] Heading hierarchy logical (no skipped levels)
- [ ] Page title is descriptive
- [ ] Links are descriptive ("Learn more" ❌ vs "Learn more about GitHub integration" ✓)

**Post-Launch (Continuous):**
- [ ] Monitor accessibility issues in user feedback
- [ ] Regular accessibility audits (monthly)
- [ ] Update with new WCAG standards as they emerge
- [ ] Maintain accessibility documentation for team
- [ ] Train new developers on accessibility practices

---

### Summary: Inclusive by Design

NextJS Todo is designed from the start to be:
- **Responsive:** Works beautifully on phones, tablets, and desktops
- **Accessible:** WCAG 2.1 AA compliant, usable by everyone
- **Performant:** Fast on mobile networks and older devices
- **Keyboard-friendly:** Power users can navigate entirely via keyboard
- **Screen-reader compatible:** Blind and low-vision users can use the app
- **Touch-optimized:** Mobile and tablet users have comfortable experience
- **Motion-conscious:** Respects user preferences for reduced motion
- **Color-independent:** Information not conveyed by color alone
