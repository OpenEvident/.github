# Contributing to OpenEvident projects

Thank you for your interest in contributing. This document describes the process that applies across OpenEvident repositories. Individual projects may add repository specific notes in their own `CONTRIBUTING.md`; where one exists, follow it alongside this guide.

## Before you start

Search existing issues and pull requests before opening a new one. For anything larger than a small fix, open an issue first and describe what you want to change and why. This avoids duplicated effort and lets a maintainer weigh in before you invest time in an implementation.

Small fixes such as typos, broken links, or obvious bugs with a clear one line fix do not need an issue first. Open a pull request directly.

## Development setup

Each repository documents its own setup steps in its README. Most OpenEvident projects use pnpm workspaces and a standard set of scripts:

```
pnpm install
pnpm run build
pnpm run lint
pnpm run typecheck
pnpm run test
```

Run these before opening a pull request. CI will run them again, but catching problems locally saves review time on both sides.

## Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org/). The format is:

```
type(scope): short summary

Longer explanation if needed, wrapped at roughly 72 characters.
```

Common types are `feat`, `fix`, `docs`, `refactor`, `test`, and `chore`. The scope is usually the package or app the change touches, for example `feat(runtime-mcp): add retry to worker client`.

## Sign off your commits

OpenEvident projects are licensed under the Apache License, Version 2.0. To keep the provenance of every contribution clear, we ask that you sign off your commits using the Developer Certificate of Origin:

```
git commit -s -m "your message"
```

This adds a `Signed-off-by` line to your commit, certifying that you wrote the change or otherwise have the right to submit it under the project's license. Pull requests with unsigned commits will be asked to amend before merge.

## Pull request process

1. Fork the repository and create a branch from `master` (or the default branch shown on the repository).
2. Make your change, including tests where the change affects behavior.
3. Confirm `lint`, `typecheck`, and `test` all pass locally.
4. Open a pull request with a clear description of what changed and why. Link the related issue if one exists.
5. A maintainer will review the pull request. Expect feedback and requested changes; this is a normal part of the process, not a sign that something went wrong.
6. Once approved, a maintainer will merge the pull request. We generally squash merge to keep history readable.

## Code style

Most repositories enforce style through ESLint and Prettier, run automatically via `pnpm run lint`. Match the conventions already used in the file you are editing. If a linter rule and an existing pattern in the codebase disagree, prefer the linter.

## Reporting bugs and requesting features

Use the issue templates provided in each repository. Include enough detail for a maintainer to reproduce the problem or understand the request without needing to ask follow up questions for basic context: your environment, the steps you took, what you expected, and what happened instead.

## Code of conduct

Participation in OpenEvident projects is governed by our [Code of Conduct](./CODE_OF_CONDUCT.md). By participating, you agree to abide by it.

## Security issues

Do not open a public issue for a security vulnerability. See [SECURITY.md](./SECURITY.md) for how to report one privately.

## Questions

If you have a question that is not a bug report or feature request, see [SUPPORT.md](./SUPPORT.md) for where to ask it.
