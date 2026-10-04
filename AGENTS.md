<!-- BEGIN:nextjs-agent-rules -->
# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` before writing any code. Heed deprecation notices.
<!-- END:nextjs-agent-rules -->

# HeliosGen agent guide

HeliosGen is a **local-only** Tauri + Next.js desktop app for visual AI image/video workflows (kie.ai / optional Azure & Codex). No cloud accounts.

Project Cursor rules live in `.cursor/rules/` — read the matching rule when editing that area:

| Rule | When |
|---|---|
| `heliosgen-core.mdc` | Always (architecture + non-negotiables) |
| `model-config.mdc` | Models / generate APIs |
| `workflow-canvas.mdc` | React Flow nodes, Zustand, pipeline |
| `api-local-storage.mdc` | `app/api/**`, guest SQLite, jobs, kie upload |
| `desktop-tauri.mdc` | Tauri / desktop packaging (`DESKTOP.md`) |
| `ui-shadcn-canvas.mdc` | UI, shadcn, node CSS |

Package manager: **pnpm**. Desktop docs: `DESKTOP.md`. shadcn skill: `.agents/skills/shadcn/`.
