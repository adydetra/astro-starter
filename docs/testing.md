# Development & Quality Assurance

Commands and workflows for linting and build validation.

## Commands

```bash
# Run local development server
bun run dev

# Run ESLint validation
bun run lint

# Auto-fix ESLint issues
bun run lint:fix

# Build static production site
bun run build

# Preview static production build locally
bun run preview
```

## Quality Checklist

Before opening a pull request or pushing commits:
1. Ensure `bun run lint` passes without errors.
2. Verify `bun run build` completes without errors and outputs to `dist/`.
