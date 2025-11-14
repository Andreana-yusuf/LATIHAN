# Aplikasi Pengukur Tinggi Badan - Panduan dan Informasi

Selamat datang di halaman aplikasi pengukur tinggi badan! Aplikasi ini dirancang untuk membantu Anda mengukur dan memantau tinggi badan dengan mudah dan akurat. Cocok untuk penggunaan pribadi, keluarga, atau bahkan profesional.

## 📌 Overview

Program ini memungkinkan pengguna untuk:

*   Memasukkan informasi pribadi (nama, usia, jenis kelamin - opsional).
*   Memasukkan nilai tinggi badan aktual (dalam cm atau inci).
*   Konversi nilai ukuran dari cm ke inci atau sebaliknya.
*   Simpan riwayat pengukuran ke file untuk ditinjau nanti.

Tidak ada solusi kode yang disediakan. Sebaliknya, Anda dapat membangun logika aplikasi lengkap sendiri!

## 🔄 Alur Program

### **1. Menu Utama**

Pengguna memilih salah satu opsi:

*   Masukkan Tinggi Badan
*   Lihat Riwayat Pengukuran
*   Keluar

### **2. Masukkan Tinggi Badan**

*   Program meminta nama pengguna (opsional).
*   Program meminta usia pengguna (opsional).
*   Program meminta jenis kelamin pengguna (opsional).
*   Program meminta tinggi badan dalam sentimeter (cm) atau inci (in).
*   Program melakukan konversi otomatis (jika diperlukan).
*   Program menyimpan data (nama, usia, jenis kelamin, tinggi badan dalam cm & inci, tanggal) ke file.

### **3. Lihat Riwayat Pengukuran**

*   Program membaca data dari file riwayat.
*   Program menampilkan daftar semua pengukuran sebelumnya (nama, usia, jenis kelamin, tinggi badan dalam cm & inci, tanggal).

### **4. Keluar**

*   Aplikasi ditutup.

*   ## 📁 Struktur Proyek

  
**Penjelasan:**

*   **`height-calculator-cli/`**: Folder akar proyek.
*   **`main.py`**: File utama yang berisi logika program utama (menu, input, output, alur program).
*   **`height_data_handler.py`** (opsional):  File yang berisi fungsi-fungsi untuk menyimpan dan membaca data tinggi badan dari file (pemisahan logika). 
*   **`history.txt` / `history.json`**: File untuk menyimpan riwayat pengukuran tinggi badan. Bisa dalam format teks biasa (`.txt`) atau JSON (`.json`). Pilih salah satu.
*   **`README.md`**: File dokumentasi proyek (deskripsi, cara menjalankan, dll.).

  ## 📘 Contoh Format Data Tinggi Badan (Opsional)

Untuk menyimpan data tinggi badan,Anda bisa menggunakan format yang sederhana,Contoh nya sebagai berikut:
json
Copy code
{
  "tanggal": "2024-01-01",
  "tinggi_badan": 175.5,
  "usia": 25,
  "catatan": "Pengukuran setelah makan siang."
}
markdown
Copy code
## 📘 Contoh Riwayat Pengukuran Tinggi Badan

Berikut ini adalah contoh bagaimana riwayat pengukuran tinggi badan dapat disimpan dalam format TXT dan JSON:

**Versi TXT:**
Copy code
Tinggi: 175.5 cm
Usia: 25 tahun
Tanggal: 2024-01-01
Catatan: Pengukuran setelah makan siang.
markdown
Copy code
**Versi JSON:**
json
Copy code
[
  {
    "tanggal": "2024-01-01",
    "tinggi_badan": 175.5,
    "usia": 25,
    "catatan": "Pengukuran setelah makan siang."
  },
  {
    "tanggal": "2024-02-15",
    "tinggi_badan": 176.0,
    "usia": 25,
    "catatan": "Pengukuran di pagi hari."
  }
]

## 🚀 Cara Menjalankan Aplikasi

1.  Pastikan Anda memiliki Python 3.6+ terinstal.
2.  Instalasikan libraries jika ada yang kurang
3.  Jalankan program:
bash
Copy code
python main.py
markdown
Copy code
## 🧩 Pengembangan Selanjutnya

Berikut beberapa ide untuk pengembangan aplikasi di masa depan:

*   **Antarmuka Pengguna Grafis (GUI):** Buat GUI menggunakan Tkinter, PyQt, atau library GUI lainnya untuk pengalaman pengguna yang lebih interaktif.
*   **Database:** Simpan riwayat pengukuran ke database (misalnya, SQLite) untuk pengelolaan yang lebih efisien dan kemampuan untuk melakukan query data.
*   **Visualisasi Data:** Implementasikan visualisasi data menggunakan library seperti Matplotlib atau Seaborn untuk menampilkan tren pertumbuhan tinggi badan dari waktu ke waktu.
*   **Fitur Notifikasi:** Tambahkan fitur notifikasi untuk mengingatkan pengguna agar melakukan pengukuran secara berkala.
*   **Integrasi Cloud:** Integrasikan dengan layanan cloud untuk menyimpan data secara online dan memungkinkan sinkronisasi antara perangkat.
*   **Analisis Statistik:** Terapkan analisis statistik sederhana untuk memberikan informasi tambahan, seperti persentil tinggi badan berdasarkan usia dan jenis kelamin.

## 📜 Lisensi

Proyek ini dilisensikan di bawah Lisensi MIT. Lihat berkas `LICENSE` untuk informasi lebih lanjut.
