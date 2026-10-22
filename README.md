# Maintenance

A Next.js application scaffold with Docker and a GitHub Actions workflow wired up.

## Stack

Next.js (App Router) · React · Tailwind CSS · Docker

## Structure

```
src/app/
  layout.js     root layout
  page.js       landing page
.github/workflows/main.yml   CI pipeline
Dockerfile
```

## Getting started

```bash
npm install
npm run dev        # http://localhost:3000
```

## Scripts

| Command | Description |
|---|---|
| `npm run dev` | Dev server with Turbopack |
| `npm run build` | Production build |
| `npm start` | Serve the production build |
| `npm run lint` | ESLint |

## Docker

```bash
docker build -t maintenance .
docker run -p 3000:3000 maintenance
```

## Status

Early scaffold — routing, Docker and CI are in place, but the application logic is still to be built.
