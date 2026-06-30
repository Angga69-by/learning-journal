# Jurnal Minggu 3: Proses Terbentuknya Executable & Format File PE/ELF

## Apa yang Dipelajari?
Minggu ini membahas bagaimana kode sumber (*source code*) yang ditulis manusia diubah menjadi instruksi mesin (*machine code*) berbentuk file *executable*. Proses tersebut melalui 4 tahapan utama:
1. **Preprocessing:** Penanganan direktif seperti `#include` atau `#define`.
2. **Compiling:** Mengubah kode sumber (misalnya bahasa C) menjadi kode Assembly.
3. **Assembling:** Mengubah kode Assembly menjadi kode mesin dalam bentuk *object file* (`.obj` atau `.o`).
4. **Linking:** Tahap akhir yang menggabungkan *object file* dengan pustaka (*library*) eksternal hingga menjadi file *executable* tunggal.

Selain itu, saya mempelajari format file *executable* paling populer berdasarkan sistem operasinya beserta penanda uniknya (*Magic Header*):
* **PE (Portable Executable):** Digunakan di Windows (`.exe`, `.dll`, `.sys`), ditandai dengan magic bytes `MZ` (0x4D 0x5A) pada awal file.
* **ELF (Executable and Linkable Format):** Digunakan di Linux, diawali dengan byte `0x7F 45 4C 46` (`.ELF`).
* **Mach-O:** Format khusus untuk macOS dan iOS.

## Kendala dan Solusi
* **Kendala:** Kesulitan melihat byte mentah (*raw bytes*) dari Magic Header file PE saat membukanya menggunakan text editor biasa.
* **Solusi:** Menggunakan aplikasi *Hex Editor* khusus (seperti HxD) untuk melihat representasi bilangan heksadesimal file secara akurat.

## Rencana Minggu Depan
Mendalami komponen struktur internal yang ada di dalam Section file Portable Executable (PE).
