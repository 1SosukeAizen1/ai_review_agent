See README.md for project overview and setup.

## Important Conventions
- Keep source files under src/ and tests under tests/.
- Keep Python module files small and focused.
- Update specs in specs/design-decisions/ when decisions change.
- Do not commit secrets; .env is local only.

## Known Gotchas
- This repository is currently scaffold-first; several files are placeholders.
- CI and tests are present as structure but implementation is intentionally minimal.

## Specs
- specs/design-decisions/architecture.md
- specs/design-decisions/domain-glossary.md
- specs/design-decisions/style-guidelines.md

## Verification
- Planned automated check: pytest -q
- Manual check: docs/testing-checklist.md
