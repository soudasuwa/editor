# Guidance for Codex agents

## Project layout
- Source TypeScript files live in `src/`.
- Built artifacts are created under `dist/` by `pnpm build` using tsup.
- Built artifacts under `dist/` must be committed, but Codex agents do not need to review them.
- Do **not** commit `node_modules/`.

## Coding style
- This project uses [Biome](https://biomejs.dev/) for formatting and linting.
- Indentation is with **tabs** and strings use **double quotes**.
- Use named exports and prefer arrow function React components.

## Required checks
Run these commands before committing changes and include any output in your PR:

```bash
pnpm run check
pnpm build
```

No testing is required at the moment.

## Pull request
Provide a concise summary of the changes. Mention relevant file paths.
