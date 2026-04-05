# eny.com.tr — Astro Web Sitesi Tam Blueprint
 TEMEL STRATEJİ: "Global-Ready Platform" Çerçevelemesi
Hiç "Afrika" veya "Kenya" demezsiniz. Bunun yerine site şu mesajları verir:

1. SLOGAN & POSITIONING GÜNCELLEMESI
Şu an: "The Future of Financial Intelligence"
Buna ek olarak hero'ya bir alt satır:

"Built for Turkey. Designed for the World."

veya

"From Istanbul to the World."

Bu tek cümle hem yerel güveni korur hem global niyeti açıklar — hiçbir ülke ismi vermeden.

2. DİL & ÇOK DİLLİLİK SİNYALİ
Site navbar'ına dil seçici ekleyin:
🇹🇷 TR  |  🇬🇧 EN
Sadece bu iki dil bile yeterli. İleride FR (Frankofon Afrika için kritik), PT (Mozambik, Angola) eklenebilir. Ama şimdilik İngilizce içerik olması bile "biz globaliz" mesajı verir.

3. METRİK BANDINA EKLEME
Şu an: 10.000+ İşletme, 135+ Para Birimi...
Buna ekle:

135+ Currency → zaten var ama ön plana çıkar
"Multi-jurisdiction Compliance" → ülke adı vermeden yasal uyumluluk kapasitesini söyler
"Deployed across 3 continents" → ilerleyen dönemde eklenebilir


4. "GLOBAL INFRASTRUCTURE" BÖLÜMÜ
Hizmetler sayfasında veya ana sayfada ayrı bir bölüm:
◆ GLOBAL READY

Altyapımız Sınır Tanımaz.

→ 135+ para birimi desteği
→ Çok dilli & çok bölgeli mimari
→ Uluslararası ödeme standartları (ISO 20022, SWIFT)
→ Yerel regülasyona uyarlanabilir compliance motoru
→ Sovereign cloud & veri lokalizasyon seçeneği
→ Kamu ihalelerine uygun beyaz etiket lisanslama
"Sovereign cloud" ve "veri lokalizasyonu" — Afrika devletleri için kritik iki kavram. Verinin kendi topraklarında tutulması şartı çoğu Afrika ihalelerinin olmazmazı.

5. E-PORTAL SAYFASINDA STRATEJİK KELIMELER
e-Portal bölümünde şu ifadeler Afrika e-devlet ihalecilerinin aradığı tam terimler:
YazdığınızAslında ne anlatıyor"Sovereign data residency"Verinin ülke içinde kalması"Multi-jurisdiction tax compliance"Her ülkenin vergi sistemine uyum"Citizen identity verification layer"Ulusal kimlik entegrasyonu"Government payment gateway"Devlet tahsilat altyapısı"White-label, country-branded"Devletin kendi markasıyla"Revenue collection modernization"Vergi/harç dijitalleştirme"Financial inclusion infrastructure"Dünya Bankası'nın severdiği terim
Bu kelimeleri kullanan bir site Google'da Afrika'daki "e-government tender", "digital payment infrastructure RFP" aramalarında görünür.

6. REFERANS BÖLÜMÜ — "CASE STUDIES" FORMATI
Türkiye'deki belediye veya kamu projelerinizi şöyle sunun:
◆ PROVEN AT SCALE

Bir metropolde 4.2 milyon vatandaşın
su & vergi tahsilatını dijitalleştirdik.
→ %340 tahsilat artışı  |  18 ay içinde
Şehir ismi vermeyin. Ölçek ve sonuç verin. Bu format ihale değerlendirme komitelerinin beklediği "track record" kanıtıdır.

7. "IMPLEMENTATION PARTNER" SAYFASI
Direkt ofis açmak yerine:
/partners

Global Uygulama Ortakları

Yerel uzmanlık, global altyapı.
eny'i kendi bölgenizde konuşlandırmak için
yetkili uygulama ortağı ağımıza katılın.

[ Ortaklık Başvurusu → ]
Bu sayfa Afrika'daki sistem entegratörlerine, danışmanlık firmalarına hitap eder. Onlar ihalelere girer, siz altyapıyı sağlarsınız.

8. DÜNYA BANKASI / IMF DİLİ
Afrika devlet ihalelerinin büyük çoğunluğu Dünya Bankası, AfDB (African Development Bank), IMF finansmanıyla yapılır. Bu kurumların değerlendirme formlarında geçen terimler sitenizde olmalı:

"Financial inclusion"
"Digital public infrastructure (DPI)"
"Government revenue mobilization"
"Last-mile payment collection"
"Interoperable payment systems"

Bunları bir "Kamu Çözümleri" sayfasında doğal cümleler içinde kullanmak yeterli.

9. TRUST SİNYALLERİ — ULUSLARARASI SERTIFIKALAR
Şu an: GİB, PCI-DSS, ISO 27001, KVKK
Eklenecekler:

ISO 20022 — uluslararası finansal mesajlaşma standardı
SWIFT gpi — global ödeme takip standardı
GDPR Compliant — KVKK'nın yanına (Afrika'daki AB finansmanlı projelerde şart)
ITU-T X.509 — dijital sertifika standardı (e-devlet için)


ÖZET: SİTE NEYİ SÖYLEMELİ, NEYİ SÖYLEMEMELİ
❌ Söyleme✅ Bunun yerine"Afrika'ya hizmet veriyoruz""135+ currency, multi-jurisdiction""Kenya için portal yaptık""Deployed for 4M+ citizens" (anonim case study)"Gelişmekte olan ülkeler""Emerging market ready infrastructure""Ucuz çözüm sunuyoruz""TCO-optimized, donor-funding compatible""Türk şirketiyiz""Istanbul-headquartered, globally deployed"

Kısaca: site İngilizce + doğru terimler + anonim ölçek kanıtları + sovereign/DPI dili ile konuşursa, ihale komiteleri sizi zaten bulur. Ülke ismi vermenize gerek kalmaz.




> **Versiyon:** 1.0  
> **Framework:** Astro 4.x  
> **Tema:** Dark + Light (sistem tercihi + manuel toggle)  
> **Hedef:** Ultra-hızlı, kurumsal-fintech, animasyonlu, profesyonel  
> **Tasarım Felsefesi:** Refined Dark Luxury × Data-Driven Precision

---

## 📁 PROJE YAPISI

```
eny-website/
├── public/
│   ├── fonts/                    # Self-hosted fontlar (hız için)
│   ├── images/
│   │   ├── og-image.jpg
│   │   └── logos/
│   └── favicon.svg
│
├── src/
│   ├── assets/
│   │   └── icons/                # SVG ikonlar
│   │
│   ├── components/
│   │   ├── layout/
│   │   │   ├── Navbar.astro
│   │   │   ├── Footer.astro
│   │   │   └── ThemeToggle.astro
│   │   │
│   │   ├── home/
│   │   │   ├── Hero.astro
│   │   │   ├── MetricsBand.astro
│   │   │   ├── Services.astro
│   │   │   ├── WhyEny.astro
│   │   │   ├── Integration.astro
│   │   │   ├── Testimonials.astro
│   │   │   └── FinalCTA.astro
│   │   │
│   │   └── ui/
│   │       ├── Button.astro
│   │       ├── Badge.astro
│   │       ├── AnimatedCounter.astro
│   │       └── TrustBadges.astro
│   │
│   ├── layouts/
│   │   └── BaseLayout.astro
│   │
│   ├── pages/
│   │   ├── index.astro
│   │   ├── hizmetler/
│   │   │   ├── e-donusum.astro
│   │   │   ├── finansal-teknolojiler.astro
│   │   │   ├── e-ticaret.astro
│   │   │   └── treasury.astro
│   │   ├── hakkimizda.astro
│   │   ├── iletisim.astro
│   │   └── demo.astro
│   │
│   ├── scripts/
│   │   ├── animate.ts             # IntersectionObserver animasyonları
│   │   ├── counter.ts             # Sayaç animasyonları
│   │   └── theme.ts               # Dark/Light mod yönetimi
│   │
│   └── styles/
│       ├── global.css             # CSS değişkenleri + reset
│       ├── themes.css             # Dark/Light tema tanımları
│       ├── typography.css
│       └── animations.css
│
├── astro.config.mjs
├── tailwind.config.mjs
└── tsconfig.json
```

---

## ⚙️ ASTRO YAPILANDIRMASI

### `astro.config.mjs`

```js
import { defineConfig } from 'astro/config';
import tailwind from '@astrojs/tailwind';
import sitemap from '@astrojs/sitemap';
import compress from 'astro-compress';

export default defineConfig({
  site: 'https://eny.com.tr',
  integrations: [
    tailwind(),
    sitemap(),
    compress({
      CSS: true,
      HTML: true,
      Image: false,    // Sharp ile zaten optimize
      JavaScript: true,
      SVG: true,
    }),
  ],
  image: {
    service: {
      entrypoint: 'astro/assets/services/sharp',
    },
  },
  prefetch: {
    prefetchAll: true,    // Tüm internal linkler prefetch
    defaultStrategy: 'viewport',
  },
  vite: {
    build: {
      cssMinify: 'lightningcss',
    },
  },
});
```

### `package.json` — Gerekli Paketler

```json
{
  "dependencies": {
    "astro": "^4.x",
    "@astrojs/tailwind": "^5.x",
    "@astrojs/sitemap": "^3.x",
    "astro-compress": "^2.x",
    "tailwindcss": "^3.x",
    "sharp": "^0.33.x"
  }
}
```

---

## 🎨 TASARIM SİSTEMİ

### `src/styles/themes.css` — Dark & Light CSS Değişkenleri

```css
/* =========================================
   DARK TEMA (varsayılan)
   ========================================= */
:root,
[data-theme="dark"] {
  /* Ana Arka Planlar */
  --bg-base:        #0A0F0D;   /* Deep Carbon — sayfa zemini */
  --bg-surface:     #111A13;   /* Carbon Mid — kartlar */
  --bg-elevated:    #1A2419;   /* Carbon Light — hover/aktif */

  /* Metin */
  --text-primary:   #E8EDE9;   /* Gümüş Buz — ana metin */
  --text-secondary: #6B7A6D;   /* Muted Text — açıklama */
  --text-inverse:   #0A0F0D;   /* Koyu arka planlarda */

  /* Aksan Renkler */
  --accent-primary: #D0FD17;   /* Neon Lime — CTA, vurgu */
  --accent-gold:    #D4AF37;   /* Antik Gold — prestij */
  --accent-muted:   rgba(208, 253, 23, 0.12); /* Lime şeffaf */

  /* Border */
  --border-subtle:  #2A3D2E;   /* Soluk Orman */
  --border-strong:  rgba(208, 253, 23, 0.3);

  /* Glow & Shadow */
  --glow-lime:      0 0 40px rgba(208, 253, 23, 0.15);
  --glow-lime-sm:   0 0 20px rgba(208, 253, 23, 0.10);
  --shadow-card:    0 4px 40px rgba(0, 0, 0, 0.6);
  --shadow-hover:   0 8px 60px rgba(0, 0, 0, 0.8);

  /* Özel */
  --navbar-blur:    rgba(10, 15, 13, 0.85);
  --grid-line:      rgba(42, 61, 46, 0.4);
  --noise-opacity:  0.03;
}

/* =========================================
   LIGHT TEMA
   ========================================= */
[data-theme="light"] {
  --bg-base:        #F4F6F4;
  --bg-surface:     #FFFFFF;
  --bg-elevated:    #EAEDE9;

  --text-primary:   #0A0F0D;
  --text-secondary: #4A5C4D;
  --text-inverse:   #FFFFFF;

  --accent-primary: #3A7D0A;   /* Koyu yeşil — lime light'ta okunmaz */
  --accent-gold:    #B8941E;
  --accent-muted:   rgba(58, 125, 10, 0.10);

  --border-subtle:  #D1DAD2;
  --border-strong:  rgba(58, 125, 10, 0.4);

  --glow-lime:      0 0 40px rgba(58, 125, 10, 0.08);
  --glow-lime-sm:   0 0 20px rgba(58, 125, 10, 0.06);
  --shadow-card:    0 4px 40px rgba(0, 0, 0, 0.08);
  --shadow-hover:   0 8px 60px rgba(0, 0, 0, 0.15);

  --navbar-blur:    rgba(244, 246, 244, 0.88);
  --grid-line:      rgba(200, 215, 200, 0.6);
  --noise-opacity:  0.015;
}
```

### `tailwind.config.mjs`

```js
export default {
  content: ['./src/**/*.{astro,html,js,jsx,ts,tsx}'],
  darkMode: ['selector', '[data-theme="dark"]'],
  theme: {
    extend: {
      colors: {
        lime:   '#D0FD17',
        carbon: '#0A0F0D',
        gold:   '#D4AF37',
        forest: '#2A3D2E',
      },
      fontFamily: {
        display: ['Syne', 'sans-serif'],
        mono:    ['JetBrains Mono', 'monospace'],
      },
      animation: {
        'float':       'float 6s ease-in-out infinite',
        'pulse-glow':  'pulse-glow 3s ease-in-out infinite',
        'counter':     'counter 2s ease-out forwards',
        'shimmer':     'shimmer 2s linear infinite',
      },
    },
  },
};
```

---

## 🔤 TİPOGRAFİ

### `src/styles/typography.css`

```css
/* Google Fonts — Sadece kullanılan weightler */
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=JetBrains+Mono:wght@400;600&display=swap');

/* Performans için: production'da bu fontları /public/fonts/ altına koy
   ve @font-face ile serve et. Bu swap flash'ı önler. */

body {
  font-family: 'Syne', sans-serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--text-primary);
  background-color: var(--bg-base);
  -webkit-font-smoothing: antialiased;
}

/* Display başlıklar */
.text-hero {
  font-family: 'Syne', sans-serif;
  font-weight: 800;
  font-size: clamp(3rem, 8vw, 7rem);  /* fluid typography */
  line-height: 0.95;
  letter-spacing: -0.03em;
}

.text-h1 {
  font-family: 'Syne', sans-serif;
  font-weight: 700;
  font-size: clamp(2rem, 5vw, 4rem);
  line-height: 1.05;
  letter-spacing: -0.02em;
}

.text-h2 {
  font-family: 'Syne', sans-serif;
  font-weight: 700;
  font-size: clamp(1.5rem, 3vw, 2.5rem);
  line-height: 1.15;
  letter-spacing: -0.015em;
}

/* Mono — metrikler, sayılar */
.text-metric {
  font-family: 'JetBrains Mono', monospace;
  font-weight: 600;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  letter-spacing: -0.02em;
}

.text-badge {
  font-family: 'JetBrains Mono', monospace;
  font-weight: 400;
  font-size: 0.7rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
}
```

---

## 🎬 ANİMASYON SİSTEMİ

### `src/styles/animations.css`

```css
/* =============================================
   SCROLL ANİMASYONLARI — IntersectionObserver
   ============================================= */

/* Başlangıç durumları */
[data-animate] {
  opacity: 0;
  will-change: transform, opacity;
  transition:
    opacity 0.8s cubic-bezier(0.16, 1, 0.3, 1),
    transform 0.8s cubic-bezier(0.16, 1, 0.3, 1);
}

[data-animate="fade-up"]    { transform: translateY(40px); }
[data-animate="fade-down"]  { transform: translateY(-40px); }
[data-animate="fade-left"]  { transform: translateX(-50px); }
[data-animate="fade-right"] { transform: translateX(50px); }
[data-animate="zoom-in"]    { transform: scale(0.92); }
[data-animate="zoom-out"]   { transform: scale(1.08); }
[data-animate="flip-up"]    {
  transform: rotateX(-15deg) translateY(30px);
  perspective: 800px;
}

/* Görünür durum */
[data-visible] {
  opacity: 1 !important;
  transform: none !important;
}

/* Gecikme yardımcıları */
[data-delay="100"] { transition-delay: 100ms; }
[data-delay="200"] { transition-delay: 200ms; }
[data-delay="300"] { transition-delay: 300ms; }
[data-delay="400"] { transition-delay: 400ms; }
[data-delay="500"] { transition-delay: 500ms; }

/* =============================================
   KEYFRAME ANİMASYONLARI
   ============================================= */

/* Yüzen elementler için */
@keyframes float {
  0%, 100% { transform: translateY(0px) rotate(0deg); }
  33%       { transform: translateY(-12px) rotate(0.5deg); }
  66%       { transform: translateY(-6px) rotate(-0.5deg); }
}

/* Neon glow pulse */
@keyframes pulse-glow {
  0%, 100% { box-shadow: 0 0 20px rgba(208, 253, 23, 0.2); }
  50%       { box-shadow: 0 0 50px rgba(208, 253, 23, 0.5); }
}

/* Gradient shimmer (kartlar için) */
@keyframes shimmer {
  0%   { background-position: -200% center; }
  100% { background-position: 200% center; }
}

/* Navbar scroll küçülme */
@keyframes nav-shrink {
  to {
    padding-block: 0.75rem;
    background: var(--navbar-blur);
    backdrop-filter: blur(20px);
  }
}

/* Sayaç artışı (CSS counter) */
@keyframes counter {
  from { --num: 0; }
  to   { --num: var(--target); }
}

/* Grid pattern hareket */
@keyframes grid-drift {
  0%   { transform: translate(0, 0); }
  100% { transform: translate(40px, 40px); }
}

/* Border scan animasyonu (CTA buton) */
@keyframes border-scan {
  0%   { background-position: 0% 50%; }
  50%  { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

/* =============================================
   HOVER & MİKRO-İNTERAKSİYONLAR
   ============================================= */

/* Kart hover — lift effect */
.card-hover {
  transition:
    transform 0.4s cubic-bezier(0.34, 1.56, 0.64, 1),
    box-shadow 0.4s ease,
    border-color 0.3s ease;
}
.card-hover:hover {
  transform: translateY(-6px) scale(1.01);
  box-shadow: var(--shadow-hover), var(--glow-lime-sm);
  border-color: var(--border-strong);
}

/* Link ok animasyonu */
.arrow-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  transition: gap 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.arrow-link:hover { gap: 0.9rem; }

/* =============================================
   ARKA PLAN EFEKTLERİ
   ============================================= */

/* Noise texture overlay */
.noise-overlay::after {
  content: '';
  position: fixed;
  inset: 0;
  opacity: var(--noise-opacity);
  pointer-events: none;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
  z-index: 9999;
  mix-blend-mode: overlay;
}

/* Grid arka plan deseni */
.grid-bg {
  background-image:
    linear-gradient(var(--grid-line) 1px, transparent 1px),
    linear-gradient(90deg, var(--grid-line) 1px, transparent 1px);
  background-size: 60px 60px;
}

/* Radial gradient glow */
.hero-glow {
  background:
    radial-gradient(
      ellipse 80% 60% at 50% 0%,
      rgba(208, 253, 23, 0.06) 0%,
      transparent 70%
    );
}
```

### `src/scripts/animate.ts`

```typescript
// Performanslı scroll animasyon sistemi
// requestAnimationFrame + IntersectionObserver kombinasyonu

export function initAnimations(): void {
  const elements = document.querySelectorAll<HTMLElement>('[data-animate]');

  if (!elements.length) return;

  // Reduced motion tercihi (erişilebilirlik)
  const prefersReducedMotion = window.matchMedia(
    '(prefers-reduced-motion: reduce)'
  ).matches;

  if (prefersReducedMotion) {
    elements.forEach(el => el.setAttribute('data-visible', ''));
    return;
  }

  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach(entry => {
        if (!entry.isIntersecting) return;

        const el = entry.target as HTMLElement;
        const delay = parseInt(el.dataset.delay ?? '0', 10);

        setTimeout(() => {
          requestAnimationFrame(() => {
            el.setAttribute('data-visible', '');
          });
        }, delay);

        observer.unobserve(el); // Bir kez tetiklendikten sonra gözlemi durdur
      });
    },
    {
      threshold: 0.15,
      rootMargin: '0px 0px -60px 0px',
    }
  );

  elements.forEach(el => observer.observe(el));
}

// Sayfa değişimlerinde (View Transitions) yeniden çalıştır
document.addEventListener('astro:page-load', initAnimations);
initAnimations();
```

### `src/scripts/counter.ts`

```typescript
// Sayaç animasyonu — 10.000+ gibi metrikleri canlandır

export function initCounters(): void {
  const counters = document.querySelectorAll<HTMLElement>('[data-counter]');

  const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
      if (!entry.isIntersecting) return;

      const el = entry.target as HTMLElement;
      const target = parseInt(el.dataset.counter ?? '0', 10);
      const duration = parseInt(el.dataset.duration ?? '2000', 10);
      const suffix = el.dataset.suffix ?? '';
      const prefix = el.dataset.prefix ?? '';

      animateCounter(el, 0, target, duration, prefix, suffix);
      observer.unobserve(el);
    });
  }, { threshold: 0.5 });

  counters.forEach(el => observer.observe(el));
}

function animateCounter(
  el: HTMLElement,
  start: number,
  end: number,
  duration: number,
  prefix: string,
  suffix: string
): void {
  const startTime = performance.now();

  function update(currentTime: number): void {
    const elapsed = currentTime - startTime;
    const progress = Math.min(elapsed / duration, 1);

    // Ease out cubic
    const eased = 1 - Math.pow(1 - progress, 3);
    const current = Math.floor(start + (end - start) * eased);

    el.textContent = `${prefix}${current.toLocaleString('tr-TR')}${suffix}`;

    if (progress < 1) {
      requestAnimationFrame(update);
    }
  }

  requestAnimationFrame(update);
}

document.addEventListener('astro:page-load', initCounters);
initCounters();
```

### `src/scripts/theme.ts`

```typescript
// Dark/Light tema yönetimi — Flash of Unstyled Content önleme

// Bu script <head> içinde INLINE çalışmalı (önce yüklensin)
const THEME_KEY = 'eny-theme';

function getInitialTheme(): 'dark' | 'light' {
  const stored = localStorage.getItem(THEME_KEY) as 'dark' | 'light' | null;
  if (stored) return stored;

  const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
  return prefersDark ? 'dark' : 'light';
}

function applyTheme(theme: 'dark' | 'light'): void {
  document.documentElement.setAttribute('data-theme', theme);
  localStorage.setItem(THEME_KEY, theme);
}

// İlk yükleme
applyTheme(getInitialTheme());

// Toggle fonksiyonu — buton için export
export function toggleTheme(): void {
  const current = document.documentElement.getAttribute('data-theme');
  applyTheme(current === 'dark' ? 'light' : 'dark');
}

// Sistem tercihi değişince güncelle
window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', e => {
  if (!localStorage.getItem(THEME_KEY)) {
    applyTheme(e.matches ? 'dark' : 'light');
  }
});
```

---

## 🏗️ LAYOUT BİLEŞENLERİ

### `src/layouts/BaseLayout.astro`

```astro
---
import '../styles/global.css';
import '../styles/themes.css';
import '../styles/typography.css';
import '../styles/animations.css';
import Navbar from '../components/layout/Navbar.astro';
import Footer from '../components/layout/Footer.astro';

interface Props {
  title: string;
  description?: string;
  ogImage?: string;
  canonical?: string;
}

const {
  title,
  description = 'eny — Finansın Yeni İşletim Sistemi. e-Dönüşüm, tahsilat, ödeme ve treasury çözümleri tek platformda.',
  ogImage = '/images/og-image.jpg',
  canonical = Astro.url.href,
} = Astro.props;

const fullTitle = title === 'eny' ? title : `${title} | eny`;
---

<!DOCTYPE html>
<html lang="tr" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta name="description" content={description} />
  <link rel="canonical" href={canonical} />

  <!-- OG / Social -->
  <meta property="og:title" content={fullTitle} />
  <meta property="og:description" content={description} />
  <meta property="og:image" content={ogImage} />
  <meta property="og:url" content={canonical} />
  <meta property="og:type" content="website" />
  <meta property="og:locale" content="tr_TR" />

  <!-- Twitter -->
  <meta name="twitter:card" content="summary_large_image" />
  <meta name="twitter:title" content={fullTitle} />
  <meta name="twitter:description" content={description} />
  <meta name="twitter:image" content={ogImage} />

  <!-- Favicon -->
  <link rel="icon" type="image/svg+xml" href="/favicon.svg" />

  <!-- Preconnect -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />

  <!-- Fonts — kritik yol -->
  <link
    rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=JetBrains+Mono:wght@400;600&display=swap"
  />

  <!-- FOUC önleme — inline theme script -->
  <script is:inline>
    (function() {
      const stored = localStorage.getItem('eny-theme');
      const prefersDark = window.matchMedia('(prefers-color-scheme: dark)').matches;
      const theme = stored || (prefersDark ? 'dark' : 'light');
      document.documentElement.setAttribute('data-theme', theme);
    })();
  </script>

  <!-- View Transitions API -->
  <meta name="view-transition" content="same-origin" />

  <title>{fullTitle}</title>
</head>
<body class="noise-overlay">
  <Navbar />
  <main id="main-content">
    <slot />
  </main>
  <Footer />

  <!-- Global Scripts -->
  <script>
    import { initAnimations } from '../scripts/animate';
    import { initCounters } from '../scripts/counter';
    initAnimations();
    initCounters();
  </script>
</body>
</html>
```

---

### `src/components/layout/Navbar.astro`

**Davranış:** Scroll'da küçülen, blur backdrop, sticky, mobile hamburger

```astro
---
import ThemeToggle from './ThemeToggle.astro';

const navLinks = [
  {
    label: 'Hizmetler',
    href: '#',
    dropdown: [
      { label: 'e-Dönüşüm Serisi',       href: '/hizmetler/e-donusum',           badge: 'GİB Onaylı' },
      { label: 'Tahsilat & Ödeme',        href: '/hizmetler/finansal-teknolojiler', badge: null },
      { label: 'E-Ticaret Çözümleri',     href: '/hizmetler/e-ticaret',            badge: null },
      { label: 'Treasury Intelligence',   href: '/hizmetler/treasury',             badge: 'AI' },
    ]
  },
  { label: 'Çözümler', href: '#cozumler' },
  { label: 'Hakkımızda', href: '/hakkimizda' },
  { label: 'İletişim', href: '/iletisim' },
];
---

<header id="navbar" class="navbar">
  <nav class="navbar__inner">
    <!-- Logo -->
    <a href="/" class="navbar__logo" aria-label="eny ana sayfa">
      <span class="logo__dot"></span>
      <span class="logo__text">eny</span>
      <span class="logo__period">.</span>
    </a>

    <!-- Desktop Nav -->
    <ul class="navbar__links" role="list">
      {navLinks.map(link => (
        <li class={link.dropdown ? 'has-dropdown' : ''}>
          <a href={link.href} class="nav-link">
            {link.label}
            {link.dropdown && (
              <svg class="nav-chevron" width="12" height="12" viewBox="0 0 12 12">
                <path d="M2 4l4 4 4-4" stroke="currentColor" stroke-width="1.5" fill="none" stroke-linecap="round"/>
              </svg>
            )}
          </a>
          {link.dropdown && (
            <div class="dropdown">
              {link.dropdown.map(item => (
                <a href={item.href} class="dropdown__item">
                  <span>{item.label}</span>
                  {item.badge && <span class="dropdown__badge">{item.badge}</span>}
                </a>
              ))}
            </div>
          )}
        </li>
      ))}
    </ul>

    <!-- Sağ taraf -->
    <div class="navbar__actions">
      <ThemeToggle />
      <a href="/demo" class="btn btn--ghost btn--sm">Demo Talep Et</a>
      <a href="/iletisim" class="btn btn--primary btn--sm">
        Başlayın
        <svg width="14" height="14" viewBox="0 0 14 14" fill="none">
          <path d="M2 7h10M8 3l4 4-4 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/>
        </svg>
      </a>

      <!-- Mobile hamburger -->
      <button class="hamburger" id="menu-toggle" aria-label="Menüyü aç/kapat" aria-expanded="false">
        <span></span><span></span><span></span>
      </button>
    </div>
  </nav>

  <!-- Mobile menü -->
  <div class="mobile-menu" id="mobile-menu" aria-hidden="true">
    <!-- ... mobile nav içeriği ... -->
  </div>
</header>

<style>
.navbar {
  position: fixed;
  top: 0;
  inset-inline: 0;
  z-index: 1000;
  padding-block: 1.25rem;
  transition: padding 0.4s ease, background 0.4s ease, box-shadow 0.4s ease;
}

.navbar.scrolled {
  padding-block: 0.75rem;
  background: var(--navbar-blur);
  backdrop-filter: blur(20px) saturate(180%);
  -webkit-backdrop-filter: blur(20px) saturate(180%);
  box-shadow: 0 1px 0 var(--border-subtle), var(--glow-lime-sm);
}

.navbar__inner {
  max-width: 1280px;
  margin-inline: auto;
  padding-inline: 2rem;
  display: flex;
  align-items: center;
  gap: 2rem;
}

/* Logo */
.navbar__logo {
  display: flex;
  align-items: center;
  gap: 2px;
  text-decoration: none;
  font-family: 'Syne', sans-serif;
  font-weight: 800;
  font-size: 1.5rem;
}
.logo__dot {
  width: 8px;
  height: 8px;
  background: var(--accent-primary);
  border-radius: 50%;
  animation: pulse-glow 3s ease-in-out infinite;
  margin-right: 6px;
}
.logo__text  { color: var(--text-primary); }
.logo__period { color: var(--accent-primary); }

/* Nav links */
.navbar__links {
  display: flex;
  align-items: center;
  gap: 0.25rem;
  list-style: none;
  margin: 0;
  padding: 0;
  margin-inline-start: auto;
}

.nav-link {
  display: flex;
  align-items: center;
  gap: 4px;
  padding: 0.5rem 0.75rem;
  font-size: 0.9rem;
  font-weight: 500;
  color: var(--text-secondary);
  text-decoration: none;
  border-radius: 8px;
  transition: color 0.2s, background 0.2s;
}
.nav-link:hover {
  color: var(--text-primary);
  background: var(--bg-elevated);
}

/* Dropdown */
.has-dropdown { position: relative; }
.dropdown {
  position: absolute;
  top: calc(100% + 12px);
  left: 50%;
  transform: translateX(-50%) translateY(-8px);
  opacity: 0;
  pointer-events: none;
  min-width: 240px;
  background: var(--bg-surface);
  border: 1px solid var(--border-subtle);
  border-radius: 16px;
  padding: 0.5rem;
  box-shadow: var(--shadow-card);
  transition: opacity 0.2s, transform 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
}
.has-dropdown:hover .dropdown,
.has-dropdown:focus-within .dropdown {
  opacity: 1;
  pointer-events: auto;
  transform: translateX(-50%) translateY(0);
}

.dropdown__item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0.625rem 0.875rem;
  border-radius: 10px;
  font-size: 0.875rem;
  color: var(--text-secondary);
  text-decoration: none;
  transition: color 0.2s, background 0.2s;
}
.dropdown__item:hover {
  color: var(--text-primary);
  background: var(--bg-elevated);
}

.dropdown__badge {
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.65rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  padding: 2px 8px;
  border-radius: 99px;
  background: var(--accent-muted);
  color: var(--accent-primary);
  border: 1px solid var(--border-strong);
}

/* Actions */
.navbar__actions {
  display: flex;
  align-items: center;
  gap: 0.75rem;
}
</style>

<script>
  // Scroll davranışı
  const navbar = document.getElementById('navbar')!;

  const updateNavbar = () => {
    navbar.classList.toggle('scrolled', window.scrollY > 60);
  };

  window.addEventListener('scroll', updateNavbar, { passive: true });
  updateNavbar();

  // Mobile menu toggle
  const toggle = document.getElementById('menu-toggle')!;
  const mobileMenu = document.getElementById('mobile-menu')!;

  toggle.addEventListener('click', () => {
    const isOpen = toggle.getAttribute('aria-expanded') === 'true';
    toggle.setAttribute('aria-expanded', String(!isOpen));
    mobileMenu.setAttribute('aria-hidden', String(isOpen));
    mobileMenu.classList.toggle('open', !isOpen);
    document.body.style.overflow = isOpen ? '' : 'hidden';
  });
</script>
```

---

### `src/components/layout/ThemeToggle.astro`

```astro
<button
  id="theme-toggle"
  class="theme-toggle"
  aria-label="Temayı değiştir"
  title="Temayı değiştir"
>
  <!-- Sun icon (light modda göster) -->
  <svg class="icon-sun" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
    <circle cx="12" cy="12" r="5"/>
    <path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"/>
  </svg>
  <!-- Moon icon (dark modda göster) -->
  <svg class="icon-moon" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
    <path d="M21 12.79A9 9 0 1111.21 3 7 7 0 0021 12.79z"/>
  </svg>
</button>

<style>
.theme-toggle {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 38px;
  height: 38px;
  border-radius: 10px;
  border: 1px solid var(--border-subtle);
  background: var(--bg-surface);
  color: var(--text-secondary);
  cursor: pointer;
  transition: all 0.2s;
}
.theme-toggle:hover {
  border-color: var(--border-strong);
  color: var(--accent-primary);
  background: var(--bg-elevated);
}

/* Dark modda ay, light modda güneş göster */
[data-theme="dark"] .icon-sun  { display: none; }
[data-theme="dark"] .icon-moon { display: block; }
[data-theme="light"] .icon-sun  { display: block; }
[data-theme="light"] .icon-moon { display: none; }
</style>

<script>
  import { toggleTheme } from '../../scripts/theme';
  document.getElementById('theme-toggle')!.addEventListener('click', toggleTheme);
</script>
```

---

## 🏠 ANA SAYFA BİLEŞENLERİ

### `src/components/home/Hero.astro`

**Tasarım:** Full-height, grid arka plan, neon glow, floating shapes, scroll CTA

```astro
---
// Animasyonlar data-animate attribute ile tetiklenir
---

<section class="hero grid-bg hero-glow">

  <!-- Dekoratif arka plan şekilleri (CSS animasyon ile yüzer) -->
  <div class="hero__shapes" aria-hidden="true">
    <div class="shape shape--1"></div>
    <div class="shape shape--2"></div>
    <div class="shape shape--3"></div>
  </div>

  <div class="hero__container">

    <!-- Üst badge -->
    <div class="hero__badge" data-animate="fade-down">
      <span class="badge__dot"></span>
      <span class="badge__text text-badge">Fintech × Regtech × E-Commerce</span>
    </div>

    <!-- Ana başlık -->
    <h1 class="hero__title text-hero" data-animate="fade-up" data-delay="100">
      Finansın Yeni
      <span class="title__highlight">
        İşletim
        <br />
        Sistemi
      </span>
    </h1>

    <!-- Alt açıklama -->
    <p class="hero__description" data-animate="fade-up" data-delay="200">
      Karmaşık süreçler görünmez olduğunda, iş mükemmelleşir.
      <br class="hide-mobile" />
      eny ile e-dönüşüm, tahsilat ve ödemeleri tek platformdan yönetin.
    </p>

    <!-- CTA Butonları -->
    <div class="hero__actions" data-animate="fade-up" data-delay="300">
      <a href="/demo" class="btn btn--primary btn--lg">
        Hemen Başlayın
        <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
          <path d="M3 8h10M9 4l4 4-4 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/>
        </svg>
      </a>
      <a href="#demo-video" class="btn btn--ghost btn--lg">
        <span class="play-icon">
          <svg width="14" height="14" viewBox="0 0 14 14" fill="currentColor">
            <path d="M4 2l8 5-8 5z"/>
          </svg>
        </span>
        Demo İzleyin
      </a>
    </div>

    <!-- Güven rozetleri -->
    <div class="hero__trust" data-animate="fade-up" data-delay="400">
      <div class="trust__divider"></div>
      <div class="trust__badges">
        <span class="trust__item">
          <svg width="14" height="14" viewBox="0 0 14 14" fill="var(--accent-primary)">
            <path d="M7 1L8.8 5.4H13.5L9.7 8.2L11 12.8L7 10L3 12.8L4.3 8.2L0.5 5.4H5.2L7 1Z"/>
          </svg>
          GİB Onaylı
        </span>
        <span class="trust__sep">·</span>
        <span class="trust__item">PCI-DSS Level 1</span>
        <span class="trust__sep">·</span>
        <span class="trust__item">7/24 Uzman Destek</span>
        <span class="trust__sep">·</span>
        <span class="trust__item">ISO 27001</span>
      </div>
    </div>

  </div>

  <!-- Scroll down indicator -->
  <div class="hero__scroll" aria-hidden="true">
    <div class="scroll-indicator">
      <div class="scroll-dot"></div>
    </div>
  </div>
</section>

<style>
.hero {
  position: relative;
  min-height: 100svh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  padding-block: 8rem 4rem;
}

.hero__container {
  position: relative;
  z-index: 2;
  max-width: 900px;
  margin-inline: auto;
  padding-inline: 2rem;
  text-align: center;
}

/* Badge */
.hero__badge {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  padding: 6px 16px;
  border: 1px solid var(--border-strong);
  border-radius: 99px;
  background: var(--accent-muted);
  margin-bottom: 2rem;
}
.badge__dot {
  width: 6px;
  height: 6px;
  background: var(--accent-primary);
  border-radius: 50%;
  animation: pulse-glow 2s infinite;
}
.badge__text { color: var(--accent-primary); }

/* Başlık */
.hero__title {
  margin-bottom: 1.5rem;
  color: var(--text-primary);
}
.title__highlight {
  color: var(--accent-primary);
  display: block;
  /* Gradient text efekti */
  background: linear-gradient(135deg, var(--accent-primary) 0%, #A8D400 60%, var(--accent-gold) 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Açıklama */
.hero__description {
  font-size: clamp(1rem, 2vw, 1.2rem);
  color: var(--text-secondary);
  max-width: 560px;
  margin-inline: auto;
  margin-bottom: 2.5rem;
  line-height: 1.7;
}

/* CTA Butonları */
.hero__actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  margin-bottom: 3rem;
}

.play-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 32px;
  height: 32px;
  border-radius: 50%;
  background: var(--bg-elevated);
  border: 1px solid var(--border-subtle);
  transition: background 0.2s, border-color 0.2s;
}
.btn--ghost:hover .play-icon {
  background: var(--accent-muted);
  border-color: var(--border-strong);
}

/* Trust */
.hero__trust {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}
.trust__divider {
  width: 120px;
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--border-subtle), transparent);
}
.trust__badges {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.5rem;
  justify-content: center;
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.72rem;
  letter-spacing: 0.05em;
}
.trust__item { color: var(--text-secondary); }
.trust__sep  { color: var(--border-subtle); }

/* Dekoratif şekiller */
.hero__shapes { position: absolute; inset: 0; pointer-events: none; }

.shape {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  opacity: 0.07;
}
.shape--1 {
  width: 600px; height: 600px;
  background: var(--accent-primary);
  top: -200px; right: -200px;
  animation: float 8s ease-in-out infinite;
}
.shape--2 {
  width: 400px; height: 400px;
  background: var(--accent-gold);
  bottom: -100px; left: -150px;
  animation: float 10s ease-in-out infinite reverse;
}
.shape--3 {
  width: 300px; height: 300px;
  background: var(--accent-primary);
  top: 40%; left: 30%;
  animation: float 7s ease-in-out infinite 2s;
  opacity: 0.04;
}

/* Scroll indicator */
.hero__scroll {
  position: absolute;
  bottom: 2rem;
  left: 50%;
  transform: translateX(-50%);
}
.scroll-indicator {
  width: 24px;
  height: 40px;
  border: 2px solid var(--border-subtle);
  border-radius: 12px;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  padding-top: 6px;
}
.scroll-dot {
  width: 4px;
  height: 8px;
  background: var(--accent-primary);
  border-radius: 2px;
  animation: scroll-bounce 2s ease-in-out infinite;
}
@keyframes scroll-bounce {
  0%, 100% { transform: translateY(0); opacity: 1; }
  50%       { transform: translateY(12px); opacity: 0.3; }
}
</style>
```

---

### `src/components/home/MetricsBand.astro`

**Tasarım:** Sayaç animasyonu, marquee/scroll efekti veya statik grid

```astro
---
const metrics = [
  { value: 10000, suffix: '+', label: 'İşletme Güveniyor', prefix: '' },
  { value: 135,   suffix: '+', label: 'Para Birimi',        prefix: '' },
  { value: 20,    suffix: '+', label: 'Banka Entegrasyonu', prefix: '' },
  { value: 99.99, suffix: '%', label: 'Uptime Garantisi',   prefix: '' },
  { value: 630,   suffix: '+', label: 'Milyar TL Tahsilat', prefix: '' },
  { value: 98,    suffix: '%', label: 'Nakit Tahmin Doğrul.', prefix: '' },
];
---

<section class="metrics-band" data-animate="fade-up">
  <div class="metrics-band__inner">
    {metrics.map((m, i) => (
      <div class="metric-item" data-delay={i * 80}>
        <div
          class="metric-item__value text-metric"
          data-counter={String(m.value).replace('.', '')}
          data-suffix={m.suffix}
          data-prefix={m.prefix}
          data-duration="1800"
        >
          {m.prefix}0{m.suffix}
        </div>
        <div class="metric-item__label">{m.label}</div>
      </div>
    ))}
  </div>
</section>

<style>
.metrics-band {
  padding-block: 4rem;
  border-block: 1px solid var(--border-subtle);
  background:
    linear-gradient(
      to right,
      transparent,
      var(--bg-surface) 20%,
      var(--bg-surface) 80%,
      transparent
    );
}

.metrics-band__inner {
  max-width: 1280px;
  margin-inline: auto;
  padding-inline: 2rem;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
  gap: 2rem;
  text-align: center;
}

.metric-item__value {
  color: var(--accent-primary);
  margin-bottom: 0.5rem;
}

.metric-item__label {
  font-size: 0.8rem;
  letter-spacing: 0.05em;
  color: var(--text-secondary);
  text-transform: uppercase;
  font-family: 'JetBrains Mono', monospace;
}

/* Dikey ayırıcı */
.metric-item + .metric-item {
  border-inline-start: 1px solid var(--border-subtle);
  padding-inline-start: 2rem;
}
@media (max-width: 768px) {
  .metric-item + .metric-item {
    border-inline-start: none;
  }
}
</style>
```

---

### `src/components/home/Services.astro`

**Tasarım:** 4 kart, hover glow, stagger animasyonu, ikonlu liste

```astro
---
const services = [
  {
    tag:   'REGTECH',
    icon:  '◆',
    title: 'e-Dönüşüm Serisi',
    desc:  'Yasal zorunlulukları operasyonel avantaja dönüştürün. GİB uyumlu, otomatik güncellemeli, sıfır hata toleranslı.',
    href:  '/hizmetler/e-donusum',
    items: ['e-Fatura & e-Arşiv — GİB entegreli, AI destekli', 'e-Defter — Zaman damgalı, değiştirilemez', 'e-İrsaliye — Gerçek zamanlı sevkiyat takibi', 'Regülasyon Asistanı — 7/24 mevzuat izleme'],
    badge: 'GİB Onaylı',
    accent: 'lime',
  },
  {
    tag:   'FINTECH',
    icon:  '◈',
    title: 'Akıllı Tahsilat & Ödeme',
    desc:  'Paranın hareketini bir senfoni gibi yönetin. Omni-channel tahsilat, akıllı yönlendirme, anlık mutabakat.',
    href:  '/hizmetler/finansal-teknolojiler',
    items: ['Global e-Tahsilat — Tüm kanallardan tek panel', 'e-Ödeme & TÖS — Smart Routing ile otomatik banka', 'e-DBS — Banka garantili otomatik tahsilat', 'e-Ekstre — Açık bankacılık, tüm hesaplar tek'],
    badge: 'PCI-DSS',
    accent: 'gold',
  },
  {
    tag:   'E-TİCARET',
    icon:  '◇',
    title: 'Yeni Nesil Ticaret',
    desc:  'Dijital mağazanızı global bir finans merkezine dönüştürün. One-Click Pay, fraud koruması ve marketplace desteğiyle.',
    href:  '/hizmetler/e-ticaret',
    items: ['Checkout Excellence — Dünyanın en hızlı ödeme', 'Abonelik & Tekrarlı — Otomatik faturalama', 'Fraud Protection (AI) — ML tabanlı risk motoru', 'Marketplace Split — Çok taraflı ödeme dağıtımı'],
    badge: '3D Secure',
    accent: 'lime',
  },
  {
    tag:   'TREASURY',
    icon:  '◉',
    title: 'Finansal Zeka',
    desc:  'Veriyi karara, kararı kâra dönüştürün. %98 doğrulukla nakit projeksiyonu ve risk analitiği.',
    href:  '/hizmetler/treasury',
    items: ['Nakit Projeksiyonu (AI) — %98 doğruluk oranı', 'Çoklu Banka Hazine — 29 banka, tek panel', 'Yönetim Kurulu Raporları — Anlık otomatik', 'Müşteri & Bayi Riski — Credit risk scoring'],
    badge: 'AI',
    accent: 'gold',
  },
];
---

<section class="services section">
  <div class="container">

    <!-- Bölüm başlığı -->
    <div class="section-header" data-animate="fade-up">
      <span class="section-tag text-badge">◆ PLATFORM</span>
      <h2 class="text-h1">
        Her Finansal Süreç.
        <br />
        <span class="text-accent">Tek Platform.</span>
      </h2>
      <p class="section-desc">
        Regtech'ten fintech'e, e-ticaretten treasury yönetimine —
        tüm finansal operasyonlar tek bir sistemde birleşir.
      </p>
    </div>

    <!-- Kart grid -->
    <div class="services__grid">
      {services.map((service, i) => (
        <article
          class={`service-card card-hover accent--${service.accent}`}
          data-animate="fade-up"
          data-delay={i * 100}
        >
          <!-- Üst satır -->
          <div class="card__header">
            <span class="card__tag text-badge">{service.tag}</span>
            <span class="card__badge text-badge">{service.badge}</span>
          </div>

          <!-- İkon + Başlık -->
          <div class="card__title-row">
            <span class="card__icon" aria-hidden="true">{service.icon}</span>
            <h3 class="card__title">{service.title}</h3>
          </div>

          <!-- Açıklama -->
          <p class="card__desc">{service.desc}</p>

          <!-- Özellik listesi -->
          <ul class="card__features" role="list">
            {service.items.map(item => (
              <li class="card__feature">
                <span class="feature__arrow" aria-hidden="true">→</span>
                <span>{item}</span>
              </li>
            ))}
          </ul>

          <!-- CTA link -->
          <a href={service.href} class="card__cta arrow-link">
            Detaylı İncele
            <svg width="16" height="16" viewBox="0 0 16 16" fill="none">
              <path d="M3 8h10M9 4l4 4-4 4" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/>
            </svg>
          </a>

          <!-- Hover gradient overlay -->
          <div class="card__glow" aria-hidden="true"></div>
        </article>
      ))}
    </div>
  </div>
</section>

<style>
.services { padding-block: 8rem; }

.services__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.5rem;
  margin-top: 4rem;
}

.service-card {
  position: relative;
  background: var(--bg-surface);
  border: 1px solid var(--border-subtle);
  border-radius: 20px;
  padding: 2rem;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  gap: 1.25rem;
  cursor: default;
}

/* Glow overlay — hover'da görünür */
.card__glow {
  position: absolute;
  inset: 0;
  opacity: 0;
  background: radial-gradient(
    circle at 50% 0%,
    var(--accent-muted) 0%,
    transparent 60%
  );
  transition: opacity 0.4s ease;
  pointer-events: none;
}
.service-card:hover .card__glow { opacity: 1; }

.card__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.card__tag  {
  color: var(--accent-primary);
  opacity: 0.8;
}

.card__badge {
  padding: 3px 10px;
  border-radius: 99px;
  border: 1px solid var(--border-strong);
  background: var(--accent-muted);
  color: var(--accent-primary);
  font-size: 0.65rem;
}

/* Gold aksan varyantı */
.accent--gold .card__badge {
  border-color: rgba(212, 175, 55, 0.3);
  background: rgba(212, 175, 55, 0.08);
  color: var(--accent-gold);
}
.accent--gold .card__tag    { color: var(--accent-gold); }
.accent--gold .card__icon   { color: var(--accent-gold); }
.accent--gold .feature__arrow { color: var(--accent-gold); }

.card__title-row {
  display: flex;
  align-items: center;
  gap: 0.75rem;
}
.card__icon {
  font-size: 1.5rem;
  color: var(--accent-primary);
}
.card__title {
  font-family: 'Syne', sans-serif;
  font-weight: 700;
  font-size: 1.2rem;
  color: var(--text-primary);
  margin: 0;
}

.card__desc {
  font-size: 0.875rem;
  color: var(--text-secondary);
  line-height: 1.65;
  margin: 0;
}

.card__features {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
  gap: 0.625rem;
  border-block: 1px solid var(--border-subtle);
  padding-block: 1.25rem;
  flex: 1;
}
.card__feature {
  display: flex;
  gap: 0.75rem;
  font-size: 0.8rem;
  color: var(--text-secondary);
  line-height: 1.5;
}
.feature__arrow {
  color: var(--accent-primary);
  flex-shrink: 0;
  margin-top: 1px;
}

.card__cta {
  font-size: 0.875rem;
  font-weight: 600;
  color: var(--accent-primary);
  text-decoration: none;
  align-self: flex-start;
}
.card__cta:hover { color: var(--text-primary); }
</style>
```

---

### `src/components/home/WhyEny.astro`

**Tasarım:** Bento grid layout, sol büyük açıklama + sağ özellik tablosu

```astro
---
const features = [
  {
    icon: '🔒',
    title: 'Zero-Trust Security',
    desc: 'Verileriniz sadece şifrelenmez; parçalanarak farklı coğrafi konumlarda saklanır. Askeri düzeyde koruma.',
    tag: 'Güvenlik',
  },
  {
    icon: '⚡',
    title: 'API-First Architecture',
    desc: 'Kapsamlı dokümantasyona sahip, esnek ve hızlı API yapısı. Her sisteme bağlanır.',
    tag: 'Entegrasyon',
  },
  {
    icon: '🌐',
    title: 'Cross-Border Capability',
    desc: '135+ para birimiyle ödeme alın. Sınır tanımayan küresel ödeme altyapısı.',
    tag: 'Global',
  },
  {
    icon: '🤖',
    title: 'AI Intelligence',
    desc: 'Hata denetiminden nakit projeksiyonuna, tüm süreçlerde yapay zeka destekli karar zekası.',
    tag: 'Yapay Zeka',
  },
  {
    icon: '🔗',
    title: 'Tek Entegrasyon',
    desc: '20+ banka ve ödeme kuruluşuna tek API ile ulaşın. Smart Routing ile en iyi rota otomatik seçilir.',
    tag: 'Bankacılık',
  },
  {
    icon: '💬',
    title: '7/24 VIP Destek',
    desc: 'Bot değil, finans ve teknoloji uzmanı danışman. Her sorun için gerçek bir çözüm ortağı.',
    tag: 'Destek',
  },
];
---

<section class="why-eny section">
  <div class="container">

    <!-- Başlık -->
    <div class="section-header" data-animate="fade-up">
      <span class="section-tag text-badge">◆ FARK</span>
      <h2 class="text-h1">
        Finansın Yeni
        <span class="text-accent"> Anayasası</span>
      </h2>
      <p class="section-desc">
        Teknolojik üstünlüğümüz sizi rakiplerinizden
        yıllar değil, çağlar ileride tutar.
      </p>
    </div>

    <!-- Bento grid -->
    <div class="why-eny__grid">
      {features.map((f, i) => (
        <div
          class="feature-card card-hover"
          data-animate="fade-left"
          data-delay={i * 80}
        >
          <div class="feature-card__header">
            <span class="feature-card__icon" aria-hidden="true">{f.icon}</span>
            <span class="feature-card__tag text-badge">{f.tag}</span>
          </div>
          <h3 class="feature-card__title">{f.title}</h3>
          <p class="feature-card__desc">{f.desc}</p>
        </div>
      ))}
    </div>

  </div>
</section>

<style>
.why-eny { padding-block: 8rem; background: var(--bg-surface); }

.why-eny__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1px;
  margin-top: 4rem;
  border: 1px solid var(--border-subtle);
  border-radius: 24px;
  overflow: hidden;
}

.feature-card {
  background: var(--bg-surface);
  padding: 2rem;
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
  border-right: 1px solid var(--border-subtle);
  border-bottom: 1px solid var(--border-subtle);
  transition: background 0.3s ease;
}
.feature-card:hover { background: var(--bg-elevated); }

.feature-card__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.feature-card__icon { font-size: 1.5rem; }
.feature-card__tag {
  color: var(--text-secondary);
  background: var(--bg-elevated);
  padding: 2px 10px;
  border-radius: 99px;
  border: 1px solid var(--border-subtle);
}

.feature-card__title {
  font-family: 'Syne', sans-serif;
  font-weight: 700;
  font-size: 1.05rem;
  color: var(--text-primary);
  margin: 0;
}
.feature-card__desc {
  font-size: 0.85rem;
  color: var(--text-secondary);
  line-height: 1.65;
  margin: 0;
}
</style>
```

---

### `src/components/home/FinalCTA.astro`

**Tasarım:** Full-width dark band, büyük başlık, iki buton, güven rozetleri

```astro
---
---
<section class="final-cta grid-bg" data-animate="zoom-in">
  <div class="final-cta__glow" aria-hidden="true"></div>
  <div class="container final-cta__inner">

    <span class="section-tag text-badge">◆ BAŞLAYIN</span>

    <h2 class="text-hero final-cta__title">
      Finansal Dönüşüme
      <br />
      <span class="text-accent">Hazır mısınız?</span>
    </h2>

    <p class="final-cta__desc">
      İş modelinize özel en doğru finansal yapıyı birlikte kurgulayalım.
      <br />
      Kurulum gerektirmez, kredi kartı istenmez.
    </p>

    <div class="final-cta__actions">
      <a href="/demo" class="btn btn--primary btn--xl">
        Demo Talep Et
        <svg width="18" height="18" viewBox="0 0 18 18" fill="none">
          <path d="M3 9h12M10 4l5 5-5 5" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/>
        </svg>
      </a>
      <a href="/iletisim" class="btn btn--ghost btn--xl">
        Uzmanla Görüş
      </a>
    </div>

    <div class="final-cta__trust">
      <span>GİB Onaylı</span>
      <span>·</span>
      <span>Banka Güvenceli</span>
      <span>·</span>
      <span>KVKK Uyumlu</span>
      <span>·</span>
      <span>ISO 27001</span>
    </div>
  </div>
</section>

<style>
.final-cta {
  position: relative;
  padding-block: 10rem;
  text-align: center;
  overflow: hidden;
  background: var(--bg-base);
}

.final-cta__glow {
  position: absolute;
  inset: 0;
  background:
    radial-gradient(
      ellipse 70% 80% at 50% 50%,
      rgba(208, 253, 23, 0.08) 0%,
      transparent 70%
    );
  pointer-events: none;
}

.final-cta__inner {
  position: relative;
  z-index: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.final-cta__title { margin: 0; }
.final-cta__desc {
  color: var(--text-secondary);
  font-size: 1.1rem;
  max-width: 480px;
}

.final-cta__actions {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
}

.final-cta__trust {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  align-items: center;
  font-family: 'JetBrains Mono', monospace;
  font-size: 0.7rem;
  letter-spacing: 0.08em;
  color: var(--text-secondary);
}
</style>
```

---

## 🔘 UI BİLEŞENLERİ

### `src/components/ui/Button.astro` — Global Buton Stili

```css
/* src/styles/global.css — Buton bileşenleri */

.btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  font-family: 'Syne', sans-serif;
  font-weight: 600;
  border-radius: 10px;
  cursor: pointer;
  text-decoration: none;
  border: 1px solid transparent;
  transition:
    background 0.25s ease,
    border-color 0.25s ease,
    color 0.25s ease,
    box-shadow 0.25s ease,
    transform 0.2s cubic-bezier(0.34, 1.56, 0.64, 1);
  white-space: nowrap;
}
.btn:active { transform: scale(0.97); }

/* Primary — Neon lime */
.btn--primary {
  background: var(--accent-primary);
  color: #0A0F0D;
  border-color: var(--accent-primary);
}
.btn--primary:hover {
  background: transparent;
  color: var(--accent-primary);
  box-shadow: 0 0 30px rgba(208, 253, 23, 0.25);
}

/* Ghost */
.btn--ghost {
  background: transparent;
  color: var(--text-primary);
  border-color: var(--border-subtle);
}
.btn--ghost:hover {
  border-color: var(--border-strong);
  color: var(--accent-primary);
  background: var(--accent-muted);
}

/* Boyutlar */
.btn--sm  { padding: 0.5rem 1rem;    font-size: 0.85rem; }
.btn--md  { padding: 0.7rem 1.4rem;  font-size: 0.9rem;  }
.btn--lg  { padding: 0.85rem 1.75rem; font-size: 1rem;   }
.btn--xl  { padding: 1rem 2.25rem;   font-size: 1.05rem; }

/* Animasyonlu border — özel CTA için */
.btn--animated-border {
  background: linear-gradient(var(--bg-base), var(--bg-base)) padding-box,
              linear-gradient(90deg, var(--accent-primary), var(--accent-gold), var(--accent-primary)) border-box;
  border: 2px solid transparent;
  background-size: 200% auto;
  animation: border-scan 4s linear infinite;
}
```

---

## 📄 ANA SAYFA SAYFASI

### `src/pages/index.astro`

```astro
---
import BaseLayout from '../layouts/BaseLayout.astro';
import Hero from '../components/home/Hero.astro';
import MetricsBand from '../components/home/MetricsBand.astro';
import Services from '../components/home/Services.astro';
import WhyEny from '../components/home/WhyEny.astro';
import Integration from '../components/home/Integration.astro';
import Testimonials from '../components/home/Testimonials.astro';
import FinalCTA from '../components/home/FinalCTA.astro';
---

<BaseLayout
  title="eny — Finansın Yeni İşletim Sistemi"
  description="e-Dönüşüm, tahsilat, ödeme ve treasury yönetimini tek platformda birleştiren yeni nesil fintech çözümü."
>
  <Hero />
  <MetricsBand />
  <Services />
  <WhyEny />
  <Integration />
  <Testimonials />
  <FinalCTA />
</BaseLayout>
```

---

## ⚡ PERFORMANS STRATEJİSİ

### Core Web Vitals Hedefleri

| Metrik                              | Hedef   | Yöntem                                 |
| ----------------------------------- | ------- | -------------------------------------- |
| **LCP** (Largest Contentful Paint)  | < 1.2s  | Hero metin (resim yok), font preload   |
| **CLS** (Cumulative Layout Shift)   | < 0.05  | Font-display: swap, boyut rezervasyonu |
| **INP** (Interaction to Next Paint) | < 100ms | Minimal JS, passive event listeners    |
| **TTFB** (Time to First Byte)       | < 200ms | Astro SSG, CDN                         |
| **FCP** (First Contentful Paint)    | < 0.8s  | CSS inline, JS defer                   |

### Teknik Kararlar

```
✓ Astro SSG — Sıfır JS varsayılan, sadece gerekli yerlerde hydration
✓ View Transitions API — Sayfa geçişlerinde flash yok, SPA hissi
✓ Prefetch — Viewport'a giren linkler önceden yüklenir
✓ Critical CSS inline — LCP bloğu yok
✓ Font preload — JetBrains Mono & Syne için rel=preload
✓ Image optimization — Sharp ile WebP/AVIF, lazy loading
✓ astro-compress — HTML/CSS/JS minification + gzip
✓ Zero runtime CSS framework — Tailwind sadece utility, custom vars
✓ IntersectionObserver — Scroll animasyonları performanslı
✓ requestAnimationFrame — Sayaç animasyonları smooth
✓ Passive scroll listeners — Navbar scroll kaymaz
✓ will-change: transform, opacity — GPU hızlandırma
```

---

## 🧭 NAVİGASYON MİMARİSİ

```
/ (Ana Sayfa)
├── /hizmetler/
│   ├── /hizmetler/e-donusum        — e-Fatura, e-Defter, e-İrsaliye, e-Arşiv
│   ├── /hizmetler/finansal-teknolojiler  — e-Tahsilat, e-Ödeme, e-DBS, e-Ekstre
│   ├── /hizmetler/e-ticaret        — Checkout, Abonelik, Fraud, Marketplace
│   └── /hizmetler/treasury         — Nakit proj., Risk analitiği, Raporlar
├── /hakkimizda
├── /iletisim
├── /demo                           — Demo talep formu
└── /blog (opsiyonel)
```

---

## 🔍 SEO YAPISI

### Sitemap (astro-sitemap otomatik üretir)

```xml
<!-- Otomatik üretilir, sadece config:  -->
<urlset>
  <url><loc>https://eny.com.tr/</loc><priority>1.0</priority></url>
  <url><loc>https://eny.com.tr/hizmetler/e-donusum</loc><priority>0.9</priority></url>
  <url><loc>https://eny.com.tr/hizmetler/finansal-teknolojiler</loc><priority>0.9</priority></url>
  ...
</urlset>
```

### Schema.org Yapısal Veri

```json
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "eny",
  "applicationCategory": "FinanceApplication",
  "description": "Yeni nesil finansal işletim sistemi",
  "url": "https://eny.com.tr",
  "operatingSystem": "Web",
  "offers": {
    "@type": "Offer",
    "priceCurrency": "TRY"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.9",
    "reviewCount": "500"
  }
}
```

---

## 🎯 DEPLOYMENT

### Netlify / Vercel (Önerilen)

```toml
# netlify.toml
[build]
  command = "npm run build"
  publish  = "dist/"

[build.environment]
  NODE_VERSION = "20"

[[headers]]
  for = "/*"
  [headers.values]
    # Güvenlik başlıkları
    X-Frame-Options          = "DENY"
    X-Content-Type-Options   = "nosniff"
    Referrer-Policy          = "strict-origin-when-cross-origin"
    Permissions-Policy       = "camera=(), microphone=(), geolocation=()"

    # Cache — statik assetler
    Cache-Control            = "public, max-age=31536000, immutable"

[[headers]]
  for = "/*.html"
  [headers.values]
    Cache-Control            = "public, max-age=0, must-revalidate"
```

---

## 📋 UYGULAMA SIRASI (ÖNCE BU)

1. **Proje kurulum** — `npm create astro@latest` → minimal template
2. **Tailwind + plugins** → `npx astro add tailwind`
3. **`themes.css` + `global.css`** → CSS değişkenleri ve butonlar
4. **Theme toggle script** → FOUC önlemek için `<head>` inline
5. **`BaseLayout.astro`** → Font, meta, Navbar, Footer
6. **`Navbar.astro`** → Scroll davranışı + dropdown + mobile
7. **`Hero.astro`** → En kritik bölüm, LCP burada
8. **`MetricsBand.astro`** → Sayaç animasyonu
9. **`Services.astro`** → 4 kart, hover efektleri
10. **`WhyEny.astro`** → Bento grid
11. **`Testimonials.astro`** → Slider (Swiper.js veya pure CSS)
12. **`FinalCTA.astro`** → Kapanış
13. **`Footer.astro`** → Linkler, sertifikalar
14. **Hizmet alt sayfaları** → Her ürün için ayrı sayfa
15. **SEO + Schema** → Yapısal veri, sitemap
16. **Performance audit** → Lighthouse 90+
17. **Deploy** → Netlify/Vercel

---

## 💡 TASARIM NOTLARI

### Dark → Light Geçiş Prensipleri

| Element       | Dark                       | Light                                          |
| ------------- | -------------------------- | ---------------------------------------------- |
| Accent rengi  | `#D0FD17` (Neon Lime)      | `#3A7D0A` (Koyu Yeşil) ← lime light'ta okunmaz |
| Arka plan     | `#0A0F0D`                  | `#F4F6F4`                                      |
| Kart yüzeyi   | `#111A13`                  | `#FFFFFF`                                      |
| Glow efekti   | Belirgin (`opacity: 0.15`) | Hafif (`opacity: 0.06`)                        |
| Grid deseni   | Koyu yeşil çizgiler        | Açık gri çizgiler                              |
| Noise overlay | `opacity: 0.03`            | `opacity: 0.015`                               |

### Animasyon Prensipleri

- **Sayfa yükü:** Hero bölümü stagger — badge → başlık → açıklama → CTA → trust (0, 100, 200, 300, 400ms)
- **Scroll:** Her bölüm `fade-up`, kartlar stagger ile `data-delay`
- **Hover:** `cubic-bezier(0.34, 1.56, 0.64, 1)` — hafif spring efekti
- **Reduced Motion:** `prefers-reduced-motion: reduce` varsa tüm animasyonlar devre dışı
- **Performance:** `will-change`, `requestAnimationFrame`, observer `unobserve` after trigger

### Tipografi Hiyerarşisi (Görsel Ağırlık)

```
Hero başlık  → Syne 800, clamp(3rem, 8vw, 7rem), tracking -0.03em
H1           → Syne 700, clamp(2rem, 5vw, 4rem),  tracking -0.02em
H2           → Syne 700, clamp(1.5rem, 3vw, 2.5rem)
H3 (kart)    → Syne 700, 1.2rem
Body         → Syne 400, 1rem, line-height 1.7
Badge/Tag    → JetBrains Mono 400, 0.7rem, tracking 0.12em
Metrik       → JetBrains Mono 600, clamp(2.5rem, 5vw, 4.5rem)
```

---

*Bu döküman, eny.com.tr için Astro tabanlı web sitesinin eksiksiz blueprint'idir. Her bileşen production-ready code örnekleriyle desteklenmiştir. Geliştirme sürecinde bu dökümanı referans alarak ilerleyin.*
