# AGENTS.md

Operating notes for AI coding agents (Claude Code, Codex, Cursor, Copilot and others) working in this repository. Everything here is derived from the files actually in the tree, so trust it over guesses, and update it when the facts change.

## What this repository is

Define filters for new meme launches that use atomic v1 creation patterns.

- Source: https://github.com/nirholas/v1-trench-radar
- Primary language: HTML
- License: Other (see the LICENSE file)

## Repository layout

- `docs/`
- `README.md`
- `LICENSE`
- `SECURITY.md`
- `package.json`

## Setup

```bash
npm install
```

## Commands

| Task | Command |
|---|---|
| dev | `npm run dev` |
| build | `npm run build` |
| test | `npm test` |

Run the test and lint commands above before you consider a change finished. If a command fails on code you did not touch, say so in your report instead of silently skipping it.

## Conventions

- `.env` files are gitignored; never commit credentials, and read configuration from environment variables.
- Read the surrounding code before adding to it, and match its naming, file organisation and error-handling style.
- Keep `README.md` accurate: if a change alters behaviour, commands or configuration, update the docs in the same commit.
- Do not leave TODO comments, stub functions, placeholder data or commented-out code behind. Finish what you start or leave it out.
- Small, focused commits with a subject line that describes the change, not the act of committing.

## Where to raise things

- Bugs and feature requests: https://github.com/nirholas/v1-trench-radar/issues
- Questions and ideas: https://github.com/nirholas/v1-trench-radar/discussions
- Security issues: follow `SECURITY.md`, never a public issue.
