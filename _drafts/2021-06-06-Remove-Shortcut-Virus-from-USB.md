---
layout: post
title: Remove Shortcut Virus from USB, Pen Drive, SD Card, Hard Drive
subtitle: 
tags: [test]
comments: true
---

Ketika virus pintasan menginfeksi perangkat, semua file yang disimpan tidak dapat diakses.  Untuk mengakses file Anda, Anda dapat menghapus virus pintasan dari drive USB, pen drive, atau kartu SD menggunakan cmd, alat penghapus virus pintasan, dan metode manual lainnya.  Jika virus atau proses penghapusan mengakibatkan hilangnya beberapa data.

This page includes the complete solutions to remove shortcut virus from USB, pen drive, external hard drive, and PC without losing data.

### Apa itu Virus Pintasan

Virus pintasan, juga dikenal sebagai virus pintasan 1kb, adalah virus Trojan umum yang menyebar luas menggunakan drive USB atau pen drive sebagai medianya.  Virus akan menyembunyikan semua folder di direktori root USB, lalu membuat shortcut dengan nama yang sama dengan folder tersebut.  File pintasan ini diakhiri dengan .EXE, .VBS.  Akhiran LNK atau .INI dan tidak dapat dibersihkan.  Setelah pengguna mengklik pintasan tersebut, virus akan dijalankan dan ditambahkan untuk memulai secara otomatis.

### Bagaimana Virus Pintasan Menyebar

virus pintasan lebih mirip program virus yang menghibernasi worm autorun.inf di komputer Anda dan berjalan otomatis di latar belakang.  akibatnya, file yang ada di perangkat yang terinfeksi menjadi tidak dapat diakses, disembunyikan, atau dienkripsi menjadi pintasan berekstensi .lnk.

berikut adalah pola kerja virus shortcut yang kami simpulkan berdasarkan penjelasan yang diberikan oleh banyak blogger dan geek:

Perangkat yang terpengaruh: PC, laptop, USB, pen drive, kartu SD, hard drive eksternal, kamera, ponsel, dll.

Jalur penyebaran: Worm virus pintasan menginfeksi komputer > menginfeksi USB, pen drive, dll. (hard drive eksternal) > menginfeksi file dan data yang disimpan (menyembunyikan atau mengenkripsinya, membuat file pintasan)

 ![shortcut-virus-spread-mode](https://github.com/hinzdc/blog/assets/24857547/d3eee18c-6e9f-495f-aeac-7fc2cc8e4b72)


Jadi bagaimana cara menghapus virus shortcut dari USB atau pen drive dan mengembalikan semua file yang hilang?  Lanjutkan membaca, Anda akan menemukan lima solusi untuk menghapus virus pintasan dengan menggunakan cmd, file .bat, penghapus virus pintasan, membersihkan virus pintasan di PC, serta menghapus kunci mencurigakan di Peninjau Suntingan Registri.

Solusi untuk penghapusan virus pintasan USB dalam tutorial ini terutama disediakan oleh editor profesional di situs web geek seperti makeuseof.com dan blogger di forum teknologi seperti quora.com.  Semua solusi telah teruji dan praktis.  Semoga trik berikut ini berhasil menyelesaikan kasus Anda.

### Metode 1. shortcut penghapus virus cmd
salah satu metode yang paling disarankan untuk menghapus virus pintasan dari pen drive atau usb flash drive adalah dengan menggunakan perintah attrib.


  peringatan
 hati-hati saat menggunakan cmd.  jika Anda tidak yakin cara mengoperasikan baris perintah, masukkan perintah hanya dari sumber tepercaya.  penggunaan cmd yang tidak tepat dapat mengakibatkan kerusakan serius pada sistem Anda.
 berikut langkah detailnya:

 Langkah 1. Hubungkan hard drive eksternal Anda ke PC dan klik kanan "Start", pilih "Search".

 Langkah 2. Ketik Command Prompt di kotak Pencarian dan klik Command Prompt untuk memunculkannya.

 Masuk dengan akun administrator dan kata sandi Anda jika sistem memintanya.

 Langkah 3. Ketik: E: dan tekan Enter.  (Ganti E: dengan huruf drive USB Anda, pen drive.)

 Langkah 4. Ketik: del *.lnk atau del autorun.inf dan tekan Enter.

 Langkah 5. Ketik: attrib -h - r -s  /s /d E:\*.* dan tekan Enter.  (Ganti E: dengan huruf drive perangkat Anda yang terinfeksi).

 Tips: Jika cara ini tidak berhasil, kemungkinan besar Anda terinfeksi virus lain.  Ganti autorun.inf dengan ekstensi virus lain seperti *.exe untuk menghapus virus mencurigakan tersebut.

 Metode 2. Buat File BAT untuk Menghapus Virus Shortcut dari USB
 Dengan membuat file BAT, Anda cukup menjalankan file BAT dan menggunakannya untuk menghapus dan menghapus virus shortcut yang ada dengan langkah-langkah di bawah ini:

 Langkah 1. Hubungkan USB, pen drive, atau kartu SD Anda ke PC dan buat notepad baru di desktop.

 Langkah 2. Salin dan simpan kode di bawah ini di notepad baru:

 @gema mati

 del *.lnk
 atribut -s -r -h G:\*.* /s /d /l
 @echo selesai

 Catatan: Ganti G: dengan huruf drive perangkat penyimpanan Anda yang terinfeksi saat ini.

 Langkah 3. Ubah ekstensi file notepad menjadi .bat dan simpan di desktop Anda.

 Langkah 4. Klik dua kali file .bat di desktop Anda dan tunggu prosesnya selesai.

 Sekarang, Anda seharusnya sudah berhasil menghapus virus pintasan dari flash drive USB, pen drive, atau kartu SD Anda menggunakan cmd.

 Metode 3. Gunakan Antivirus - Penghapus Virus Pintasan USB
 Saat Anda mencari alat penghapus virus pintasan atau perangkat lunak penghapus virus secara online, hasil pencarian yang luar biasa ditampilkan di browser Anda.

 Di sini, Anda akan melihat daftar alat yang direkomendasikan yang dapat membantu Anda menghapus virus pintasan dari USB, kartu SD, atau perangkat penyimpanan lainnya：

 Penghapus Virus Pintasan
 Penghapus Virus Pintasan USB
 Perbaikan USB Gratis
 Penghilang Virus USB
 Pemecah Virus Pintasan
 Anda dapat memilih salah satu alat yang terdaftar dan menerapkannya untuk menghapus dan membersihkan virus dari perangkat penyimpanan Anda.

  Pemberitahuan:
 Semua metode yang disediakan di atas dapat melepaskan perangkat penyimpanan dan file Anda dari infeksi virus pintasan.
 Ketika proses penghapusan virus selesai, Anda dapat membuka kembali perangkat penyimpanan Anda untuk memeriksa data yang disimpan.
 Jika Anda tidak dapat melihat file atau kehilangan sebagian data di perangkat Anda, lihat Bagian selanjutnya untuk mendapatkan solusi pemulihan data yang lengkap.
