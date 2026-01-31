# SaaSPulse

> The heartbeat of your development workflow.

SaaSPulse is a simplified, full-stack issue tracker designed for indie hackers and developers managing multiple SaaS projects. It provides a unified dashboard to track bugs, features, and tasks without the complexity of enterprise tools.

## Tech Stack

- **Framework:** Next.js 14+ (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **Database:** SQLite (via Prisma ORM)
- **Architecture:** Server Components & Server Actions

## Features

- **Multi-Project Support:** Organize work by specific SaaS product.
- **Issue Tracking:** Create, update, and delete issues with ease.
- **Priority System:** Tag issues as Low, Medium, High, or Critical.
- **Pulse Dashboard:** Get an at-a-glance view of your total workload.
- **Responsive Design:** Manage your projects from desktop or mobile.

## Getting Started

1. **Clone the repository**
   ```bash
   git clone <repo-url>
   cd saaspulse
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Setup Database**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open the app**
   Visit `http://localhost:3000` in your browser.

## Documentation

- [TASKLIST.md](./TASKLIST.md) - Detailed breakdown of development tasks.
- [LEARNINGS.md](./LEARNINGS.md) - Context and knowledge base for the AI agent.
- [.dev0/RULES.md](./.dev0/RULES.md) - Project-specific rules and guidelines.