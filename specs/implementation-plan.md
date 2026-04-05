# Eny Platform UX Finalization & Identity Update

## User Review Required
- **Logo Transition**: Moving from SVG-text logo to the provided PNG assets for better brand continuity.
- **Header Visibility**: Fixing subpage navigation accessibility.
- **Vertical Text Bug**: Resolving the layout issue on secondary pages.

## Proposed Changes

### Phase 1: Brand Identity Update (Logo & Favicon)
The user has provided high-quality PNG logos. I will transition from SVG-text logos to these assets.

#### Assets Setup
- Copy `b:\DEV\eny.com.tr\assets\logo\any_logo_with text (1).png` -> `public/images/logo/eny_logo_light.png`
- Copy `b:\DEV\eny.com.tr\assets\logo\any_logo_with text (2).png` -> `public/images/logo/eny_logo_dark.png`
- Copy `b:\DEV\eny.com.tr\assets\logo\eny_logo_square (1).png` -> `public/favicon.png`

#### [MODIFY] Header.astro
- Update logo section to use `<img>` tags pointing to the new PNG assets.
- Ensure proper sizing for retina displays.

#### [MODIFY] Footer.astro
- Update brand column with the new logos.

#### [MODIFY] Layout.astro
- Update `<head>` to use the new `favicon.png`.

### Phase 2: Final UX Bug Squashing

#### 1. Header Visibility on Subpages
- **Issue**: Header is hidden on subpages until scroll.
- **Fix**: Refine `.forced-show` logic in `Header.astro` and ensure CSS specificity in `global.css`.

#### 2. Vertical Text (Dikey Metin) Bug
- **Issue**: Hero paragraphs on subpages (like /lokalizasyon) are splitting into vertical words.
- **Root Cause**: Likely a SplitText script in `index.astro` or `Layout.astro` targeting too broad or a leakage in `global.css`.
- **Fix**: Scoped targeting of animation scripts to only the `IntroAnimation` component or specific homepage hero IDs.

## Verification Plan
1.  **Visual Audit**: Verify new logos look sharp in both themes.
2.  **Navigation Check**: Verify header is visible on `/hizmetler`, `/lokalizasyon`, etc.
3.  **Layout Check**: Verify `/lokalizasyon` hero text is horizontal.
