# Course-Scheduler

## Latar Belakang

Mengapa perlu Course Scheduler? Melihat indeks nilai semester-semester sebelumnya tentu membuat kita ingin menjadwalkan mata kuliah yang akan kita ambil supaya memperoleh nilai yang maksimal. Tidakkah Anda penasaran bagaimana cara membuatnya? Dynamic Programming adalah solusi yang Anda butuhkan (apabila Anda memiliki data). Tunggu apa lagi? Anda mungkin akan membuat salah satu Course Scheduler yang sangat diandalkan.

## Spesifikasi Wajib

Course Scheduler dibuat <b>berbasis web</b>. Bahasa dan Framework dibebaskan untuk Frontend dan tetapi wajib menggunakan <b>Golang</b> untuk Backend dan <b>SQL</b> untuk Basis Data. Course Scheduler harus mengandung beberapa fitur utama di bawah ini:

1. Pembagian <b>Frontend</b> dan <b>Backend</b> wajib dibuat pada repository GitHub yang terpisah.
2. Penambahan data MK (Mata Kuliah) yang dapat dilakukan baik secara satu per satu maupun batch dengan file berformat <b>.json</b>. Data MK terdiri dari:
    - Nama MK
    - Jumlah SKS MK
    - Jurusan atau Fakultas MK
    - Semester minimal pengambilan MK
    - Prediksi nilai MK
        - <b>Note:</b> Nilai berupa A, AB, B, BC, C, D, atau E
3. Aplikasi dapat menerapkan algoritma <b>Dynamic Programming</b> untuk mendapatkan seluruh MK yang dapat diambil sehingga memberikan nilai maksimal dengan input oleh pengguna sebagai berikut.
    - Jurusan atau Fakultas
    - Semester pengambilan MK saat ini
    - Batasan SKS yang dapat diambil
4. Aplikasi dapat menampilkan <b>visualisasi</b> untuk seluruh MK yang diambil dan menampilkan nilai akhir yang akan didapatkan. Framework untuk visualisasi dibebaskan.
5. Aplikasi dapat dijalankan dengan menggunakan <b>Docker</b> pada lokal komputer baik untuk Frontend, Backend, maupun Basis Data.
    - Buatlah Dockerfile masing-masing untuk Frontend dan Backend agar dapat membuat image pada container.
    - Buatlah script docker-compose pada repository Backend untuk menjalankan container Backend dan Basis Data.
    - Buatlah script docker-compose pada repository Frontend untuk menjalankan container Frontend.
    - Aplikasi pada masing-masing repository dapat dijalankan hanya dengan command ```docker-compose up -d```.
    - Pastikan migrasi basis data dapat berlangsung ketika aplikasi dijalankan.
6. Buatlah readme pada masing-masing repository yang menjelaskan:
    - Deskripsi Program
    - Teknologi dan Framework
    - (Backend) Penjelasan Dynamic Programming
    - (Backend) Analisis Algoritma
    - (Frontend) Screenshot Hasil Percobaan
    - Cara menjalankan aplikasi (docker-compose up -d)
    - Referensi Belajar

## Spesifikasi Bonus

1. Aplikasi dapat menambahkan Fakultas dan Jurusan secara satu per satu <b>atau</b> batch dengan file berformat <b>.json</b>.
    - Fakultas memiliki hubungan <b>One-to-Many</b> terhadap Jurusan
2. Menerapkan logika keterhubungan antara Fakultas dan Jurusan pada MK yang akan diambil. 
    - <b>Contoh:</b> Mahasiswa Jurusan Teknik Informatika dapat mengambil MK yang terdapat dalam Fakultas STEI
    - <b>Note:</b> Wajib mengerjakan bonus pertama terlebih dahulu sebelum mengerjakan bonus ini
3. Melakukan <b>deployment</b> terhadap aplikasi.
