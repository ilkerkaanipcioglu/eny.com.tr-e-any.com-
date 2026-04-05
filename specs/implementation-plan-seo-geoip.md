# Implementation Plan - SEO Ecosystem & Geo-Location i18n

This plan outlines the changes to align `eny.com.tr` with the Harezm Ecosystem blueprint and implement automatic geo-location based language detection.

## User Review Required

> [!IMPORTANT]
> **Geo-IP Detection Service**: I propose using `ipapi.co` or `ip-api.com` (free tiers) for client-side detection. This requires a client-side fetch on the first visit. 
> **Redirection Logic**: Users from Turkey will be directed to the Turkish version (`/`), while all other users will be directed to the English version (`/en/`). 
> **Persistence**: A `eny-lang-pref` key will be stored in `localStorage` to remember manual selections and prevent unwanted auto-redirects after the first visit.

## Proposed Changes

### 1. Geo-Location & i18n Logic

#### [MODIFY] [Layout.astro](file:///b:/DEV/eny.com.tr/src/layouts/Layout.astro)
- Add a blocking script in the `<head>` to handle geo-redirection.
- Logic: 
  1. Check `localStorage` for `eny-lang-pref`.
  2. If exists, do nothing (respect user choice).
  3. If not exists, fetch country from IP API.
  4. If country is NOT 'TR' and current path is NOT `/en/*`, redirect to `/en/`.
  5. If country IS 'TR' and current path IS `/en/*`, redirect to `/`.
  6. Store result in `localStorage`.

#### [MODIFY] [Header.astro](file:///b:/DEV/eny.com.tr/src/components/Header.astro)
- Update language switcher links to include an `onclick` handler that sets `localStorage.setItem('eny-lang-pref', 'en' | 'tr')`. This ensures the auto-redirect doesn't override manual choices.

### 2. SEO & Ecosystem Integration

#### [MODIFY] [Footer.astro](file:///b:/DEV/eny.com.tr/src/components/Footer.astro)
- Refine the "eny Ecosystem" section to link to external Harezm brands:
    - **Harezm**: Trust/Corporate (`harezm.com`)
    - **e-any.info**: Knowledge/Blog hub
    - **e-any.online**: Free tools
    - **AgentAndBot**: AI & Future tech
    - **ipcioglu.com**: Founder authority
- Use consistent styling (grayscale icons with hover effects).

#### [MODIFY] [index.astro](file:///b:/DEV/eny.com.tr/src/pages/index.astro) (TR)
- Ensure the title and meta-tags emphasize "Turkish Financial Operating System" and GİB compliance.

#### [MODIFY] [en/index.astro](file:///b:/DEV/eny.com.tr/src/pages/en/index.astro) (EN)
- Ensure title and meta-tags emphasize "Global Financial Infrastructure" and 135+ currency support.

### 3. Metadata & Technical SEO

#### [MODIFY] [Layout.astro](file:///b:/DEV/eny.com.tr/src/layouts/Layout.astro)
- Add `hreflang` tags for better multi-lingual SEO indexing.
- Ensure `title` and `description` are correctly localized.

## Open Questions

- **Specific Links**: Do you have the final URLs for `e-any.info`, `e-any.online`, etc., or should I use placeholders/best guesses based on the blueprint?
- **Redirection UX**: Should the redirect happen instantly in the head (faster but no UI) or with a small loading overlay? (Proposed: Instant in head for better SEO/UX).

## Verification Plan

### Automated Tests
- Use the browser subagent to:
    1. Verify that visiting `/` as a non-TR user (mocked) redirects to `/en/`.
    2. Verify that clicking the language switcher stops the auto-redirection.
    3. Check footer links for correctness.

### Manual Verification
- Verify the site's metadata using browser dev tools.
