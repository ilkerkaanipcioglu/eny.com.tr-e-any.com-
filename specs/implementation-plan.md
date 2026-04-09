# Implementation Plan: Eny Product-Only Pivot

The objective is to remove all legacy consultancy/consulting residues (Harezm heritage) from `eny.com.tr` and transition the brand to be strictly focused on its "e-product" suite (e-Fatura, e-Defter, e-Tahsilat, etc.).

## User Review Required

> [!IMPORTANT]
> - **Navigation Change**: "Hizmetler" (Services) will be renamed to "Çözümler" (Solutions) or "Ürünler" (Products) to move away from the service provider identity.
> - **Page Removal/Merge**: `lokalizasyon.astro` (Consultancy focused) will be removed or merged into the product suite.
> - **Hakkımızda (About Us)**: The narrative will shift from "15 years of consultancy" to "Evolution as a Finance Operating System Provider".

## Proposed Changes

### 1. Internationalization (i18n)
#### [MODIFY] [translations.ts](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/i18n/translations.ts)
- **Purge**: Delete keys related to `svcOutsourceTitle`, `svcAmsTitle`, `svcGlobalTitle` (Roll-out).
- **Rename**: Change `navServices` to "Çözümler" (Solutions).
- **Rebrand**: Update `aboutP1`, `aboutP2`, `aboutP3` to reflect a software/product company identity.
- **Product Focus**: Update `svcPageDesc` and other headers to emphasize "Product Infrastructure".

### 2. Navigation & Layout
#### [MODIFY] [Header.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/components/Header.astro)
- Rename the "Hizmetler" menu item to "Çözümler".
- Remove "Roll-out & Lokalizasyon" or merge it into the "Çözümler" dropdown as a product capability.
- Ensure the mega-menu focuses on product icons and direct product links.

#### [MODIFY] [Footer.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/components/Footer.astro)
- Standardize labels to "Ürünler" and "Çözümler".
- Remove "Lokalizasyon" and "Roll-out" links.

### 3. Core Pages
#### [MODIFY] [index.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/index.astro)
- Update "Expertise" badges to "Product Capability" badges.
- Ensure all "Detaylı İncele" links point to product pages or a unified solutions explorer.

#### [MODIFY] [hizmetler.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hizmetler.astro)
- **Major Refactor**: Convert this into a "Solutions Overview" page.
- Remove sections: "AMS", "Outsourcing", "ERP Modernization (as a service)".
- Instead, showcase how the `eny` products solve these enterprise problems.

#### [DELETE] [lokalizasyon.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/lokalizasyon.astro)
- This content is currently consultancy-heavy. Relevant regulatory compliance content will be moved to the "e-Government Series" product descriptions.

#### [MODIFY] [hakkimizda.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hakkimizda.astro)
- Remove Harezm consultancy history if present.
- Define `eny` as the "Finance Infrastructure Firm".

## Open Questions

> [!NOTE]
> 1. Should we keep the "Sektörler" (Industries) page? It is somewhat product-agnostic but useful for showcasing product fit.
> 2. For the "Ürünler" menu, should we group them by "Regtech" vs "Fintech" vs "E-commerce" categories?

## Verification Plan

### Automated Tests
- `npm run build` to ensure no broken links or missing translation keys.

### Manual Verification
- Visual audit of the Header/Footer to ensure no "Consultancy" or "Service" vibe.
- Check /hizmetler (or the new /cozumler) to ensure it only lists product-based value propositions.
- Verify `translations.ts` doesn't contain "danışmanlık" (consultancy) or "dış kaynak" (outsourcing).
