# Implementation Plan - Layout & Typography Fixes

The user reported that some text elements are vertically stacked and do not fit the page layout. After a browser inspection, several specific issues were identified across the site, primarily on product pages and the "Hakkımızda" page.

## Proposed Changes

### 1. Service Detail Layout & Product Pages
The `ServiceDetailLayout` component and the pages using it (e-pos, e-tahsilat, e-ticaret, etc.) suffer from redundant numbering and a broken layout in the bottom CTA section.

#### [MODIFY] [ServiceDetailLayout.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/layouts/ServiceDetailLayout.astro)
-   **Bottom CTA Fix**: Remove `flex justify-center` from the bottom CTA section and use a standard block layout with `text-center` and better width constraints to prevent character-by-character stacking on narrow screens.
-   **Typography**: Ensure `h2` and `p` in the CTA have proper `max-width` and `mx-auto`.

#### [MODIFY] [e-ticaret.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/e-ticaret.astro) (and other product pages)
-   **Remove Redundant Numbers**: Remove hardcoded "01 —", "02 —", "03 —" from `problemTitle`, `solutionTitle`, and `resultTitle` props, as the layout already generates these numbers.
-   **Apply to all**: Repeat this for `e-pos.astro`, `e-tahsilat.astro`, `e-payment.astro`, `e-cashflow.astro`, `e-dbs.astro`, `e-ekstre.astro`, `e-ticaret.astro`, `lokalizasyon.astro`, `teknoloji.astro`, and `urunler.astro`.

### 2. Hakkımızda (About Us) Page
The "Hakkımızda" page has a "wall of text" issue in the Insight section and potential overlap issues on mobile.

#### [MODIFY] [hakkimizda.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hakkimizda.astro)
-   **Data Sovereignty Section**: Split the 1000+ character paragraph into İKİ distinct paragraphs for better readability and to avoid the "vertical stacking" feeling on mobile.
-   **Hero Section**: Increase the top padding/margin to ensure the Header (which is fixed) does not overlap the content on small screens.

### 3. Global Styles
#### [MODIFY] [global.css](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/styles/global.css)
-   Add a utility class or safety rule to prevent containers from collapsing to zero width, which causes character stacking.
-   Refine `text-wrap: balance` usage to ensure it doesn't trigger unexpected line breaks on very narrow containers.

## Verification Plan

### Automated Tests
-   Run `npm run build` to ensure no syntax errors were introduced.

### Manual Verification
-   **Browser Inspection**: Use the browser tool to verify:
    -   The "Mimari Değişim" text at the bottom of `/e-ticaret` is readable and not stacked character-by-character.
    -   Product pages show single numbering (e.g., "01 Kompleks Operasyon" instead of "01 01 — Kompleks Operasyon").
    -   The "Data Sovereignty" text on `/hakkimizda` is broken into readable chunks.
    -   Mobile view (375px) of `/hakkimizda` hero section has no header overlap.
