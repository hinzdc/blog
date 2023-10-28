---
layout: post
title: Remove Shortcut Virus from USB, SD Card, Hard Drive
subtitle: 
tags: Tutorial
comments: true
readtime: true
---

Ketika virus shortcut menginfeksi perangkat, semua file yang disimpan tidak dapat diakses.  Untuk mengakses file Anda, Anda dapat menghapus virus shortcut dari drive USB, pen drive, atau kartu SD menggunakan cmd, Tools penghapus virus shortcut, dan metode manual lainnya.

Halaman ini berisi solusi lengkap untuk menghapus virus shortcut dari USB, pen drive, hard drive eksternal, dan PC tanpa kehilangan data.

### Apa itu Virus Pintasan

Virus shortcut, juga dikenal sebagai virus shortcut 1kb, adalah virus Trojan umum yang menyebar luas menggunakan drive USB atau pen drive sebagai medianya.  Virus akan menyembunyikan semua folder di direktori root USB, lalu membuat shortcut dengan nama yang sama dengan folder tersebut.  File pintasan ini diakhiri dengan .EXE, .VBS.  Akhiran .LNK atau .INI dan tidak dapat dibersihkan.  Setelah pengguna mengklik shortcut tersebut, virus akan dijalankan dan ditambahkan untuk memulai secara otomatis.

### Bagaimana Virus Pintasan Menyebar

Virus shortcut lebih mirip program virus yang menghibernasi worm autorun.inf di komputer Anda dan berjalan otomatis di latar belakang.  akibatnya, file yang ada di perangkat yang terinfeksi menjadi tidak dapat diakses, disembunyikan, atau dienkripsi menjadi pintasan berekstensi .lnk.

Berikut adalah pola kerja virus shortcut yang kami simpulkan berdasarkan penjelasan yang diberikan oleh banyak blogger dan geek:

Perangkat yang terpengaruh: PC, laptop, USB, pen drive, kartu SD, hard drive eksternal, kamera, ponsel, dll.

Jalur penyebaran: Worm virus shortcut menginfeksi komputer > menginfeksi USB, pen drive, dll. (hard drive eksternal) > menginfeksi file dan data yang disimpan (menyembunyikan atau mengenkripsinya, membuat file pintasan)

 ![shortcut-virus-spread-mode](https://github.com/hinzdc/blog/assets/24857547/d3eee18c-6e9f-495f-aeac-7fc2cc8e4b72)

Jadi bagaimana cara menghapus virus shortcut dari USB atau pen drive dan mengembalikan semua file yang hilang?  Lanjutkan membaca, Anda akan menemukan lima solusi untuk menghapus virus pintasan dengan menggunakan cmd, file .bat, penghapus virus shortcut, membersihkan virus shortcut di PC, serta menghapus key mencurigakan di Registry Editor.

### Metode 1. Menghapus Virus Shortcut Menggunakan CMD
Salah satu metode yang paling disarankan untuk menghapus virus shortcut dari pen drive atau usb flash drive adalah dengan menggunakan perintah attrib.

{: .box-warning}
**Peringatan**
Hati-hati saat menggunakan cmd.  jika Anda tidak yakin cara mengoperasikan command line, masukkan perintah hanya dari sumber tepercaya.  penggunaan cmd yang tidak tepat dapat mengakibatkan kerusakan serius pada sistem Anda.

Berikut langkah detailnya:
1. Hubungkan hard drive eksternal Anda ke PC dan klik kanan "Start", pilih "Search".
2. Ketik Command Prompt di kotak Pencarian dan klik kanan Command Prompt lalu pilih Run administrator untuk memunculkannya.
3. Ketik: E: dan tekan Enter.  (Ganti E: dengan huruf drive USB Anda.)
4. Ketik: `del *.lnk` atau `del autorun.inf` dan tekan Enter.
5. Ketik: `attrib -h - r -s  /s /d E:\*.*` dan tekan Enter.  (Ganti E: dengan huruf drive perangkat Anda yang terinfeksi).

{: .box-note}
Tips: Jika cara ini tidak berhasil, kemungkinan besar Anda terinfeksi virus lain.  Ganti autorun.inf dengan ekstensi virus lain seperti *.exe untuk menghapus virus mencurigakan tersebut.

### Metode 2. Buat File BAT untuk Menghapus Virus Shortcut dari USB
Dengan membuat file BAT, Anda cukup menjalankan file BAT dan menggunakannya untuk menghapus dan menghapus virus shortcut yang ada dengan langkah-langkah di bawah ini:

1. Hubungkan USB, pen drive, atau kartu SD Anda ke PC dan buat notepad baru di desktop.
2. Copy dan paste kode di bawah ini di notepad baru:

~~~
 @echo off
 del *.lnk
 atribut -s -r -h G:\*.* /s /d /l
 echo Done..
~~~
Catatan: Ganti G: dengan huruf drive perangkat penyimpanan Anda yang terinfeksi saat ini.
3. Save dan beri nama `virus shortcut remover.bat`, pada ___Type as files___ ubah menjadi ___All Files___ dan simpan di desktop Anda.
4. Klik dua kali file .bat di desktop Anda dan tunggu prosesnya selesai.

Sekarang, Anda seharusnya sudah berhasil menghapus virus pintasan dari flash drive USB, pen drive, atau kartu SD Anda menggunakan cmd.

Metode 3. Gunakan Antivirus - Remover virus shortcut USB
Saat Anda mencari alat penghapus virus pintasan atau perangkat lunak penghapus virus secara online, hasil pencarian yang luar biasa ditampilkan di browser Anda.

Di sini, Anda akan melihat daftar alat yang direkomendasikan yang dapat membantu Anda menghapus virus shortcut dari USB, kartu SD, atau perangkat penyimpanan lainnya：

- Shortcut Virus Remover
- USB Shortcut Virus Remover
- Free USB Repair
- USB Virus Remover
- Shortcut Virus Fixer
Anda dapat memilih salah satu alat yang terdaftar dan menerapkannya untuk menghapus dan membersihkan virus dari perangkat penyimpanan Anda.

{: .box-note}
Pemberitahuan:
Semua metode yang disediakan di atas dapat melepaskan perangkat penyimpanan dan file Anda dari infeksi virus shortcut.
Ketika proses penghapusan virus selesai, Anda dapat membuka kembali perangkat penyimpanan Anda untuk memeriksa data yang disimpan.

