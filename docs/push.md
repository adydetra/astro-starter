# Repository & Push Workflow

Every code change must adhere to consistent commit standards and branch hygiene before pushing.

## 1. Branch Naming

Create short, descriptive branches prefixed with the change type:

```text
feat/short-description
fix/short-description
docs/short-description
chore/short-description
refactor/short-description
```

## 2. Commit Standards

Use focused commits with imperative Conventional Commit messages:

```text
feat: add blog post layout template
fix: resolve card glow calculation on resize
docs: update status and architecture notes
chore: bump astro to latest release
```

## 3. Pre-Push Validation Checklist

- [ ] `bun run lint` passes cleanly.
- [ ] `bun run build` completes without errors.
- [ ] Commit message follows Conventional Commits format.
