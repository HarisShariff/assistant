# Repository Instructions

## Commits

Use lowercase Angular-style commits without scopes:

`<type>: <imperative description>`

Allowed types: `feat`, `fix`, `test`, `refactor`, `docs`, `chore`.

Keep commits concise and focused on one logical change.

## Branches and Pull Requests

- Pull the latest `main` before creating a branch.
- For issue-based work, use: `issue-<number>/<description>`.
- For standalone documentation, use: `<type>/<description>`.
- Valid documentation prefixes include `prd/`, `design/`, `rfc/`, `adr/`, and `docs/`.
- Before opening a PR, update the branch with the latest `main`.
- Never push directly to `main`.
- Open a PR into `main` using the repository PR template.

Examples:

- `issue-23/add-whatsapp-handler`
- `prd/whatsapp-support-agent`
- `rfc/agent-runtime`
- `adr/use-strands`
- `docs/update-readme`

## AGENTS.md

Keep instructions concise and token-efficient. Add only rules that materially affect implementation.
