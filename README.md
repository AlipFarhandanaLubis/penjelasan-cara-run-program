# penjelasan-cara-run-program
# Program Backup Otomatis Menggunakan Python

Program ini dibuat untuk memenuhi **Soal Nomor 4 UAS**.  
Fungsi utama program adalah melakukan **backup otomatis folder**, menyimpannya dalam bentuk **file ZIP**, menghapus backup lama (lebih dari 7 hari), dan mencatat semua aktivitas ke dalam file log.

---

## Tujuan Program
1. Membuat backup data secara otomatis
2. Mencegah backup ganda dalam satu hari
3. Menghapus backup lama agar penyimpanan tetap efisien
4. Mencatat aktivitas backup ke file log

---

## Library Python yang Digunakan
Program ini hanya menggunakan **library bawaan Python**, yaitu:
- `os` → untuk mengecek, membuat, dan menghapus folder/file
- `shutil` → untuk membuat file backup dalam format ZIP
- `datetime` → untuk mendapatkan tanggal dan waktu saat ini
- `timedelta` → untuk menghitung batas waktu backup (7 hari)

Library bawaan dipilih karena ringan dan tidak perlu instalasi tambahan.

---

## Pseudocode Singkat

