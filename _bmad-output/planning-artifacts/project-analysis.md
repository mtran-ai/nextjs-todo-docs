# Project Analysis: NextJS Todo

## Project Overview

**Yet Another ToDo** is an open-source task management web application built with Next.js 14. It's a brownfield project with a functional todo application that supports collaborative features.

**Live Demo:** https://nextjs-14-todo.vercel.app/

## Current Technology Stack

**Frontend:**
- Next.js 14 (App Router, Server Actions)
- React 18
- TypeScript
- Tailwind CSS + shadcn-ui
- react-hook-form + Zod validation
- next-themes (dark mode support)

**Backend:**
- Next.js Route Handlers & Server Actions
- Prisma ORM
- next-safe-action (type-safe action wrapper)
- bcrypt (password hashing)

**Database:**
- PostgreSQL (Neon.tech)
- Prisma migrations

**Testing:**
- Vitest (unit/integration)
- Playwright (E2E)

**Deployment:**
- Vercel

## Core Data Model

### Users
- Username/password authentication
- One-to-many relationship with Tasks
- One-to-many relationship with Comments

### Tasks
- Title, description, due date
- Done/completion status
- Ownership by author
- Related comments
- Optional GitHub repo link

### Comments
- Text content
- Author (User) reference
- Task reference (cascade delete)

### GitHub Repos
- Linked to tasks (one-to-one)
- Stores: owner, repo name, full name
- Cascade delete when task deleted

## Implemented Features

✅ **Authentication & Authorization**
- Sign-up / Sign-in with username & password
- Session management with next-auth v5

✅ **Task Management**
- Create, read, update, delete tasks
- Mark tasks as done/incomplete
- Filter tasks by name & description
- Share tasks via URL (public view)

✅ **Comments**
- Add comments to tasks
- Comment metadata (creator, timestamp)

✅ **GitHub Integration**
- Link public GitHub repos to tasks
- Display repo metadata
- Dedicated route for repo information

## Project Structure

```
src/
├── app/
│   ├── (auth)/          # Auth pages
│   ├── [username]/      # User task views
│   └── api/             # API routes
├── components/          # React components
├── lib/                 # Utilities & database
└── prisma/              # Schema & migrations
```

## Infrastructure & DevOps

- Environment variables via dotenvx
- Automated test setup with Prisma
- E2E test database separate from dev

## Current Quality & Testing

- Unit tests with Vitest
- E2E tests with Playwright
- TypeScript strict mode
- ESLint + Prettier configuration
