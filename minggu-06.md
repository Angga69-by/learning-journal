# Jurnal Minggu 6: Pemeriksaan Import Address Table (IAT) & Windows API

## Apa yang Dipelajari?
Materi minggu ini membahas pemeriksaan komponen krusial pada file PE, yaitu **Import Address Table (IAT)**. IAT mencatat daftar pustaka dinamis (`.dll`) serta fungsi-fungsi Windows API eksternal yang dipanggil oleh aplikasi untuk menjalankan tugas tertentu.

Dengan menganalisis fungsi impor, kita bisa menebak kapabilitas atau perilaku sebuah program secara akurat:
* **Pustaka KERNEL32.dll** dengan fungsi seperti `CreateFileW`, `WriteFile`, atau `VirtualAlloc` menandakan aplikasi memiliki kemampuan memanipulasi file lokal atau mengalokasikan ruang memori baru.
* **Pustaka USER32.dll** dengan fungsi `MessageBoxW` menandakan program dapat menampilkan jendela interaksi grafis/pop-up ke pengguna.
* **Pustaka WININET.dll / WS2_32.dll** mengindikasikan adanya fungsi komunikasi jaringan internet.

## Kendala dan Solusi
* **Kendala:** Banyak nama Windows API yang terdengar asing bagi saya saat pertama kali melihat visualisasi IAT.
* **Solusi:** Selalu membuka dokumentasi resmi *Microsoft Learn (MSDN)* untuk memahami fungsi dan parameter dari setiap Windows API yang dicurigai.

## Rencana Minggu Depan
Mulai mengeksplorasi penggunaan perkakas mutakhir untuk analisis tingkat lanjut seperti dekompiler Ghidra dan debugger x64dbg.
