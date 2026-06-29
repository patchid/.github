# patchid — Internal Org Guide

This repo (`.github`) contains org-level community health files, issue/PR templates, and the public org profile.

> For the public-facing org profile, see [`profile/README.md`](./profile/README.md).

---

## Repos at a glance

| Repo | Visibility | Stack | Purpose |
|---|---|---|---|
| [`func-kode`](https://github.com/patchid/func-kode) | Public | Next.js, Supabase, Cloudflare | Community platform, landing page, developer dashboard |
| [`core`](https://github.com/patchid/core) | Private | TypeScript, API | Reputation scoring engine, signal aggregation, score API |
| [`console`](https://github.com/patchid/console) | Private | TBD | Partner and recruiter dashboard |
| [`admin`](https://github.com/patchid/admin) | Private | TBD | Internal ops, analytics, admin tooling |
| [`docs`](https://github.com/patchid/docs) | Public | Markdown / MDX | Public API docs, integration guides |
| [`.github`](https://github.com/patchid/.github) | Public | — | This repo — org profile, templates, community files |

---

## Branch strategy (all repos)

| Branch | Purpose | Deploys to |
|---|---|---|
| `main` | Production — PR only, protected | Production URL |
| `dev` | Active integration branch | Preview only |
| `staging/demo` | QA / investor demo | Preview only |
| `feat/*` | Feature branches | No auto-deploy |
| `fix/*` | Bug fixes | No auto-deploy |
| `hotfix/*` | Emergency production fixes | Merge to `main` via PR |

**Rule:** Never push directly to `main`. All changes go through a PR targeting `dev` first.

---

## Teams

| Team | Access |
|---|---|
| `founders` | Admin on all repos |
| `engineering` | Write on all repos |
| `frontend` | Write on `func-kode`, read on `core` |
| `core-engine` | Admin on `core`, write on `docs` |
| `contributors` | Write on `func-kode`, `docs` only |

---

## Label system

All repos use the same label taxonomy:

**Type:** `type: feature` `type: bug` `type: chore` `type: docs` `type: research` `type: security`

**Priority:** `priority: P0` `priority: P1` `priority: P2` `priority: P3`

**Scope:** `scope: landing` `scope: dashboard` `scope: auth` `scope: scoring` `scope: api` `scope: infra` `scope: onboarding` `scope: docs`

**Sprint:** `sprint: current` `sprint: next` `sprint: backlog` `sprint: blocked`

**Status:** `status: needs-spec` `status: needs-review` `status: good-first-issue`

---

## URLs

| URL | What it serves |
|---|---|
| `patch-id.com/` | Landing page — public |
| `patch-id.com/oss` | Open source community page |
| `patch-id.com/connect` | GitHub OAuth entry point |
| `app.patch-id.com/` | Developer dashboard (auth required) |
| `partner.patch-id.com/` | Partner console — Phase 2 |
| `admin.patch-id.com/` | Internal admin — Phase 2 |

---

## Contacts

| Role | Contact |
|---|---|
| Security issues | security@patch-id.com |
| Business enquiries | hello@patch-id.com |
| Conduct violations | conduct@patch-id.com |
