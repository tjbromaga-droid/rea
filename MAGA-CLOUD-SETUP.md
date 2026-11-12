# MAGA cloud setup

## Scope
Prepare REA for development in a GitHub Codespace. Start with a local sample application you own; use website observation only for publicly accessible UI and authorized testing. Do not collect credentials or private network data.

## Setup
1. Open this branch in GitHub Codespaces (a Codespaces account and available quota are required).
2. Check `node --version`, `npm --version`, and `ps --version`. The repository specifies Node 24.22.1 in `.nvmrc`; follow the supported runtime range in `package.json`.
3. From a trusted directory outside the checkout, follow the official README's `npx rea-agents setup` instructions. Review and approve the selected agent's configuration changes; restart that agent.
4. Verify the CLI with `npx rea-agents --help`. Confirm the selected agent lists the REA MCP tools after restarting.
5. For source development, follow `CONTRIBUTING.md` and the repository's dependency, build, and test instructions rather than assuming a successful installation.

## Acceptance checks
- [ ] Codespace created and terminal available
- [ ] Node/npm and Linux process prerequisites verified
- [ ] REA CLI help runs successfully
- [ ] MCP registration reviewed and approved
- [ ] Agent discovers REA tools
- [ ] Local owned sample analyzed; record observations and limitations

No runtime checks have been executed by the GitHub connector. Record actual versions, command output and failures here after running in the Codespace. Never commit API keys or credentials.
