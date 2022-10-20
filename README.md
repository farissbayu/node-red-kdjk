# Node-Red
<h1 align="center"><img src="https://upload.wikimedia.org/wikipedia/commons/2/2b/Node-red-icon.png"></h1>

# Sekilas Tentang
Node-RED adalah alat pemrograman untuk menghubungkan perangkat keras, API, dan layanan online dengan cara baru dan menarik. Aplikasi ini menyediakan editor berbasis browser yang memudahkan untuk menyatukan aliran menggunakan berbagai node dalam palet yang dapat digunakan untuk runtime dalam satu klik.

# Instalasi
### Requirement
- Node.js versi 8.x atau lebih

### Instalasi via CLI
1. Untuk menjaga agar semua paket Anda tetap mutakhir/terbaru di Debian atau distribusi Linux berbasis Debian
   ```
   $ sudo apt update
   ```
   mengambil versi terbaru dari daftar paket dari repositori perangkat lunak distro Anda, dan setiap repositori pihak ketiga yang mungkin telah Anda konfigurasikan.
   ```
   $ sudo apt upgrade
   ```
   Mengunduh dan menginstal pembaruan untuk setiap paket usang dan ketergantungan pada sistem Anda.
2. Menginstall nodejs:
   ```
   $ curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
   $ sudo apt install nodejs
   $ node --version
   $ npm --version
   ```
3. Menginstall aplikasin Node-RED menggunakan npm:
   ```
   $ sudo npm install -g --unsafe-perm node-red
   $ node-red
   ```
4. Mengecek IP public VPS:
   ```
   $ dig +short myip.opendns.com @resolver1.opendns.com
   ```
5. Mengizinkan port 1880 melalui firewall:
   ```
   $ sudo ufw allow 1880
   $ sudo ufw enable
   $ sudo ufw status
   ```
6. Menginstall pm2 agar aplikasi dapat berjalan di background:
   ```
   $ npm install pm2 -g
   $ pm2 start node-red
   $ pm2 list
   ```

# Cara Pemakaian
1. Buka ip address dari node-red yang sudah di deploy pada VPS
   ```
   Ip Address: 103.187.146.3
   Port number: 1880
   Link: 103.187.146.3:1880
   ```
   
2. Tampilan awal atau menu utama node-red
   - Bagian samping kiri, terdapat node yang dapat digunakan untuk membuat sebuah flow pemrograman
   - Bagian kanan akan menampilkan informasi dari flow yang sudah kita buat
   - Bagian tengah adalah tempat untuk membuat flow
   <h3><img src="https://lh6.googleusercontent.com/KUWFJFOqcFz7Fi5Roo1v3aVRpfoUuw7R5UXt9B9H88Pjp8tKlv5lfP4Xxy2-KPy-B_qjXDS6ldoZ3sm4T-dcSER1qPehzCTQ6ms5U6ZXlIwlhcGWmW2tsSqj8kl0J9R51P7wVSNK907yZSHGasgGqcMPym4vlODQKQv5P5kD70Pyj2ZiwpUD4x5REA"></h3>

3. Untuk menampilkan hasil flow yang sudah dibuat, memerlukan plugin atau palette tambahan yaitu node-red-dashboard. Palette tambahan bisa diinstal melalui button pada pojok kanan atas dan klik manage palette. Kemudian cari node-red-dashboard pada bagian install
   <h3><img src="https://lh4.googleusercontent.com/IFCkcAcfnOqSKmFUPlj61vBvLIBOvni4tLnKTzhPo1jwae4ZFOJaX5dlNhTLQccsyg_ScZaJkNai7t3qX72E06I4Km-ATiCd4BxW8ROQjR7shGnSR4_m9BvTpW-kqsxDjl2lR4jYZAnnVf9oAbB7vI2D8nWPNPyeL462bG8nuZOwaBo4g-PmTbNuzg"></h3>

4. 
