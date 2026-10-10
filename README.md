# Sri Lankan AI — NENAPIYUMA

A project bundle containing a React/Vite interface and the `NENAPIYUMA-AI-USB` Python desktop application prototype for local AI chat and USB security utilities.

## Project contents

- `src/` — React + TypeScript UI (chat playground, USB guard sandbox, repository explorer, package exporter, hardware calculator).
- `NENAPIYUMA-AI-USB/` — Python/PySide6 desktop app, model registry and inference engine, local storage, security scanner, quarantine/integrity modules, build scripts, tests, and Windows build workflow.

## Important status notes

- This source bundle does **not** include a verified, usable GGUF model. The placeholder model files were excluded from the public-ready archive; see `NENAPIYUMA-AI-USB/models/README.txt`.
- The Windows executable has not been built or verified in this repository.
- Treat this as source code that still needs dependency installation, tests, and a Windows build—not as a ready-to-run release.

## Web UI

Requirements: Node.js. Run `npm install`, then `npm run dev`. Build with `npm run build`.

## Python desktop app

See `NENAPIYUMA-AI-USB/README.md`, `NENAPIYUMA-AI-USB/README_SI.md`, and `NENAPIYUMA-AI-USB/BUILD_WINDOWS.md` for setup and build instructions.

## Security

Do not commit real API keys or credentials. `.env.example` contains placeholders only; create a local `.env.local` if needed and keep it untracked. Review `NENAPIYUMA-AI-USB/SECURITY.md` before using USB scanning or quarantine features.