# Flutter Profile App

Aplikasi profil sederhana yang dibangun menggunakan Flutter. Proyek ini difokuskan pada pemahaman struktur dasar *widget*, penyelesaian masalah tata letak (*layout crash/overflow*), dan penerapan praktik *clean code* dengan memisahkan UI menjadi komponen-komponen yang dapat digunakan kembali (*reusable widgets*).

### Data Mahasiswa
- **Nama:** Fadhil Hidayattulloh
- **NIM:** 1124160087
- **Kelas:** TI SE 2 P

---

## Ringkasan Progres & Riwayat Commit

### 29 Oktober 2026 - Inisialisasi & Setup Awal
* **`first commit code dari docs`** 
  Menginisialisasi struktur awal proyek berdasarkan kode dari dokumentasi.
* **`fix commit - add import package`** 
  Memperbaiki struktur file dengan menambahkan baris *import package* yang dibutuhkan.
* **`remove ");" karna tidak di gunakan`** 
  Membersihkan sisa *syntax* berlebih untuk mencegah *error build*.

### 30 Oktober 2026 - Perbaikan Bug Data & Testing
* **`fix line 94, fix tipe data count (bukan string)`** 
  Melakukan penyesuaian tipe data pada properti angka statistik aplikasi.
* **`fix: ganti nama MainApp di widget test dan benerin error const di widget test`** 
  Menyelaraskan nama kelas *root* menjadi `MainApp` dan mengatasi masalah *const constructor* pada file pengujian (`widget_test.dart`).
* **`fix: benerin koma di list experiences dan SizedBox statistik`** 
  Memperbaiki *syntax error* akibat koma yang terlepas pada list pengalaman, serta memperbaiki penggunaan `SizedBox` (mengubah orientasi *height* ke *width*) agar tata letak statistik menjadi sejajar dan rapi.

### 31 Oktober 2026 - Perbaikan Layout Crash & Scrolling
* **`fix: bungkus body dengan SingleChildScrollView agar bisa di scroll`** 
  Mencegah layar terpotong (*overflow*) pada perangkat layar kecil dengan menambahkan fitur *scroll* vertikal.
* **`fix: tambah shrinkWrap dan physics NeverScrollable di ListView`** 
  Mengatasi masalah layar kosong (*unbounded height crash*) saat merender `ListView` di dalam kolom dengan membatasi ukurannya menggunakan `shrinkWrap` dan mematikan *scroll* internalnya agar tidak bentrok dengan *scroll* utama.

### 1 November 2026 - Refactoring & Finalisasi
* **`refactor: pisah" UI profil menjadi beberapa reusable widget`** 
  Merombak keseluruhan kode agar lebih modular. Memisahkan struktur UI bertumpuk menjadi kelas-kelas mandiri seperti `ProfileScreen`, `ProfileHeader`, `ProfileStats`, `StatItem`, dan `ExperienceSection`.
* **`update experience kerja ke experience project`** 
  Memperbarui label teks antarmuka dari "Pengalaman Kerja" menjadi "Pengalaman Project" agar lebih relevan dengan isi portofolio.

### 3 November 2026 - Dokumentasi Tambahan
* **`docs: update README dengan riwayat commit lengkap`**
  Menambahkan `README.md` ini untuk mendokumentasikan progres pengerjaan tugas secara rinci dari awal pembuatan hingga *refactoring* selesai.
