# AHS Etiket - Proje Rehberi

## Proje Hakkında
AHS Etiket ve Barkod Sistemleri San. Tic. Ltd. Şti. kurumsal web sitesi. Etiket, ribon ve barkod sistemleri ürünlerini tanıtan statik bir tek sayfa (SPA tarzı) web sitesidir. Dil: Türkçe.

## Teknoloji Yığını
- **HTML5** - Tek sayfa: `index.html`
- **CSS3** - Özel stiller: `css/ahsetiket-style.css`
- **JavaScript** - jQuery 2.2.3 tabanlı
- **Bootstrap 3.3.6** - Responsive grid ve bileşenler
- **Font Awesome** - İkon kütüphanesi
- **Owl Carousel** - Slider/carousel bileşeni
- **Google Fonts** - Muli, Nunito

## Build/Paket Yönetimi
Yok. Saf statik site — npm, webpack veya herhangi bir build aracı kullanılmıyor. Tüm kütüphaneler doğrudan dosya olarak dahil edilmiş.

## Dizin Yapısı
```
ahsetiket/
├── index.html              # Ana sayfa (tüm içerik burada)
├── .htaccess               # Apache yapılandırması
├── robots.txt              # SEO robot kuralları
├── sitemap.xml             # Arama motoru site haritası
├── css/
│   ├── bootstrap.min.css
│   ├── font-awesome.min.css
│   ├── owl.carousel.css
│   ├── owl.theme.default.min.css
│   └── ahsetiket-style.css # Ana özel stiller
├── js/
│   ├── jquery.js
│   ├── bootstrap.min.js
│   ├── owl.carousel.min.js
│   ├── smoothscroll.js
│   └── custom.js           # Ana uygulama mantığı
├── fonts/                  # Font Awesome font dosyaları
└── images/                 # Ürün ve UI görselleri
```

## Site Bölümleri (Anchor Navigasyon)
- `#home` - Ana sayfa / Tanıtım
- `#service` - Teknik Servis
- `#ribon` - Ribon ürünleri (Wax, Wax Resin, Resin)
- `#etiket` - Etiket ürünleri (Kuşe, Vellum, Termal, PP, Silvermat, Fastyre)
- `#akmaz` - Akmaz etiketler (yıkama dayanıklı)
- `#contact` - İletişim bilgileri

## Stil ve Tasarım
- **Birincil renk:** `#41a7ee` (mavi)
- **Aksan renk:** `#3f51b5` (koyu mavi)
- **Koyu arka plan:** `#252525`
- **Responsive breakpoints:** 480px, 580px, 767px, 768px, 992px, 1170px

## Özel JavaScript (custom.js)
- Preloader animasyonu
- Navbar scroll davranışı (sabitlenme)
- Owl Carousel başlatma (home-slider, owl-courses, owl-client)
- Smooth scroll navigasyon
- Mobil menü otomatik kapanma

## Bilinen Eksiklikler
- `components/contact.js` ve `components/footer.js` referans edilmiş ancak dosyalar mevcut değil
- Form doğrulama (validation) mantığı yok
- Backend entegrasyonu yok

## Deployment
Apache sunucusu üzerinde `.htaccess` ile yönlendirme. Statik dosya sunumu.
