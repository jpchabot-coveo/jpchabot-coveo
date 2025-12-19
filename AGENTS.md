# AGENTS.md

## Scope
This file applies to the entire repository unless a subdirectory contains its own `AGENTS.md`, which overrides these rules for that subtree.

## Coding conventions
- Follow the existing project style; prefer readability over cleverness.
- No `try/catch` (or language equivalent) around import statements.
- Keep functions small and purposeful; extract helpers when a function exceeds ~40 lines.

## Testing
- Run the full test suite before committing: `npm test`.
- For quick checks during development, you may run targeted tests (e.g., `npm test -- component.test.tsx`), but always run the full suite before a PR.

## Git / PR etiquette
- Use descriptive commit messages (imperative mood).
- Every change must include necessary tests and documentation updates.
- Keep PR titles brief and meaningful; summarize key changes in the PR body.

## Documentation & comments
- Update README or module-level docs when adding new features or flags.
- Prefer inline comments that explain *why* rather than *what*.
- Document public functions with short docstrings describing inputs, outputs, and side effects.

## Review checklist
Before marking work complete, verify:
- ✅ Tests pass locally.
- ✅ New or changed behavior is documented.
- ✅ No linting errors or warnings.
- ✅ No unused imports or dead code.

## Tooling notes
- Use `rg` instead of recursive `ls`/`grep` for searches.
- If making visible UI changes, capture a screenshot (with description) for reviewers.

## Non-negotiables
- Do not commit secrets or credentials.
- Do not introduce new dependencies without approval in the PR description.
