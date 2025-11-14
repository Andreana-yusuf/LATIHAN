# Studi Kasus Pemrograman Python

Repositori ini berisi kumpulan studi kasus pemrograman Python untuk berbagai tingkat keahlian, mulai dari pemula hingga mahir. Setiap studi kasus dirancang untuk menguji dan meningkatkan keterampilan Anda dalam memecahkan masalah dan menerapkan konsep-konsep pemrograman Python.

## Daftar Isi

*   [Studi Kasus Tingkat Pemula](#studi-kasus-tingkat-pemula)
    *   [1. Kalkulator Sederhana](#1-kalkulator-sederhana)
    *   [2. Konversi Satuan Panjang](#2-konversi-satuan-panjang)
    *   [3. Program Tebak Angka](#3-program-tebak-angka)
*   [Studi Kasus Tingkat Menengah](#studi-kasus-tingkat-menengah)
    *   [4. Manajemen Kontak](#4-manajemen-kontak)
    *   [5. Analisis Teks Sederhana](#5-analisis-teks-sederhana)
    *   [6. Permainan Batu Gunting Kertas](#6-permainan-batu-gunting-kertas)
*   [Studi Kasus Tingkat Lanjutan](#studi-kasus-tingkat-lanjutan)
    *   [7. Sistem Manajemen Perpustakaan](#7-sistem-manajemen-perpustakaan)
    *   [8. Analisis Data Cuaca](#8-analisis-data-cuaca)
    *   [9. Aplikasi Chat Sederhana](#9-aplikasi-chat-sederhana)

## Studi Kasus Tingkat Pemula

### 1. Kalkulator Sederhana

Buat sebuah program kalkulator sederhana yang dapat melakukan operasi penjumlahan, pengurangan, perkalian, dan pembagian. Program menerima dua angka dan operator sebagai input, lalu menampilkan hasilnya.

```python
def kalkulator(angka1, angka2, operator):
  """Melakukan operasi aritmatika sederhana."""
  if operator == '+':
    return angka1 + angka2
  elif operator == '-':
    return angka1 - angka2
  elif operator == '*':
    return angka1 * angka2
  elif operator == '/':
    if angka2 == 0:
      return "Error: Pembagian dengan nol tidak diizinkan"
    return angka1 / angka2
  else:
    return "Error: Operator tidak valid"

# Contoh penggunaan
angka1 = float(input("Masukkan angka pertama: "))
angka2 = float(input("Masukkan angka kedua: "))
operator = input("Masukkan operator (+, -, *, /): ")

hasil = kalkulator(angka1, angka2, operator)
print("Hasil:", hasil)
