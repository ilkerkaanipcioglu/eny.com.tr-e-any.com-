# Implementation Plan - Unconventional Icon System Refinement

The user has requested to eliminate all instances of the `Bug` icon. The mobile menu icon must be replaced with the standard 3-line (`Menu`) icon. For all other `Bug` replacements, unique nature, plant, or animal icons will be used, strictly ensuring no repeated usage across different headings.

## Proposed Changes

### 1. `src/components/Header.astro`
- Update mobile menu toggle from `Bug` to `Menu`.
- Replace `Bug` in Solutions Mega Menu Trigger with `Sprout`.
- Replace `Bug` in About Mega Menu Trigger with `Leaf`.
- Replace `Bug` in Hakkımızda List Header with `Mushroom`.
- Replace `Bug` in İçerik & Yasal List Header with `Feather`.

### 2. `src/pages/urunler.astro`
- Replace `Bug` in "e-Ticaret & Operasyon" header with `TreePine`.
- Replace `Bug` in "eny Insight Series" block with `Fish`.

### 3. `src/pages/teknoloji.astro`
- Replace `Bug` under "Finansal Yapay Zeka" with `Cat`.
- Replace `Bug` under "Low-Code Platformlar" with `Dog`.
- Replace `Bug` under "Süreç Madenciliği" with `Trees`.
- Replace `Bug` in "eny Insight Series" block with `CloudRain`.

### 4. `src/pages/sektorler.astro`
- Replace `Bug` for "Üretim ve Otomotiv Sanayi" with `Cherry`.
- Replace `Bug` for "İnşaat ve Gayrimenkul (GYO)" with `Mountain`.

### 5. `src/pages/index.astro`
- Replace `Bug` for "API-First Mimari" with `Clover`.

### 6. `src/pages/hakkimizda.astro`
- Replace `Bug` for "Domain Uzmanlığı" with `Flower`.

### 7. `src/layouts/ServiceDetailLayout.astro`
- Replace `Bug` mapped to `analytics` with `TreeDeciduous`.
- Replace `Bug` mapped to `account_tree` with `Tent`.
- Replace `Bug` in the "eny Platform Vision" block with `Campfire`.

## Open Questions

None. The specific icons proposed are standard Lucide nature/animal icons and they will be imported explicitly.

## Verification Plan
- Build check: `npm run build`
- Manual browser verification to ensure no missing icon imports (`lucide`) cause build errors.
