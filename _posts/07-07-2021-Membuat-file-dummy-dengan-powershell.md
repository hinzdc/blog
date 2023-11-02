---
layout: post
title: Membuat File Dummy di Windows 10/11 dengan PowerShell
subtitle: 
tags: [Tutorial, powershell]
comments: true
readtime: true 
---

PowerShell adalah salah satu alat yang kuat yang disertakan dengan sistem operasi Windows 10 dan Windows 11. Dengan PowerShell, Anda dapat melakukan berbagai tugas administratif, termasuk membuat file dummy. File dummy adalah file berukuran besar yang digunakan untuk menguji atau mengukur kinerja penyimpanan, mengisi ruang kosong pada disk, atau tujuan lainnya seperti mengecek bad sector pada harddisk. Artikel ini akan membahas cara membuat file dummy menggunakan PowerShell.

## Langkah 1: Buka PowerShell

Langkah pertama adalah membuka PowerShell. Anda dapat melakukannya dengan mengetik "PowerShell" dalam kotak pencarian di Windows dan memilih "Windows PowerShell" atau "Windows PowerShell (Admin)" tergantung pada hak akses yang Anda butuhkan.

## Langkah 2: Menjalankan Perintah

Sekarang, Anda perlu menjalankan perintah PowerShell berikut:

```powershell
$out = new-object byte[] 10000000; (new-object Random).NextBytes($out); [IO.File]::WriteAllBytes('C:\dummy\dum.dat', $out)
```

Perintah ini akan membuat sebuah objek byte array sebesar 10.000.000 byte (sekitar 10 MB), mengisi array dengan data acak, dan menyimpannya dalam file bernama "dum.dat" di lokasi "C:\dummy\". Anda dapat mengganti ukuran file dummy dengan mengubah angka "10000000" sesuai dengan kebutuhan Anda. Anda juga dapat mengganti path tujuan dengan path yang anda inginkan.

## Langkah 3: Verifikasi File Dummy

Setelah menjalankan perintah, Anda dapat memeriksa file dummy yang baru dibuat di lokasi yang Anda tentukan (dalam contoh ini, "C:\dummy\dum.dat"). File ini akan berisi data acak sesuai dengan ukuran yang Anda tetapkan.

## Kesimpulan

PowerShell adalah alat yang kuat untuk berbagai tugas administratif di Windows, termasuk pembuatan file dummy. Dengan perintah PowerShell yang sesuai, Anda dapat membuat file dummy dengan mudah sesuai dengan kebutuhan Anda.

Ini adalah panduan singkat tentang cara membuat file dummy di Windows 10/11 menggunakan PowerShell. Semoga informasi ini bermanfaat untuk Anda dalam tugas-tugas Anda yang melibatkan penggunaan file dummy.
