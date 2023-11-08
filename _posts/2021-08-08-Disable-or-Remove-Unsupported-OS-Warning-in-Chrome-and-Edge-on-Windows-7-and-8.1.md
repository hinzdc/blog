---
layout: post
title: Disable or Remove Unsupported OS Warning in Chrome and Edge on Windows 7 and 8.1
subtitle: 
tags: [Tutorial, registry]
comments: true
readtime: true
---

Windows 7 dan 8.1 adalah sistem operasi yang telah mencapai akhir dukungan resmi dari Microsoft. Beberapa peramban web modern seperti Google Chrome dan Microsoft Edge mungkin menampilkan peringatan "sistem operasi tidak didukung." Anda dapat menonaktifkan atau menghapus peringatan ini dengan mengedit Registry Editor (Regedit) menggunakan opsi "SuppressUnsupportedOSWarning." Artikel ini akan memandu Anda tentang cara melakukan ini di Windows 7 dan 8.1.

## Peringatan: Mengedit Registry Editor

Sebelum kita mulai, penting untuk diingat bahwa mengedit Registry Editor adalah tindakan yang sangat sensitif. Kesalahan dalam mengedit registri dapat merusak sistem operasi Anda. Pastikan Anda mengikuti petunjuk ini dengan hati-hati dan backup registri Anda sebelum memulai.

## Langkah 1: Buka Registry Editor

1. Tekan tombol "Windows + R" pada keyboard untuk membuka jendela "Run."

2. Ketik "regedit" dan tekan "Enter." Ini akan membuka Registry Editor.

## Langkah 2: Navigasi ke Key Registry yang Tepat

Anda perlu menavigasi ke lokasi yang benar dalam Registry Editor untuk menonaktifkan peringatan sistem operasi tidak didukung dengan opsi "SuppressUnsupportedOSWarning."

### Untuk Google Chrome:

1. Buka `HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Google\Chrome` (jika tidak ada, Anda perlu membuatnya).

2. Di dalam key "Chrome," cari "SuppressUnsupportedOSWarning" atau buat nilai DWORD (32-bit) baru jika tidak ada.

3. Ubah nilai "SuppressUnsupportedOSWarning" menjadi 1 untuk menonaktifkan peringatan.

### Untuk Microsoft Edge:

1. Buka `HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\Edge` (jika tidak ada, Anda perlu membuatnya).

2. Di dalam kunci "Edge," cari "SuppressUnsupportedOSWarning" atau buat nilai DWORD (32-bit) baru jika tidak ada.

3. Ubah nilai "SuppressUnsupportedOSWarning" menjadi 1 untuk menonaktifkan peringatan.

## Langkah 3: Restart Komputer

Setelah Anda mengedit registri, Anda perlu me-restart komputer Anda agar perubahan berlaku.

Sebelum mengambil langkah ini, pertimbangkan juga risiko keamanan yang mungkin terkait dengan menggunakan sistem operasi yang sudah tidak didukung. Jika memungkinkan, pertimbangkan untuk meningkatkan ke sistem operasi yang lebih baru dan didukung untuk pengalaman online yang lebih aman.
