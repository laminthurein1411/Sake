# Sake

Sake is a small personal reading stack built around a Svelte web app and a KOReader plugin.

The idea is simple: keep your library in one place, sync reading progress between devices, and make the KOReader workflow less annoying.

## What is in this repo?

- `sake/` - the main web app and API (`Svelte 5` + `SvelteKit`)
- `koreaderPlugins/` - the KOReader plugins used by Sake

## Features

- Personal reading hub for managing books, metadata, shelves, ratings, and reading state
- KOReader integration for syncing books, progress, and plugin updates across devices
- Provider-based search with direct download or import into your library
- Local account auth plus device API keys for secure browser and device access
- Self-hostable stack with libSQL and S3-compatible storage
- Built to keep your library, progress, and KOReader workflow in one place

## Notes

- Database migrations live in `sake/` and are managed with Drizzle.
- KOReader plugin releases are served by the `sake` app, while plugin artifacts are stored in S3-compatible object storage.
- API route lookup is available in the app at `/api/_routes` and `/api/docs`.
- A self-host reference stack is available at `docker-compose.selfhost.yaml`.

## License

This repository is licensed under `AGPL-3.0-only`.
See `LICENSE` for the full text.
