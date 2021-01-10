+++
date = 2021-01-06T17:00:00Z
description = "Pada kesempatan kali ini saya akan mempraktekkannya di Linux Ubuntu dan menggunakan module WebDAV dari Apache2. Tapi sebelum itu, usahakan sedia yang namanya internet, kopi, gorengan. Biar kalau error bisa browsing cara solving error-nya sambil sruput kopi."
summary = "Pada kesempatan kali ini saya akan mempraktekkannya di Linux Ubuntu dan menggunakan module WebDAV dari Apache2. Tapi sebelum itu, usahakan sedia yang namanya internet, kopi, gorengan. Biar kalau error bisa browsing cara solving error-nya sambil sruput kopi."
tags = ["Linux", "IT", "Server"]
title = "Cara Membuat File Sharing Server Dengan Apache di Linux Ubuntu (WebDAV)"

+++
Pada kesempatan kali ini saya akan mempraktekkannya di Linux Ubuntu dan menggunakan module [WebDAV](https://hanivan.github.io/blog/posts/membuat-file-sharing-dengan-apache2/ "WebDAV") dari Apache2. Tapi sebelum itu, usahakan sedia yang namanya internet, kopi, gorengan. Biar kalau error bisa browsing cara solving error-nya sambil sruput kopi.

Pada settingan default, Apache tidak mengaktifkan yang namanya WebDAV. Jadi kita harus mengaktifkannya secara manual. Cara gampang saja. Ikuti perintah-perintah dibawah ini.

### Enabling Module

    sudo a2enmod dav
    sudo a2enmod dav_fs
    sudo systemctl restart apache2

Step selanjutnya, kalian harus membuat folder-nya terlebih dahulu, kalian bebas ingin menempatkan dimana saja. Disini saya akan menempatkannya pada folder /var/www/webdav.

    sudo mkdir /var/www/webdav
    sudo chown -R www-data: /var/www/webdav

Selanjutnya, kita buat file konfigurasi virtual host baru untuk WebDAV. Pada kali ini, saya akan menamainya webdav.conf.

    sudo nano etc/apache2/sites-available/webdav.conf

Lalu masukkan settingan ini

    NameVirtualHost *
    <VirtualHost *:80>
    # ServerAdmin webmaster@domain # Ubah ke email jika diperlukan
    
    DocumentRoot /var/www/webdav/
    <Directory /var/www/webdav/>
    Options Indexes MultiViews
    AllowOverride None
    Order allow,deny
    allow from all
    </Directory>
    
    </VirtualHost>
    Alias /webdav /var/www/webdav
    <Location /webdav>
    DAV On
    AuthType Basic
    AuthName "webdav"
    AuthUserFile /var/www/webdav/passwd.dav
    Require valid-user
    </Location>

Lalu kita aktifkan konfigurasi-nya dengan mengetikkan:

    sudo a2ensite webdav.conf

Sebelum me-restart apache2, kalian harus menambahkan user dan password linux untuk service WebDAV. _Disarankan jangan user root_

    sudo htpasswd -c /var/www/webdav/passwd.dav $USER

Lalu kita ubah file permission-nya agar user root dan www-data saja yang dapat mengakses-nya, lalu restart apache2.

    sudo chown -R root:www-data /var/www/webdav/passwd.dav
    sudo chmod 640 /var/www/webdav/webdav.dav
    sudo systemctl restart apache2

Untuk mengecek apakah service WebDAV berjalan lancar, kunjungi alamat ini di web browser kalian:

_http://localhost/webdav_

Jika muncul pop-up username dan password, maka semua sudah berjalan dengan lancar.

### Referensi

[TechRepublic: How to enable WebDAV on your Ubuntu server](https://www.techrepublic.com/article/how-to-enable-webdav-on-your-ubuntu-server/ "TechRepublic: How to enable WebDAV on your Ubuntu server")