1. pertama jalankan perintah "apt-get update"(gambar 01)
2. setelah itu jalankan perintah "apt-get install nginx"(gambar 02)
3. setelah itu masuk ke direktori "/etc/nginx/sites-enabled" atau "/etc/nginx/sites-available" menggunakan perintah "cd" tapi disini saya menggunakan site-enabled(gambar 05)
4. lalu copy file "default" ke file konfigurasi kita dengan perintah "cp". contoh : "cp default dumbways.conf"(gambar 05)
5. setelah itu rubah konfigurasi pada file konfigurasi(dumbways.conf) menggunakan perintah "nano", contoh "nano dumbways.conf". disini yang saya rubah server_name (dumbways-dikitaufikgurohman.xyz) setelah itu simpan dengan CTRL+X lalu tekan Y (gambar 03)
6. setelah itu cantumkan server_name(dumbways-dikitaufikgurohman.xyz) pada "/etc/hosts" dengan perintah "nano" lalu cantumkan server_name dengan ip localhost disampingnya seperti pada gambar, lalu save.(gambar 04)
7. lalu jalankan perintah "curl -I 127.0.0.1" enter(gambar 05).
8. ketikkan domain/server_name yang kita cantumkan di browser, akan muncul 404 not found karena pada root direktori "var/www/html" tidak kita isi/buat jadi yang dikeluarkan adalah 404 not found page(default dari NGINX)(gambar 06)

gambar ada pada direktori folder_img/08/
