# Contributing

Thanks for your interest in contributing to an Aartsen project! This guide
applies to every repository in the organisation unless that repository has
its own `CONTRIBUTING.md`.

## Before you start

- For anything larger than a small fix, open an issue first so the change can
  be discussed.
- Never commit secrets, credentials, customer data or personal data. Every
  repository is scanned for leaked secrets.
- To report a security issue, follow [SECURITY.md](SECURITY.md) instead of
  opening an issue.

## Workflow

1. Create a branch from the default branch, for example `feat/short-description`
   or `fix/short-description`.
2. Keep changes small and focused. Smaller pull requests get reviewed faster.
3. Open a pull request and fill in the template.
4. Make sure all checks pass and get at least one approving review.

## Pull request titles

PR titles follow [Conventional Commits](https://www.conventionalcommits.org/)
and are checked automatically:

```text
<type>(<optional scope>): <description>

feat: add export to CSV
fix(api): handle empty response
docs: update setup instructions
```

Allowed types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`,
`build`, `ci`, `chore`, `revert`.

## Automated checks

Most repositories run the shared Aartsen workflows:

| Check | What it does |
| --- | --- |
| CodeQL | Static analysis for security issues |
| Dependency review | Blocks newly added vulnerable dependencies |
| Gitleaks | Detects secrets in commits |
| Trivy | Scans dependencies and configuration for vulnerabilities |
| PR title | Enforces Conventional Commits |
| Lint | Markdown, YAML and GitHub Actions workflow linting |
