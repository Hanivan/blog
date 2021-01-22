+++
date = 2021-01-22T14:25:00Z
description = "Cyber Security+: Pencegahan dan Penanggulangan Rootkit"
summary = ""
tags = ["CompTIA", "Cyber Security+", "IT"]
title = "Cyber Security+: Pencegahan dan Penanggulangan Rootkit"

+++
Rootkit yang berhasil diinstal memungkinkan pengguna yang tidak sah untuk mendapatkan akses ke sistem dan bertindak sebagai pengguna root atau administrator. Rootkit disalin ke komputer sebagai file binary; file biner ini dapat dideteksi oleh program antivirus berbasis tanda tangan dan heuristik. Namun, setelah rootkit dieksekusi, bisa jadi sulit untuk dideteksi. Ini karena kebanyakan rootkit adalah kumpulan program yang bekerja bersama yang dapat membuat banyak modifikasi pada sistem.

Ketika subversi sistem operasi terjadi, OS tidak dapat dipercaya, dan sulit untuk mengetahui apakah program antivirus Anda berjalan dengan baik, atau apakah ada upaya Anda yang lain yang memiliki efek. Meskipun produsen perangkat lunak keamanan berusaha mendeteksi rootkit yang berjalan, diragukan bahwa mereka akan berhasil. Cara terbaik untuk mengidentifikasi rootkit adalah dengan menggunakan media yang dapat dilepas (USB flash drive atau disk penyelamat khusus) untuk mem-boot komputer. Dengan cara ini, sistem operasi tidak berjalan, dan karena itu rootkit tidak berjalan, membuatnya lebih mudah dideteksi oleh media eksternal.

Terkadang, rootkit akan bersembunyi di MBR. Seringkali, produsen sistem operasi merekomendasikan untuk membersihkan MBR (menulis ulang, misalnya, dalam Opsi Pemulihan Sistem atau lingkungan pemulihan lainnya) dan kemudian memindai dengan perangkat lunak antivirus. Ini tergantung pada jenis rootkit. Penggunaan GPT sebagai pengganti MBR membantu untuk mencegah rootkit. Saya sarankan menggunakan GPT jika memungkinkan.

Sayangnya, karena kesulitan dalam menghapus rootkit, cara terbaik untuk memerangi rootkit adalah menginstal ulang semua perangkat lunak. Secara umum, teknisi PC, setelah mendeteksi rootkit, akan melakukan hal itu, karena biasanya membutuhkan waktu lebih sedikit daripada upaya untuk memperbaiki semua masalah rootkit, ditambah lagi dapat memverifikasi bahwa rootkit telah dihapus sepenuhnya.

Selanjutnya: Pencegahan dan Penanggulangan Spam

Sebelumnya: Pencegahan dan Penanggulangan Spyware