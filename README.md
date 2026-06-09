# AI Review Agent

AI Review Agent is a starter repository for building an AI-assisted code review tool. The goal is to scan repositories, surface bugs and quality issues, and suggest safer code and build improvements.

## How To Install And Run

This repository is currently a scaffold, so setup is focused on preparing the environment.

1. Clone the repository.
2. Create and activate a virtual environment.
3. Install dependencies.
4. Run the CLI once implementation is added.

```bash
git clone https://github.com/1SosukeAizen1/ai_review_agent.git
cd ai_review_agent
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python -m ai_code_reviewer.cli --repo .
```

## How To Test

Use:

```bash
pytest -q
```

Expected working result (after tests are implemented):

```text
N passed in X.XXs
```

Note: test files currently exist as placeholders and are intentionally empty.

## Built With

- Python (planned runtime)
- Pytest (planned test runner)
- GitHub Actions (planned CI)

## Folder Structure

```text
ai_review_agent/
	.gitignore
	README.md
	AGENTS.md
	CLAUDE.md
	pyproject.toml
	requirements.txt
	docs/
		testing-checklist.md
	specs/
		design-decisions/
			architecture.md
			domain-glossary.md
			style-guidelines.md
	src/
		ai_code_reviewer/
			__init__.py
			cli.py
			scanner.py
			analyzers/
				__init__.py
			report/
				__init__.py
				writer.py
	tests/
		test_cli.py
		test_scanner.py
	.github/
		copilot-instructions.md
		workflows/
			ci.yml
		skills/
			code-review/
				SKILL.md
	.claude/
		skills/
			code-review/
				SKILL.md
```

## Contributing Notes

- Keep commit messages descriptive: verb + what changed.
- Update relevant files in `specs/` when behavior or architecture decisions change.
- Run tests before commit once tests are implemented.