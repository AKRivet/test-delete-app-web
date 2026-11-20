# test implementation-123

A React web application scaffolded with Vite, TypeScript, ESLint, and Prettier.

## Tech Stack

| Tool | Version | Purpose |
|------|---------|---------|
| React | 19.3.1 | UI framework |
| TypeScript | 6.0.3 | Type safety |
| Vite | 8.3.8 | Dev server & bundler |
| ESLint | 10.15.0 | Linting (flat config) |
| Prettier | 3.10.1 | Code formatting |

> **Note on TypeScript version:** TypeScript 7.0.2 is the current stable release, but
> `@typescript-eslint@8.73` only supports TypeScript `<6.1.0`. This project uses TypeScript 6.0.3
> (the latest compatible version) until a new `@typescript-eslint` release adds TypeScript 7 support.

## Project Structure

```
.
├── public/            # Static assets served as-is
├── src/
│   ├── assets/        # Images, fonts, etc. (imported by source)
│   ├── components/    # Reusable React components
│   ├── App.tsx        # Root component
│   ├── index.css      # Global styles (CSS reset + design tokens)
│   ├── main.tsx       # React entry point
│   └── vite-env.d.ts  # Vite client type declarations
├── eslint.config.js   # ESLint flat config
├── prettier.config.js # Prettier config
├── tsconfig.json      # TypeScript project references root
├── tsconfig.app.json  # TypeScript config for src/
├── tsconfig.node.json # TypeScript config for vite.config.ts
└── vite.config.ts     # Vite configuration
```

## Getting Started

```bash
# Install dependencies
npm install

# Start development server (http://localhost:5173)
npm run dev

# Production build (output: dist/)
npm run build

# Preview production build locally
npm run preview
```

## Code Quality

```bash
# Lint source files
npm run lint

# Auto-fix lint issues
npm run lint:fix

# Format all files with Prettier
npm run format

# Check formatting without writing
npm run format:check
```

## Security Audit

Run `npm audit` at any time to check for known vulnerabilities.

**Audit result at scaffold time (2026-11-20):** 0 vulnerabilities found across 164 packages.
