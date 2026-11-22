# SuaraKita — Ruang Cerita Anonim

SuaraKita adalah prototipe komunitas berbagi cerita anonim berbahasa Indonesia. Pengunjung dapat membaca cerita, membuat posting, memberi dukungan, menulis tanggapan, mencari cerita, dan menjelajahi kategori.

## Demo lokal

Buka `index.html` di browser atau jalankan server statis:

```bash
python -m http.server 8000
```

Lalu buka http://localhost:8000.

## Deploy ke GitHub Pages

1. Buat repository GitHub bernama `SuaraKita` (atau nama lain).
2. Unggah `index.html`, `styles.css`, `app.js`, dan `README.md` ke root repository.
3. Buka **Settings → Pages**.
4. Pilih **Deploy from a branch**, branch `main`, folder `/(root)`, lalu Save.
5. Tunggu proses deployment selesai di tab **Actions**.
6. Alamat umumnya `https://USERNAME.github.io/NAMA-REPOSITORY/`.

Jika memakai repository `Muhzarx/SuaraKita`, alamatnya: https://muhzarx.github.io/SuaraKita/

## Fitur prototipe

- Feed cerita terbaru dan populer.
- Kategori: percintaan, keluarga, pertemanan, pendidikan, kehidupan, dan bebas cerita.
- Buat cerita dengan nama samaran.
- Reaksi dukungan, komentar, pencarian, dan berbagi.
- Pelaporan konten (simulasi antarmuka).
- Penyimpanan lokal menggunakan `localStorage`.
- Desain responsif untuk desktop dan ponsel.

## Penting: status penyimpanan dan anonimitas

Versi ini adalah **frontend demo**. Data disimpan di browser/perangkat pengguna melalui `localStorage`. Artinya posting, reaksi, dan komentar belum tersinkron antarperangkat atau terlihat oleh pengguna lain. Menghapus data browser dapat menghapus konten demo. Nama samaran juga bukan jaminan anonimitas teknis.

Untuk menjadikannya komunitas publik sungguhan, sambungkan backend seperti Firebase atau Supabase. Implementasi produksi sebaiknya mencakup:

- Authentication anonim atau akun dengan nama publik terpisah dari identitas login.
- Database real-time untuk posting, komentar, dan reaksi.
- Storage untuk lampiran jika diperlukan.
- Rate limiting, validasi server-side, anti-spam, dan pembatasan penyalahgunaan.
- Alur laporan, antrean moderasi, blokir pengguna, serta kebijakan privasi dan ketentuan komunitas.
- Aturan keamanan database agar pengguna hanya dapat mengubah konten miliknya dan tidak dapat memanipulasi jumlah reaksi.

Jangan mempublikasikan layanan komunitas anonim tanpa moderasi aktif. Hindari mengumpulkan data pribadi yang tidak diperlukan.

## Struktur

```text
SuaraKita/
├── index.html
├── styles.css
├── app.js
└── README.md
```

## Lisensi

MIT — silakan gunakan, modifikasi, dan kembangkan lebih lanjut.
