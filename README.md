# Thunder Client

Thunder Client is a lightweight REST API client extension for Visual Studio Code created by Ranga Vadhineni, providing a clean interface for sending HTTP requests, managing collections, and testing APIs without leaving the editor. With nearly 7 million installs, it pioneered GUI-based API testing in VS Code with 100% local storage, scriptless testing, Git Sync for team collaboration, GraphQL support, and an advanced CLI for CI/CD integration.

- **Human URL:** [https://www.thunderclient.com](https://www.thunderclient.com)
- **Version:** 2.40.10

## Description

Thunder Client supports importing collections from Postman, Insomnia, Hoppscotch, and OpenAPI 3.0, and offers pre/post-request scripting and environment variables. The CLI (@thunderclient/cli) enables CI/CD integration with support for parallel execution and multiple report formats (CLI, CSV, HTML, JSON, XML, NUnit).

## Links

- [Documentation](https://docs.thunderclient.com/)
- [Getting Started](https://docs.thunderclient.com/get-started)
- [CLI Documentation](https://docs.thunderclient.com/cli)
- [Scripting API Reference](https://docs.thunderclient.com/scripting/api)
- [GitHub Support](https://github.com/thunderclient/thunder-client-support)
- [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client)
- [Pricing](https://www.thunderclient.com/pricing)
- [npm CLI Package](https://www.npmjs.com/package/@thunderclient/cli)
- [Changelog](https://github.com/thunderclient/thunder-client-support/releases)

## APIs

| API | Description |
|-----|-------------|
| Thunder Client | VS Code REST API client extension with collections, environments, scriptless testing, and Git Sync |
| Thunder Client CLI | Node.js CLI tool for running requests and collections from the terminal with CI/CD support |

## CLI Quick Reference

```bash
# Install the CLI
npm i -g @thunderclient/cli

# List all collections
tc list

# List requests in a collection
tc list 'myCollection'

# Run a collection
tc --col 'myCollection'

# Run all collections
tc --col all

# Run with concurrency
tc --col 'myCollection' --concurrent 5

# Stop on first failure
tc --col 'myCollection' --stop-on-fail

# Run a folder within a collection
tc --fol 'myFolder'

# List all environments
tc list env
```

## Pricing

| Tier | Price | Features |
|------|-------|----------|
| Free | $0/month | Basic local usage, limited collection runs |
| Pro | $3/month | Team sync, collections sharing, environment sharing |
| Enterprise | $16/user/month | Unlimited collection runs, full team management |

## Artifacts

### JSON Schema

| File | Description |
|------|-------------|
| [thunder-client-collection-schema.json](json-schema/thunder-client-collection-schema.json) | JSON Schema for Thunder Client collection files covering requests, folders, headers, auth, body, and test assertions |
| [thunder-client-environment-schema.json](json-schema/thunder-client-environment-schema.json) | JSON Schema for Thunder Client environment files with variable definitions |

### JSON Structure

| File | Description |
|------|-------------|
| [thunder-client-collection-structure.json](json-structure/thunder-client-collection-structure.json) | Structural documentation for all Thunder Client data models |

### JSON-LD Context

| File | Description |
|------|-------------|
| [thunder-client-context.jsonld](json-ld/thunder-client-context.jsonld) | JSON-LD context mapping Thunder Client vocabulary to linked data semantics |

### Examples

| File | Description |
|------|-------------|
| [thunder-client-collection-example.json](examples/thunder-client-collection-example.json) | Example Thunder Client collection demonstrating requests, folders, auth, body, and test assertions |
| [thunder-client-environment-example.json](examples/thunder-client-environment-example.json) | Example Thunder Client environment with variable definitions |

### Vocabulary

| File | Description |
|------|-------------|
| [thunder-client-vocabulary.yml](vocabulary/thunder-client-vocabulary.yml) | Domain vocabulary covering requests, collections, environments, CLI commands, testing, and pricing concepts |

## Tags

API Client, API Testing, CI/CD, CLI, Collections, GraphQL, REST Client, VS Code
