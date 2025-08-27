# semantic-release-dual-ci-template

Template that automatically publishes releases using semantic-release both in **GitHub Actions** and **Azure DevOps**.

## Prerequisites

- Commits must follow the **Conventional Commits** standard.
- **GitHub**: no need to manually create a token; the action uses `GITHUB_TOKEN`.
- **Azure DevOps**: create a secret variable `GitHubToken` with `repo` permissions (if publishing Release Notes to GitHub).

## First Release

1. Make conventional commits (e.g., `feat: ...`, `fix: ...`).
2. Push to `main`.
3. The workflow/pipeline runs and automatically creates the release.

## Useful Links

- Docs: GitHub Actions + semantic-release  
- ADO Plugin: semantic-release-ado  

