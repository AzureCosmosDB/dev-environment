# GitHub Copilot instructions

Follow the shared repository instructions in [`../AGENTS.md`](../AGENTS.md).

Before implementing Azure Cosmos DB code:

1. Read the Microsoft Learn article URL included in the user prompt.
1. Install and apply the Azure Cosmos DB Agent Kit:

   ```bash
   npx --yes skills add AzureCosmosDB/cosmosdb-agent-kit
   ```

1. Generate focused, runnable code that matches the article.
1. Use placeholder configuration values only. Don't store secrets in source files.
1. Restore, build, and validate before finishing.
