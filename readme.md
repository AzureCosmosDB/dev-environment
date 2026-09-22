# Dev environment for Azure Cosmos DB projects

This repository provides shared setup guidance for AI coding agents launched from Azure Cosmos DB documentation.

Use this repository as a neutral starting point for agent-assisted quickstart work. The agent should read the source Microsoft Learn article named in the prompt, generate a small runnable app, use safe placeholder configuration values, and validate the result before finishing.

## Agent guidance

- [`AGENTS.md`](AGENTS.md) contains the shared instructions for all coding agents.
- [`CLAUDE.md`](CLAUDE.md) contains Claude Code-specific entry-point guidance.
- [`.github/copilot-instructions.md`](.github/copilot-instructions.md) contains GitHub Copilot-specific entry-point guidance.
- [`.github/SECURITY.md`](.github/SECURITY.md) explains how agents should handle credentials, placeholders, and generated code.

## Azure Cosmos DB Agent Kit

Agents should install the Azure Cosmos DB Agent Kit before working on generated Azure Cosmos DB apps:

```bash
npx --yes skills add AzureCosmosDB/cosmosdb-agent-kit
```
