# Agent Guide

Astro 7 starter template with Tailwind CSS v4, atomic design components, and ESLint.

Read only the document needed:
- `docs/architecture.md`: Astro island architecture, atomic component organization, and routing.
- `docs/style.md`: Tailwind CSS v4 setup with `@tailwindcss/vite` and global CSS styles.
- `docs/testing.md`: linting commands, Astro build validation, and preview.
- `docs/push.md`: branch naming, commit standards, pull request lifecycle, and pre-push validation.
- `docs/status.md`: implemented features, key dependencies, and roadmap.

## Source Map

- `astro.config.mjs`: Astro configuration integrating `@tailwindcss/vite`.
- `src/pages/index.astro`: root home page rendering component hierarchy.
- `src/components/atoms/SpotlightCard.astro`: atomic card component with mouse-tracking radial gradient glow.
- `src/components/molecules/TechStackCard.astro`: molecular card displaying technology stack information.
- `src/components/organism/TheExample.astro`: organism section composing atoms and molecules.
- `src/styles/global.css`: Tailwind CSS v4 entry point and custom base styles.
- `eslint.config.mjs`: ESLint flat configuration with `@antfu/eslint-config` and `eslint-plugin-astro`.
- `package.json`: scripts and dependency declarations.

## Invariants

- Use pure `.astro` components for zero-JS client bundle unless client-side interactivity explicitly requires a framework island (`client:load`, etc.).
- Follow atomic design: keep components partitioned in `src/components/atoms`, `molecules`, and `organism`.
- Prefer Tailwind utility classes over ad-hoc CSS. Use CSS variables for radial gradient positions.
- Adhere to `@antfu/eslint-config` and `eslint-plugin-astro` standards (`bun run lint`).

## Change Workflow

Read `package.json` before altering dependencies or scripts. Run `bun run lint` and `bun run build` before committing any code changes. Follow `docs/push.md` for git conventions, and keep `docs/` updated if architectural invariants change.
