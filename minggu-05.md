# Jurnal Minggu 5: Analisis String & Deteksi Karakteristik Binary

## Apa yang Dipelajari?
Minggu ini berfokus pada salah satu teknik mendasar dalam analisis statis, yaitu **Analisis String** (*Strings Analysis*). Tujuannya adalah mengekstraksi karakter teks polos (ASCII atau Unicode) yang tertanam di dalam executable tanpa menjalankan programnya.

Manfaat utama dari deteksi string ini adalah mencari petunjuk atau indikator penting, seperti:
* Alamat IP atau nama domain URL tersembunyi yang digunakan aplikasi untuk berkomunikasi.
* Pesan kesalahan (*error messages*) yang membantu memahami alur logika program.
* Path direktori penyimpanan source code asli saat dikompilasi oleh developer.
* Kunci rahasia (*hardcoded password/key*) yang sering kali disimpan secara ceroboh di dalam kode.

## Kendala dan Solusi
* **Kendala:** Terlalu banyak string acak (*noise*) tidak bermakna yang muncul saat melakukan ekstraksi mentah.
* **Solusi:** Menggunakan parameter filter panjang minimum karakter (misal minimal 5 karakter alfabet berurutan) agar hasilnya lebih bersih.

## Rencana Minggu Depan
Menganalisis dependensi fungsi eksternal melalui pemeriksaan tabel fungsi impor binary.
