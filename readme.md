![Evalite: the TypeScript-native, local-first tool for testing LLM-powered apps.](https://raw.githubusercontent.com/mattpocock/evalite/refs/heads/main/repo-card.jpg)

> **SpaceThree fork.** This is the SpaceThree fork of [evalite](https://github.com/mattpocock/evalite), published as `@spacethree/evalite` to GitHub Packages. The primary deviation from upstream is the Postgres storage adapter (`@spacethree/evalite/postgres-storage`); see `apps/evalite-docs/src/content/docs/guides/storage.mdx`. We maintain this fork until upstream merges the postgres adapter PR, at which point we plan to switch back to the public package.

- [View the upstream docs](https://www.evalite.dev/)
- [Join the upstream Discord](https://www.mattpocock.com/ai-discord)

## Contributing

1. Create a .env file inside `packages/example` containing an `OPENAI_API_KEY`:

```sh
OPENAI_API_KEY=your-api-key
```

2. Run development commands:

```bash
pnpm run dev          # Build, then run tsc -w on evalite + vitest on evalite-tests
pnpm run example      # Build, then run evalite watch + UI dev server at http://localhost:5173
pnpm run test         # Build and run all tests
```

> [!IMPORTANT]
>
> You may need to run `pnpm build` in root, then `npm link` inside `packages/evalite` to get the global `evalite` command to work.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for full documentation.
