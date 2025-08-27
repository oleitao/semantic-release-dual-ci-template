# semantic-release-dual-ci-template

Template que publica releases automáticos com semantic-release tanto em **GitHub Actions** quanto em **Azure DevOps**.

## Pré-requisitos

- Commits no padrão **Conventional Commits**.
- **GitHub**: não precisa criar token manual; a action usa `GITHUB_TOKEN`.
- **Azure DevOps**: crie uma variável secreta `GitHubToken` com permissões de `repo` (se publicar Notas de Release no GitHub).

## Primeira release

1. Faça commits convencionais (ex.: `feat: ...`, `fix: ...`).
2. Faça push para `main`.
3. O workflow/pipeline corre e cria a release automaticamente.

## Links úteis
- Docs: GitHub Actions + semantic-release  
- Plugin ADO: semantic-release-ado



semantic-release-dual-ci-template/
├─ .github/
│  └─ workflows/
│     └─ release.yml
├─ azure-pipelines.yml
├─ package.json
├─ .releaserc.json
└─ README.md
