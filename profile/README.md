<p align="center">
  <img src="https://raw.githubusercontent.com/togo-framework/.github/main/profile/assets/togo-mark.svg" width="120" alt="ToGO" />
</p>

<h1 align="center">ToGO</h1>

<p align="center">
  <b>Ship your Go backend and React frontend as a single deployable app.</b><br/>
  An open-source, API-first full-stack framework — a Laravel-artisan-grade CLI for the Go&nbsp;+&nbsp;sqlc&nbsp;+&nbsp;Atlas&nbsp;+&nbsp;React stack.
</p>

<p align="center">
  <a href="https://to-go.dev"><img alt="Website" src="https://img.shields.io/badge/website-to--go.dev-1FC7DC?style=flat-square" /></a>
  <a href="https://www.npmjs.com/package/@togo-framework/cli"><img alt="npm" src="https://img.shields.io/npm/v/@togo-framework/cli?style=flat-square&color=2D8CE6&label=cli" /></a>
  <img alt="License" src="https://img.shields.io/badge/license-MIT-1659C8?style=flat-square" />
</p>

---

## What is ToGO?

ToGO gives Go developers the productivity of Laravel. One CLI scaffolds a full app — a
**Go API** (chi · Huma REST/OpenAPI · gqlgen GraphQL · sqlc · Atlas migrations) and a
**React frontend** (TanStack or Next.js, powered by the `@togo-framework/ui` design
system) — that compiles into **one binary, one repo, zero glue**.

- **Generators first** — `togo make:resource Post title:string body:text` emits the model, queries, schema, GraphQL, REST, seeder, and UI page, then regenerates the registries. The manifest `togo.resources.yaml` is the source of truth.
- **Everything is a plugin** — a thin microkernel; auth, dashboard, cache, queue, storage, realtime, i18n, and **database drivers** are installed via `togo install owner/repo`.
- **Pick your database** — `sqlite` (default) · `postgres` · **`togo-postgres`** (ParadeDB + pgvector + pg_cron) · `supabase` · `mysql` · `mongodb`, wired from day 0.
- **API-first** — every resource is exposed over **GraphQL** and **REST/OpenAPI**, generated and kept in sync.
- **AI-native** — every app is born agent-ready: a `.claude/` tree (skills, agents, rules) + a pre-wired MCP server so Claude Code can drive it end to end.

## Quick start

```bash
npm install -g @togo-framework/cli      # or: curl -fsSL https://to-go.dev/install.sh | sh
togo new myapp                           # pick a frontend (TanStack / Next.js) + a database
cd myapp
togo make:resource Post title:string body:text
togo generate && togo migrate && togo serve
# → Go API + React UI, serving on http://localhost:8080
```

## The ecosystem

| | |
|---|---|
| **[togo](https://github.com/togo-framework/togo)** | The microkernel — config, hooks, plugin loader, DB dialect registry, server bootstrap |
| **[cli](https://github.com/togo-framework/cli)** | The `togo` binary — generators, `make:*`, `migrate`, `generate`, `install`, `mcp`, `deploy` |
| **[create-togo-app](https://github.com/togo-framework/create-togo-app)** | The project template (TanStack + Next.js frontends), bundled into the CLI |
| **[ui](https://github.com/togo-framework/ui)** | `@togo-framework/ui` — the token-driven, RTL-ready design system (ToGO brand) |
| **[db](https://github.com/togo-framework/db)** | `togo-postgres` — the batteries-included Postgres image (ParadeDB + pg_cron + pg_partman) |
| **[mcp](https://github.com/togo-framework/mcp)** | MCP server exposing generators + project introspection as agent tools |
| **db-postgres · db-mysql · db-mongodb** | Database driver plugins (the kernel ships sqlite) |
| **auth · dashboard · cache · queue · storage · realtime · search · i18n · notifications · mail · log · validation · worker · faker · testing** | First-party capability plugins — `togo install togo-framework/<name>` |

**→ Browse all 40+ repos with rendered docs at [to-go.dev/repos](https://to-go.dev/repos).**

## Links

[**Website**](https://to-go.dev) · [**Docs**](https://docs.to-go.dev) · [**UI / Storybook**](https://ui.to-go.dev) · [**Demo**](https://demo.to-go.dev) · [**npm**](https://www.npmjs.com/org/togo-framework)

---

## 💎 Premium sponsors

ToGO is proudly sponsored by **ID8 Media** and **One Studio**.

<p align="center">
  <a href="https://id8media.com"><img src="https://raw.githubusercontent.com/togo-framework/.github/main/profile/assets/id8media.svg" height="46" alt="ID8 Media" /></a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://one-studio.co"><img src="https://raw.githubusercontent.com/togo-framework/.github/main/profile/assets/one-studio.jpeg" height="46" alt="One Studio" /></a>
</p>
