<h1 align="center">togo</h1>
<p align="center"><em>Go, the artisan way.</em></p>

<p align="center">
An open-source, API-first application framework for the
<strong>Go + sqlc + Atlas + GraphQL/OpenAPI + Next.js</strong> stack —
with a Laravel-artisan-like developer experience.
</p>

## Get started

```bash
curl -fsSL https://raw.githubusercontent.com/togo-framework/cli/main/install.sh | sh
togo new myapp && cd myapp
togo make:resource Post title:string body:text:nullable
togo generate && togo migrate && togo serve
```

## Repositories

| Repo | Role |
|---|---|
| [**togo**](https://github.com/togo-framework/togo) | Microkernel — Plugin contract + Kernel |
| [**cli**](https://github.com/togo-framework/cli) | The `togo` binary — generators, codegen, plugins, MCP, deploy |
| [**create-togo-app**](https://github.com/togo-framework/create-togo-app) | Project template (`togo new`) |
| [**plugin-template**](https://github.com/togo-framework/plugin-template) | Starter for togo plugins |
| [**togo-mcp**](https://github.com/togo-framework/togo-mcp) | MCP server for AI agents |

## Why togo

- **API-first** — every resource over GraphQL *and* REST/OpenAPI 3.1.
- **Everything is a plugin** — thin microkernel; capabilities installed by the CLI.
- **Generator-first** — one command scaffolds across model, sqlc, Atlas, GraphQL, REST, and Next.js.
- **AI-native** — projects ship `.claude/` skills/agents + MCP wiring for Claude Code.
- **Deploy anywhere** — built-in Terraform via `togo deploy`.

---

<p align="center">💛 <a href="https://github.com/sponsors/fadymondy">Sponsor togo</a></p>
