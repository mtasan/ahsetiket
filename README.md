# AHS Etiket - Kurumsal Web Sitesi

<p align="center">
  <img src="images/logo-new.svg" alt="AHS Etiket Logo" width="280">
</p>

<p align="center">
  <strong>AHS Etiket ve Barkod Sistemleri San. Tic. Ltd. Sti.</strong><br>
  Profesyonel Etiket, Ribon ve Barkod Cozumleri
</p>

<p align="center">
  <a href="https://ahsetiket.com">ahsetiket.com</a> &bull;
  <a href="https://ahsetiket.vercel.app">ahsetiket.vercel.app</a>
</p>

---

## Hakkinda

AHS Etiket'in kurumsal web sitesidir. Etiket, ribon, barkod yazici ve teknik servis hizmetlerini tanitan modern, responsive tek sayfa (SPA tarzi) web sitesidir.

### Ozellikler

- Tamamen responsive tasarim (mobil, tablet, masaustu)
- AI destekli musteri asistani (Google Gemini 2.5 Flash)
- WhatsApp entegrasyonu
- SEO optimizasyonu (Schema.org, Open Graph, Twitter Card)
- Hizli yukleme suresi (statik site)
- SSL sertifikasi (Vercel otomatik)

## Teknoloji Yigini

| Katman | Teknoloji |
|--------|-----------|
| **Frontend** | HTML5, CSS3 (Custom), JavaScript |
| **AI Chatbot** | Google Gemini 2.5 Flash API |
| **Backend (API)** | Vercel Serverless Functions (Node.js) |
| **Hosting** | Vercel |
| **Domain** | ahsetiket.com (Isimtescil) |
| **Versiyon Kontrolu** | Git + GitHub |

## Proje Yapisi

```
ahsetiket/
├── index.html              # Ana sayfa (tum icerik, CSS ve JS inline)
├── api/
│   └── chat.js             # Gemini API proxy (Vercel Serverless)
├── vercel.json             # Vercel yapilandirmasi
├── images/
│   ├── logo-new.svg        # Ana logo (SVG)
│   ├── logo-footer.svg     # Footer logosu
│   ├── logo-icon.svg       # Favicon/ikon
│   ├── ribbon.jpg          # Ribon urun gorseli
│   ├── kuse-etiket.jpg     # Kuse etiket gorseli
│   ├── barcode.webp        # Barkod gorseli
│   └── ...                 # Diger urun gorselleri
├── robots.txt              # SEO robot kurallari
├── sitemap.xml             # Arama motoru site haritasi
├── .gitignore              # Git haric tutulan dosyalar
└── CLAUDE.md               # Claude AI proje rehberi
```

## Site Bolumleri

| Bolum | Aciklama |
|-------|----------|
| **Ana Sayfa** | Hero alani, tanitim |
| **Neden Biz** | Firma avantajlari |
| **Hizmetler** | Satis, teknik servis, teslimat |
| **Urunler** | Etiket ve ribon cesitleri |
| **Hakkimizda** | Firma bilgileri |
| **Teknik Servis** | Bakim ve onarim |
| **Iletisim** | Adres, telefon, harita |

## AI Asistan

Site, **AHS Asistan** adinda yapay zeka destekli bir musteri asistani icerir:

- **Model:** Google Gemini 2.5 Flash
- **Ozellikler:**
  - Urun bilgisi (etiket, ribon, barkod yazici)
  - Fiyat teklifi yonlendirmesi
  - Teknik servis bilgisi
  - Hizli yanit cip'leri
- **Guvenlik:** API anahtari Vercel Environment Variables ile saklanir, client-side'da asla gozukmez

## Kurulum

### Yerel Gelistirme

```bash
# Repoyu klonlayin
git clone https://github.com/mtasan/ahsetiket.git
cd ahsetiket

# .env dosyasi olusturun
echo "GEMINI_API_KEY=your_api_key_here" > .env

# Yerel sunucu baslatin (herhangi biri)
python3 -m http.server 8080
# veya
npx serve .
```

> **Not:** AI chatbot yerel sunucuda calismaz (Vercel Serverless gerektirir). Sadece frontend'i test edebilirsiniz.

### Vercel'e Deploy

```bash
# Vercel CLI yukleyin
npm i -g vercel

# Deploy edin
vercel --prod

# Environment variable ekleyin
vercel env add GEMINI_API_KEY
```

### Otomatik Deploy

GitHub'a push yapildiginda Vercel otomatik olarak production deploy yapar:

```bash
git add .
git commit -m "Degisiklik aciklamasi"
git push origin main
# Vercel otomatik deploy eder
```

## Ortam Degiskenleri

| Degisken | Aciklama | Nerede |
|----------|----------|--------|
| `GEMINI_API_KEY` | Google Gemini API anahtari | Vercel Dashboard > Settings > Environment Variables |

## Tasarim Sistemi

| Ozellik | Deger |
|---------|-------|
| **Birincil Renk (Navy)** | `#0a1e33` |
| **Aksan Renk (Amber)** | `#e8960c` |
| **Ikincil Renk (Blue)** | `#1a4b7a` |
| **Baslik Fontu** | Outfit |
| **Govde Fontu** | DM Sans |
| **Responsive Breakpoints** | 380px, 480px, 768px, 1024px |

## SEO

- **Schema.org:** LocalBusiness + OfferCatalog (JSON-LD)
- **Open Graph:** Facebook/LinkedIn paylasim onizleme
- **Twitter Card:** Twitter paylasim onizleme
- **Canonical URL:** `https://www.ahsetiket.com/`
- **Sitemap:** XML formatinda tum bolumler
- **Robots.txt:** Arama motoru erisim kurallari
- **Lazy Loading:** Gorsellerde `loading="lazy"`
- **Alt Text:** Tum gorsellerde aciklayici alt metinleri

## Iletisim

- **Telefon:** +90 (216) 706 85 00
- **Mobil:** +90 (530) 264 99 45
- **E-posta:** info@ahsetiket.com
- **Adres:** Cevizli Mah. Karadeniz Sok. No:1, Kartal / Istanbul
- **Web:** [ahsetiket.com](https://ahsetiket.com)

## Lisans

Bu proje AHS Etiket ve Barkod Sistemleri San. Tic. Ltd. Sti.'ye aittir. Tum haklari saklidir.

---

<p align="center">
  <sub>AHS Etiket &copy; 2026 &mdash; Profesyonel Etiket ve Barkod Cozumleri</sub>
</p>
