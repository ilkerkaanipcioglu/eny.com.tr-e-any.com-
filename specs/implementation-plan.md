# Integration of E-Ödeme (Bulk Payment System)

This plan outlines the steps to add the **E-Ödeme / E-TÖS (Toplu Ödeme Sistemi)** product to the `eny.com.tr` platform, including multilingual support and visual consistency with other products like E-POS and E-DBS.

## User Review Required

> [!IMPORTANT]
> The product will be referred to as **E-Ödeme (Toplu Ödeme Sistemi)** in Turkish and **E-Payment (Bulk Payment System)** in English.

## Proposed Changes

### [Product Detail Pages]

#### [NEW] [e-payment.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/e-payment.astro)
*   Create the Turkish product detail page.
*   Use `ServiceDetailLayout` with the provided content (Multi-recipient transfers, simultaneous bank integration, approval workflows, ERP integration, etc.).

#### [NEW] [e-payment.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/en/e-payment.astro)
*   Create the English product detail page.
*   Translate the content into English as provided in the request.

---

### [Navigation and Grids]

#### [MODIFY] [Header.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/components/Header.astro)
*   Add **E-Ödeme Sistemi** / **E-Payment System** to the "Çözümler" (Solutions) mega menu.
*   Icon will be `payments` or `hub`.

#### [MODIFY] [hizmetler.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hizmetler.astro)
*   Add a card for E-Ödeme to the services grid.

#### [MODIFY] [services.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/en/services.astro)
*   Add a card for E-Payment to the English services grid.

#### [MODIFY] [urunler.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/urunler.astro)
*   Update the existing "e-Ödeme" card to point to `/e-payment` instead of `/iletisim`.
*   Update its description and label to match the new branding "E-Ödeme Sistemleri".

#### [MODIFY] [products.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/en/products.astro)
*   Update the existing "e-Payment" card to point to `/en/e-payment` instead of `/en/contact`.

## Verification Plan

### Manual Verification
*   Verify the existence and appearance of `/e-payment` and `/en/e-payment`.
*   Ensure navigation links in the header and footer work correctly.
*   Check that the services grids and product overview pages reflect the new links and branding.
