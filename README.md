# 🧊 Manajemen Tugas Mahasiswa  
> Aplikasi web interaktif untuk mengelola tugas kuliah dengan tampilan modern bergaya **glassmorphism** dan dukungan penyimpanan lokal (`localStorage`).

---

## 📛 Badges

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-FFD700?style=for-the-badge&logo=javascript&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

---

## 🚀 Live Demo  
🔗 **[Klik di sini untuk mencoba aplikasi](https://username.github.io/manajemen-tugas-mahasiswa/)**  
*(Pastikan kamu mengganti `username` dengan username GitHub kamu setelah mengunggah project ini.)*

---

## 🧠 Deskripsi Singkat

Aplikasi ini dirancang untuk membantu mahasiswa dalam:
- Mengatur dan memantau tugas kuliah
- Menandai status tugas (selesai/belum selesai)
- Menyimpan data tugas secara otomatis di browser melalui `localStorage`
- Menampilkan total tugas yang belum diselesaikan
- Menyediakan mode **Light** dan **Dark Mode** untuk kenyamanan visual

---

## 🧩 Fitur-Fitur Utama

| Fitur | Deskripsi |
|-------|------------|
| ➕ **Tambah Tugas** | Tambahkan tugas baru dengan nama, mata kuliah, dan deadline |
| ✏️ **Edit Tugas** | Ubah data tugas yang telah dibuat |
| ✅ **Tandai Selesai** | Tandai tugas yang telah diselesaikan |
| ❌ **Hapus Tugas** | Hapus tugas dari daftar |
| 🔍 **Pencarian** | Cari tugas berdasarkan nama atau mata kuliah |
| 🧭 **Filter** | Filter tugas berdasarkan status (selesai/belum) |
| 💾 **LocalStorage** | Simpan data tugas agar tetap ada setelah reload |
| 🌗 **Dark/Light Mode** | Ganti tampilan sesuai preferensi pengguna |
| ⚠️ **Validasi Form** | Cegah input kosong atau tanggal tidak valid |

---

## 🖼️ Tampilan Aplikasi

> Semua screenshot dapat kamu letakkan di folder `/screenshots/`

### 🌤️ 1. Tampilan Light Mode
![Light Mode](screenshots/lightmode.png)

### 🌙 2. Tampilan Dark Mode
![Dark Mode](screenshots/darkmode.png)

### ➕ 3. Fitur Tambah Tugas
![Tambah Tugas](screenshots/tambah-tugas.png)

### 🔍 4. Fitur Searching
![Searching](screenshots/searching.png)

### ❌ 5. Fitur Hapus Tugas
![Hapus Tugas](screenshots/hapus-tugas.png)

### ✏️ 6. Fitur Edit Tugas
![Edit Tugas](screenshots/edit-tugas.png)

---

## ⚙️ Cara Menjalankan Aplikasi

Clone repository ini
   ```bash
   git clone https://github.com/username/manajemen-tugas-mahasiswa.git
**Masuk ke folder proyek**

cd manajemen-tugas-mahasiswa


Jalankan aplikasi

Buka file index.html di browser.

Tidak perlu server tambahan — semuanya berjalan lokal.

🧠 Penjelasan Teknis
💾 Penggunaan localStorage

Aplikasi menggunakan localStorage untuk menyimpan data tugas agar tidak hilang saat browser ditutup.
Data disimpan dalam format JSON dan dimuat kembali setiap kali halaman dibuka.

localStorage.setItem("tugasMahasiswa", JSON.stringify(daftarTugas));
let data = JSON.parse(localStorage.getItem("tugasMahasiswa")) || [];

✅ Validasi Form

Setiap kali pengguna menambahkan tugas baru, sistem memvalidasi input:

Nama tugas dan mata kuliah tidak boleh kosong

Deadline harus tanggal valid dan tidak boleh sebelum hari ini

if (namaTugas.trim() === "" || mataKuliah.trim() === "") {
  showError("Nama tugas dan mata kuliah wajib diisi");
  return;
}
if (new Date(deadline) < new Date()) {
  showError("Deadline tidak boleh sebelum hari ini");
  return;
}

🧰 Teknologi yang Digunakan
Teknologi	Fungsi
HTML5	Struktur halaman
CSS3 (Glassmorphism)	Efek kaca transparan, animasi, dan tema dark/light
JavaScript ES6	Logika aplikasi dan manipulasi DOM
localStorage API	Penyimpanan data tugas di sisi pengguna
💡 Struktur Folder
📦 manajemen-tugas-mahasiswa
 ┣ 📂 screenshots
 ┃ ┣ lightmode.png
 ┃ ┣ darkmode.png
 ┃ ┣ tambah-tugas.png
 ┃ ┣ searching.png
 ┃ ┣ hapus-tugas.png
 ┃ ┗ edit-tugas.png
 ┣ 📜 index.html
 ┣ 🎨 style.css
 ┣ ⚙️ script.js
 ┗ 📘 README.md

🪪 Lisensi

Proyek ini dirilis di bawah lisensi MIT License — silakan gunakan, ubah, atau distribusikan kembali dengan tetap mencantumkan atribusi.
Lihat file LICENSE
 untuk detailnya.

👨‍💻 Pembuat

Taufik Hidayat NST
🎓 Mahasiswa Informatika – Institut Teknologi Sumatera
💬 “Bangun kode yang bermanfaat, bukan hanya yang berjalan.”
