# Panduan Deployment GitHub Pages (PWA)

Folder `pwa/` ini berisi kerangka Progressive Web App (PWA) untuk **Kok Kepikiran Nyemil**:
- `manifest.json`: Konfigurasi aplikasi installable (Android & Windows Edge/Chrome).
- `sw.js`: Service Worker untuk caching shell aplikasi saat offline.

## Langkah Publish ke GitHub Pages
1. Buat repository baru di GitHub (misalnya `kkn-kasir`).
2. Upload seluruh isi project (`pwa/` + `Index.html` yang di-rename menjadi `index.html` di folder `pwa/` atau root, serta backend `*.gs` di folder `backend-appsscript/`).
3. Untuk menghubungkan `index.html` di GitHub Pages ke backend Google Apps Script, tambahkan endpoint `doPost(e)` di `Code.gs` atau embed Web App URL di dalam `iframe` / `fetch`.
4. Di GitHub repository: buka **Settings > Pages > Source: Deploy from a branch (`main`)**.
5. Buka URL GitHub Pages di Chrome (Android) atau Edge/Chrome (Windows), lalu klik **Install App / Tambahkan ke Layar Utama**.
