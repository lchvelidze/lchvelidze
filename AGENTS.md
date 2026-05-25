# AGENTS.md

## Cursor Cloud specific instructions

This is a minimal demo repository with two components:

1. **`github-action-packages-new-main/`** — A trivial npm package exporting a `sayHello` function. Run tests with `npm test` from that directory.
2. **`snake.html`** — A standalone browser-based "Neon Snake" game (no build step, no dependencies).

### Running the application

- **npm package**: `cd github-action-packages-new-main && npm test`
- **Snake game**: Serve the repo root with any static HTTP server, e.g. `npx http-server /workspace -p 8080`, then open `http://localhost:8080/snake.html` in Chrome.

### Notes

- There are no external services, databases, or Docker dependencies.
- The npm package has zero `dependencies`/`devDependencies`; `npm install` is effectively a no-op but safe to run.
- Node.js v22+ is available via nvm in the environment.
- No lint or build tooling is configured in this repository.
