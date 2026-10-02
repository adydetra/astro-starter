# Style & Design System

The application uses Tailwind CSS v4 configured via `@tailwindcss/vite` in `astro.config.mjs`.

## Setup & Configuration

- Styles are loaded in `src/styles/global.css` via `@import "tailwindcss";`.
- Included on Astro pages via `import '../styles/global.css';`.

## Styling Conventions

- **Utility Classes**: Use standard Tailwind utilities for spacing, typography, grid, and flex layouts.
- **Scoped Styles**: Astro automatically scopes `<style>` tags within components if custom CSS is necessary.
- **Interactive Radial Effects**: Radial hover glows are implemented via CSS custom properties mapped through inline client scripts when interactive cards are hovered.
