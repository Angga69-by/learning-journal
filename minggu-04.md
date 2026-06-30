# Jurnal Minggu 4: Struktur Internal Portable Executable (PE) Section

## Apa yang Dipelajari?
Materi minggu ini mendalami pembagian struktur di dalam file PE Windows. File PE secara umum terbagi menjadi beberapa bagian penting yang disebut dengan *Sections*:
* **Header:** Berisi metadata penting mengenai karakteristik file, arsitektur CPU target, nilai Entry Point, dan jumlah total section.
* **.text Section:** Bagian yang menyimpan instruksi kode mesin utama yang akan dieksekusi oleh prosesor.
* **.data Section:** Berisi variabel global atau variabel statis yang sudah diinisialisasi oleh program.
* **.rdata Section:** Menyimpan data konstan yang bersifat *read-only*, termasuk string konstan dan informasi tabel fungsi impor.
* **.rsrc Section:** Menyimpan sumber daya eksternal aplikasi seperti ikon, menu, gambar, atau manifest enkapsulasi.

Saya juga mempelajari konsep **Endianness**, yaitu aturan pengurutan byte di memori:
* **Little Endian:** Menyimpan byte terkecil (*Least Significant Byte*) di alamat memori terendah. Arsitektur x86/x64 Windows menggunakan metode ini.
* **Big Endian:** Menyimpan byte terbesar (*Most Significant Byte*) di alamat memori terendah, sering dipakai pada sistem mainframe atau jaringan.

## Kendala dan Solusi
* **Kendala:** Kebingungan membaca urutan byte data heksadesimal di memori akibat efek susunan terbalik dari Little Endian.
* **Solusi:** Melakukan latihan konversi manual byte per byte dari representasi memori ke nilai desimal aslinya secara berulang.

## Rencana Minggu Depan
Mulai mempraktikkan teknik analisis statis dasar untuk mencari string penting di dalam binary.
