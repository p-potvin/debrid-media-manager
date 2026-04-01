# Agent Manifest — Debrid Media Manager (VaultWares Fork)

## Project Overview
A VaultWares fork of [debridmediamanager/debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager).
Next.js 15 (Pages Router) · TypeScript (strict) · Tailwind CSS · Prisma · React 19

## Key Commands
```bash
npm install              # Install dependencies
npm run dev              # Start development server (http://localhost:3000)
npm run build            # Production build
npm start                # Start production server
npm run lint             # ESLint
npm run typecheck        # tsc --noEmit
npm test                 # Vitest (all tests)
npm run test:unit        # Unit tests only
npm run test:integration # Integration tests only
```

## Folder Structure
```
src/
  components/   — React components (PascalCase filenames)
  contexts/     — React context providers
  hooks/        — Custom hooks (camelCase, prefix: use)
  lib/          — Shared utilities and Zod schemas
  pages/        — Next.js pages and API routes
  scrapers/     — Torrent/metadata scrapers
  services/     — External API service clients
  styles/       — Global CSS / Tailwind config
  torrent/      — Torrent parsing utilities
  types/        — Global TypeScript interfaces
  utils/        — Pure utility functions (kebab-case filenames)
```

## VaultWares Standards Applied Here
- **Indentation:** 4 spaces (no tabs)
- **Naming:** PascalCase components, camelCase hooks (`useXxx`), kebab-case utils
- **Types:** No `any`; use Zod for API/form validation
- **Logging:** Include `correlationId` (7 alphanumeric chars, starts with lowercase `c`) in all log lines
- **Error handling:** Centralised error-boundary + react-hot-toast (no bare `console.log`)
- **Theming:** Tailwind dark mode + Solarized-inspired palette; Glass UI components in moderation

## Environment Setup
Copy `.env.example` to `.env.local` and fill in required values before running.
