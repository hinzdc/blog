---
layout: post
title: Cara Membuat File Dummy dengan fsutil di Windows
subtitle: 
tags: [test]
comments: true
readtime: true
---

`fsutil` adalah alat yang tersedia di lingkungan command prompt Windows yang berguna untuk mengelola sistem berkas NTFS. Salah satu penggunaan umum dari `fsutil` adalah untuk membuat file dummy, yaitu file berukuran besar yang sering digunakan untuk menguji kinerja penyimpanan atau mengisi ruang kosong pada disk. Artikel ini akan membahas cara menggunakan `fsutil` untuk membuat file dummy di Windows.

## Langkah 1: Buka Command Prompt

Langkah pertama adalah membuka Command Prompt di Windows. Anda dapat melakukannya dengan mencari "Command Prompt" di menu Start dan menjalankannya.

## Langkah 2: Menjalankan Perintah fsutil

Setelah Command Prompt terbuka, Anda dapat menjalankan perintah `fsutil` berikut untuk membuat file dummy:

```plaintext
fsutil file createnew C:\dummy\dummyfile.dat 10000000
```

Perintah ini akan menciptakan file baru dengan nama "dummyfile.dat" di lokasi "C:\dummy\". Angka "10000000" dalam perintah menunjukkan ukuran file dalam byte. Anda dapat mengganti ukuran file sesuai kebutuhan Anda.

## Langkah 3: Verifikasi File Dummy

Setelah menjalankan perintah, Anda dapat memeriksa file dummy yang baru dibuat di lokasi yang Anda tentukan (dalam contoh ini, "C:\dummy\dummyfile.dat"). File ini akan memiliki ukuran yang sesuai dengan yang Anda tetapkan dalam perintah.

Begitulah cara membuat file dummy menggunakan fsutil pada command prompt 
