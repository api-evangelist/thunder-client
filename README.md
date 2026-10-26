# Thunder Client

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
