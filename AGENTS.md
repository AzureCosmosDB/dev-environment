# Agent instructions

This repository is a neutral development environment for AI coding agents launched from Azure Cosmos DB documentation.

## First steps

1. Read the full prompt that launched this session.
1. If the prompt includes a Microsoft Learn article URL, read the article before creating code.
1. Install the Azure Cosmos DB Agent Kit if it isn't already available:

   ```bash
   npx --yes skills add AzureCosmosDB/cosmosdb-agent-kit
   ```

1. Apply the Azure Cosmos DB Agent Kit guidance when choosing SDK patterns, authentication, data access code, and validation steps.

## Build the requested app

- Generate a small, runnable app that matches the article and prompt.
- Prefer a file-based .NET app when the prompt asks for one.
- Keep the implementation focused on the operations shown in the article.
- Use current Azure SDK and Azure Cosmos DB SDK patterns from the article.
- Prefer Microsoft Entra ID authentication when the article supports it.
- Use safe placeholder configuration values only. Don't invent real endpoints, keys, tenant IDs, subscription IDs, or production resource names.
- Don't create, delete, or modify Azure resources unless the prompt explicitly asks you to do so.

## Configuration placeholders

Use clear placeholder names, such as:

- `COSMOS_ENDPOINT`
- `COSMOS_DATABASE_NAME`
- `COSMOS_CONTAINER_NAME`
- `AZURE_TENANT_ID`
- `AZURE_CLIENT_ID`

Never hard-code secrets, connection strings, account keys, tokens, or production configuration values.

## Validation

Before finishing:

1. Restore dependencies.
1. Build the app.
1. Run the app when it can run safely with placeholders or documented emulator/local configuration.
1. Report any validation command that couldn't run and explain what configuration is required.

For .NET apps, prefer:

```bash
dotnet restore
dotnet build
dotnet run
```

## Final response

Summarize:

- What files you created or changed.
- Which article instructions you implemented.
- Which commands you ran.
- Any configuration values the user must provide.
- Any validation that couldn't complete.
