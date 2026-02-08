# CLAUDE.md

Exposes Apple Music playback controls, library browsing, playlist management, and search as MCP tools. Talks to Music.app through AppleScript.

## Stack

TypeScript, Node >=18, ESM, MCP SDK, Vitest, ESLint 9 flat config, Prettier

## Build & Test

```sh
npm run build           # tsc
npm test                # vitest run
npm run test:coverage   # vitest with coverage
npm run lint            # eslint .
npm run format:check    # prettier --check .
```

## Conventions

- All source in `src/index.ts`; tests in `src/__tests__/`
- Husky pre-commit runs lint-staged (eslint --fix + prettier)
- macOS automation is done entirely through AppleScript
