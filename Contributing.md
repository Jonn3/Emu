# Contributing to <GrammerChecker>

Thanks for improving this project! Please follow these guidelines.

## Branching & Workflow
- Create an issue first. No changes without an issue.
- Branch naming: feature/<short>, fix/<short>, docs/<short>, test/<short>
- Conventional commits: feat:, fix:, docs:, test:, refactor:, chore:
- Open PRs to `main`. Require at least 1 approval + all checks passing.

## Dev Setup
- Java: JDK 17+, Gradle/Maven. `./gradlew test` or `mvn test`.
- Python: 3.11+, `python -m venv .venv && source .venv/bin/activate`, `pip install -r requirements.txt`, `pytest -q`.

## Code Style
- Java: Google Java Style; run formatter before commit.
- Python: black + isort + flake8 (line length 100).

## Testing
- New/changed code must include tests.
- Aim for ≥80% coverage on touched packages.
- Do not make network calls in tests; mock I/O.

## Issues & PRs
- Every PR must reference an issue: `Fixes #123`.
- Add screenshots for UI changes; attach UML/diagrams when relevant.
- Keep PRs under 400 LOC where possible.

## Security & Data
- No secrets in repo. Use `.env` and `.gitignore`.
- Respect third-party ToS when scraping; add polite delays or mocks.

## Attribution
- Credit is assigned by commit authorship. Pairing? Use Co-authored-by trailers.