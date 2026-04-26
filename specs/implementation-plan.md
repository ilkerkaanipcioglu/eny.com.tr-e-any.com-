# ENY.COM.TR Renk Sistemi Güncelleme Planı

Bu plan, `eny.com.tr` için sağlanan yeni renk paletinin `brand` dizinindeki ana manifestoya ve `eny.com.tr` projesine entegre edilmesini amaçlamaktadır.

## User Review Required

Yeni renk paleti iki ana tondan oluşuyor: **Mavi/Mor (Primary)** ve **Yeşil/Sarı (Accent)**.
Mevcut sistemde tek bir `h, s, l` değeri (Lime) ile çalışılıyordu. Bu değişiklikle beraber:
- **Primary Renk:** Majorelle Blue (`#6050DC`)
- **Accent Renk:** Maximum Green Yellow (`#CCDC50`) 
olarak sisteme tanımlanacak. Bu ayrım uygun mudur? Lütfen onaylayın veya değiştirilmesini istediğiniz noktaları belirtin.

## Proposed Changes

### `b:\DEV\HAREZM_EKOSISTEMI\brand\manifest.toml`
Mevcut `[brands.eny]` yapısını yeni primary renge (Majorelle Blue) uyarlayacağız.
- `[brands.eny]` değerlerini `h=247`, `s=67`, `l=59` (Majorelle Blue) olarak güncelleyeceğiz.
- `[light_contrast.eny]` altındaki `accent_color` değerini yeni Accent rengine (Maximum Green Yellow) uyarlayacağız.
- Değişiklik sonrası `node generate_tokens.mjs` komutunu çalıştırarak token çıktılarını üreteceğiz.

### `b:\DEV\HAREZM_EKOSISTEMI\eny.com.tr\src\styles\global.css`
Tailwind v4 `@theme` yapısına yeni renk paletini 6 kademeli (Primary ve Accent tonları) olarak doğrudan ekleyeceğiz.
- `--color-eny-blue-dark: #3625BA;`
- `--color-eny-blue-base: #6050DC;`
- `--color-eny-blue-light: #9A90E9;`
- `--color-eny-green-dark: #A9BA25;`
- `--color-eny-green-base: #CCDC50;`
- `--color-eny-green-light: #DFE990;`
- Eski `accent` (lime) kullanımını yeni `eny-green-base` ile değiştireceğiz.

### `b:\DEV\HAREZM_EKOSISTEMI\eny.com.tr\src\styles\tokens.css`
- Güncellenen `tokens.css` dosyasını brand klasöründen buraya kopyalayarak entegrasyonu tamamlayacağız.

## Verification Plan

### Manual Verification
- `npm run dev` komutuyla projeyi çalıştırıp UI üzerinde yeni mavi ve sarı/yeşil tonların kontrast sorunları oluşturmadan doğru şekilde uygulandığını kontrol edeceğiz.
- Buton, etiket ve arkaplanlardaki yansımaları gözden geçireceğiz.
