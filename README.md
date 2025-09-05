# MCP Registry (gh-pages)

This repository publishes the MCP servers index as a static JSON file via GitHub Pages.

- **Public URL:** `https://mcp-accelerator.github.io/mcp-registry/servers.index.json`
- Consumers (like the catalog site) fetch this file at runtime; no redeploy is needed when the index changes.

## How to update

1. Edit `servers.index.json` on the `gh-pages` branch.
2. Commit directly to `gh-pages`.
3. Wait ~30–60s for Pages to update, then refresh the consumer site.

## Notes

- Keep the JSON valid against our draft-07 schema (no extra fields).
- For hosted endpoints, only add `connect.endpoint_url` when you have a stable, public URL.
- Use `auth.token_guide_url` to point users to the official key/token page.
