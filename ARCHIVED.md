# ⚠️ ARCHIVED — This repo has been consolidated into the Shannon Agent monorepo

**This repository is no longer maintained.** All development has moved to:

👉 **https://github.com/diff-lab-com/shannon-agent**

## What happened

`shannon-gateway` (TypeScript chat-platform bridge) has been merged into the
[shannon-agent](https://github.com/diff-lab-com/shannon-agent) monorepo
alongside `shannon-code` and `shannon-desktop`. The three products are now
individually shippable from a single repository with one shared engine and one
shared wire protocol (`shannon-api-protocol`).

| Old location | New location |
|---|---|
| `shannon-gateway/src/` (adapters, router, engine client) | `gateway/src/` in the monorepo |
| `shannon-gateway/package.json` | `gateway/package.json` (independent package) |
| Bun-compiled binary build | `cd gateway && pnpm build:binary` |

## For users

The prebuilt `shannon-gateway` standalone binary (Bun-compiled, no Node needed)
will be published from the monorepo's release workflow. Download from
[GitHub Releases](https://github.com/diff-lab-com/shannon-agent/releases).

## For contributors

- Open issues and PRs on https://github.com/diff-lab-com/shannon-agent
- The full history of this repo is preserved as git commits inside the monorepo
  (merged via `git subtree` in Phase 1 of the consolidation).
- This repo is now read-only.

## Reference

- Migration runbook: `MIGRATION.md` at the monorepo root
- License: Apache-2.0 (unchanged)