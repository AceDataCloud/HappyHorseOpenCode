# HappyHorseOpenCode

This repository owns only the OpenCode 2 native HappyHorse adapter and onboarding.
HappyHorse API transport, schemas, task normalization and billing remain in
AceDataCloud/MCPs (`happyhorse/`, published as HappyHorseMCP). Do not duplicate them here.

- Run `npm test`, `npm run check` and `npm pack --dry-run` before a PR.
- Add no billable generation, model request, task submission or retry to install,
  startup, tests or CI. Live acceptance requires an explicitly approved budget.
- Credential destinations are fixed to `https://happyhorse.mcp.acedata.cloud/mcp`.
  Never accept a user-configurable host with a saved token.
- Keep native credential storage in OpenCode; never write credentials to config,
  Skill content, logs or README. Credential changes must update in-memory headers.
- Existing user-owned MCP entries take precedence over plugin defaults.
- Keep English and Chinese onboarding in sync. Cite screenshot dates and distinguish
  native integration from upstream directory approval and paid task acceptance.
