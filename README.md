# Personal Portfolio — Indra Dwiyantoro

Website portfolio satu halaman untuk tugas UTS Pemrograman Web. Dibuat hanya dengan **HTML5 dan CSS3**, tanpa JavaScript dan tanpa framework.

## Struktur folder

```text
UTS_Web_312510495_Indra_Dwiyantoro/
├── index.html
├── style.css
├── images/
│   └── profil.jpg
├── media/
│   ├── perkenalan.mp4
│   ├── perkenalan.mp3
│   └── README.md
├── screenshots/
│   ├── portfolio-desktop.png
│   └── portfolio-mobile.png
└── README.md
```

> Sebelum dikumpulkan, ubah nama folder `UTS_Web_NIM_Indra_Dwiyantoro` dengan NIM milikmu yang benar. `NIM` pada nama folder masih berupa placeholder.

## Komponen yang memenuhi spesifikasi UTS

1. **Struktur dokumen & Semantic HTML5:** menggunakan `header`, `nav`, `main`, `section`, `article`, `table`, `form`, dan `footer`.
2. **Header, navigasi, dan hero panel:** navigasi desktop dan menu mobile HTML5 `<details>` / `<summary>`, serta hero dengan teks “Hello, my name is Indra Dwiyantoro”.
3. **Biografi & profil utama:** identitas, profesi, lokasi, platform commission, dan jumlah proyek.
4. **Tabel riwayat pendidikan:** Budi Mulia Karawang Vocational High School (2021–2024), Computer and Network Engineering, serta Junior High School 1 South Cikarang (2017–2020).
5. **Tabel riwayat pengalaman kerja:** Motion Graphics Intern di Truggl (Februari–Juli 2025), Motion Graphics Intern di MAHA5 / Rentacks Creative Works (September 2025–Juli 2026), dan Freelance Projects (2024–sekarang).
6. **Riwayat keahlian:** menggunakan unordered list yang memuat motion graphics, video editing, After Effects, Premiere Pro, Photoshop, Illustrator, color grading, dan visual transitions.
7. **Elemen multimedia:** enam video YouTube ditampilkan melalui `iframe` pada bagian Multimedia & Selected Work. Video perkenalan lokal (`media/perkenalan.mp4`) dan audio perkenalan (`media/perkenalan.mp3`) tersedia pada bagian Introduction dengan kontrol pemutar bawaan browser.
8. **Form kontak & validasi:** memakai validasi bawaan HTML5 melalui `required`, `type="email"`, `minlength`, dan `maxlength`. Form memakai `mailto:` untuk membuka aplikasi email; ganti `YOUR_EMAIL_ADDRESS` di atribut `action` pada `index.html` dengan alamat email penerima sebelum website dipublikasikan. Form tidak memerlukan JavaScript, tetapi memerlukan aplikasi email default yang terkonfigurasi.
9. **Styling & layout CSS3:** layout responsif, tabel dengan horizontal scroll di layar kecil, aksen biru, hover transitions, serta parallax/fade hero menggunakan CSS scroll-driven animations pada browser yang mendukungnya.

## Data CV

Data pendidikan, pengalaman, dan keahlian mengikuti informasi yang diberikan melalui screenshot CV. Kalimat bahasa Inggris dirapikan agar konsisten, sementara organisasi, periode, dan substansi tanggung jawab dipertahankan.

## Cara menjalankan

1. Extract ZIP.
2. Buka `index.html` menggunakan browser.
3. Koneksi internet diperlukan untuk Google Fonts dan video embed YouTube.

## Efek parallax dan fade hero

Efek dibuat sepenuhnya dengan CSS `view-timeline`, `animation-timeline`, dan `animation-range`. Fade berjalan saat hero meninggalkan viewport dan bergerak balik saat pengguna scroll ke atas. Parallax foto memakai variabel `--parallax-distance`: default 52px pada desktop dan 30px pada mobile. Ubah variabel ini di blok `@supports (animation-timeline: view())` pada bagian bawah `style.css` untuk mengatur sensitivitas.

Browser yang belum mendukung CSS scroll-driven animations akan menampilkan hero secara normal tanpa parallax/fade. Pengaturan `prefers-reduced-motion` juga mematikan animasi untuk pengguna yang memilih pengurangan gerakan.

## Menu navigasi mobile

Menu mobile menggunakan elemen HTML native `<details>` dan `<summary>`. Pengguna dapat membuka atau menutupnya tanpa JavaScript. Setelah memilih tautan section, menu dapat ditutup kembali dengan menekan ikon menu.

## Form kontak

Form memakai validasi native browser. Setelah data valid dikirim, browser akan membuka aplikasi email default melalui tautan `mailto:`. Tidak ada pengolahan data, clipboard API, atau pengiriman otomatis ke server. Pastikan mengganti `YOUR_EMAIL_ADDRESS` pada form action sebelum menggunakannya secara publik.
