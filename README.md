# Course-Scheduler

## Latar Belakang

Mengapa perlu Course Scheduler? Melihat indeks nilai semester-semester sebelumnya tentu membuat kita ingin menjadwalkan mata kuliah yang akan kita ambil supaya memperoleh nilai yang maksimal. Tidakkah Anda penasaran bagaimana cara membuatnya? Dynamic Programming adalah solusi yang Anda butuhkan (apabila Anda memiliki data). Tunggu apa lagi? Anda mungkin akan membuat salah satu Course Scheduler yang sangat diandalkan.

## Spesifikasi Wajib

Course Scheduler dibuat <b>berbasis web</b>. Bahasa dan Framework dibebaskan untuk Frontend dan tetapi wajib menggunakan <b>Golang</b> untuk Backend dan <b>SQL</b> untuk Basis Data. Course Scheduler harus mengandung beberapa fitur utama di bawah ini:

1. Pembagian <b>Frontend</b> dan <b>Backend</b> wajib dibuat pada repository GitHub yang terpisah.
2. Penambahan data Fakultas yang terdiri dari:
    - Nama Fakultas
2. Penambahan data Jurusan yang terdiri dari:
  - Nama Jurusan
  - Asal Fakultas
3. Penambahan data MK (Mata Kuliah) yang terdiri dari:
  - Nama MK
  - Jumlah SKS MK
  - Jurusan atau Fakultas MK
  - Semester minimal pengambilan MK
  - Prediksi nilai MK (<strong>Note:</strong> Nilai berupa A, AB, B, BC, C, D, atau E)
4. Aplikasi dapat menerapkan algoritma <b>Dynamic Programming</b> untuk mendapatkan seluruh MK yang dapat diambil sehingga memberikan nilai maksimal dengan input oleh pengguna sebagai berikut.
  - Jurusan atau Fakultas
  - Semester pengambilan MK saat ini
  - Batasan SKS yang dapat diambil
5. Aplikasi dapat menampilkan <b>visualisasi</b> untuk seluruh MK yang diambil dan menampilkan nilai akhir yang akan didapatkan. Framework untuk visualisasi dibebaskan.
6. Aplikasi dapat dijalankan dengan menggunakan <b>Docker</b> pada lokal komputer baik untuk Frontend, Backend, maupun Basis Data.
  - Buatlah Dockerfile masing-masing untuk Frontend dan Backend agar dapat membuat image pada container.
  - Buatlah script docker-compose pada repository Backend untuk menjalankan container Backend dan Basis Data.
  - Buatlah script docker-compose pada repository Frontend untuk menjalankan container Frontend.
  - Aplikasi pada masing-masing repository dapat dijalankan hanya dengan command ```docker-compose up -d```.
  - Pastikan migrasi basis data dapat berlangsung ketika aplikasi dijalankan.
7. Buatlah readme pada masing-masing repository yang menjelaskan:
  - Deskripsi Program
  - Teknologi dan Framework
  - (Backend) Penjelasan Dynamic Programming
  - (Backend) Analisis Algoritma
  - (Frontend) Screenshot Hasil Percobaan
  - Cara menjalankan aplikasi (docker-compose up -d)
  - Referensi Belajar
