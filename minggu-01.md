# Jurnal Minggu 1: Pengenalan Reverse Engineering & Arsitektur CPU

## Apa yang Dipelajari?
Pada minggu pertama ini, saya mempelajari konsep dasar Reverse Engineering (RE), yaitu proses menganalisis suatu sistem atau *binary* untuk mengetahui cara kerjanya, strukturnya, atau fungsinya ketika *source code* asli tidak tersedia. Fokus utama minggu ini adalah memahami arsitektur CPU x86/x64 dan bagaimana komponen penting seperti register bekerja.

Beberapa register penting yang saya pelajari antara lain:
* **RAX/EAX**: Biasanya digunakan sebagai *accumulator* dan menyimpan *return value* dari sebuah fungsi.
* **RBX/EBX**: Base register, sering digunakan sebagai penunjuk basis data.
* **RSP/ESP**: Stack Pointer, menunjuk ke bagian teratas dari *stack* memori saat ini.
* **RIP/EIP**: Instruction Pointer, menyimpan alamat instruksi berikutnya yang akan dieksekusi oleh CPU.

## Kendala dan Solusi
* **Kendala:** Awalnya saya sempat bingung membedakan antara penamaan register berbasis 32-bit (awalan 'E') dan 64-bit (awalan 'R').
* **Solusi:** Saya mempelajari dokumentasi tambahan bahwa `EAX` sebenarnya adalah bagian 32-bit bawah dari register `RAX` yang berukuran 64-bit.

## Rencana Minggu Depan
Mulai mempelajari manajemen memori dasar serta perbedaan arsitektur manajemen memori pada bahasa C dan Java.
