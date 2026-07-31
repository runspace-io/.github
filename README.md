<p align="center">
  <img src="https://raw.githubusercontent.com/runspace-io/runspace/main/apps/web/public/brand/runspace-logo.svg" alt="Runspace" width="520" />
</p>

<p align="center">
  <a href="https://runspace.io"><img src="https://img.shields.io/badge/website-runspace.io-blue" alt="Website" /></a>
  <a href="https://github.com/runspace-io/runspace/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green" alt="License: MIT" /></a>
</p>

---

Runspace is collaborative intelligence for software engineering. Not an AI that
replaces you, and not a chatbot you ping from the sidelines. You and the agent
share a realtime workspace — terminal, diffs, pull requests, and a live timeline
where you see every decision as it happens. You bring intent. The agent brings
speed. Together you ship.

## Features

- **Sandboxed agents** run in isolated Docker containers with bounded file access
- **Live timeline** streams agent messages, logs, and file changes in realtime
- **Built-in code review** with Monaco diff viewer and direct PR creation
- **Multi-resource channels** let you attach repos and local folders to the same conversation
- **Host integration** connects local folders without uploading, via a loopback agent
- **Git-native** branches, changes, commits, and PR publishing without leaving the workspace
- **Self-hosted** under the MIT license, runs on your own infrastructure with Docker Compose

## Quick start

```bash
git clone https://github.com/runspace-io/runspace.git
cd runspace
cp .env.example .env
docker compose up -d --build
```

Open `http://localhost:3000` and sign in with `admin` / `admin`.

## Repositories

| Repo | Description |
|------|-------------|
| [runspace](https://github.com/runspace-io/runspace) | Core workspace — Go gateway, Next.js web app, agent runtime |
| [.github](https://github.com/runspace-io/.github) | Organization profile and community health files |

## Stack

| Layer | Technology |
|-------|------------|
| Frontend | Next.js, TypeScript, Monaco Editor, xterm.js |
| Gateway | Go, NATS, WebSocket |
| Persistence | PostgreSQL |
| Runtime | Docker (isolated per-agent containers) |

## Links

- [Website](https://runspace.io)
- [Contributing](https://github.com/runspace-io/runspace/blob/main/CONTRIBUTING.md)
- [Security policy](https://github.com/runspace-io/runspace/blob/main/SECURITY.md)
- [Code of conduct](https://github.com/runspace-io/runspace/blob/main/CODE_OF_CONDUCT.md)
