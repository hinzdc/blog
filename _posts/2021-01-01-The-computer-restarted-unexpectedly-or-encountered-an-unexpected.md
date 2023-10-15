---

layout: post
title: The computer restarted unexpectedly or encountered an unexpected loop error on Windows 10/11
subtitle: Cara mengatasi dan memperbaikinya
cover-img: /assets/img/error-loop-the-computer-restarted-unexpectedly-or.png
thumbnail-img: /assets/img/error-loop-the-computer-restarted-unexpectedly-or.png
tags: [error, registry, windows, install, trick]
comments: true

---

Dalam beberapa kasus, saat instalasi Window, mengupgrade ke Windows 11 baru, menginstal build Windows 10 baru, Anda mungkin menerima kesalahan. "Komputer tiba-tiba restart atau mengalami kesalahan yang tidak terduga. Instalasi Windows tidak dapat dilanjutkan ". Ketika Anda mengklik OK, komputer restart, dan jendela kesalahan muncul lagi, dan begitu seterusnya…
Apa yang dapat Anda lakukan dalam kasus ini untuk melanjutkan instalasi Windows?

Masalah ini mungkin muncul setelah reboot
selama instalasi (atau pembaruan) Windows dan terlihat seperti ini:

>The computer restarted unexpectedly or encountered an unexpected error. Windows installation cannot proceed. To install Windows, click “OK” to restart the computer, and then restart the installation.

![eror unexpectedly](/assets/img/error-loop-the-computer-restarted-unexpectedly-or.png)

Seperti yang saya katakan sebelumnya, jika kesalahan “The computer restarted unexpectedly or encountered an unexpected error.” terjadi, baik klik tombol OK maupun restart wizard instalasi Windows tidak membantu - kesalahan masih berulang.

Untuk memperbaiki masalah ini, Anda tidak perlu menutup pesan kesalahan atau klik OK:

1. Tekan Shift + F10 tepat di layar yang error. Pada beberapa laptop, Anda perlu menggunakan pintasan keyboard Shift+Fn+F10.

![run regedit](/assets/img/run-regedit-in-winpe.png)

2. Pada command prompt yang muncul, jalankan Registry Editor menggunakan perintah `regedit`.

3. Di Registry Editor, pergi ke reg key  `HKEY_LOCAL_MACHINE\SYSTEM\Setup\Status\ChildCompletion`

4. Di panel kanan, temukan parameter bernama setup.exe . Value kemungkinan besar 1. Ubah menjadi 3 dan save perubahannya.
![change reg key value](/assets/img/windows-registry-key-childcompletion-setup-exe.png)

{: .box-note}

**Note:** Oleh karena itu kami memaksa penginstal Windows untuk melanjutkan ke tahap instalasi berikutnya.

5. Tutup Registry Editor, dan reboot komputer Anda dengan mengklik OK di jendela kesalahan atau gunakan perintah ini : shutdown -r -t 0 pada command prompt.

Setelah restart, proses instalasi/pembaruan Windows 10 akan berlanjut secara normal.

Masalah ini umum terjadi tidak hanya pada Windows 10 dan Windows 11. Solusi instalasi sistem operasi yang terputus ini juga berfungsi dengan baik di Windows 7, Windows 8.1, dan Windows Server.
