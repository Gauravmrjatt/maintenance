# Maintenance

A Next.js app with Docker and a CI workflow already wired up. The plumbing works, the application logic is still to come.

## What it does

- Next.js App Router with a root layout and a landing page
- GitHub Actions workflow on every push
- Dockerfile for a container build

About 185 lines across 7 files.

## Stack

Next.js, React, Tailwind CSS, Docker.

## Layout

```
src/app/
  layout.js     root layout
  page.js       landing page
.github/workflows/main.yml
Dockerfile
```

## Run it

```bash
npm install
npm run dev        # http://localhost:3000
```

## Scripts

| Command | What it does |
|---|---|
| `npm run dev` | Dev server with Turbopack |
| `npm run build` | Production build |
| `npm start` | Serve the build |
| `npm run lint` | ESLint |

## Docker

```bash
docker build -t maintenance .
docker run -p 3000:3000 maintenance
```

## Status

Scaffold. Routing, Docker and CI are in place. No forms, no database, no requests yet.
