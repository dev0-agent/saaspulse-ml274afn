# Task List

This file shows the current progress of all tasks in this project.
It is automatically updated by dev0 as tasks are completed.

---

## Phase 1

- [ ] ⏳ **Project Initialization & Configuration**
  Initialize a new Next.js app with TypeScript and Tailwind CSS. Configure ESLint and Prettier. Set up the folder structure for the App Router, including `components`, `lib`, and `types` directories.

- [ ] ⏳ **Database Schema & Prisma Setup**
  Install Prisma. Define the schema with models for `Project` (id, name, description, slug) and `Issue` (id, title, description, status, priority, projectId). Run the initial migration to create the local SQLite database.

- [ ] ⏳ **Global Layout & Navigation**
  Create the root layout component. Implement a responsive sidebar navigation that links to Dashboard, Projects, and Settings. Include a placeholder header. Ensure the layout is persistent across routes.

## Phase 2

- [ ] ⏳ **Project Management Server Actions**
  Create Server Actions for Projects: `createProject`, `getProjects`, `updateProject`, and `deleteProject`. Ensure proper error handling and revalidation of paths using `revalidatePath`.

- [ ] ⏳ **Projects List UI**
  Build the `/projects` page. Fetch the list of projects using RSC. Display them in a grid of cards showing the name and a brief description. Add a 'New Project' button that invokes the creation Server Action via a simple form or modal.

- [ ] ⏳ **Issue Management Server Actions**
  Create Server Actions for Issues: `createIssue`, `updateIssueStatus`, `deleteIssue`. These actions must accept a `projectId` to link the issue correctly.

- [ ] ⏳ **Project Detail & Issue List View**
  Create the dynamic route `/projects/[id]`. Display project details at the top. Below, list all issues associated with this project. Implement a table or list view showing Title, Status, and Priority.

- [ ] ⏳ **Issue Creation Component**
  Build a reusable `CreateIssueForm` component. It should include fields for Title, Description, Priority (select), and Status (default to Backlog). Integrate this into the Project Detail page.

## Phase 3

- [ ] ⏳ **Dashboard Aggregation Logic**
  Implement logic to calculate dashboard stats: Total Projects, Total Open Issues, and High Priority Issues count. This should be a utility function or a dedicated data-fetching component.

- [ ] ⏳ **Main Dashboard UI**
  Build the home page `/`. Display the aggregated stats cards created in the previous task. Add a 'Recent Activity' section listing the 5 most recently created or updated issues.

- [ ] ⏳ **Issue Filtering and Sorting**
  Add client-side or server-side filtering to the Project Detail issue list. Allow users to filter by Status (e.g., show only 'In Progress') and sort by Priority.

## Phase 4

- [ ] ⏳ **UI Polish & Status Badges**
  Create color-coded badges for Status (e.g., Green for Done, Yellow for In Progress) and Priority (Red for Critical). Apply these badges across the Dashboard and Project views. Improve empty states.

- [ ] ⏳ **Loading States & Error Handling**
  Implement `loading.tsx` and `error.tsx` for the App Router to handle data fetching states gracefully. Add skeleton loaders for the dashboard and project lists.

## Phase 5

- [ ] ⏳ **Final Testing & Documentation**
  Perform a manual walkthrough of all flows (Create Project -> Add Issue -> Complete Issue). Fix any layout bugs. Ensure the README is up to date with setup instructions.

---

_Last updated by dev0 automation_
