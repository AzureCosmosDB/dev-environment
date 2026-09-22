# Security guidance

This repository is intended for disposable development environments and agent-assisted quickstart prototypes.

## Secrets and credentials

Do not commit or generate real secrets, credentials, tokens, connection strings, account keys, or production configuration values.

Use placeholders or environment variables instead:

```bash
COSMOS_ENDPOINT="https://<account-name>.documents.azure.com:443/"
COSMOS_DATABASE_NAME="<database-name>"
COSMOS_CONTAINER_NAME="<container-name>"
```

## Agent-generated code

Review generated code before running it. Confirm that the code:

- Doesn't print secrets or tokens.
- Doesn't include hard-coded credentials.
- Doesn't create, update, or delete Azure resources unless explicitly requested.
- Uses least-privilege authentication and authorization patterns.
- Uses placeholder values for any configuration that depends on the user's environment.

## Reporting security issues

Don't open public issues for security vulnerabilities. Follow the Microsoft security reporting process for Microsoft-owned repositories.
