# Contributing

Thanks for contributing to a Pulse Tech Ltd project. These rules apply to every repository unless the repo has its own `CONTRIBUTING.md`.

## Workflow
1. Branch from `main` using a prefix: `feat/`, `fix/`, `docs/`, `refactor/`, `chore/`.
2. Commit with [Conventional Commits](https://www.conventionalcommits.org/) — e.g. `feat(orders): add bulk export`.
3. Open a pull request into `main`. Direct pushes to `main` are not allowed.
4. Fill in the PR template, link the related issue or task, and request a review.
5. Squash or merge once approved and CI is green.

## Before you open a PR
- [ ] Linter passes
- [ ] Tests pass (add tests for new behaviour)
- [ ] Dead code and debug output removed
- [ ] Docs / README updated if behaviour changed
- [ ] No secrets, credentials or `.env` files committed

## Code standards
- Keep files under ~300 lines and functions short and focused.
- No magic numbers — name your constants.
- Comments explain *why*, not *what*.
- Configuration comes from environment variables, never hardcoded.
- Follow the language's conventions: PEP 8 for Python, ESLint for JS/TS, PSR-12 for PHP, `dart format` for Dart.

## Databases
Schema changes go through migrations. Never run `UPDATE`, `DELETE`, `DROP` or `TRUNCATE` against production without explicit approval.
