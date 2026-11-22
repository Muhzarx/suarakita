# SuaraKita — Ruang Cerita Anonim

**Ceritakan tanpa harus dikenal.** SuaraKita adalah prototipe platform komunitas untuk berbagi cerita, membaca pengalaman orang lain, dan saling memberi dukungan melalui identitas samaran.

## 🌐 Demo

**[Buka SuaraKita](https://muhzarx.github.io/suarakita/)**

> Jika tautan belum dapat dibuka, pastikan GitHub Pages sudah diaktifkan melalui **Settings → Pages** pada repository ini.

## ✨ Fitur

- Membaca feed cerita terbaru dan populer.
- Membuat cerita menggunakan nama samaran.
- Memilih kategori cerita: percintaan, keluarga, pertemanan, pendidikan, kehidupan, dan bebas cerita.
- Memberikan reaksi dukungan pada cerita.
- Menulis komentar atau tanggapan.
- Mencari cerita dan menjelajahi kategori.
- Melaporkan konten melalui antarmuka demo.
- Tampilan responsif untuk desktop dan perangkat seluler.

## 🚀 Menjalankan secara lokal

1. Clone repository ini:

   ```bash
   git clone https://github.com/Muhzarx/suarakita.git
   ```

2. Masuk ke folder proyek:

   ```bash
   cd suarakita
   ```

3. Buka `index.html` di browser. Alternatifnya, jalankan server lokal:

   ```bash
   python -m http.server 8000
   ```

4. Buka `http://localhost:8000`.

## 📦 Deploy ke GitHub Pages

1. Pastikan `index.html`, `styles.css`, dan `app.js` berada di root repository.
2. Buka **Settings → Pages**.
3. Pada bagian **Build and deployment**, pilih **Deploy from a branch**.
4. Pilih branch `main` dan folder `/(root)`, lalu klik **Save**.
5. Tunggu proses publikasi selesai. Statusnya dapat diperiksa pada tab **Actions**.
6. Buka [https://muhzarx.github.io/suarakita/](https://muhzarx.github.io/suarakita/).

## 🛠️ Teknologi

- HTML
- CSS
- JavaScript
- Browser `localStorage` untuk penyimpanan data demo

## ⚠️ Catatan penting

Versi saat ini merupakan **prototype frontend**. Cerita, komentar, dan reaksi disimpan di `localStorage` pada browser masing-masing. Karena itu, data belum dibagikan atau disinkronkan antar pengguna maupun perangkat. Fitur pelaporan juga masih berupa simulasi antarmuka, belum mengirim laporan ke moderator.

Agar SuaraKita menjadi komunitas publik sungguhan, proyek ini perlu dihubungkan ke backend seperti Firebase atau Supabase untuk autentikasi, database real-time, dan penyimpanan data bersama. Sebelum dibuka untuk publik, tambahkan validasi sisi server, pembatasan spam, sistem moderasi, pelaporan yang benar-benar berfungsi, serta kebijakan privasi dan pedoman komunitas.

Nama samaran membantu menyembunyikan nama publik, tetapi tidak otomatis menjamin anonimitas teknis. Jangan membagikan informasi pribadi di dalam cerita.

## 📁 Struktur proyek

```text
suarakita/
├── index.html
├── styles.css
├── app.js
└── README.md
```

## 📄 Lisensi

MIT. Silakan gunakan, pelajari, dan kembangkan proyek ini lebih lanjut.
