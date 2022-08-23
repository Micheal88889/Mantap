

# Khusus Untuk OS
* • Debian 10 & 9
atau
* • Ubuntu 18.04 & 20.04
* Working For VPS AWS,AZURE,DO

  
### 3.

  <img src="https://img.shields.io/badge/Install_Semua_Layanan_VPN%20-green">

* Install Semua Layanan VPN /Install All VPN Service
   
```html
rm -f setup.sh && apt update && apt upgrade -y && update-grub && sleep 2 && apt-get update -y && apt-get upgrade && sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt install -y bzip2 gzip coreutils screen curl unzip && wget https://raw.githubusercontent.com/fisabiliyusri/Mantap/main/setup.sh && chmod +x setup.sh && sed -i -e 's/\r$//' setup.sh && screen -S setup ./setup.sh
  
```
  

### 4. DONE / SELESAI
<img src="https://img.shields.io/badge/DONE%20_/_%20SELESAI-green">

* • jika tidak bisa login di vps ,gunakan port ssh
* • 22, 2253

### Shopee https://shopee.com.my/v2rayxios?categoryId=100634&itemId=8030082359


### 5. MENU, INFO ,UPDATE ,FIX
* untuk menampilkan menu
```html
menu
```
* untuk update menu dan update info
```html
updatemenu
```
* otomatis untuk memperbaiki error SSLH, WS-TLS
```html
sl-fix
```
```html
reboot
```
* Perbaiki SSL ERROR
* otomatis untuk memperbaiki error Sertifikat SSL/TLS dan SUBDOMAIN
* perbaiki error di bagian acme domain
* untuk update Sertifikat SSL/TLS
```html
slhost && certv2ray
```
* lalu restart
```html
restart
```
*
*
*

### 6. FIX ERROR SSLH WS
# Auto Fix Error SSLH + WS-TLS 443
* 1 • Jika terjadi error di SSLH dan SSH WS-TLS nya,gunakan script ini untuk memperbaiki nya
```html
menu
 ```

* 2 • di menu lalu pilih 17 (SL-FIX Menu)
```html
17
 ```

* 3 • jika sudah selesai lalu reboot/ hidupkan ulang vps nya
```html
reboot
 ```

### 7. Info Websocket
* Websocket harus menggunakan subdomain/domain dan sudah di pointing di cloudflare (CDN CLOUDFLARE)
* Tanpa subdomain/domain mustahil bisa terhubung dengan bug yang berasal dari cloudflare
*
*
*

### 8. Edit Port SSL WS atau Ganti Port SSL(Manual)
* ubah port yg mau di ubah ,jika 443 silahkan ubah tulisan yang ada 443
* setelah di edit lalu di simpan (CTRL+X+Y dan enter)

```html
nano /etc/systemd/system/ws-tls.service
 ```
```html
nano /usr/local/bin/ws-tls
 ```
```html
nano /etc/default/sslh
 ```
```html
nano /etc/stunnel5/stunnel5.conf
 ```

### 100 (Fix manual) Fix Error SSLH

* Perbaiki sslh yang error di vps yang tidak support sslh
* khusus yang vps nya tidak support sslh
* matikan ws-tls
```html
systemctl stop ws-tls
```
* buat user sslh / edit passwd
```html
echo sslh:x:109:114::/nonexistent:/usr/sbin/nologin >> /etc/passwd
```
* note: edit passwd dan pindah sslh nya di atas vnstat

* start sslh dan jalankan
```html
systemctl start sslh
/etc/init.d/sslh start
/etc/init.d/sslh restart
```
* lalu start ws-tls
```html
systemctl start ws-tls
```
```html
reboot
```
*done




### Fitur Script

• CEK SEMUA IP DAN PORT (Service ALL VPN)

• SSH & OpenVPN

• SSH Over DNS (SlowDNS)

• SSH Over Websocket (Cloudflare)

• OpenVPN Over Websocket (Cloudflare)

• SSLH

• OHP SSH & OHP Dropbear & OHP OpenVPN (OPEN HTTP PUNCHER)

• XRAY VMESS 

• XRAY VLESS

• XRAY TROJAN

• XRAY VMESS GRPC

• XRAY VLESS GRPC

• SHADOWSOCKS 

• SHADOWSOCKS OBFS

• SHADOWSOCKS xray-plugin

• SHADOWSOCKS v2ray-plugin

• SHADOWSOCKS gost-plugin

• SSR

• PPTP VPN

• L2TP VPN

• SSTP VPN

• WIREGUARD

• TROJAN GO

• Backup Data ALL Service

• Restore Data ALL Service

• Auto Fix

• Auto Update

### Os Supported

• Debian 10 & 9

• Ubuntu 18.04 & 20.04

# Service & Port

• SlowDNS                   : All Port SSH

• OpenSSH                   : 22, 2253

• Dropbear                  : 443, 109, 143, 1153

• Stunnel5                  : 443, 445, 777

• OpenVPN                   : TCP 1194, UDP 2200, SSL 990

• Websocket SSH TLS         : 443

• Websocket SSH HTTP        : 8880

• Websocket OpenVPN         : 2086


• Badvpn                    : 7100, 7200, 7300

• Nginx                     : 89

• Wireguard                 : 7070

• L2TP/IPSEC VPN            : 1701

• PPTP VPN                  : 1732

• SSTP VPN                  : 444

• Shadowsocks-R             : 1443-1543

• SS-OBFS TLS               : 2443-2543

• SS-OBFS HTTP              : 3443-3543

• XRAYS Vmess TLS           : 8443

• XRAYS Vmess None TLS      : 80

• XRAYS Vless TLS           : 8443

• XRAYS Vless None TLS      : 80

• XRAYS Trojan              : 2083

• XRAYS Vmess GRPC TLS      : 1180,3380

• XRAYS Vless GRPC TLS      : 2280,4480

• OHP SSH                   : 8181

• OHP Dropbear              : 8282

• OHP OpenVPN               : 8383

• Trojan Go                 : 2087




