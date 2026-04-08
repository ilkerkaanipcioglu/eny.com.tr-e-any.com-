# Implementation Plan - Fixing Icon Reference Errors

This plan addresses the `ReferenceError: Acorn is not defined` error occurring during Vercel builds, and cleans up inconsistent icon usage across the project.

## Proposed Changes

### Icon Imports & References

#### [MODIFY] [teknoloji.astro](src/pages/teknoloji.astro)
- Add `Acorn` to the Lucide icon imports in the frontmatter.

#### [MODIFY] [sektorler.astro](src/pages/sektorler.astro)
- Remove manual aliases (`Acorn`, `Bird`, `Fish`, `Leaf`, `Sprout`, `Waves`).
- Import the actual icons from `@lucide/astro`: `Acorn`, `Bird`, `Fish`, `Leaf`, `Sprout`, `Waves`.

#### [MODIFY] [iletisim.astro](src/pages/iletisim.astro)
- Verify `Shrimp` and `Fish` are correctly imported and used.

## Verification Plan

### Automated Tests
- Run `npm run build` locally.
