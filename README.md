# VPN-OpenSource-Firezone

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Firezone](https://img.shields.io/badge/Firezone-FF5A5F?style=for-the-badge&logo=firezone&logoColor=white)

Repositori ini berisi panduan dan konfigurasi untuk menjalankan Firezone VPN menggunakan Docker. Firezone adalah solusi open-source untuk membangun jaringan privat virtual (VPN) berbasis WireGuard yang mudah digunakan dan aman. Dengan Docker, Anda dapat dengan cepat mengatur dan menjalankan Firezone di lingkungan produksi atau pengembangan.


## Fitur Utama
- **Mudah Digunakan**: Konfigurasi minimal dengan Docker.
- **Skalabilitas**: Cocok untuk lingkungan pengembangan maupun produksi.
- **Keamanan**: Menggunakan protokol WireGuard untuk koneksi yang aman.
- **Open Source**: Semua kode dan konfigurasi tersedia secara bebas.

## Prasyarat
Sebelum memulai, pastikan Anda telah menginstal:
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Cara Menggunakan

### 1. Clone Repositori
```bash
git clone https://github.com/zaklabs/VPN-OpenSource-Firezone.git
cd vpn-opensource-firezone
```

### 2. Penyesuaian enviroment/lingkungan server
Salin file **.env.example** menjadi **.env** dan sesuaikan variabel lingkungan sesuai kebutuhan Anda:
```bash
cp .env.example .env
```

### 3. Jalankan Container
Gunakan **Docker Compose** untuk memulai layanan Firezone:
```bash
docker-compose up -d
```

### 4. Akses Dashboard Admin
Setelah container berjalan, Anda dapat mengakses dashboard admin Firezone sesuai dengan subdomain yang anda tentukan. sesuai dengan bawaan repo ini anda dapat melakukan akses menggunakan **ip-server:8189**. Anda juga dapat menggunakan sub domain sesuai keinginan anda (silahkan bisa create issue).

### 5. Menambahkan Pengguna
Untuk menambahkan pengguna baru, Anda dapat menggunakan dashboard admin atau CLI Firezone.


## Lisensi
Proyek ini dilisensikan di bawah MIT License .


## Kontribusi
Kontribusi sangat diterima! Jika Anda memiliki ide atau perbaikan, silakan buat pull request atau issue.


## Referensi
* [Firezone Documentation](https://www.firezone.dev/docs)
* [WireGuard Official Site](https://www.wireguard.com/)
* [Docker Documentation](https://docs.docker.com/)
