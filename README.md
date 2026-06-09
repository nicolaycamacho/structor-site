# structor-site

Landing page for [Structor](https://github.com/nicolaycamacho/structor) — a local CLI that
generates a repository-local AI engineering harness with versioned, enforceable policy and
drift-failing validators.

Built with [Astro](https://astro.build).

## Commands

All commands are run from the root of the project, from a terminal. Requires Node `>=22.12.0`.

| Command           | Action                                       |
| :---------------- | :------------------------------------------- |
| `npm install`     | Installs dependencies                        |
| `npm run dev`     | Starts local dev server at `localhost:4321`  |
| `npm run build`   | Build the production site to `./dist/`       |
| `npm run preview` | Preview the build locally, before deploying  |

## Structure

- `src/layouts/Layout.astro` — global design tokens, fonts, and the page shell.
- `src/components/*.astro` — one component per section (Nav, Hero, Wedge, Walkthrough,
  DemoSlot, Proof, Scorecard, Install, Honesty, Footer).
- `src/pages/index.astro` — composes the sections into the page.

To drop in the demo video, replace the `.demo-placeholder` block in
`src/components/DemoSlot.astro` with your Loom `<iframe>`.
