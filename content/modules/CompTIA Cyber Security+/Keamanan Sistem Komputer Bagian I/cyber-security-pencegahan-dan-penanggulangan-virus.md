+++
date = 2021-01-22T14:16:00Z
description = "Cyber Security+: Pencegahan dan Penanggulangan Virus"
summary = ""
tags = ["CompTIA", "Cyber Security+", "IT"]
title = "Cyber Security+: Pencegahan dan Penanggulangan Virus"

+++
Kita dapat melakukan beberapa hal untuk melindungi sistem komputer dari virus. Pertama, setiap komputer harus memiliki platform perlindungan titik akhir yang kuat — artinya perangkat lunak antivirus harus berjalan di atasnya. Ada banyak penyedia perlindungan antivirus, ditambah pabrikan sistem operasi sering membundel perangkat lunak AV dengan OS atau menawarkan unduhan gratis. Kedua, perangkat lunak AV harus diperbarui, yang berarti bahwa perangkat lunak tersebut memerlukan lisensi saat ini; ini diperbarui setiap tahun dengan sebagian besar penyedianya. Saat memperbarui, pastikan untuk memperbaharui mesin AV, bisa dengan cara manual. Jika tidak, setel perangkat lunak AV untuk secara otomatis memperbarui pada interval berkala, misalnya, setiap hari atau setiap minggu. Merupakan ide bagus untuk menjadwalkan pemindaian penuh sistem secara teratur dalam perangkat lunak AV.

Selama anti virus diperbaharui, sistem antivirus biasanya menemukan virus bersama dengan malware lain seperti worm dan Trojan. Namun, sistem ini biasanya tidak menemukan logic bombs, rootkit, dan aktivitas botnet. Sebagai penggantinya, perlu diingat bahwa perangkat lunak AV penting, tetapi itu bukan obat untuk semuanya.

Selanjutnya, kita ingin memastikan bahwa komputer memiliki pembaruan terbaru yang tersedia. Ini berlaku untuk sistem operasi dan aplikasi. Backdoor di dalam OS dan aplikasi lainnya tidak umum, dan pembuat OS biasanya merilis perbaikan untuk bugs keamanan ini. Windows menawarkan program Pembaruan Windows. Ini harus diaktifkan, dan Anda harus memeriksa pembaruan secara berkala atau mengatur sistem untuk memeriksa pembaruan secara otomatis. Mungkin organisasi Anda memiliki aturan yang mengatur bagaimana fungsi Pembaruan Windows berfungsi. Jika demikian, konfigurasikan Pembaruan Otomatis sesuai dengan kebijakan perusahaan Anda.

Penting juga untuk memastikan bahwa firewall tersedia, diaktifkan, dan diperbarui. Firewall menutup semua port masuk ke komputer Anda — atau jaringan — dalam upaya untuk memblokir penyusup. Misalnya, Windows Firewall adalah fitur berbasis perangkat lunak bawaan yang disertakan dalam Windows. Anda dapat melihat bahwa firewall pada gambar diaktifkan untuk jaringan pribadi dan tamu / publik. Selalu verifikasi fungsionalitas firewall titik akhir!

![Pencegahan dan Penanggulangan Virus](https://course.adinusa.id/media/markdownx/47bef9b7-fc37-4aca-9b53-bd45b13d0ec4.jpg)

Anda mungkin juga memiliki firewall berbasis perangkat keras; misalnya, router yang termasuk dalam router kantor kecil / kantor rumah (SOHO). Dengan menggunakan keduanya, Anda memiliki dua lapisan perlindungan dari berbagai serangan yang mungkin termasuk muatan dengan malware. Ingatlah bahwa Anda mungkin perlu menetapkan pengecualian untuk program yang perlu mengakses Internet. Ini dapat dilakukan oleh program, atau port yang digunakan oleh protokol, dan dapat dikonfigurasikan untuk memungkinkan aplikasi tertentu untuk berkomunikasi melalui firewall sambil menjaga sisa port tetap tertutup.

Cara lain untuk membantu mencegah virus adalah dengan menggunakan apa yang disebut "pemisahan OS dan data." Metode ini membutuhkan dua hard drive. Sistem operasi diinstal ke drive C: dan data disimpan pada drive D: (atau huruf apa pun yang Anda gunakan untuk drive kedua). Ini mengelompokkan sistem dan data, membuatnya lebih sulit bagi virus untuk menyebar dan lebih mudah mengisolasi mereka ketika memindai. Ini juga memungkinkan instalasi ulang yang mudah tanpa harus membuat cadangan data! Cara yang lebih murah untuk melakukannya adalah dengan menggunakan dua partisi pada drive yang sama.

Enkripsi adalah salah satu cara terbaik untuk melindungi data, yang jika tidak akan rusak (atau hilang) karena aktivitas virus di komputer. Sistem operasi Windows menggunakan Encrypting File System (EFS), yang dapat mengenkripsi file secara individual. Ketika file dienkripsi dengan cara ini, nama file muncul berwarna hijau dalam Windows Explorer atau File Explorer. Ini mencegah clear-text access dan menolak modifikasi dalam kebanyakan kasus. Enkripsi jenis ini mungkin tidak akan mencegah virus muncul, tetapi dapat membantu melindungi file individual dari gangguan. Kita akan berbicara lebih banyak tentang enkripsi di bagian selanjutnya.

Terakhir, beri tahu pengguna tentang bagaimana virus dapat menginfeksi sistem. Instruksikan mereka tentang cara menyaring email mereka, dan beritahu mereka untuk tidak membuka lampiran yang tidak dikenal. Tunjukkan pada mereka cara memindai removable media sebelum menyalin file ke komputer. Terkadang pendidikan terhadap pengguna berfungsi; terkadang tidak. Salah satu cara untuk membuat pendidikan pengguna lebih efektif adalah memiliki pelatih teknis yang mendidik pengguna Anda, daripada melakukannya sendiri. Atau, pertimbangkan untuk membuat tutorial pembelajaran online interaktif. Metode-metode ini dapat memberikan lingkungan belajar yang lebih menarik.

Dengan menggunakan semua teknik ini, infeksi virus dapat sangat berkurang. Namun, jika komputer terinfeksi oleh virus, Anda ingin tahu apa yang harus dicari sehingga Anda dapat "menyembuhkan" komputer.

Berikut adalah beberapa gejala khas virus:

* Komputer berjalan lebih lambat dari biasanya.
* Komputer sering terkunci atau berhenti merespon sama sekali
* Komputer restart sendiri atau sering crash
* Hard drive, optical drive, dan aplikasi tidak dapat diakses atau tidak berfungsi dengan baik
* Ada suara aneh terdengar
* Muncul notifikasi pesan error yang tidak biasa
* Tampilan gambar distorsi
* Ada Icon baru muncul dan Icon lama hilang
* Ada extension rangkap di file yang sama, contohnya: .txt.vbs, .txt.exe.
* Program anti virus tidak dapat berjalan dan tidak dapat diinstall
* File gambar rusak atau muncul banyak folder tiba-tiba
* Kemampuan pemulihan sistem tidak ada atau terhapus

Berikut ini adalah prosedur yang disarankan untuk menghapus malware secara umum:

1. Identifikasi gejala Malware
2. Karantina sistem yang terinfeksi
3. Nonaktifkan sistem pemulihan
4. Remediasi sistem yang terinfeksi: a) perbaharui perangkat lunak anti Malware, b) Gunakan teknik pemindaian dan penghapusan, seperti Safe Mode dan lingkungan pre-instalasi.
5. Jadwalkan pemindaian dan jalankan pembaruan perangkat lunak
6. Aktifkan sistem pemulihan dan buat titik pemulihan
7. Berikan informasi bagi pengguna

Sebelum melakukan perubahan apapun pada komputer, pastikan Anda mencadangkan data penting dan memverifikasi bahwa pembaruan terbaru telah diinstal ke OS dan perangkat lunak AV. Kemudian lakukan pemindaian menyeluruh terhadap sistem menggunakan utilitas pindai perangkat lunak AV; jika diizinkan oleh perangkat lunak, jalankan pemindaian dalam Safe Mode.

Pilihan lain adalah memindahkan drive yang terpengaruh ke "mesin bersih," komputer yang tidak terhubung ke jaringan apa pun, dan digunakan semata-mata dengan tujuan memindai malware. Ini dapat dilakukan dengan menggunakan kit konverter USB atau sistem drive yang dapat dilepas, atau dengan memindahkan drive yang terpengaruh ke port hard drive lain dari komputer lain. Kemudian, jalankan perangkat lunak AV pada mesin bersih itu untuk memindai drive itu. Tukang service PC menggunakan konsep mesin bersih yang terisolasi ini.

Semoga, perangkat lunak AV menemukan dan mengkarantina virus pada sistem. Jika pemindaian perangkat lunak AV tidak menemukan masalah, atau jika perangkat lunak AV telah terinfeksi dan tidak dapat dijalankan, Anda dapat mencoba menggunakan pemindai online gratis.

Dalam kasus yang jarang terjadi, Anda mungkin perlu menghapus file individual dan menghapus entri Registry. Ini mungkin satu-satunya solusi ketika virus baru telah menginfeksi sistem dan tidak ada fitur antivirus yang dirilis. Petunjuk tentang cara menghapus virus dengan cara ini dapat ditemukan di situs web produsen perangkat lunak AV.

Ketika terjadi virus pada boot sector, perangkat lunak AV Anda masih merupakan taruhan terbaik. Perangkat lunak AV mungkin menggunakan flash drive USB yang dapat di-boot atau disk yang dapat di-boot untuk menyelesaikan pemindaian sektor boot, atau mungkin memiliki pelindung boot bawaan. Beberapa program UEFI / BIOS memiliki kemampuan untuk memindai sektor boot hard drive saat startup; ini mungkin perlu diaktifkan di pengaturan UEFI / BIOS terlebih dahulu. Anda juga dapat menggunakan lingkungan pemulihan dan baris perintah untuk memperbaiki sektor boot.

Kemungkinan lain adalah dengan menggunakan alat berbasis Linux yang dapat diunduh secara bebas dan membuat Live CD Linux seperti Knoppix, yang dapat digunakan untuk mem-boot dan memperbaiki komputer.

Perlu diingat bahwa lingkungan pemulihan dan metode baris perintah lainnya mungkin tidak memperbaiki masalah; mereka mungkin membuat hard drive tidak dapat beroperasi tergantung pada jenis virus. Jadi, yang terbaik adalah terlebih dahulu menggunakan berbagai utilitas perangkat lunak AV yang telah Anda beli untuk sistem.

Selanjutnya: Pencegahan dan Penanggulangan Worm dan Trojan

Sebelumnya: Pengiriman Malware