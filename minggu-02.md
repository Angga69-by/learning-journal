# Jurnal Minggu 2: Arsitektur Memori & Manajemen Memori C vs Java

## Apa yang Dipelajari?
Minggu ini berfokus pada arsitektur memori RAM modern dan bagaimana sistem operasi mengalokasikan ruang untuk aplikasi. Saya mempelajari dua area utama alokasi memori, yaitu Stack (manajemen otomatis, cepat, struktur LIFO) dan Heap (alokasi dinamis/manual untuk data berukuran besar).

Kami juga mendiskusikan perbedaan mendasar antara manajemen memori pada bahasa C dan Java:
* **Bahasa C (Manual):** Menggunakan fungsi seperti `malloc()` atau `calloc()` untuk memesan memori di Heap dan harus dibebaskan secara manual menggunakan `free()`. Ketidakhati-hatian dalam proses ini membuat bahasa C sangat rentan terhadap serangan keamanan level rendah seperti *Memory Corruption* (misalnya *Buffer Overflow*).
* **Java (Otomatis):** Memiliki komponen *Garbage Collection* (pembersih otomatis) yang bertugas mendeteksi dan menghapus objek di memori yang sudah tidak digunakan lagi oleh program. Walaupun mempermudah developer, keberadaan Garbage Collection ini terkadang menyulitkan seorang *Reverse Engineer* dalam melacak alur asli data yang sudah dihapus secara instan dari memori.

## Kendala dan Solusi
* **Kendala:** Bingung memahami bagaimana data pointer di Heap bisa dimanipulasi hingga menyebabkan crash atau pembajakan program.
* **Solusi:** Membaca referensi tambahan mengenai mekanisme instruksi pointer dan menyimulasikan diagram alur memori secara visual.

## Rencana Minggu Depan
Mempelajari siklus hidup terbentuknya file binary executable serta anatomi format file populer seperti PE dan ELF.
