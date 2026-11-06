# Next.js Dashboard

My work-in-progress build of the invoice dashboard from the official [Next.js App Router course](https://nextjs.org/learn). The app, "Acme", is a fictional example from the course.

## Project status

**Done:**

- Dashboard overview with summary cards, a revenue chart, and the latest invoices
- Streaming with React Suspense and loading skeletons
- Invoice list with search and pagination through URL parameters
- Database seed and test query routes

**Not finished yet:**

- Creating, editing, and deleting invoices (the form and buttons exist, but they aren't connected)
- Login (the home page links to `/login`, which doesn't exist yet)
- The customers page, which is still a placeholder

## Tech stack

- Next.js (App Router) and React
- TypeScript
- Tailwind CSS
- PostgreSQL, using the `postgres` client

## Getting started

You need Node.js, pnpm, and a PostgreSQL database that accepts SSL connections.

1. Install the dependencies:

   ```bash
   pnpm install
   ```

2. Create a `.env` file with your connection string:

   ```bash
   POSTGRES_URL=postgresql://user:password@host:5432/database
   ```

3. Start the development server:

   ```bash
   pnpm dev
   ```

4. Open <http://localhost:3000/seed> once to create the tables and load the sample data.

5. Open <http://localhost:3000/dashboard>.

## Scripts

| Command | Description |
|---|---|
| `pnpm dev` | Start the development server with Turbopack |
| `pnpm build` | Create a production build |
| `pnpm start` | Serve the production build |
