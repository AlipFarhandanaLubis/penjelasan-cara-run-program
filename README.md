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
Mulai
Cek folder backup
Jika folder belum ada, buat folder
Jika backup hari ini belum ada
Buat file ZIP
Tulis log berhasil
Jika backup hari ini sudah ada
Tulis log tidak dibuat ulang
Hapus backup yang lebih dari 7 hari
Tulis log aktivitas
Selesai

Struktur folder program adalah sebagai berikut:
backup_otomatis/
│
├── backup.py
├── data_penting/
├── backup_results/
└── backup_log.txt

Keterangan:
- `backup.py` : File utama program
- `data_penting/` : Folder yang akan dibackup
- `backup_results/` : Folder hasil backup ZIP
- `backup_log.txt` : File pencatatan aktivitas

---

## Cara Menjalankan Program
1. Pastikan Python sudah terinstall  
   Cek dengan perintah:
   
2. Buka Command Prompt / Terminal

3. Masuk ke folder program:

4. Jalankan program:

---

## Alur Kerja Program
1. Program dijalankan
2. Program mengecek folder `backup_results`
3. Jika belum ada, folder dibuat otomatis
4. Program mengecek apakah backup hari ini sudah ada
5. Jika belum ada, file ZIP dibuat
6. Backup lama lebih dari 7 hari dihapus
7. Semua aktivitas dicatat ke file log
8. Program selesai

---

## Kesimpulan
Program backup otomatis ini membantu menjaga keamanan data dengan cara mencadangkan folder secara rutin, mencegah duplikasi backup, dan membersihkan file lama secara otomatis.

Program ini sederhana, efisien, dan sesuai dengan kebutuhan dasar otomasi menggunakan Python.


