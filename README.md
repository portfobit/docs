# Portfobit Docs

The public documentation source for Portfobit. It is built with [Mintlify](https://www.mintlify.com/) and is intended to be published at `docs.portfobit.com`.

## Local preview

Use Node.js 20.17+ and run:

```bash
npm run dev
```

The preview opens at `http://localhost:3000` and refreshes as you edit. Use
`npm run dev:no-open` to start it without opening a browser, or `npm run validate`
to validate the documentation before committing.

## Contributing

This is a public repository. Read [AGENTS.md](AGENTS.md) before editing; it
defines the public-information boundary, API documentation rules, and required
validation without depending on any private repository.

## Structure

- `guides/` — onboarding, MCP setup, account connections, and safe operation.
- `api-reference/` — REST concepts and the generated OpenAPI reference.
- `openapi/portfobit-openapi.yaml` — the public REST API specification consumed by the docs site.
- `changelog/` — one public release-notes page, organized by year.
