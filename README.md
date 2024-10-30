# TugasLinuxServer_Hikmah

**Nama : Hikmah Maharani**

**Nim : 09011282328058**

**Kelas : SK3A**

---

# Protokol SSH
Secure Shell (SSH) adalah protokol jaringan yang memungkinkan pengguna untuk mengontrol dan mengakses perangkat atau sistem dari jarak jauh dengan aman. Protokol ini menggunakan enkripsi untuk menjaga keamanan data yang dikirim melalui jaringan, sehingga informasi sensitif seperti kata sandi, data konfigurasi, atau perintah tidak dapat diakses oleh pihak ketiga.

---

# Pembahasan 

**1. Unduh Ubuntu versi 24.04.1 LTS**

![Screenshot 2024-10-30 112358](https://github.com/user-attachments/assets/2b5c7f51-76ff-4919-8964-78ecc2cedc18)

**2. Install *ifconfig*. Proses ini memastikan ifconfig tersedia dan dapat digunakan untuk mengelola antarmuka jaringan pada Ubuntu Server.**

![Screenshot 2024-10-30 112827](https://github.com/user-attachments/assets/b7c4c2e3-a779-4d00-8718-bf7bb7e15403)


**3. Gunakan perintah *$ifconfig* untuk mengkonfigurasi IP address**

![Screenshot 2024-10-30 114039](https://github.com/user-attachments/assets/1fe8cc0a-66f0-4ec7-b928-74d2a460be07)


**4. Gunakan perintah *$ssh* untuk membuat koneksi Secure Shell (SSH) ke komputer atau server jarak jauh. Lalu gunakan *$apt install nmap*  untuk memerintahkan sistem mengunduh dan menginstal paket nmap dari repositori Ubuntu**

![Screenshot 2024-10-30 113439](https://github.com/user-attachments/assets/eec5daf2-eada-48a2-98a8-1277b17d4f5c)


**5. Perintah nmap ini digunakan untuk melakukan pemindaian jaringan pada alamat IP 10.8.136.25 untuk mengidentifikasi port yang terbuka dan layanan yang berjalan pada host tersebut**

![Screenshot 2024-10-30 114141](https://github.com/user-attachments/assets/47c97137-f9da-426e-befc-846c2731a196)


**6. Perintah ini digunakan untuk membuka sesi SSH ke server dengan alamat IP 10.8.136.25 menggunakan port 22. Pengguna yang digunakan adalah "hikmah"**

![Screenshot 2024-10-30 114254](https://github.com/user-attachments/assets/bcc9f482-c0ea-4f94-83e1-e508c9f49d1c)


**7. Perintah *$sudo su*  digunakan untuk beralih ke pengguna root. Perintah *$cp /etc/ssh/ssh_config /etc/ssh/ssh_config.backup* digunakana untuk menyalin file konfigurasi SSH untuk membuat cadangan dengan nama *ssh_config.backup*. Perintah *nano /etc/ssh/ssh* berguna untuk membuka editor teks nano untuk mengedit file konfigurasi SSH yang terletak di */etc/ssh/ssh*. Selanjutnya edit port 22 ke port 40 dan masukkan protocol 2**

![Screenshot 2024-10-30 114456](https://github.com/user-attachments/assets/76a036e6-e4e2-419f-9872-32f3ab770146)

![Screenshot 2024-10-30 114701](https://github.com/user-attachments/assets/b2df14cf-dea6-4b6f-84c1-3be25789301a)


**8. Perintah *$ufw allow 40/tcp* berguna untuk mengizinkan semua koneksi masuk ke port 40 menggunakan protokol TCP. Perintah *$ufw enable* digunakan untuk mengaktifkan firewall UFW dan membuatnya berjalan saat sistem dihidupkan ulang. perintah *$ufw status* digunakan untuk memeriksa status firewall UFW**

![Screenshot 2024-10-30 114955](https://github.com/user-attachments/assets/507729b3-1773-4a2c-8da7-56ad2d60e112)


**9. Perintah *$ss -tuln | grep ssh* digunakan untuk memantau status koneksi SSH pada sistem linux**

![Screenshot 2024-10-30 115126](https://github.com/user-attachments/assets/901854fa-9fda-4249-bde7-fd09c18d0beb)


**10. Perintah *$ssh -p 40 hikmah@10.8.136.25* digunakan untuk membuka sesi terminal jarak jauh ke server yang memiliki alamat IP 10.8.136.25 dan menggunakan port 40 untuk layanan SSH.**

![Screenshot 2024-10-30 115603](https://github.com/user-attachments/assets/bcb174ff-b8b5-48f3-9127-50a648272d5b)








