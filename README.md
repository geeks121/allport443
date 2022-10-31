Apa itu Auto Script Install Xray
Auto Script Install Xray adalah script install otomatis yang dapat menginstall software yang dibutuhkan seperti Vmess , Vless, TrojanGo , Shadowsock dan SSH

dengan adanya Script Xray kita perlu bersusah payah dalam proses instalasi secara manual dan kita lebih mudah dalam memajemen user, kita dapat lebih mudah membuat user menghapus user

OS Didukung & Spek Minimal Auto Script Installer Xray
kita perlu menggunakan sistem operasi OS Linux sebagai berikut ini:

Debian 10 (Rekomendasi)
Ubuntu 18 LTS
Ubuntu 20
RAM Minimal 1GB (Max Akun 8-12)
CPU Minimal 1 (2 Lebih bagus/Lebih cepet installnya)
Fitur – Fitur Auto Script Installer Xray
VMESS WS TLS 443
VMESS WS NON TLS 80
VMESS GRPC 443
VLESS WS TLS 443
VLESS GRPC 443
TROJAN/TROJAN GO WS TLS 443
TROJAN/TROJAN GO GRPC 443
SHADOWSOCKS WS 443
SHADOWSOCKS GRPC 443
Panduan pasang Auto installer Script Xray Multi port 443
kita perlu melakukan tahapan secara urut supaya script yang ingin kita jalankan tidak mengalami eror

Setting Xray Untuk Cloudflare
kita perlu menggunakan akun cloudflare supaya GPRC dan websocket bisa berjalan dengan baik, tapi sebelumnya kamu perlu memiliki domain , kamu bisa memeli domain .my.id karena murah cuma 10.000 / tahun , untuk tutorial di bawah ini

Buka Aplikasi Google Chrome
akses situs Cloudflare
Login dengan Akun Cloudflare kamu
pastikan kamu sudah memasang domain kamu ke cloudflare
Pilih DNS add recode , buat subdmain mengarah ke IP VPS kamu
Pergi ke cloudflare ini konfiurasinya tab TLS/SSL Harus pilih yang FULL
jika kamu belum jelas bisa melihat gambar di bawah ini

![tls-cf](https://user-images.githubusercontent.com/16743443/198913949-405fb5d2-983e-4eb1-834e-f5f84a3ca41c.jpg)

Lalu pergi ke edge certificates disini kamu harus matiin Always HTTPS

![https-cf](https://user-images.githubusercontent.com/16743443/198913971-1339295f-86c7-4d11-9e66-3802b10d7e75.jpg)

Buka tab Network di cloudflare kamu aktifin WebSocket dan gRPC nya

![network-cf](https://user-images.githubusercontent.com/16743443/198914010-2c037d46-bfd4-4270-ac9d-e86eb77a3ad1.jpg)

setelah kamu berhasil konfigurasi akun cloudflare sesuai petunjuk diatas , selanjutnya ke tahapan selanjutnya yaitu install xray ke vps kamu , untuk panduan sebagai berikut ini

Cara pasang Auto install XRAY
Login VPS kamu menggunakan Aplikasi Putty dll
pastikan kamu login dengan menggunakan Akses root
kemudian masukan kode perintah di bawah ini

'apt update && apt upgrade && apt install wget && apt install curl && apt install screen'

kemudian masukan kode untuk install xray

wget https://raw.githubusercontent.com/hidessh99/allport443/sae/setup.sh && chmod +x setup.sh && ./setup.sh

tunggu proses beberapa menit hingga proses installer berhasil

Cara Penggunaan Xray di VPS
Login VPS kamu menggunakan Aplikasi Putty dll
pastikan kamu login dengan menggunakan Akses root
Kemudian Ketik menu
pilih nomer yang kamu inginkan ,
misalnya nomer 7  untuk membuat akun V2ray

Masukan username dan masa aktif akun tersebut
selesai , secara otomatis config Xray V2ray secara otomatis berfungsi


