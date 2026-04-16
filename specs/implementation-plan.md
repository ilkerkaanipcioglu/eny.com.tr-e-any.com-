# Implementation Plan - Fix Vertical Text Rendering

This plan addresses the issue where text (specifically the "Every Financial Process" heading) renders vertically (letter by letter) on the English homepage. This is likely due to a CSS conflict between global heading styles and inline `max-width` constraints.

## Proposed Changes

### Styles & Layout

#### [MODIFY] [global.css](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/styles/global.css)
- Refine heading styles to ensure consistent width and prevent unexpected letter-by-letter wrapping.
- Specifically, I will check if `text-wrap: balance` and `overflow-wrap: break-word` are causing the collapse and adjust accordingly.

#### [MODIFY] [index.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/en/index.astro)
- Standardize the `h2` heading style.
- Remove redundant inline `max-width` that may be conflicting with responsive Tailwind classes.
- Ensure the text uses `w-full` and `max-w-[600px]` classes correctly.

## Git Workflow
1. Apply CSS/Astro fixes.
2. `git add .`
3. `git commit -m "fix: resolve vertical text rendering on English homepage"`
4. `git push`

## Verification Plan

### Automated Tests
- Run `npm run build` to ensure no regression or build errors.

### Manual Verification
- Verify the layout logic.
- After pushing, the user can verify the live site.
