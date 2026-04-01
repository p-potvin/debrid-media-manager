# Roadmap

## Phase 1 — Foundation (Current)
- [ ] Import upstream debrid-media-manager codebase
- [ ] Apply VaultWares code standards (strict TypeScript, 4-space indentation, Zod validation)
- [ ] Set up CI/CD pipeline with Google Cloud Build
- [ ] Configure Docker / Cloud Run deployment

## Phase 2 — VaultWares UI
- [ ] Integrate VaultWares Glass UI library
- [ ] Implement light/dark theme with Solarized-inspired colour palette
- [ ] Responsive layout improvements
- [ ] Animated transitions (performance-aware)

## Phase 3 — Privacy & Observability
- [ ] Add CorrelationId tracing to all API routes and log lines
- [ ] Centralised error-boundary with user-friendly Toast feedback
- [ ] Enhanced audit logging for user actions
- [ ] Row-Level Security review for all database queries

## Phase 4 — Extended Integrations
- [ ] Google Cloud SQL (CloudSQL) support alongside existing MySQL
- [ ] TanStack Query for client-side data fetching
- [ ] Zustand for local state management
- [ ] Trakt and metadata API improvements

## Backlog
- Multi-skin support (9 premade VaultWares skins)
- Stremio addon VaultWares branding
- Windows native client (WinUI 3)
