# Architecture

Content-driven, ultra-fast website built with Astro 7 and Tailwind CSS v4.

## Island Architecture & Component Organization

Astro leverages an Island Architecture that compiles `.astro` components into pure, static HTML with zero JavaScript shipped to the client by default.

```text
src/pages/index.astro (Page Route)
└── src/components/organism/TheExample.astro (Organism)
    ├── src/components/molecules/TechStackCard.astro (Molecule)
    └── src/components/atoms/SpotlightCard.astro (Atom)
```

- **Atoms (`src/components/atoms/`)**: Basic visual building blocks (e.g. `SpotlightCard.astro`).
- **Molecules (`src/components/molecules/`)**: Small functional combinations of atoms (e.g. `TechStackCard.astro`).
- **Organisms (`src/components/organism/`)**: Cohesive layout sections (e.g. `TheExample.astro`).
- **Pages (`src/pages/`)**: File-based routing rendering full HTML documents with `<!DOCTYPE html>`.

## Build Pipeline

- **Framework**: Astro 7 with Vite under the hood.
- **Styling**: Tailwind CSS v4 integration using `@tailwindcss/vite` declared in `astro.config.mjs`.
