+++
date = 2021-01-06T17:00:00Z
description = "WebDAV (Web Distributed Authoring and Versioning) adalah perpanjangan dari Hypertext Transfer Protocol (HTTP) yang memungkinkan klien melakukan operasi pembuatan konten Web jarak jauh. WebDAV ditentukan di RFC 4918 oleh grup kerja dari Internet Engineering Task Force."
summary = "WebDAV (Web Distributed Authoring and Versioning) adalah perpanjangan dari Hypertext Transfer Protocol (HTTP) yang memungkinkan klien melakukan operasi pembuatan konten Web jarak jauh. WebDAV ditentukan di RFC 4918 oleh grup kerja dari Internet Engineering Task Force."
tags = ["Linux", "IT", "Server"]
title = "Apa itu WebDAV?"

+++
WebDAV (Web Distributed Authoring and Versioning) adalah perpanjangan dari Hypertext Transfer Protocol (HTTP) yang memungkinkan klien melakukan operasi pembuatan konten Web jarak jauh. WebDAV ditentukan di RFC 4918 oleh grup kerja dari Internet Engineering Task Force.

Protokol WebDAV1 menyediakan kerangka kerja bagi pengguna untuk membuat, mengubah, dan memindahkan dokumen di server. Fitur terpenting dari protokol WebDAV mencakup pemeliharaan properti tentang penulis atau tanggal modifikasi, manajemen namespace, koleksi, dan perlindungan penimpaan. Pemeliharaan properti mencakup hal-hal seperti pembuatan, penghapusan, dan kueri informasi file. Manajemen namespace berhubungan dengan kemampuan untuk menyalin dan memindahkan halaman web dalam namespace server. Koleksi berhubungan dengan pembuatan, penghapusan, dan daftar berbagai sumber daya. Terakhir, perlindungan penimpaan menangani aspek-aspek yang terkait dengan penguncian file.

Banyak sistem operasi modern menyediakan dukungan sisi klien built-in untuk WebDAV.

## Sejarah

WebDAV dimulai pada tahun 1996 ketika Jim Whitehead, seorang lulusan PhD dari UC Irvine, bekerja dengan World Wide Web Consortium (W3C) untuk menyelenggarakan dua pertemuan untuk membahas masalah penulisan terdistribusi di World Wide Web dengan orang-orang yang tertarik. Visi asli Tim Berners-Lee tentang Web melibatkan media untuk membaca dan menulis. Nyatanya, peramban web pertama Berners-Lee, yang disebut WorldWideWeb, dapat melihat dan menyunting laman web; tetapi, seiring pertumbuhan Web, ini menjadi media hanya-baca bagi sebagian besar pengguna. Whitehead dan orang-orang yang berpikiran sama ingin mengatasi batasan itu.

Pertemuan tersebut menghasilkan pembentukan kelompok kerja IETF, karena upaya baru akan mengarah pada ekstensi ke HTTP, yang telah mulai distandarisasi oleh IETF.

Ketika pekerjaan dimulai pada protokol, menjadi jelas bahwa menangani baik penulisan terdistribusi dan pembuatan versi bersama-sama akan melibatkan terlalu banyak pekerjaan dan bahwa tugas harus dipisahkan. Grup WebDAV berfokus pada penulisan terdistribusi, dan pembuatan versi kiri untuk masa depan. (Ekstensi Delta-V menambahkan versi nanti - lihat bagian Ekstensi di bawah.)

Kelompok kerja WebDAV menyelesaikan pekerjaannya pada Maret 2007, setelah Internet Engineering Steering Group (IESG) menerima pembaruan tambahan untuk RFC 2518. Ekstensi lain yang belum selesai pada saat itu, seperti metode BIND, telah diselesaikan oleh masing-masing penulisnya, independen dari kelompok kerja formal.

## Penerapan

WebDAV memperluas kumpulan kata kerja dan header HTTP standar yang diizinkan untuk metode permintaan. Kata kerja yang ditambahkan meliputi:

**COPY**
Menyalin sumber daya dari satu URI ke URI lainnya

**LOCK**
Mengunci sumber daya. WebDAV mendukung kunci bersama dan eksklusif

**MKCOL**
Membuat koleksi (alias direktori)

**MOVE**
Memindahkan sumber daya dari satu URI ke URI lainnya

**PROPFIND**
Mengambil properti, disimpan sebagai XML, dari sumber daya web. Ini juga kelebihan beban untuk memungkinkan seseorang mengambil struktur koleksi (juga dikenal sebagai hierarki direktori) dari sistem jarak jauh

**PROPPATCH**
Mengubah dan menghapus beberapa properti pada sumber daya dalam satu tindakan atom

**UNLOCK**
Menghapus kunci dari sumber daya

## Web Server Support

* Apache
* Caddy
* lighttpd
* Mailfence
* Microsoft's IIS
* MyWorkDrive Server
* Nextcloud
* Nginx
* ownCloud
* SabreDAV

## Client Support

* Git
* Linux melalui GVfs, termasuk File GNOME dan melalui KIO, termasuk Konqueror dan Dolphin
* macOS, termasuk dukungan asli untuk CalDAV dan CardDAV, yang desainnya didasarkan pada WebDAV
* Microsoft Windows, termasuk dukungan asli di File Explorer
* Microsoft Office

**Sumber**

[Wikipedia: WebDAV](https://en.wikipedia.org/wiki/WebDAV "Wikipedia: WebDAV")