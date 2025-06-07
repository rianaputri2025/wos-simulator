# Changelog: Chief Gear Simulator v1.2

**Tanggal Rilis:** 7 Juni 2025

---

Versi 1.2 merupakan pembaruan besar yang berfokus pada perombakan total desain visual, perbaikan bug kritis, dan peningkatan pengalaman pengguna secara keseluruhan, baik di desktop maupun mobile.

## ✨ Fitur Baru & Peningkatan Visual (Features & Visual Enhancements)

### 🎨 Desain Ulang Total Tampilan (UI Overhaul)

- Mengganti tema warna lama dengan palet **Violet & Indigo** yang modern, bersih, dan profesional.
- Memperkenalkan efek **gradient** pada elemen-elemen kunci seperti judul dan tombol untuk tampilan premium.
- Menggunakan font **Poppins** dari Google Fonts untuk tipografi yang lebih baik di seluruh situs.

### 🏠 Halaman Home yang Sepenuhnya Baru

- Mengubah halaman Home dari satu blok teks menjadi **landing page** yang terstruktur dengan beberapa bagian: Hero, Deskripsi Fitur, dan Kartu Donasi.
- Menghapus header navigasi dan menggantinya dengan desain minimalis (hanya logo di atas) untuk pengalaman yang lebih fokus.
- Menambahkan tombol "call-to-action" yang jelas di dalam kartu deskripsi untuk mengarahkan pengguna langsung ke halaman simulator.

### 🌟 Animasi Ikon Interaktif

- Menambahkan animasi pada ikon fitur di halaman Home saat kursor diarahkan.
- Ikon gear (`fa-cogs`) kini berputar secara berlawanan untuk efek mekanik yang realistis, menggunakan kustomisasi SVG.
- Ikon perisai (`fa-shield-alt`) kini memancarkan efek "aura" atau _glow_ yang halus.

### 🔄 Peningkatan Alur Pengguna (User Flow)

- Halaman simulator kini memiliki tombol "**Back to Home**" yang jelas, menggantikan navigasi header untuk alur yang lebih intuitif.
- Menata ulang posisi tombol-tombol aksi (⚙️, 🔄, 🧹) agar lebih rapi dan mudah diakses.

---

## 🚀 Perbaikan Bug & Optimasi (Fixes & Optimizations)

- **[FATAL] Bug Upgrade Material 0 Diperbaiki:** Memperbaiki bug kritis di mana pengguna bisa melakukan upgrade meskipun material yang dimiliki adalah 0. Logika pengecekan material telah dikembalikan ke versi asli yang stabil.

- **[FATAL] Bug Posisi Preview Diperbaiki:**

  - Menghapus total metode posisi pratinjau gear berbasis JavaScript (`updateGearPreviewPosition`) yang tidak stabil dan menyebabkan posisi "melompat" atau salah tempat.
  - Menggantinya dengan metode **CSS murni** (`position` + `transform`) yang menjamin posisi pratinjau selalu sempurna dan stabil di semua perangkat.

- **Bug Sinkronisasi Modal "Set Start Levels":** Memperbaiki masalah di mana modal tidak menampilkan level gear terbaru setelah pengguna melakukan upgrade.

- **Bug Modal Tidak Muncul:** Memperbaiki kesalahan logika JavaScript di mana beberapa modal tidak muncul karena penggunaan class `.show` dan `.hidden` yang tidak konsisten.

- **Perbaikan Tampilan Mobile Menyeluruh:**

  - Menyesuaikan ukuran font, padding, dan margin di seluruh halaman simulator agar terlihat rapi di layar kecil.
  - Memastikan tata letak gear tidak lagi terlalu mepet ke pinggir layar.
  - Memperbaiki ukuran gambar pratinjau yang sebelumnya terlalu besar di perangkat mobile.

- **Peningkatan Lainnya:**
  - Memperbaiki jarak antar bintang (⭐) pada gear yang sebelumnya terlalu renggang.
  - Memastikan semua suara (klik, upgrade) berfungsi kembali seperti seharusnya.
  - Menyatukan semua gaya CSS untuk setiap halaman ke dalam filenya masing-masing (`home.css` dan `gears.css`) untuk menghindari konflik dan mempermudah pengelolaan.
