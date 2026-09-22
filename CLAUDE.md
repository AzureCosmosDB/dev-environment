# Claude Code guidance

Follow the shared repository instructions in [`AGENTS.md`](AGENTS.md).

When launched from a `claude-cli://open` deep link:

1. Use the `q` prompt value as the primary task.
1. Read any Microsoft Learn article URL included in the prompt before writing code.
1. Install and apply the Azure Cosmos DB Agent Kit:

   ```bash
   npx --yes skills add AzureCosmosDB/cosmosdb-agent-kit
   ```

1. Generate the requested app in this repository unless the prompt specifies a different target folder.
1. Use placeholder configuration values only. Don't request or store secrets.
1. Build and validate the app before finishing.
