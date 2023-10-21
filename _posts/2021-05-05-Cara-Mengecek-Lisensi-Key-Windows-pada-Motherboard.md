---
layout: post
title: Cara Mengecek Lisensi Key Windows Yang terpasang pada Motherboard
subtitle: 
tags: [Windows, Tutorial, cmd]
comments: true
---

Apakah Anda ingin memastikan bahwa lisensi produk Windows yang terpasang pada motherboard komputer Anda masih aktif? Mengecek lisensi key pada motherboard bisa menjadi langkah penting untuk memahami status lisensi perangkat lunak Anda. Dalam artikel ini, saya akan membahas cara melakukan hal ini dengan menggunakan utility bawaan windows yaitu WMIC.

>WMIC adalah tool command line yang digunakan untuk melakukan operasi WMIC (Windows Management Instrumentation Command line)

Lisensi Produk Windows adalah kunci yang memungkinkan Anda menggunakan sistem operasi Windows secara legal. Pada perangkat baru license key ini sering kali terintegrasi langsung pada motherboard komputer Anda, dan itu berarti Anda tidak perlu memasukkannya secara manual ketika Anda menginstal ulang Windows. Namun, untuk alasan tertentu, Anda mungkin ingin memeriksa kunci lisensi motherboard Anda. Berikut Caranya.

### Langkah 1: Buka Command Prompt

Pertama, Anda perlu membuka Command Prompt. Caranya adalah dengan menekan tombol "Win + X" dan memilih "Windows Terminal (Admin)" atau "Command Prompt (Admin)" jika Anda menggunakan Windows 10 atau Windows versi lebih baru. Jika Anda menggunakan versi Windows yang lebih baru. Anda juga bisa membuka command prompt dengan melakukan pencarian oada pencarian windows dengan mengetikam `command promt` atau `cmd` lalu klik kanan pilih Run Administrator.

### Langkah 2: Gunakan Perintah "wmic"

Setelah Command Prompt terbuka, ketik perintah berikut:
```
wmic path softwarelicensingservice get oa3xoriginalproductkey
```
Kemudian, tekan "Enter."

### Langkah 3: Cek Hasilnya

Setelah Anda menjalankan perintah di atas, sistem akan memberikan hasil berupa lisensi key yang terkait dengan motherboard Anda. Anda dapat mencatat atau menyimpan informasi ini sebagai referensi untuk masa depan.

{: .box-note}
Penting untuk diingat bahwa informasi ini hanya akan berguna jika Anda ingin memasang ulang Windows atau memverifikasi lisensi sistem Anda. Pastikan Anda menyimpan lisensi key ini dengan aman dan tidak membagikannya kepada orang lain.

Sekarang Anda tahu cara mengecek lisensi key pada motherboard Anda dengan perintah "wmic." Dengan informasi ini, Anda dapat lebih baik mengelola lisensi produk Windows pada komputer Anda.
