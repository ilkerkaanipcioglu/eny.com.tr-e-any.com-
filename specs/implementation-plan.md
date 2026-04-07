# Implementation Plan - Removing SAP Modules from eny.com.tr

The goal is to transition the `eny.com.tr` platform from an SAP-centric service provider to a general, software-agnostic financial technology and "e-product" platform. This involves removing all SAP module names (FI/CO, TRM, RE-FX, etc.) and branding (SAP Joule, SAP BTP, etc.) and replacing them with functional, high-level fintech terminology.

## User Review Required

> [!IMPORTANT]
> The 'Teknoloji' page will be significantly restructured to focus on "Agentic AI" and "Financial Operating Systems" rather than specific SAP products.
> 
> All services currently listed as "SAP [Module]" will be renamed to their functional equivalents (e.g., "SAP TRM" -> "Hazine & Risk Yönetimi").

## Proposed Changes

### [Teknoloji Page](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/teknoloji.astro)

#### [MODIFY] [teknoloji.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/teknoloji.astro)
- Replace "Modern SAP ekosistemi" with "Modern finansal teknoloji ekosistemi".
- Replace "S/4HANA Cloud" with "Bulut Tabanlı ERP Entegrasyonu".
- Replace "Joule (SAP AI)" with "Finansal Yapay Zeka Ajanları".
- Replace "SAP BTP" with "Düşük Kodlu (Low-Code) Platformlar".
- Replace "SAP Signavio" with "Süreç Madenciliği & Optimizasyon".
- Replace "SAP Build" with "Otonom İş Akışları".
- Generalize the "Insight" and "Vision" sections to remove SAP-specific product names while keeping the architectural wisdom.

---

### [Hizmetler Page](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hizmetler.astro)

#### [MODIFY] [hizmetler.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/hizmetler.astro)
- **Generalize Cards**:
    - "SAP FI & CO" -> "Finansal Muhasebe & Maliyet Yönetimi".
    - "S/4HANA" -> "Dijital ERP Dönüşümü".
    - "SAP RE-FX" -> "Gayrimenkul Portföy Yönetimi".
    - "SAP Cash Management" -> "Nakit ve Likidite Yönetimi".
    - "SAP TRM" -> "Hazine ve Risk Yönetimi".
    - "SAP Sabit Kıymet" -> "Varlık ve Sabit Kıymet Yönetimi".
    - "SAP Finansal Konsolidasyon" -> "Finansal Konsolidasyon ve Gruplama".
    - "SAP & OpenText" -> "Dijital Arşiv ve Fatura Otomasyonu".
    - "SAP Joule" -> "Yapay Zeka ve Otonom Finans Ajanları".
    - "SAP Eğitimleri" -> "Akademi ve Yetkinlik Merkezi".
    - "SAP Check-Up" -> "Sistem Optimizasyonu & Check-Up".

---

### [Sektörler Page](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/sektorler.astro)

#### [MODIFY] [sektorler.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/sektorler.astro)
- **Perakende**: Remove "SAP POSDTA" and "SAP Cash Management" mentions; replace with "POS Veri Ambarı ve Nakit Yönetim Entegrasyonu".
- **Üretim**: Remove "Material Ledger" and "SAP TRM"; replace with "Gelişmiş Maliyet Analizi ve Hazine Risk Yönetimi".
- **İnşaat**: Remove "SAP RE-FX"; replace with "Merkezi Gayrimenkul ve Kira Yönetimi".
- **Lojistik**: Remove "SAP ve OpenText VIM"; replace with "Akıllı Fatura ve Gider Yönetim Sistemleri".

---

### [Other Pages & Components]

#### [MODIFY] [kvkk.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/kvkk.astro)
- Remove mentions of "SAP projeleri" and "SAP danışmanlığı".

#### [MODIFY] [online-dbs.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/pages/online-dbs.astro)
- Generalize "SAP Treasury (TRM)" to "Kurumsal Hazine Yönetimi".

#### [MODIFY] [Header.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/components/Header.astro) and [Footer.astro](file:///b:/DEV/HAREZM_EKOSISTEMI/eny.com.tr/src/components/Footer.astro)
- Update any menu items that might still lead to "SAP" branded sections.

## Open Questions

- Should I keep the URLs like `/sap-trm` or redirect them to more general slugs like `/hazine-yonetimi`? 
- Are there any specific "e-product" names (like e-Fatura, e-DBS) that should be prioritized over the general descriptions?

## Verification Plan

### Automated Tests
- N/A (Build verification only)

### Manual Verification
- Verify that no "SAP" text remains on the site using `grep`.
- Review the modified pages visually (using browser tool) to ensure the layout remains premium and the new terminology fits perfectly.
