# Sistem Absensi Kelas Berbasis Web

Prototipe interaktif web sistem absensi kelas akademik dengan 3 peran pengguna (*Admin*, *Dosen/Guru*, *Mahasiswa/Siswa*) serta dukungan mode Desktop dan Mobile, dibuat berdasarkan dokumen desain dan arsitektur informasi pada `Sistem_Absensi_Kelas_Lengkap.pdf`.

## 🚀 Fitur Utama

### 1. Tiga Ruang Kerja Pengguna (Role-Based Workspaces)
- **Admin**:
  - **Dashboard Admin**: Ringkasan statistik (total pengguna, kelas, mata pelajaran, sesi aktif), grafik bar kehadiran mingguan (90%), aktivitas terbaru, dan ringkasan hari ini.
  - **Manajemen Pengguna**: Tabel daftar pengguna, filter peran & status, formulir interaktif ubah/tambah akun pengguna.
  - **Kelas & Mata Pelajaran**: Kelola kelas aktif (TI-3A, TI-3B, SI-3A, SI-3B) dan kurikulum mata pelajaran (Basis Data, Pemrograman Web, Statistika, dsb.).
  - **Pengaturan Jadwal**: Tabel jadwal mingguan dengan status deteksi benturan otomatis (*"Tidak ada benturan"*).

- **Dosen / Guru**:
  - **Dashboard Dosen**: Jadwal mengajar hari ini, banner sesi aktif, dan progres persentase kehadiran per kelas.
  - **Buat Sesi Absensi**: Formulir pembuatan sesi baru yang terhubung langsung dengan kartu *Ringkasan Sesi* secara dinamis.
  - **Pemantauan Kehadiran & Rekap**: Metrik kehadiran real-time (*Peserta kelas*, *Hadir*, *Izin*, *Belum mengisi*), tabel kehadiran per mahasiswa, tombol unduh laporan CSV dan cetak.

- **Mahasiswa / Siswa**:
  - **Dashboard Mahasiswa**: Ringkasan kehadiran semester (90,6%), kartu Hadir/Izin/Alpa, dan jadwal hari ini.
  - **Halaman Absensi Interaktif**: Tombol *"Kirim kehadiran sekarang"* yang dapat diklik langsung untuk merekam kehadiran (`Hadir` tercatat pada `09.21.14 WIB`), menampilkan banner sukses, mengunci tombol agar tidak dobel submit, dan menyinkronkan status ke layar Dosen.
  - **Riwayat Kehadiran**: Filter riwayat kehadiran semester ganjil per mata pelajaran dan status.

### 2. Simulator Tampilan Mobile
- Tampilan frame smartphone interaktif lengkap dengan status bar waktu `09.20 WIB` dan navigasi bawah (*Bottom Navigation Bar*).
- Menampilkan *Mobile Dashboard* dan *Mobile Halaman Absensi* persis seperti panduan desain.

---

## 💻 Cara Menjalankan

Cukup buka file `index.html` langsung di peramban web (*Google Chrome, Edge, Firefox, Safari*). Tidak membutuhkan instalasi dependensi atau web server khusus.

```bash
# Atau jika menggunakan Live Server / browser:
start index.html
```

---

## 🛠️ Teknologi yang Digunakan
- **HTML5 & Vanilla JavaScript** (interaktivitas instan tanpa build step)
- **Tailwind CSS** (via CDN untuk utility-first styling)
- **Lucide Icons** (ikon modern & bersih)
- **Google Fonts** (Plus Jakarta Sans)
