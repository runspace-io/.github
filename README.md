# Runspace

**Open-source engineering workspace — humans and AI agents collaborate on Git repositories through chat, terminal, diffs, and pull requests.**

[![Website](https://img.shields.io/badge/website-runspace.io-blue)](https://runspace.io)
[![License](https://img.shields.io/badge/license-MIT-green)](https://github.com/runspace-io/runspace/blob/main/LICENSE)

---

Runspace is a shared engineering workspace where AI agents behave like collaborators rather than detached chatbots. A developer gives an agent a task in the context of a repository, watches the work happen in real-time, intervenes when needed, reviews the resulting changes, and publishes them as a pull request — all without leaving the workspace.

### What makes Runspace different

- **Live collaboration timeline** — agent messages, logs, and file changes stream into the UI as they happen
- **Repository-native** — works with GitHub repos, local folders, and Git mirrors
- **Sandboxed execution** — agents run in isolated Docker containers with bounded file access
- **Built-in code review** — inspect diffs with Monaco editor and open PRs directly
- **Multi-resource channels** — attach multiple repos and folders to the same conversation
- **Host integration** — connect local folders without uploading, via a loopback agent

### Quick start

```bash
git clone https://github.com/runspace-io/runspace.git
cd runspace
cp .env.example .env
docker compose up -d --build
```

Open `http://localhost:3000` and sign in with `admin` / `admin`.

### Repositories

| Repo | Description |
|------|-------------|
| [runspace](https://github.com/runspace-io/runspace) | Core workspace — Go gateway, Next.js web app, agent runtime |
| [.github](https://github.com/runspace-io/.github) | Organization profile and community health files |

### Tech stack

**Backend** — Go, PostgreSQL, NATS, Docker  
**Frontend** — TypeScript, Next.js, Monaco Editor, xterm.js  
**Infrastructure** — Docker Compose, Traefik  

### Links

- [Website](https://runspace.io)
- [Documentation](https://github.com/runspace-io/runspace/tree/main/docs)
- [Product specification](https://github.com/runspace-io/runspace/blob/main/docs/mvp/PRODUCT_SPEC.md)

---

Built in Bangladesh. Open source under the MIT License.
