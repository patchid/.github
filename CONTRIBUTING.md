# Contributing to Patch ID

Thanks for your interest in contributing. We're building in the open and welcome developers who want to help shape the future of developer reputation.

## What you can contribute to

- [`func-kode`](https://github.com/patchid/func-kode) — community platform, landing page, dashboard UI
- [`docs`](https://github.com/patchid/docs) — API documentation, guides, integration examples

## Getting started

1. **Fork** the repo you want to contribute to
2. **Create a branch** from `dev` (not `main`)
   ```bash
   git checkout dev
   git checkout -b feat/your-feature-name
   ```
3. **Make your changes** — keep commits small and focused
4. **Open a Pull Request** targeting the `dev` branch
5. A maintainer will review within 48 hours

## Branch naming

| Prefix | Use for |
|---|---|
| `feat/` | New features |
| `fix/` | Bug fixes |
| `chore/` | Maintenance, dependency updates |
| `docs/` | Documentation changes |
| `hotfix/` | Emergency production fixes (maintainers only) |

## Pull Request rules

- Target `dev` — never open PRs directly to `main`
- Keep PRs focused — one feature or fix per PR
- Write a clear description of what changed and why
- Link related issues with `Closes #issue-number`
- All checks must pass before merge

## Commit style

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add score breakdown chart
fix: resolve OAuth redirect loop
chore: update dependencies
docs: add API authentication guide
```

## Code standards

- TypeScript — strict mode, no `any`
- Tailwind CSS for styling
- Prettier + ESLint — run `npm run lint` before pushing
- Tests — add tests for any new utility functions

## Reporting bugs

Open an issue using the **Bug Report** template.

## Feature requests

Open an issue using the **Feature Request** template.

## Code of Conduct

All contributors must follow our [Code of Conduct](CODE_OF_CONDUCT.md).

---

*Patch ID is built by a small team. We genuinely appreciate every contribution.*
