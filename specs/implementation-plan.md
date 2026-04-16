# Plan - Adjusting Illustration Highlights to Brand Color

The user wants the highlight color of the illustrations on `eny.com.tr` to match the "neon lime" color of the "E-KONUŞALIM" button (`#D0FD17`) exactly.

## User Review Required

> [!IMPORTANT]
> The subagent determined that a `hue-rotate(22deg)` (down from `40deg`) with increased saturation is the best way to match the original yellow-gold highlights of the art to the neon lime brand color.

## Proposed Changes

### [Component] ArtIllustration

#### [MODIFY] src/components/ArtIllustration.astro
- Update the `hue-rotate` values and increase saturation/brightness for the `brand` and `minimal` variants to achieve the correct neon lime look.

```css
/* Brand: Neon Lime #D0FD17 */
.art-variant-brand img {
  filter: hue-rotate(22deg) saturate(2) brightness(1.1);
}

/* Minimal: Subtle lime tint with the correct brand hue */
.art-variant-minimal img {
  filter: hue-rotate(22deg) saturate(0.7) brightness(1.05);
}
```

## Verification Plan

### Automated Tests
- N/A (Visual adjustment)

### Manual Verification
- View `http://localhost:4321/tuval` in the browser.
- Compare the "Vizyon" (brand variant) and "Büyüme" (minimal variant) highlights with the "E-KONUŞALIM" button.
- A browser screenshot will be captured to confirm the match.
