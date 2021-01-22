+++
date = 2021-01-22T13:47:00Z
description = "Cyber Security+: Tipe Perangkat Lunak Berbahaya"
draft = true
summary = ""
tags = ["CompTIA", "Cyber Security+", "IT"]
title = "Cyber Security+: Tipe Perangkat Lunak Berbahaya"

+++
## Virus

Virus komputer merupakan kode yang berjalan di komputer tanpa sepengetahuan pengguna, virus menginfeksi komputer ketika kode tersebut terakses dan tereksekusi. Agar virus dapat bekerja, pertama virus harus dijalankan oleh pengguna dengan berbagai cara. Virus juga memiliki kemampuan reproduksi dan dapat menyebarkan salinannya sendiri ke seluruh sistem komputer.

Salah satu contoh virus yang terkenal adalah Love Bug. Berasal pada tahun 2000, virus ini akan tiba melalui email berjudul "I love you" dengan lampiran bernama love-letter-for-you.txt.vbs, atau salah satu dari beberapa permutasi lain dari cinta fiktif ini. Beberapa pengguna akan tertipu untuk berpikir ini adalah file teks, tetapi ekstensi itu sebenarnya .vbs, kependekan dari skrip Visual Basic. Virus ini menghapus file, mengirim nama pengguna dan kata sandi ke pembuatnya, menginfeksi 15 juta komputer, dan diduga menyebabkan kerusakan sebanyak $ 5 miliar. Ajarilah pengguna anda tentang cara menyaring surel mereka.

Anda mungkin menemukan beberapa tipe virus:

* **Boot sector**: Virus yang menginisialisasi dirinya di sektor pertama harddisk, ketika komputer menyala, otomatis virus akan masuk kedalam memory.
* **Macro:** Biasanya disematkan di email atau pesan berupa dokumen.
* **Program:** Infects executable files.
* **Encrypted:** Menggunakan enkripsi sederhana untuk mengenkripsi dirinya sendiri. Virus ini terdiri dari kode yang terenkripsi untuk mengkindari deteksi dan suatu modul deksipsi.
* **Polymorphic**: DIbangun mirip seperti encrypted virus, tetapi modul untuk dekripsinya selalu berubah setiap virus ini menginfeksi.
* **Metamorphic:** Mirip seperti polymorphic tetapi virus ini melakukan rewrite codenya secara keseluruhan setiap saat virus ini menginfeksi.
* **Stealth:** Menggunaka banyak cara untuk mengelabui anti virus.
* **Armored**: Virus ini melakukan proteksi terhadap anti virus dengan mengelabui lokasi virus tersebut. Proteksi ini digunakan juga untuk mengelabui seorang analis.
* **Multipartite:** Tipe hybrid boot sector dan program virus. Virus ini menyerang boot sector atau file system kemudian menyerang file lain di sistem tersebut.

## Worms

Worms seperti virus, kecuali jika ia bereplikasi sendiri, sedangkan virus tidak. Worm melakukan ini dalam upaya untuk menyebar ke komputer lain. Worms memanfaatkan celah keamanan dalam sistem operasi dan aplikasi, termasuk backdoor, yang akan kita bahas nanti. Worms mencari target lain di jaringan atau melalui Internet yang menjalankan aplikasi yang sama dan mereplikasi dirinya ke sistem lain. Dengan worm, pengguna tidak perlu mengakses dan menjalankannya. Virus membutuhkan sesuatu untuk membawanya ke tempat yang diinginkan dan memerlukan instruksi eksplisit untuk dieksekusi, atau harus dijalankan oleh pengguna. Worm tidak memerlukan sesuatu tersebut atau instruksi eksplisit untuk dieksekusi.

Contoh worm yang terkenal adalah Nimda (admin backward), yang disebarkan secara otomatis melalui Internet dalam 22 menit pada tahun 2001, yang menyebabkan kerusakan luas. Ini menyebar melalui jaringan bersama, surel massal, dan kerentanan sistem operasi.

Terkadang, Worm tidak membawa muatan, yang berarti bahwa dalam dan dari dirinya sendiri, itu tidak mengandung kode yang dapat membahayakan komputer. Ini mungkin atau mungkin tidak termasuk malware lain, tetapi bahkan jika tidak, ia dapat menyebabkan gangguan umum terhadap lalu lintas jaringan dan operasi komputer karena sifat kemampuannya yang dapat bereplikasi sendiri.

## Trojan Horses

Trojan horse, atau Trojan, muncul untuk melakukan tugas yang diinginkan tetapi sebenarnya melakukan tugas berbahaya di belakang layar. Ini sebenarnya bukan virus secara teknikal dan dapat dengan mudah diunduh tanpa diketahui. Trojan juga dapat ditransfer ke komputer melalui media removable, terutama USB flash drive. Salah satu contoh Trojan adalah file yang terkandung dalam program yang diunduh seperti generator kunci — dikenal sebagai “keygen” yang digunakan dengan perangkat lunak bajakan — atau yang dapat dieksekusi lainnya. Jika pengguna mengeluh tentang kinerja sistem yang lambat dan banyak peringatan antivirus, dan mereka baru-baru ini menginstal program yang tidak jelas dari Internet atau dari USB flash drive, komputer mereka bisa jadi terinfeksi oleh Trojan.

Remote access Trojans (RATs) adalah jenis Trojan yang paling umum, contohnya termasuk Back Orifice, NetBus, dan SubSeven; kemampuan mereka untuk memungkinkan penyerang memiliki hak administratif yang lebih tinggi daripada pemilik sistem, membuat mereka cukup berbahaya. Perangkat lunak ini secara efektif bertindak sebagai alat administrasi jarak jauh, yang kebetulan merupakan nama lain untuk singkatan RAT. Program-program ini memiliki kemampuan untuk memindai host yang tidak dilindungi dan membuat semua jenis perubahan ke host ketika terhubung. RAT tidak selalu dirancang untuk digunakan secara jahat, tetapi mudah bagi orang biasa untuk mengunduh dan memanipulasi komputer. Lebih buruk lagi, ketika komputer target dikendalikan oleh penyerang, ia bisa dengan mudah menjadi robot, atau bot, yang menjalankan rencana penyerang sesuai perintah. Kami akan membahas bot nanti di bab ini.

RAT juga dapat ditulis menggunakan bahasa PHP (atau bahasa lain) untuk memungkinkan akses jarak jauh ke situs web. Contohnya adalah web shell, yang memiliki banyak permutasi. Ini memungkinkan penyerang untuk mengkonfigurasi server web dari jarak jauh tanpa persetujuan pengguna. Seringnya, penyerang akan meretas kata sandi FTP untuk mengunggah RAT.

RAT sering digunakan untuk terus-menerus menargetkan entitas tertentu seperti pemerintahan atau perusahaan tertentu. Salah satu contohnya adalah RAT PlugX. Perangkat lunak berbahaya seperti ini dikenal sebagai ancaman persisten tingkat lanjut (APT). Kelompok-kelompok yang memiliki sumber daya yang sangat besar dapat memanfaatkan APT ini untuk menjalankan tujuan melawan musuh-musuh skala besar. Grup APT dapat menggunakan bentuk faksi peretas besar, dan bahkan beberapa perusahaan dan pemerintah di seluruh dunia.

## Ransomware

Beberapa orang yang kurang memiliki reputasi menggunakan malware yang sangat licik yang dikenal sebagai ransomware — jenis malware yang membatasi akses ke sistem komputer dan menuntut tebusan dibayarkan. Juga dikenal sebagai crypto-malware, ini mengenkripsi file dan, atau mengunci sistem. kemudian memberitahu pengguna bahwa untuk mendekripsi file, atau membuka kunci komputer untuk mendapatkan kembali akses ke file, pembayaran harus dilakukan ke salah satu dari beberapa layanan perbankan, sering di luar negeri. Ini sering menyebar sebagai Trojan atau worm, dan biasanya menggunakan enkripsi untuk menyebabkan file pengguna tidak dapat diakses. Penggunaan enkripsi ini juga dikenal sebagai pemerasan cryptoviral. Salah satu contohnya adalah CryptoLocker.

Trojan ransomware ini mengenkripsi file tertentu pada drive komputer menggunakan kunci publik RSA. (Kunci pribadi rekanan disimpan di server pembuat malware.) Meskipun Trojan dapat dengan mudah dikalahkan dengan dikarantina atau dihapus, file tetap dienkripsi, dan hampir mustahil untuk didekripsi (diberi kekuatan kunci RSA). Pembayaran sering diperlukan dalam bentuk voucher, atau dalam bentuk mata uang digital seperti Bitcoin. Serangan Ransomware tumbuh terus selama beberapa tahun hingga 2013 ketika CryptoLocker (dan Trojan ransomware serupa lainnya) muncul — sekarang ratusan ribu komputer di seluruh dunia terpengaruh setiap tahun.

## Spyware

Spyware adalah jenis perangkat lunak berbahaya yang diunduh tanpa disadari dari situs web atau diinstal bersama dengan beberapa perangkat lunak pihak ketiga lainnya. Biasanya, malware ini mengumpulkan informasi tentang pengguna tanpa persetujuan pengguna. Spyware bisa sesederhana bagian kode yang mencatat situs web apa yang Anda akses, atau program yang merekam penekanan tombol Anda (dikenal sebagai keylogger). Spyware juga dikaitkan dengan periklanan (pop-up yang tidak hilang begitu saja!), Dan kadang-kadang terkait dengan iklan jahat, atau maliklan — penggunaan iklan berbasis Internet (sah dan tidak sah) untuk mendistribusikan perangkat lunak berbahaya.

Spyware mungkin dapat mengubah konfigurasi komputer tanpa interaksi pengguna; misalnya, mengarahkan ulang peramban untuk mengakses situs web selain yang diinginkan. Adware biasanya jatuh ke ranah spyware karena muncul iklan berdasarkan apa yang telah dipelajari dari memata-matai pengguna. Grayware adalah istilah umum lain yang menjelaskan aplikasi yang berperilaku tidak tepat tetapi tanpa konsekuensi serius. Ini terkait dengan program spyware, adware, dan lelucon.

Salah satu contoh (dari banyak) spyware adalah Internet Optimizer, yang mengalihkan halaman error dari Internet Explorer ke halaman iklan situs web lain. Spyware can even be taken to the next level and be coded in such a way to hijack a person’s computer. Going beyond this, spyware can be used for cyber-espionage, as was the case with Red October—which was installed to users’ computers when they unwittingly were redirected to websites with special PHP pages that exploited a Java flaw, causing the download of the malware.

## Rootkits

Rootkit adalah jenis perangkat lunak yang dirancang untuk mendapatkan kontrol tingkat administrator atas sistem komputer tanpa terdeteksi. Istilah ini adalah kombinasi dari kata "root" (artinya pengguna root dalam sistem Unix / Linux atau administrator dalam sistem Windows) dan "kit" (artinya perangkat lunak kit). Biasanya, tujuan rootkit adalah untuk melakukan operasi jahat pada komputer target di kemudian hari tanpa sepengetahuan administrator atau pengguna komputer itu. Rootkit adalah variasi pada virus yang mencoba menggali ke tingkat yang lebih rendah dari sistem operasi — komponen OS yang mulai sebelum layanan anti-malware ikut bermain.

Rootkit dapat menargetkan UEFI / BIOS, boot loader, kernel, dan lainnya. Contoh dari rootkit boot loader adalah Evil Maid Attack; serangan ini dapat mengekstrak kunci enkripsi dari sistem enkripsi keseluruhan disk, yang akan kita bahas lebih lanjut. Contoh lain (lebih terkini) adalah rootkit Alureon, yang memengaruhi master boot record (MBR) dan driver sistem tingkat rendah (seperti atapi.sys). Rootkit khusus ini didistribusikan oleh botnet, dan mempengaruhi lebih dari 200.000 sistem operasi Microsoft.

Rootkit sulit dideteksi karena diaktifkan sebelum sistem operasi sepenuhnya boot. Rootkit mungkin memasang file tersembunyi, proses tersembunyi, dan akun pengguna tersembunyi.Karena rootkit dapat diinstal pada perangkat keras atau perangkat lunak, rootkit dapat mencegat data dari koneksi jaringan, keyboard, dan sebagainya.

## Spam

Pernahkah Anda menerima email yang meminta Anda mengirim uang ke orang asing di negara yang jauh? Atau email yang menawarkan jam tangan Rolex yang sangat murah? Atau saham terbaik berikutnya? Semua ini adalah contoh spam. Spam adalah penyalahgunaan sistem pesan elektronik seperti email, SMS, media sosial, media siaran, pesan instan, dan sebagainya. Spammer mengirim pesan massal yang tidak diminta tanpa pandang bulu, biasanya tanpa keuntungan bagi spammer yang sebenarnya, karena mayoritas spam dibelokkan atau diabaikan. Perusahaan dengan etika yang diragukan memanfaatkan jenis pemasaran ini (biasanya dirancang sebagai skema piramida) sehingga orang-orang yang berada di puncak rantai pemasaran dapat memperoleh manfaat; namun, biasanya tidak bermanfaat bagi orang yang mengirim spam.

Bentuk spam yang paling umum adalah spam e-mail, yang merupakan salah satu spam terburuk untuk administrator jaringan. Spam dapat menyumbat sumber daya dan mungkin menyebabkan jenis denial-of-service ke server email. Ini juga dapat menyesatkan pengguna, dalam upaya rekayasa sosial. Dan sebagian besar virus berbasis jaringan ditransfer melalui email spam. Jenis spamming terburuk adalah ketika seseorang menggunakan server email organisasi lain untuk mengirim spam. Jelas ilegal, itu juga bisa menciptakan masalah hukum bagi organisasi yang memiliki server email.

Turunan dari spam, yang disebut spim (spam di atas pesan instan), adalah penyalahgunaan sistem pesan instan, ruang obrolan, dan fungsi obrolan dalam game secara khusus. Ia juga dikenal sebagai spam pesan, atau spam IM.

Selanjutnya: Rangkuman Ancaman Malware

Sebelumnya: Pendahuluan