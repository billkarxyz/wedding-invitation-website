# Wedding Invitation Website

Template undangan pernikahan digital berbahasa Indonesia — elegan, nuansa hijau sage dan emas, mobile-first.

> **Semua data di template ini adalah CONTOH.** Nama mempelai "Amara & Rizky", tanggal Sabtu 12 Juni 2027, tempat The Sultan Hotel Jakarta, nomor rekening, nomor e-wallet, alamat kirim kado, nomor WhatsApp, dan kisah cinta semuanya fiktif sebagai contoh. Ganti dengan data asli sebelum dipakai.

## Fitur

- **Sampul undangan** — tombol "Buka Undangan" membuka isi undangan; nama tamu dipersonalisasi lewat parameter URL, contoh: `index.html?to=Budi`
- **Musik latar** — tombol musik di pojok kanan bawah memutar melodi lembut yang dibuat dengan WebAudio (tanpa file audio eksternal, tanpa hotlink)
- **Countdown live** — hitung mundur ke 12 Juni 2027 08.00 WIB
- **Profil mempelai** — kartu kedua mempelai beserta orang tua
- **Akad & Resepsi** — kartu acara dengan tombol "Lihat Lokasi" (Google Maps) dan "Simpan Tanggal" (Google Calendar)
- **Dress code** — sage green & emas
- **Love story** — timeline kisah pasangan
- **Galeri foto** — 6 foto dengan lightbox (foto dari Unsplash; kalau sebuah foto gagal dimuat, tampilannya tetap rapi)
- **RSVP interaktif** — form nama + kehadiran + ucapan; konfirmasi tampil, ucapan masuk ke dinding ucapan (tersimpan di `localStorage`), plus tautan "Kirim via WhatsApp"
- **Amplop digital** — tombol salin untuk rekening bank, e-wallet, dan alamat kirim kado

## Cara membuka

Tidak perlu build step, tidak ada dependensi, tidak ada backend.

**Lokal:** buka file `index.html` langsung di browser (klik dua kali).

**GitHub Pages:** Settings → Pages → pilih branch `main`, folder `/ (root)` → situs terbit di `https://billkarxyz.github.io/wedding-invitation-website/`.

## Cara personalisasi

Edit langsung di `index.html` (cari dan ganti):

| Yang diganti | Cari |
|---|---|
| Nama mempelai | `Amara` / `Rizky` (judul, sampul, hero, footer) |
| Tanggal acara | `12 Juni 2027` dan target countdown `2027-06-12T08:00:00+07:00` di JavaScript |
| Tempat & alamat | `The Sultan Hotel Jakarta` |
| Nama orang tua | di kartu mempelai |
| Link Google Maps | parameter `query=` pada tautan `google.com/maps/search` |
| Link Google Calendar | parameter `text`, `dates`, `location` pada tautan `calendar.google.com` |
| Nomor rekening / e-wallet / alamat | di bagian Amplop Digital (atribut `data-copy` dan teksnya) |
| Nomor WhatsApp RSVP | `6281234567890` di JavaScript (fungsi RSVP) |
| Foto galeri | URL `images.unsplash.com/...` di bagian galeri |
| Kisah cinta | teks di bagian Love Story |

## Struktur

```
wedding-invitation-website/
├── index.html   # Satu file: HTML + CSS + JavaScript (tanpa dependensi)
└── README.md
```

## Lisensi

Bebas dipakai dan dimodifikasi untuk undangan pribadi.
