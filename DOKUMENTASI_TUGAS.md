# DOKUMENTASI TUGAS PRAKTIK: LANDING PAGE BISNIS DIGITAL
**Mata Kuliah:** Web Development Lab (BDI63304)  
**Dosen Pengampu:** Dr. Bimo Haryo Setyoko, M.Kom  
**Nama Mahasiswa:** Rido Azimi  
**NIM:** 63050250037  
**Program Studi:** S1 Bisnis Digital (Kelas 3B)  
**Fakultas:** Fakultas Ekonomi dan Bisnis Islam, UIN Salatiga  

---

## 1. Business Brief & Konsep Bisnis
* **Nama Bisnis:** Dorizz Creative
* **Bidang Usaha:** Studio Jasa Branding & Pengembangan Landing Page UMKM
* **Target Pasar:**
  1. Pelaku Usaha Mikro, Kecil, dan Menengah (UMKM) lokal yang ingin bermigrasi ke ekosistem digital.
  2. Brand fashion, kuliner/F&B, dan jasa rintisan yang belum memiliki identitas brand konsisten.
  3. Pemilik bisnis yang membutuhkan media promosi cepat dan langsung terhubung ke WhatsApp penjualan tanpa kerumitan teknis.
* **Tujuan Website:**
  Menjadi landing page satu halaman (single-page) yang berorientasi pada konversi penjualan (*conversion-driven*), mempermudah calon klien memahami portofolio layanan, melihat transparansi harga, dan langsung menghubungi tim via formulir konsultasi atau WhatsApp.

---

## 2. Struktur Konten & Elemen Halaman (Pemenuhan 8 Komponen Wajib)
1. **Header / Navbar:** Memuat logo brand, tautan menu jangkar (*smooth scrolling* ke setiap section), serta tombol aksi cepat "Hubungi Kami". Responsif menjadi tombol hamburger saat diakses via ponsel.
2. **Hero Section:** Menampilkan *Value Proposition* yang kuat ("Tingkatkan Omzet UMKM Lewat Identitas Brand yang Kuat"), subjudul penjelas, badge kredibilitas, dan 2 tombol Call-to-Action (CTA) kontras.
3. **Tentang Bisnis:** Uraian latar belakang berdirinya Dorizz Creative disertai kartu statistik metrik pencapaian (50+ UMKM, 98% Kepuasan).
4. **Produk / Layanan (Card Bootstrap):** Menampilkan 3 paket layanan dengan kartu sejajar (`h-100`):
   - *Social Media Branding* (Mulai Rp 350.000/bln)
   - *Landing Page UMKM* (Mulai Rp 500.000/web - Paling Populer)
   - *Desain Visual & Logo* (Mulai Rp 250.000/paket)
5. **Keunggulan (Value Proposition):** 3 poin diferensiasi utama: Harga Terjangkau UMKM, Berorientasi Penjualan, dan Pendampingan Konsultasi Intensif.
6. **Testimoni Pelanggan:** Menampilkan ulasan riil pelanggan fiktif (Owner Kedai Kopi & Founder Brand Hijab) lengkap dengan rating bintang dan avatar inisial untuk memperkuat faktor kepercayaan (*social proof*).
7. **Formulir Kontak / CTA:** Formulir pendaftaran konsultasi (Nama, WhatsApp, Nama Usaha, Pilihan Layanan, Catatan Kebutuhan) dengan validasi dasar `required`.
8. **Footer:** Bagian penutup berisi deskripsi singkat agensi, tautan navigasi cepat, kontak resmi (alamat, email, nomor WhatsApp), dan hak cipta.

---

## 3. Keputusan Desain, Tipografi & Warna
* **Alasan Pemilihan Warna:**
  - *Warna Primer (Primary Blue #0d6efd / Deep Navy #0a2540):* Melambangkan profesionalitas, teknologi, keamanan, dan stabilitas khas agensi digital modern.
  - *Warna Aksen (Warning Yellow #ffc107):* Memberikan kontras tinggi pada badge penawaran dan tombol Call to Action penting agar langsung menarik mata pembeli (*visual focal point*).
  - *Warna Latar (Light Grey #f8f9fa & Putih #ffffff):* Memberikan ruang negatif (*whitespace*) yang lega, menjaga keterbacaan teks (*readability*), dan memberi kesan bersih (clean).
* **Tipografi:** Menggunakan *system font stack* modern (`system-ui, -apple-system, Segoe UI, Roboto`) yang ringan, cepat dimuat pada koneksi seluler, dan tajam di berbagai resolusi layar.

---

## 4. Implementasi Teknis HTML & CSS
1. **Semantic HTML5:** Memanfaatkan tag semantik `<header>`, `<nav>`, `<section>`, dan `<footer>` alih-alih hanya menggunakan tag `<div>` generik.
2. **Bootstrap 5 CDN:** Memanfaatkan sistem Grid 12 kolom (`.container`, `.row`, `.col-*`) untuk memastikan tata letak otomatis rapi di layar desktop (3 kolom) dan layar ponsel (1 kolom full-width) tanpa horizontal scrolling.
3. **External CSS (`style.css`):** Digunakan untuk styling khusus yang tidak disediakan Bootstrap bawaan, meliputi:
   - CSS variables (`:root`) untuk konsistensi warna brand.
   - Efek transisi halus kartu terangkat saat disentuh kursor (`transform: translateY(-6px)`).
   - Efek latar belakang gradien hero section (`linear-gradient`).
   - Pergerakan gulir halus antar menu (`scroll-behavior: smooth`).
