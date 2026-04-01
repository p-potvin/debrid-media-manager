# Debrid Media Manager — VaultWares Fork

A VaultWares-enhanced fork of [debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager) with additional features tailored for self-hosted media server deployments.

## What is this?

This fork builds on the original Debrid Media Manager — a free, open source web app that makes it easy to download movies and TV shows directly to your Debrid library (Real-Debrid, AllDebrid, TorBox) — and adds VaultWares-specific improvements for privacy-first media hosting.

## Additional Features (VaultWares Fork)

- VaultWares Glass UI styling with light/dark theme support
- Enhanced privacy controls and audit logging with CorrelationId tracing
- Google Cloud Run / Cloud SQL deployment support
- Improved type safety (strict TypeScript, Zod validation)

## Prerequisites

- Node.js 20+
- MySQL / PostgreSQL database (CloudSQL recommended)
- A Debrid account: [Real-Debrid](https://real-debrid.com), [AllDebrid](https://alldebrid.com), or [TorBox](https://torbox.app)

## Setup

1. Clone this repository
2. Copy the environment template: `cp .env.example .env.local` and fill in the required values
3. Install dependencies: `npm install`
4. Run in development mode: `npm run dev`
5. Or build and start in production: `npm run build && npm start`

## Docker

```bash
cp .env.example .env.local
# Fill in your settings in .env.local
docker swarm init
docker stack deploy -c docker-compose.yml dmm
```

The app will be accessible at `http://localhost:3000`.

## Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start dev server |
| `npm run build` | Build for production |
| `npm start` | Start production server |
| `npm run lint` | Lint source files |
| `npm run typecheck` | Type-check TypeScript |
| `npm test` | Run all tests |

## Upstream

This project is a fork of [debridmediamanager/debrid-media-manager](https://github.com/debridmediamanager/debrid-media-manager).
See the upstream repository for the full feature list.

## License

This project is licensed under the [AGPL-3.0](LICENSE).
