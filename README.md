# Tugas 1 - Implementasi Antrean (Queue) Menggunakan Dart

**Nama:** Talitha Maharani Nashier 
**NIM:** H1D024098
**Shift Awal:** H
**Shift Akhir:** D

## 📌 Deskripsi Tugas

Tugas ini mengimplementasikan struktur data antrean (*queue*) menggunakan
bahasa pemrograman Dart. Antrean menerapkan prinsip **FIFO (First-In,
First-Out)**, yaitu data yang pertama kali dimasukkan menjadi data pertama
yang dikeluarkan.

Implementasi ini menggunakan `List<T>` dari Dart untuk menyimpan data. Class
`Queue<T>` dibuat sendiri, tanpa menggunakan library tambahan.

## 💻 Penjelasan Kode

Kode program berada di file [`modul_1.dart`](./modul_1.dart) dan terdiri dari
class `Queue<T>` serta fungsi `main()`:

1. **Class `Queue<T>`**
   - Merupakan class generik yang dapat menyimpan berbagai tipe data. Contoh
     program menggunakan `Queue<String>` dan `Queue<int>`.
   - Properti `_data` bertipe `List<T>` dan bersifat privat.
   - **`enqueue(T item)`** menambahkan data ke bagian belakang antrean dengan
     `_data.add(item)`.
   - **`pop()`** menghapus dan mengembalikan data paling depan dengan
     `_data.removeAt(0)`. Jika antrean kosong, method mencetak pesan dan
     mengembalikan `null`.
   - **`tampilkan()`** mencetak isi antrean dari depan ke belakang atau
     menampilkan pesan jika antrean kosong.

2. **Fungsi `main()`**
   - Membuat antrean nama dengan tipe `Queue<String>`.
   - Menambahkan dan mengeluarkan nama untuk menunjukkan urutan FIFO.
   - Menunjukkan perilaku `pop()` saat antrean kosong.
   - Membuat antrean angka dengan tipe `Queue<int>` sebagai contoh penggunaan
     tipe data lain.

## 🧠 Konsep yang Digunakan

| Konsep | Penerapan pada Kode |
| :--- | :--- |
| **Kelas dan Objek** | Class `Queue<T>` digunakan untuk membuat objek antrean. |
| **Fungsi / Metode** | Method `enqueue()`, `pop()`, dan `tampilkan()` mengelola serta menampilkan data antrean. |
| **Generic** | `<T>` memungkinkan antrean menyimpan tipe data berbeda dengan keamanan tipe. |
| **List** | `List<T>` menyimpan data antrean; data baru ditambahkan di belakang dan data terdepan dihapus saat `pop()`. |
| **Struktur Kontrol** | `if` memeriksa apakah antrean kosong sebelum data dikeluarkan. |
| **Nilai nullable** | `T?` pada `pop()` memungkinkan method mengembalikan `null` ketika antrean kosong. |

## 🚀 Cara Menjalankan

### Persiapan

Pastikan Dart SDK sudah terpasang. Bisa memasang Dart SDK secara terpisah atau
memasang Flutter, yang sudah menyertakan Dart. Setelah instalasi, buka terminal
dan pastikan perintah berikut menampilkan versi Dart:

```powershell
dart --version
```

### Mengunduh dan menjalankan dari GitHub

1. Clone repository dan masuk ke folder proyek:

```powershell
git clone https://github.com/talithanashier/H1D024098-Talitha-Maharani-Nashier-FlutterPraktikumPemmob.git
cd H1D024098-Talitha-Maharani-Nashier-FlutterPraktikumPemmob
```

3. Jalankan program:

```powershell
dart run modul_1.dart
```

Program ini tidak memerlukan package tambahan. Jika belum memasang Git, unduh
repository melalui tombol **Code → Download ZIP** di GitHub, ekstrak ZIP,
buka terminal di folder hasil ekstrak, lalu jalankan `dart run modul_1.dart`.
