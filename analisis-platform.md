# Analisis Komparatif Platform: Web, Desktop, dan Mobile
Mata Kuliah: Pemograman Berbasis Platform

Nama: Fakhri Azis Luthfiansyah | NIM: 240511113 | Kelas: TI24F

## Tabel Perbandingan

| Aspek | Web | Desktop | Mobile |
|---|---|---|---|
| **Bahasa utama** | HTML, CSS, JavaScript/TypeScript (frontend); PHP, Node.js, Python, Java (backend) | C#/.NET, C++, Java, Python; JavaScript via Electron | Kotlin/Java (Android), Swift (iOS); Dart (Flutter), JavaScript (React Native) |
| **Arsitektur** | Client-server: browser sebagai client, server menyediakan API dan database lewat HTTP/HTTPS | Aplikasi berjalan langsung di sistem operasi (standalone), mengakses file, hardware, dan API OS secara lokal; dapat juga terhubung ke server | Aplikasi terpasang di perangkat dan berjalan di atas SDK/OS mobile, umumnya terhubung ke backend/API cloud; memakai sensor perangkat (GPS, kamera) |
| **Cara distribusi** | Dideploy ke server/hosting lalu diakses lewat URL; tanpa instalasi | Installer (.exe, .msi, .dmg, .deb) atau toko aplikasi seperti Microsoft Store | Toko aplikasi resmi (Google Play Store, Apple App Store) atau APK untuk sideload di Android |
| **Keunggulan** | Lintas platform lewat browser, tanpa instalasi, pembaruan instan bagi semua pengguna, mudah diakses | Performa tinggi, akses penuh ke hardware dan file sistem, dapat bekerja offline | Akses sensor perangkat, notifikasi push, pengalaman pengguna yang dekat dengan pengguna, mobilitas tinggi |
| **Keterbatasan** | Bergantung pada koneksi internet dan browser; akses hardware terbatas; performa di bawah aplikasi native | Harus dibuat/dikemas per sistem operasi; instalasi dan pembaruan manual; kurang portabel | Biaya dan proses review toko aplikasi; fragmentasi perangkat (terutama Android); ukuran layar dan baterai terbatas |
| **Contoh aplikasi** | Google Docs, Tokopedia (web), GitHub | Visual Studio Code, Microsoft Word, Adobe Photoshop | WhatsApp, Gojek, Instagram |

## Referensi

1. Mozilla Developer Network. *Learn Web Development*. https://developer.mozilla.org/en-US/docs/Learn
2. Android Developers. *Android Developer Guides*. https://developer.android.com/guide
3. Microsoft. *Windows App Development Documentation*. https://learn.microsoft.com/en-us/windows/apps/

## Refleksi

Platform yang paling menarik untuk saya pelajari adalah web. Alasannya, web hanya memerlukan browser sehingga aplikasi dapat diakses dari perangkat apa pun tanpa instalasi, dan hasil pembaruannya langsung dirasakan semua pengguna. Selain itu, HTML, CSS, dan JavaScript juga menjadi dasar bagi pendekatan lintas platform seperti Electron untuk desktop dan framework hybrid untuk mobile, sehingga keterampilan yang saya pelajari dapat dipakai di platform lain.

Tantangan terbesar saat setup environment adalah ketika perintah `npm --version` gagal dijalankan di terminal VS Code, padahal Node.js sudah terpasang dan `node --version` berhasil. Muncul pesan bahwa menjalankan skrip dinonaktifkan di sistem, karena kebijakan eksekusi (execution policy) PowerShell memblokir file npm.ps1. Awalnya saya bingung karena pesan errornya panjang dan terlihat seperti instalasi saya gagal.

Saya mengatasinya dengan membaca pesan error dengan teliti, lalu menjalankan perintah `Set-ExecutionPolicy -Scope CurrentUser RemoteSigned` agar skrip yang aman dapat berjalan. Jika masalah serupa muncul lagi, saya akan membaca pesan error dari awal, memastikan penulisan perintah sudah benar, dan bertanya ke teman sekelas jika belum berhasil.