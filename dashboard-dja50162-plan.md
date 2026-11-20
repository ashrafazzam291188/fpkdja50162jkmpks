# Plan: Dashboard Fail Penyelaras Kursus — DJA50162 Vehicle Dynamics

## Overview

Bina sebuah dashboard HTML statik bergaya rasmi Politeknik Kuching Sarawak (PKS) untuk **Fail Penyelaras Kursus DJA50162 Vehicle Dynamics**. Dashboard ini merangkumi maklumat kursus, maklumat penyelaras, komponen penilaian dengan carta pai interaktif, jadual kuliah, dan senarai dokumen. Reka bentuk menggunakan warna rasmi PKS (biru tua `#003580` dan emas `#FFB800`), responsif, dan mesra cetak.

### Maklumat Utama

- **Institusi:** Politeknik Kuching Sarawak (PKS)
- **Kod Kursus:** DJA50162
- **Nama Kursus:** Vehicle Dynamics
- **Sesi:** Sesi I: 2026/2027
- **Penyelaras Kursus:** Ashraf Azzam Bin Zulkifli Amin
- **Jabatan:** Kejuruteraan Mekanikal
- **Email:** ashraf@poliku.edu.my
- **No. Tel:** 082-845 596

### Komponen Penilaian

| Komponen | Wajaran |
|----------|---------|
| Test | 15% |
| Quiz 1 | 5% |
| Quiz 2 | 5% |
| Presentation | 10% |
| Case Study | 15% |
| Final Exam | 50% |
| **Jumlah** | **100%** |

---

## Sub-Task 1: Struktur HTML Asas & Header

**Status:** [x] done

### Intent
Bina fail `index.html` dengan struktur HTML lengkap termasuk header rasmi PKS, metadata, dan import library (Chart.js).

### Expected Outcomes
- Fail `index.html` wujud dengan struktur HTML5 yang sah
- Header menunjukkan logo placeholder PKS, nama institusi, nama kursus, kod kursus, dan sesi
- Chart.js dimuatkan melalui CDN

### Todo List
- [ ] Cipta fail `index.html` dengan boilerplate HTML5
- [ ] Tambah `<head>` dengan metadata, link CSS, dan CDN Chart.js
- [ ] Bina `<header>` dengan logo PKS, nama institusi, tajuk kursus, dan maklumat sesi
- [ ] Bina struktur navigasi tab (`Maklumat Kursus`, `Penilaian`, `Jadual`, `Dokumen`)
- [ ] Tambah `<main>` dan `<footer>` sebagai placeholder untuk sub-task seterusnya

### Relevant Context
- Warna header: biru tua `#003580`, teks emas `#FFB800`
- Logo PKS boleh menggunakan placeholder teks "PKS" dalam bulatan berwarna emas
- Nama institusi: "POLITEKNIK KUCHING SARAWAK"
- Tajuk dokumen: "Fail Penyelaras Kursus | DJA50162 Vehicle Dynamics"

---

## Sub-Task 2: CSS Gaya Rasmi PKS

**Status:** [x] done

### Intent
Cipta fail `style.css` dengan keseluruhan gaya visual bergaya rasmi PKS, termasuk kad, jadual, butang, dan responsif.

### Expected Outcomes
- Fail `style.css` wujud dengan semua gaya yang diperlukan
- Palet warna PKS digunakan secara konsisten
- Layout responsif untuk desktop dan mudah alih
- Gaya mesra cetak dengan `@media print`

### Todo List
- [ ] Cipta fail `style.css`
- [ ] Tetapkan CSS variables untuk palet warna PKS
- [ ] Gaya header, nav bar, dan footer
- [ ] Gaya info cards (4 kad statistik) dengan bayangan dan hover effect
- [ ] Gaya jadual penilaian dengan warna baris berselang
- [ ] Gaya senarai dokumen dengan ikon dan butang muat turun
- [ ] Tambah `@media` query untuk responsif (tablet & telefon)
- [ ] Tambah `@media print` untuk cetakan rasmi

### Relevant Context
- Warna utama: `#003580` (biru tua PKS)
- Warna aksen: `#FFB800` (emas PKS)
- Latar belakang: `#F5F7FA` (kelabu cerah)
- Font: Google Fonts 'Poppins' atau 'Inter' untuk tampilan profesional
- Kad dengan `border-radius: 12px` dan `box-shadow` untuk kedalaman visual

---

## Sub-Task 3: Bahagian Maklumat Kursus & Penyelaras

**Status:** [x] done

### Intent
Bina bahagian info cards statistik dan panel dua kolum untuk maklumat kursus dan penyelaras.

### Expected Outcomes
- 4 kad statistik pantas ditunjukkan di bahagian atas
- Panel maklumat kursus (kiri) dan maklumat penyelaras (kanan) ditunjukkan bersebelahan
- Semua data kursus dan penyelaras diisi dengan betul

### Todo List
- [ ] Bina 4 info cards: Jumlah Pelajar (placeholder), Komponen Penilaian (6), Kredit Jam (3), Sesi (Sesi I: 2026/2027)
- [ ] Bina panel maklumat kursus: Kod DJA50162, Nama Vehicle Dynamics, Kredit 3 jam, Jabatan Kejuruteraan Mekanikal
- [ ] Bina panel maklumat penyelaras: Nama Ashraf Azzam, Jabatan Kejuruteraan Mekanikal, Email ashraf@poliku.edu.my, No Tel 082-845 596
- [ ] Tambah ikon SVG atau emoji untuk setiap item maklumat

### Relevant Context
- Layout 2 kolum menggunakan CSS Grid atau Flexbox
- Gunakan kad bersempadan biru dengan tajuk berlatar biru tua dan teks putih

---

## Sub-Task 4: Bahagian Penilaian & Carta Pai

**Status:** [x] done

### Intent
Bina jadual penilaian lengkap dengan 6 komponen dan carta pai interaktif menggunakan Chart.js.

### Expected Outcomes
- Jadual penilaian menunjukkan 6 komponen dengan wajaran yang betul (jumlah 100%)
- Carta pai interaktif dipaparkan bersebelahan jadual
- Badge status boleh dikemaskini (Belum Mula / Dalam Proses / Selesai)

### Todo List
- [ ] Bina jadual HTML untuk 6 komponen penilaian dengan kolum: No, Komponen, Wajaran, Status
- [ ] Tambah baris jumlah (100%) di bawah jadual
- [ ] Bina `<canvas>` untuk Chart.js carta pai
- [ ] Tulis JavaScript dalam `main.js` untuk render carta pai dengan data 6 komponen
- [ ] Gunakan warna yang berbeza untuk setiap segmen carta pai
- [ ] Tambah badge status berwarna untuk setiap komponen

### Relevant Context
- Chart.js dimuatkan dari CDN
- Data carta pai: Test 15%, Quiz 1 5%, Quiz 2 5%, Presentation 10%, Case Study 15%, Final Exam 50%
- Warna segmen carta: gunakan palet warna harmoni yang sesuai dengan tema PKS
- Fail JavaScript: `main.js`

---

## Sub-Task 5: Bahagian Jadual Kuliah & Senarai Dokumen

**Status:** [x] done

### Intent
Bina bahagian jadual kuliah/tutorial (dengan data placeholder boleh diisi) dan senarai dokumen kursus rasmi.

### Expected Outcomes
- Jadual kuliah menunjukkan hari, masa, tempat, dan jenis sesi (placeholder)
- Senarai dokumen menunjukkan 4 dokumen rasmi dengan butang muat turun (placeholder)
- Footer menunjukkan maklumat hak cipta PKS

### Todo List
- [ ] Bina jadual timetable dengan kolum: Hari, Masa, Tempat, Jenis Sesi
- [ ] Isi 2 baris placeholder untuk kuliah dan tutorial
- [ ] Bina senarai dokumen: RPP, Rubrik Penilaian, Soalan Peperiksaan, Borang Pemantauan
- [ ] Tambah butang "Muat Turun" (placeholder `href="#"`) untuk setiap dokumen
- [ ] Bina footer dengan nama institusi, logo placeholder, dan tahun hak cipta
- [ ] Pastikan tab navigasi berfungsi dengan JavaScript untuk show/hide bahagian

### Relevant Context
- Butang muat turun bergaya biru PKS dengan hover effect emas
- Footer latar biru tua dengan teks putih/emas
- Tab navigasi menggunakan JavaScript mudah (tambah/buang class `active`)
