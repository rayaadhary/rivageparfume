# Rivage Parfume

Landing page toko parfum refill di Indramayu. Satu tujuan: klik WhatsApp.

Astro static, tanpa JavaScript, tanpa framework CSS.

## Jalankan

```bash
npm install
npm run dev      # http://localhost:4321
npm run build    # output ke dist/
npm run preview
```

## Isi

- `src/pages/index.astro` satu halaman
- `src/styles/global.css` design system (paper/ink, satu aksen bronze)
- `src/layouts/BaseLayout.astro` meta, OG, JSON-LD LocalBusiness
- `public/images/` hero (640w dan 1080w) dan versi OG
- `public/fonts/` Cormorant Garamond + Plus Jakarta Sans, latin subset, variable

## Data bisnis

Alamat, jam buka, dan koordinat mengikuti listing Google Maps. Kalau listing diubah, ubah juga `src/layouts/BaseLayout.astro` dan section lokasi.

## Deploy

Build command `npm run build`, publish directory `dist`, Node 24.

Domain aktif sementara: `https://rivageparfume.vercel.app`. Saat pindah ke `rivageparfume.com`, cukup ubah `site` di `astro.config.mjs`; canonical, OG, dan JSON-LD ikut menyesuaikan.
