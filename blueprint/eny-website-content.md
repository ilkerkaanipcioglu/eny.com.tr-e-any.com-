# eny.com.tr — Web Sitesi İçerik Dökümanı

> **Marka:** eny (eny.com.tr / e-any.com)  
> **Slogan:** *The Future of Financial Intelligence.*  
> **Dil:** Türkçe (Birincil) / İngilizce (İkincil)  
> **Format:** Tam web sitesi içerik mimarisi + tasarım kılavuzu

---

## 🎨 TASARIM SİSTEMİ & KİMLİK

### Renk Paleti

| Renk Adı        | HEX Kodu  | Kullanım Alanı                            |
| :-------------- | :-------- | :---------------------------------------- |
| Neon Lime       | `#D0FD17` | CTA butonları, vurgu çizgileri, ikonlar   |
| Deep Carbon     | `#0A0F0D` | Ana arka plan, primary surface            |
| Carbon Mid      | `#111A13` | Kart arka planları, ikincil yüzeyler      |
| Antik Gold      | `#D4AF37` | Prestij aksan, pricing başlıkları         |
| Gümüş Buz       | `#E8EDE9` | Body metin, açıklamalar                   |
| Soluk Orman     | `#2A3D2E` | Ayırıcı çizgiler, border'lar              |
| Saf Beyaz       | `#FFFFFF` | Ters kontrastlı bölümler (özel kullanım) |

### Tipografi

```
BAŞLIK FONTLARİ
─────────────────────────────────────
Font: Syne (Google Fonts)
Ağırlık: 700 (Bold), 800 (ExtraBold)
Kullanım: H1, H2, hero başlıklar, büyük sloganlar
Karakter: Otoriter, geniş, geleceği çağrıştıran

VERİ / KOD / TABlo FONTLARİ
─────────────────────────────────────
Font: JetBrains Mono (Google Fonts)
Ağırlık: 400 (Regular), 600 (SemiBold)
Kullanım: Metrikler, sayılar, badge'ler, kod blokları
Karakter: Teknik, kesin, güvenilir

BODY / AÇIKLAMA FONTLARİ
─────────────────────────────────────
Font: Syne (400 Regular)
Kullanım: Paragraflar, açıklamalar, madde listeler
Karakter: Tutarlı marka kimliği

IMPORT KODU (HTML <head>)
─────────────────────────────────────
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
```

### CSS Değişkenleri (Design Tokens)

```css
:root {
  /* Renkler */
  --color-bg:          #0A0F0D;
  --color-surface:     #111A13;
  --color-border:      #2A3D2E;
  --color-lime:        #D0FD17;
  --color-gold:        #D4AF37;
  --color-text:        #E8EDE9;
  --color-text-muted:  #6B7A6D;
  --color-white:       #FFFFFF;

  /* Tipografi */
  --font-display: 'Syne', sans-serif;
  --font-mono:    'JetBrains Mono', monospace;

  /* Boyutlar */
  --radius-sm:   6px;
  --radius-md:   12px;
  --radius-lg:   20px;
  --radius-full: 9999px;

  /* Spacing */
  --space-section: 120px;
  --space-block:   64px;
  --max-width:     1280px;
}
```

### Tasarım Prensipleri

- **Dark Mode Dominant:** Tüm site derin karbon (#0A0F0D) zemin üzerine kurulur.
- **Neon Aksanlar:** Lime (#D0FD17) yalnızca kritik noktalarda kullanılır — her yerde değil.
- **Minimalist Yoğunluk:** Boşluk bolluğu; ama hiçbir alan boşa harcanmaz.
- **Sıfır Sürtünme:** Her CTA anında görünür, her aksiyon tek tıkla ulaşılabilir.
- **Mikro Animasyonlar:** Hover'da yumuşak transform, scroll'da staggered reveal, cursor glow efekti.

---

## 📄 SAYFA MİMARİSİ

```
eny.com.tr
│
├── / (Ana Sayfa)
├── /hizmetler
│   ├── /e-donusum
│   │   ├── /e-fatura
│   │   ├── /e-defter
│   │   ├── /e-irsaliye
│   │   ├── /e-arsiv
│   │   └── /e-devlet-entegrasyonlari
│   ├── /finansal-teknolojiler
│   │   ├── /e-tahsilat
│   │   ├── /e-odeme
│   │   └── /e-dbs
│   └── /e-ticaret
│       ├── /altyapi
│       ├── /odeme-sistemleri
│       └── /marketplace
├── /cozumler
│   ├── /erp-entegrasyonu
│   └── /kucuk-isletmeler
├── /hakkimizda
├── /iletisim
└── /demo-talebi
```

---

## 🏠 ANA SAYFA (/)

### SEO Meta

```
title: eny — Yeni Nesil Finansal İşletim Sistemi | e-Dönüşüm & Fintech
description: e-Fatura, e-Defter, e-Tahsilat, e-Ödeme ve e-DBS çözümleriyle finansal süreçlerinizi tek platformda yönetin. Yapay zeka destekli, banka güvenceli.
keywords: e-fatura, e-dönüşüm, e-tahsilat, e-ödeme, fintech, eny, dijital fatura
```

---

### BÖLÜM 1 — HERO

**[Navigasyon Barı]**

```
Logo: eny  [Lime nokta animasyonu]

Navigasyon Linkleri:
  Hizmetler  |  Çözümler  |  Entegrasyonlar  |  Hakkımızda  |  İletişim

Sağ CTA:
  [ Demo Talep Et ]   ← Lime arka planlı, siyah metin
```

**[Hero Başlık Bloğu]**

```
[Küçük badge — JetBrains Mono, Lime]
  ◆ Fintech × Regtech × E-Commerce

[Ana Başlık — Syne ExtraBold, çok büyük]
  Finansın Yeni
  İşletim Sistemi

[Alt Başlık — Syne Regular, soluk gümüş]
  Karmaşık süreçler görünmez olduğunda,
  iş mükemmelleşir. eny ile e-dönüşüm,
  tahsilat ve ödemeleri tek platformdan yönetin.

[CTA Grubu]
  [ Hemen Başlayın →  ]   [ Demo İzleyin ▶ ]
  (Lime / Solid)           (Şeffaf / Outline)

[Güven Göstergesi — JetBrains Mono, küçük]
  Banka Seviyesinde Güvenlik  ·  GİB Onaylı  ·  7/24 Uzman Destek
```

**[Hero Görsel / Animasyon Alanı]**
> Sağ tarafta veya arka planda: Karanlık ekranda akan finansal veri dashboard mockup'ı. Lime renkli animasyonlu ödeme akışı çizgileri. Parallax efektiyle hareket eden metrik kartları.

---

### BÖLÜM 2 — GÜVEN BANDI (LOGO / METRİK BANDI)

```
[Yatay kayan bant — Soluk görünümlü, sürekli loop]

  Metrikler (JetBrains Mono):
  
  ◆ 10.000+  İşletme        ◆ 135+  Para Birimi
  ◆ 20+      Banka Entegrasyonu  ◆ %98   Nakit Tahmin Doğruluğu
  ◆ 7/24     VIP Destek     ◆ 0      Manuel Hata Riski
```

---

### BÖLÜM 3 — ÜRÜN GRUPLARI (ANA HİZMETLER)

**[Bölüm Başlığı]**
```
[Üst etiket — JetBrains Mono, Lime]
  01 / PLATFORM

[H2 — Syne ExtraBold]
  Her Finansal Süreç.
  Tek Platform.

[Açıklama — Syne Regular, muted]
  Regtech'ten fintech'e, e-ticaretten treasury yönetimine —
  ihtiyaç duyduğunuz her çözüm eny çatısı altında.
```

**[Ürün Kartları — 2×2 Grid veya Tab Navigasyonlu]**

---

**Kart 1: Regtech Elite — e-Dönüşüm**
```
[İkon: Belge / Yasal]  [Etiket: JetBrains Mono]  REGTECH
─────────────────────────────────────────────────────────
e-Dönüşüm Serisi
─────────────────────────────────────────────────────────
Yasal zorunlulukları operasyonel avantaja dönüştürün.
GİB uyumlu, otomatik güncellemeli, sıfır hata toleranslı.

  →  e-Fatura & e-Arşiv
  →  e-Defter
  →  e-İrsaliye
  →  Regülasyon Asistanı

[Alt CTA — Lime metin]  Detaylı İncele →
```

---

**Kart 2: Money Orchestration — Fintech**
```
[İkon: Para Akışı]  [Etiket: JetBrains Mono]  FINTECH
─────────────────────────────────────────────────────────
Akıllı Tahsilat & Ödeme
─────────────────────────────────────────────────────────
Paranın hareketini bir senfoni gibi yönetin.
Omni-channel tahsilat, akıllı yönlendirme, anlık mutabakat.

  →  Global e-Tahsilat
  →  e-Ödeme & TÖS
  →  e-DBS
  →  Açık Bankacılık (e-Ekstre)

[Alt CTA — Lime metin]  Detaylı İncele →
```

---

**Kart 3: E-Commerce Pro**
```
[İkon: Alışveriş]  [Etiket: JetBrains Mono]  E-TİCARET
─────────────────────────────────────────────────────────
Yeni Nesil Ticaret Çözümleri
─────────────────────────────────────────────────────────
Dijital mağazanızı global bir finans merkezine dönüştürün.
One-Click Pay, fraud koruması ve marketplace desteğiyle.

  →  Checkout Excellence
  →  Abonelik & Tekrarlı Ödemeler
  →  Fraud Protection (AI)
  →  Marketplace Split Payment

[Alt CTA — Lime metin]  Detaylı İncele →
```

---

**Kart 4: Treasury Intelligence**
```
[İkon: Grafik / Analytics]  [Etiket: JetBrains Mono]  TREASURY
─────────────────────────────────────────────────────────
Nakit Akışı & Finansal Analitik
─────────────────────────────────────────────────────────
Veriyi karara, kararı kâra dönüştürün.
%98 doğrulukla nakit projeksiyonu ve risk analitiği.

  →  Nakit Akışı Projeksiyonu (AI)
  →  Yönetim Kurulu Raporları
  →  Müşteri & Bayi Risk Analitiği

[Alt CTA — Lime metin]  Detaylı İncele →
```

---

### BÖLÜM 4 — NEDEN ENY? (FARK YARATAN ÖZELLİKLER)

**[Bölüm Başlığı]**
```
[Üst etiket — JetBrains Mono, Lime]
  02 / FARK

[H2 — Syne ExtraBold]
  Finansın Yeni
  Anayasası

[Açıklama — Syne Regular, muted]
  Teknolojik üstünlüğümüz sizi rakiplerinizden
  yıllar değil, çağlar ileride tutar.
```

**[Özellik Satırları — Yatay Liste, İkonlu]**

```
┌─────────────────────────────────────────────────────────────────┐
│  🔒  Zero-Trust Security                                        │
│      Verileriniz sadece şifrelenmez; parçalanarak farklı        │
│      coğrafi konumlarda saklanır. Askeri düzeyde koruma.        │
├─────────────────────────────────────────────────────────────────┤
│  ⚡  API-First Architecture                                     │
│      Dünyanın en kapsamlı dokümantasyonuna sahip,               │
│      en esnek ve en hızlı API yapısı.                           │
├─────────────────────────────────────────────────────────────────┤
│  🌐  Cross-Border Capability                                    │
│      135+ para birimiyle ödeme alın. Sınır tanımayan            │
│      küresel ödeme altyapısı.                                   │
├─────────────────────────────────────────────────────────────────┤
│  💬  24/7 VIP Uzman Destek                                     │
│      Bot değil, finans ve teknoloji uzmanı danışman.           │
│      Her sorun için gerçek bir çözüm ortağı.                   │
├─────────────────────────────────────────────────────────────────┤
│  🤖  Yapay Zeka Entegrasyonu                                   │
│      Hata denetiminden nakit projeksiyonuna,                    │
│      tüm süreçlerde AI destekli karar zekası.                  │
├─────────────────────────────────────────────────────────────────┤
│  🔗  Tek Entegrasyon, Tüm Bankalar                              │
│      20+ banka ve ödeme kuruluşuna tek API bağlantısıyla       │
│      ulaşın. Smart Routing ile en iyi rota otomatik seçilir.   │
└─────────────────────────────────────────────────────────────────┘
```

---

### BÖLÜM 5 — ERP ENTEGRASYONU

**[Bölüm Başlığı]**
```
[Üst etiket — JetBrains Mono, Lime]
  03 / ENTEGRASYON

[H2 — Syne ExtraBold]
  Mevcut Sisteminizle
  Kusursuz Çalışır

[Açıklama — Syne Regular, muted]
  SAP başta olmak üzere tüm ERP sistemleriyle
  native entegrasyon. Ya da sıfırdan, kendi kendine yeten
  bir finansal işletim sistemi olarak kullanın.
```

**[İki Kolon Karşılaştırması]**

```
ERP KULLANANLAR İÇİN              ERP KULLANMAYANLAR İÇİN
──────────────────────            ──────────────────────────────
✓ SAP tam uyumlu                  ✓ Hızlı kurulum (< 1 gün)
✓ Diğer ERP'lerle entegrasyon     ✓ Kullanımı kolay arayüz
✓ API-first mimari                ✓ Tüm süreçler tek panelde
✓ Veri senkronizasyonu            ✓ ERP'ye gerek yok
✓ Gerçek zamanlı akış             ✓ Hemen başlayın

[CTA]  Entegrasyon Dökümanı →     [CTA]  Ücretsiz Deneyin →
```

---

### BÖLÜM 6 — SOSYAL KANIT / REFERANS

**[Bölüm Başlığı]**
```
[Üst etiket — JetBrains Mono, Lime]
  04 / GÜVEN

[H2 — Syne ExtraBold]
  İşletmeler eny'e
  Neden Güveniyor?
```

**[Metrik Kartları — Yatay 4'lü Grid]**

```
┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
│  10.000+    │  │  %99.99     │  │  < 2 dk     │  │  135+       │
│  İşletme   │  │  Uptime     │  │  Ortalama   │  │  Para       │
│  Güveniyor  │  │  Garantisi  │  │  Entegrasyon│  │  Birimi     │
│             │  │             │  │  Süresi     │  │             │
│  [JB Mono] │  │  [JB Mono] │  │  [JB Mono] │  │  [JB Mono] │
└─────────────┘  └─────────────┘  └─────────────┘  └─────────────┘
```

**[Müşteri Yorumları — Carousel]**

```
Yorum 1:
"eny'yi kullanmaya başladıktan sonra e-fatura süreçlerimiz
tamamen otomatikleşti. Manuel hatalar sıfıra indi."
— Operasyon Müdürü, Üretim Sektörü

Yorum 2:
"Bayi tahsilatlarımızı tek panelden yönetmek inanılmaz bir
kolaylık sağladı. Nakit akışımız artık tahmin edilebilir."
— CFO, Dağıtım Şirketi

Yorum 3:
"API entegrasyonu için bir saatimizi bile almadı.
Teknik dokümantasyon gerçekten mükemmel."
— CTO, Fintech Startup
```

---

### BÖLÜM 7 — CTA / KAPANIŞ

```
[Büyük, tam ekran bölüm — Lime arka plan veya Lime çerçeveli]

[H2 — Syne ExtraBold, Siyah veya Karbon]
  Finansal Dönüşüme
  Bugün Başlayın.

[Alt metin — Syne Regular]
  Ücretsiz demo ile eny'yi keşfedin.
  Kurulum gerektirmez, kredi kartı istenmez.

[CTA Butonları]
  [ Demo Talep Et →  ]   [ Uzmanla Konuş ]
  (Siyah / Solid)        (Beyaz Outline)

[Alt güven notu — JetBrains Mono, küçük]
  GİB Onaylı  ·  Banka Güvenceli  ·  KVKK Uyumlu
```

---

### BÖLÜM 8 — FOOTER

```
[Logo: eny]
The Future of Financial Intelligence.

Hizmetler                 Çözümler              Şirket
─────────                 ────────              ──────
e-Fatura                  ERP Entegrasyonu      Hakkımızda
e-Defter                  Küçük İşletmeler      İletişim
e-İrsaliye                E-ticaret             Gizlilik Politikası
e-Arşiv                   API Dökümanı          KVKK
e-Tahsilat                                      Kariyer
e-Ödeme
e-DBS

────────────────────────────────────────────────────────────────
© 2025 eny — eny.com.tr | e-any.com
Tüm hakları saklıdır.

GİB Onaylı Hizmet Sağlayıcı  ·  ISO 27001  ·  PCI-DSS Uyumlu
```

---

## 📑 HİZMET SAYFASI: E-DÖNÜŞÜM (/hizmetler/e-donusum)

### SEO Meta
```
title: e-Dönüşüm Çözümleri — e-Fatura, e-Defter, e-İrsaliye, e-Arşiv | eny
description: GİB onaylı e-Fatura, e-Defter, e-İrsaliye ve e-Arşiv çözümleriyle yasal uyumluluğu otomatikleştirin. Yapay zeka destekli hata denetimi ve anlık güncelleme.
```

### İçerik

**[Hero]**
```
[Etiket — JetBrains Mono, Lime]
  REGTECH ELİTE

[H1 — Syne ExtraBold]
  Yasal Zorunluluk mu?
  Artık Stratejik Avantaj.

[Açıklama]
  GİB uyumlu e-dönüşüm altyapımız, sizi
  düzenleyici değişikliklerden her zaman bir adım önde tutar.
  Otomatik güncelleme. Sıfır hata. Tam uyum.
```

---

**e-Fatura & e-Arşiv**
```
Sadece fatura değil: Finansal zeka.

Yapay zeka destekli hata denetimi, otomatik kategorizasyon
ve anlık maliyet analizini tek paket içinde sunan
muhasebe çözümü.

✓ GİB entegreli, otomatik iletim
✓ AI ile hata önleme ve kategorizasyon
✓ Anlık maliyet ve KDV analizi
✓ e-Arşiv ile yasal saklama garantisi
✓ ERP ve muhasebe yazılımlarıyla tam uyum

[CTA]  Demo İste →
```

---

**e-Defter**
```
Verileriniz güvende. Her zaman, her yerde.

Dünyanın en güvenli bulut sunucularında,
zaman damgalı ve mühürlü olarak saklanan
dijital muhasebe defterleriniz.

✓ Zaman damgalı, değiştirilemez kayıtlar
✓ Denetim süreçleri tek tıkla paylaşım
✓ Otomatik BA-BS mutabakatı
✓ Çoklu kullanıcı ve yetkilendirme

[CTA]  Demo İste →
```

---

**e-İrsaliye**
```
Lojistiği dijital haritaya taşıyın.

Kağıt karmaşasına son verin. Sevkiyatlarınızı
gerçek zamanlı takip edin, müşterilerinize
anlık teslimat onayı gönderin.

✓ Gerçek zamanlı sevkiyat takibi
✓ Anlık GİB iletimi ve onayı
✓ Depo ve lojistik sistemi entegrasyonu
✓ Mobil uyumlu sürücü uygulaması

[CTA]  Demo İste →
```

---

**Regülasyon Asistanı**
```
Gelecek her zaman hazır.

GİB ve diğer yasal otoritelerdeki güncellemeleri
anlık takip eden, sisteminizi otomatik olarak
uyumlu hale getiren akıllı altyapı.

✓ 7/24 mevzuat izleme
✓ Otomatik sistem güncelleme
✓ Uyumsuzluk uyarı mekanizması
✓ Geçmiş mevzuat arşivi

[CTA]  Demo İste →
```

---

## 💳 HİZMET SAYFASI: FİNANSAL TEKNOLOJİLER (/hizmetler/finansal-teknolojiler)

### SEO Meta
```
title: e-Tahsilat, e-Ödeme ve e-DBS Çözümleri | eny Finansal Teknolojiler
description: Omni-channel e-tahsilat, akıllı ödeme yönlendirme ve e-DBS ile nakit akışınızı güvence altına alın. 20+ banka entegrasyonu, tek platform.
```

### İçerik

**[Hero]**
```
[Etiket — JetBrains Mono, Lime]
  MONEY ORCHESTRATİON

[H1 — Syne ExtraBold]
  Paranın Hareketini
  Bir Senfoni Gibi Yönetin.

[Açıklama]
  Tahsilat, ödeme ve mutabakat süreçlerini
  tek akıllı platformda birleştirin.
  20+ banka, 135+ para birimi, sıfır sürtünme.
```

---

**e-Tahsilat (Omni-Channel)**
```
Her kanaldan tahsilat. Tek panelde kontrol.

Müşterilerinize nasıl ödeme yapmak isterlerse
o kanaldan ulaşın. Tüm tahsilatlar anında
eny panelinde görünür.

✓ Link ile Ödeme (WhatsApp / SMS / E-posta)
✓ QR Kod Ödeme (Fiziksel & Dijital)
✓ Bayi Tahsilat Portalı
✓ Sanal POS ve Fiziksel POS
✓ Anlık mutabakat ve raporlama

[CTA]  Demo İste →
```

---

**e-Ödeme & TÖS (Toplu Ödeme Sistemi)**
```
Akıllı ödeme. Düşük maliyet. Yüksek başarı.

Smart Routing teknolojimiz, her ödemeyi
otomatik olarak en düşük komisyonlu veya
en yüksek başarı oranlı bankaya yönlendirir.

✓ 20+ banka ve ödeme kuruluşuyla tek entegrasyon
✓ Smart Routing ile otomatik banka seçimi
✓ Toplu ödeme (TÖS) desteği
✓ Gerçek zamanlı ödeme durum takibi
✓ Otomatik hata yönetimi ve retry

[CTA]  Demo İste →
```

---

**e-DBS (Doğrudan Borçlandırma Sistemi)**
```
Banka garantisiyle tahsilat. Manuel risk sıfır.

Geniş bayi ağınız için otomatik borçlandırma.
Her tahsilat banka güvencesiyle gerçekleşir,
nakit akışınız her zaman öngörülebilir olur.

✓ Banka garantili otomatik tahsilat
✓ Bayi limit ve risk yönetimi
✓ Gecikme uyarıları ve otomatik takip
✓ Muhasebe entegrasyonu

[CTA]  Demo İste →
```

---

**e-Ekstre (Açık Bankacılık)**
```
Tüm banka hareketleri. Tek ekranda.

Açık bankacılık altyapımız sayesinde tüm
banka hesap hareketleriniz saniyeler içinde
ERP sisteminize akar. Manuel veri girişi devri kapandı.

✓ Çoklu banka hesabı bağlantısı
✓ ERP'ye otomatik veri aktarımı
✓ Anlık bakiye ve hareket takibi
✓ Kategori bazlı harcama analizi

[CTA]  Demo İste →
```

---

## 🛒 HİZMET SAYFASI: E-TİCARET (/hizmetler/e-ticaret)

### SEO Meta
```
title: E-Ticaret Altyapısı ve Ödeme Çözümleri | eny E-Commerce Pro
description: Hızlı checkout, fraud koruması, marketplace split payment ve abonelik yönetimiyle e-ticaret mağazanızı global bir finansal merkeze dönüştürün.
```

### İçerik

**[Hero]**
```
[Etiket — JetBrains Mono, Lime]
  E-COMMERCE PRO

[H1 — Syne ExtraBold]
  Dijital Mağazanızı
  Global Finans Merkezine
  Dönüştürün.

[Açıklama]
  Dünya standartlarında checkout deneyimi,
  AI tabanlı fraud koruması ve esnek marketplace
  çözümleriyle satışlarınızı büyütün.
```

---

**Checkout Excellence**
```
Dünyanın en hızlı ödeme sayfası.

Her saniye önemlidir. Her milisaniye daha hızlı
yüklenen ödeme sayfanız, daha yüksek dönüşüm
oranı demektir.

✓ One-Click Pay — Tekrar eden müşteri için tek tık
✓ 3D Secure 2.0 ile güvenli ödeme
✓ Mobil öncelikli, duyarlı tasarım
✓ 50+ ödeme yöntemi desteği
✓ Sepet terk oranını minimize eden akış

[CTA]  Demo İste →
```

---

**Abonelik & Tekrarlı Ödemeler**
```
Tahsilatı otomatikleştirin, geliri sabitleyin.

SaaS, içerik platformları veya her türlü
abonelik modeli için otomatik faturalama
ve tahsilat döngüsü.

✓ Esnek abonelik modelleri (aylık, yıllık, özel)
✓ Otomatik yenileme ve bildirim
✓ Başarısız ödeme retry mantığı
✓ Abone yönetim paneli

[CTA]  Demo İste →
```

---

**Fraud Protection**
```
Sahte işlemler gerçekleşmeden durur.

Makine öğrenmesi tabanlı risk motorumuz,
anormal işlem kalıplarını gerçek zamanlı
analiz eder ve şüpheli işlemleri anında bloke eder.

✓ AI destekli anomali tespiti
✓ Gerçek zamanlı risk skorlaması
✓ Özelleştirilebilir kural motoru
✓ Chargeback koruması

[CTA]  Demo İste →
```

---

**Marketplace Çözümleri**
```
Alt satıcı ödemeleri otomatik, yasal, anında.

Karmaşık split payment mantığını
saniyeler içinde, mevzuata tam uygun
şekilde gerçekleştirin.

✓ Çok taraflı ödeme dağıtımı (Split Payment)
✓ Alt satıcı onboarding ve KYC
✓ Platform komisyonu otomasyonu
✓ Yasal uyumluluk garantisi

[CTA]  Demo İste →
```

---

## ℹ️ HAKKIMIZDA (/hakkimizda)

### SEO Meta
```
title: Hakkımızda — eny'nin Hikayesi ve Vizyonu
description: eny, işletmelerin finansal ve dijital dönüşüm süreçlerini sadeleştirmek için kurulmuş yenilikçi bir fintech markasıdır. Harezm ekosisteminin prestijli halkası.
```

### İçerik

**[Hero]**
```
[Etiket — JetBrains Mono, Lime]
  BİZ KİMİZ

[H1 — Syne ExtraBold]
  Finansın Yeni
  Anayasasını Yazıyoruz.

[Açıklama — Syne Regular]
  eny, karmaşık finansal ve yasal süreçleri
  işletmeler için tamamen görünmez kılmak amacıyla
  kurulmuş bir teknoloji markasıdır.
```

---

**Misyon**
```
[H2 — Syne Bold]
Misyonumuz

İşletmelerin enerjisini büyümeye harcaması için,
finansal operasyonların yükünü tamamen ortadan kaldırmak.

Fatura kesmekten banka mutabakatına, tahsilattan ödemeye —
tüm bu süreçler arka planda, sessizce, mükemmel şekilde işler.
Siz yalnızca işinize odaklanırsınız.
```

---

**Vizyon**
```
[H2 — Syne Bold]
Vizyonumuz

Türkiye'nin en güvenilir, global ölçekte rekabetçi
finansal işletim sistemi olmak.

Apple'ın tasarım anlayışı, Stripe'ın mühendislik
mükemmeliyeti ve banka güvencesiyle harmanlanan bir platform.
```

---

**Değerlerimiz**
```
[H2 — Syne Bold]
Değerlerimiz

  ◆ Güvenilirlik
    Verileriniz, sistemleriniz ve süreçleriniz —
    her zaman güvende. Uzlaşma yok.

  ◆ Sadelik
    Karmaşıklığı biz çözeriz. Size sade, hızlı,
    sorunsuz bir deneyim sunarız.

  ◆ Yenilik
    Regülasyonlar değişir, teknoloji ilerler.
    Biz her zaman bir adım öndeyiz.

  ◆ Ortaklık
    Müşterilerimizi müşteri olarak değil,
    uzun vadeli iş ortağı olarak görürüz.
```

---

**Teknoloji Felsefesi**
```
[H2 — Syne Bold]
Teknoloji Felsefemiz

Biz sadece kod yazmıyoruz.
Finansın yeni anayasasını oluşturuyoruz.

  Zero-Trust Security     →  Veri güvenliğinde askeri standart
  API-First Architecture  →  Her sisteme açık, esneklik birinci
  AI-Powered Processes    →  Öğrenen, tahmin eden, optimize eden
  Cross-Border Ready      →  135+ para birimi, global ölçek
```

---

## 📞 İLETİŞİM (/iletisim)

### SEO Meta
```
title: İletişim — eny ile Tanışın | Demo & Satış
description: eny ekibiyle iletişime geçin. Demo talebi, satış görüşmesi veya teknik destek için buradayız.
```

### İçerik

**[Hero]**
```
[Etiket — JetBrains Mono, Lime]
  İLETİŞİM

[H1 — Syne ExtraBold]
  Uzmanlarımız
  Hazır.

[Açıklama]
  Sorularınız için, demo talebiniz için
  veya sadece tanışmak için bize yazın.
  En geç 24 saat içinde dönüş garantisi.
```

---

**İletişim Bilgileri**
```
[Sol Kolon — İletişim Detayları]

  🌐  Web
      eny.com.tr

  📧  E-posta
      info@eny.com.tr

  📞  Telefon
      +90 (212) ___ __ __

  🏢  Adres
      [Harezm / eny Ofis Adresi]

  🕐  Çalışma Saatleri
      Pazartesi – Cuma: 09:00 – 18:00
      7/24 Teknik Destek mevcut

[Sağ Kolon — İletişim Formu]

  Ad Soyad         [_____________________]
  Şirket           [_____________________]
  E-posta          [_____________________]
  Telefon          [_____________________]
  Konu             [Demo Talebi ▼        ]
                    → Demo Talebi
                    → Satış Görüşmesi
                    → Teknik Destek
                    → İş Birliği
                    → Diğer
  Mesajınız        [_____________________]
                   [                     ]
                   [_____________________]

  [ Gönder →  ]  ← Lime buton
```

---

## 🚀 DEMO TALEP SAYFASI (/demo-talebi)

```
[H1 — Syne ExtraBold]
  Ücretsiz Demo
  Talep Edin.

[Açıklama]
  15 dakikada eny'nin tüm kapasitesini görün.
  Kurulum gerektirmez. Taahhüt yok.

[Form]
  Ad Soyad          [_____________________]
  Şirket            [_____________________]
  Sektör            [Seçin ▼             ]
  Çalışan Sayısı    [Seçin ▼             ]
  E-posta           [_____________________]
  Telefon           [_____________________]
  İlgilendiğiniz    [☐ e-Dönüşüm        ]
  Hizmetler:        [☐ e-Tahsilat        ]
                    [☐ e-Ödeme           ]
                    [☐ e-DBS             ]
                    [☐ E-ticaret         ]
                    [☐ ERP Entegrasyonu  ]

  [ Demo Talep Et →  ]

[Alt Not — JetBrains Mono, küçük, muted]
  GİB Onaylı  ·  KVKK Uyumlu  ·  En geç 24 saatte dönüş garantisi
```

---

## 📋 İÇERİK YAZIMI KURALLARI (Copywriting Guide)

### Ses Tonu (Brand Voice)

| Özellik          | Açıklama                                                    |
| :--------------- | :---------------------------------------------------------- |
| **Otoriter**     | Bilgi sahibi, güven veren, özgüvenli — kibarca değil net   |
| **Minimalist**   | Gereksiz kelime yok. Her cümle iş yapar.                   |
| **Prestijli**    | Kalabalığa değil, seçkinlere hitap eder                    |
| **Teknik ama sade** | Jargon açıklanır, basitleştirilmez — sadelik başarıdır |
| **Sıcak değil, güvende hissettiren** | Samimi ama asla şakacı değil        |

### Başlık Formülleri

```
✓ Soru → Cevap:     "Yasal Zorunluluk mu? Artık Stratejik Avantaj."
✓ Zıtlık:           "Daha Az İşlem. Daha Çok Kontrol."
✓ Sonuç Odaklı:     "Nakit Akışınızı %98 Doğrulukla Tahmin Edin."
✓ İddia:            "Finansın Yeni Anayasasını Yazıyoruz."
✓ Dönüşüm:         "Veriyi Karara, Kararı Kâra Dönüştürün."
```

### Yasaklı İfadeler

```
✗ "Finrota" veya herhangi bir iş ortağı ismi
✗ "Ucuz", "Bedava", "İndirim" — Prestij markası fiyat odaklı konuşmaz
✗ "Biz en iyiyiz" — İddia değil, kanıt konuşur
✗ Emoji aşırı kullanımı (yalnızca tablolarda, teknik listelerde)
✗ Pasif cümle yapısı — aktif, kısa, güçlü cümleler
✗ "Kullanıcı dostu" — Çok klişe; bunun yerine somut özellik yaz
```

---

## 🔧 TEKNİK NOTLAR

### Font Import

```html
<!-- HTML <head> içine eklenecek -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
```

### Temel Bileşen Stilleri

```css
/* BAŞLIKLAR */
h1, h2, h3 {
  font-family: var(--font-display);
  font-weight: 800;
  color: var(--color-white);
  line-height: 1.1;
  letter-spacing: -0.02em;
}

/* METRİKLER & KOD */
.metric, .badge, code, .mono {
  font-family: var(--font-mono);
  font-weight: 600;
  color: var(--color-lime);
}

/* BODY METİN */
p, li {
  font-family: var(--font-display);
  font-weight: 400;
  color: var(--color-text);
  line-height: 1.7;
}

/* CTA BUTON — PRİMARY */
.btn-primary {
  background: var(--color-lime);
  color: #000;
  font-family: var(--font-display);
  font-weight: 700;
  padding: 14px 28px;
  border-radius: var(--radius-full);
  border: none;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
}
.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 24px rgba(208, 253, 23, 0.4);
}

/* CTA BUTON — SECONDARY */
.btn-secondary {
  background: transparent;
  color: var(--color-text);
  font-family: var(--font-display);
  font-weight: 700;
  padding: 14px 28px;
  border-radius: var(--radius-full);
  border: 1px solid var(--color-border);
  cursor: pointer;
  transition: border-color 0.2s, color 0.2s;
}
.btn-secondary:hover {
  border-color: var(--color-lime);
  color: var(--color-lime);
}

/* KART */
.card {
  background: var(--color-surface);
  border: 1px solid var(--color-border);
  border-radius: var(--radius-lg);
  padding: 32px;
  transition: border-color 0.3s, transform 0.3s;
}
.card:hover {
  border-color: var(--color-lime);
  transform: translateY(-4px);
}
```

### Animasyon Tavsiyeleri

```css
/* Scroll Reveal — Staggered */
.reveal {
  opacity: 0;
  transform: translateY(24px);
  transition: opacity 0.6s ease, transform 0.6s ease;
}
.reveal.visible {
  opacity: 1;
  transform: translateY(0);
}

/* Lime Glow Pulse — CTA butonlar için */
@keyframes lime-pulse {
  0%, 100% { box-shadow: 0 0 0 0 rgba(208, 253, 23, 0); }
  50%       { box-shadow: 0 0 20px 6px rgba(208, 253, 23, 0.25); }
}
.btn-primary {
  animation: lime-pulse 3s ease infinite;
}
```

---

*Bu döküman, eny.com.tr web sitesinin tüm sayfa içeriklerini, tasarım sistemini, tipografi kılavuzunu ve geliştirici notlarını kapsamaktadır.*

**eny.com.tr | e-any.com**
*The Future of Financial Intelligence.*
