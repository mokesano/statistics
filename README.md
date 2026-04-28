# 📊 Statistics Plugin for OJS — *Archived Edition*

**Plugin visualisasi statistik berbasis grafik untuk Open Journal Systems (OJS) versi 2.4.3 hingga 2.4.8-1. Plugin ini membaca data dari tabel `METRICS` dan menyajikannya dalam bentuk grafik interaktif langsung dari dashboard editor.**

---

<p align="center">
  <img src="https://img.shields.io/badge/OJS-2.4.3%20--%202.4.8--1-21759B?style=for-the-badge&logo=open-access&logoColor=white" alt="OJS Version">
  <img src="https://img.shields.io/badge/PHP-5.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Version">
  <img src="https://img.shields.io/badge/status-archived-inactive?style=for-the-badge&logo=github" alt="Status">
  <img src="https://img.shields.io/badge/license-GPL%202.0-blue?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/last%20commit-2016-lightgrey?style=for-the-badge" alt="Last Commit">
</p>

<br>

> ⚠️ **Repositori ini telah di-arsipkan.** Tidak ada pengembangan, pembaruan, atau dukungan lebih lanjut. Plugin ini hanya kompatibel dengan **OJS 2.4.x** dan tidak akan berfungsi pada OJS 3.x ke atas.

---

## 📖 Latar Belakang

Plugin ini merupakan versi yang diperbarui dari plugin statistik lawas yang pertama kali dipublikasikan pada tahun 2013 di forum PKP. Tujuannya sederhana: memberikan visualisasi data statistik yang tersimpan di tabel `METRICS` OJS secara langsung di antarmuka editor, tanpa perlu menggunakan aplikasi analitik eksternal.

**Fork ini** dipertahankan oleh [mokesano](https://github.com/mokesano) sebagai cadangan dan referensi historis. Versi asli dikembangkan oleh **Fran Máñez** (Universitat Politècnica de Catalunya · BarcelonaTech).

---

## ⚙️ Kompatibilitas

| Komponen | Versi |
| :--- | :--- |
| **OJS** | 2.4.3, 2.4.4-0, 2.4.4-1, 2.4.5, 2.4.6, 2.4.7, 2.4.7-1, 2.4.8, 2.4.8-1 |
| **PHP** | 5.x |
| **Database** | MySQL (tabel `METRICS`) |

> ❌ **Tidak kompatibel dengan OJS 3.x** — arsitektur plugin dan struktur database telah berubah total.

---

## 📦 Instalasi

1. Unduh kode dari [repositori ini](https://github.com/mokesano/statistics).
2. Ganti nama folder menjadi `statistics/`.
3. Kompres folder menjadi `statistics.tar.gz`:
   ```bash
   tar -pczf statistics.tar.gz statistics/
   ```
4. Masuk ke OJS: **Home → User → Journal Management → Plugin Management → Install A New Plugin**.
5. Unggah file `statistics.tar.gz`.

---

## 🧩 Struktur Plugin

| Berkas | Fungsi |
| :--- | :--- |
| `index.php` | Entry point plugin |
| `StatisticsPlugin.inc.php` | Registrasi plugin ke OJS |
| `StatisticsHandler.inc.php` | Handler permintaan data statistik |
| `StatisticsChartsDAO.inc.php` | Akses data ke tabel `METRICS` |
| `index.tpl` | Template utama (Smarty) |
| `css/` | Stylesheet |
| `js/` | Grafik interaktif |
| `locale/` | Terjemahan |
| `version.xml` | Metadata plugin (v1.0.0.0) |

---

## 📄 Lisensi

**GNU General Public License v2.0** — sama dengan lisensi OJS itu sendiri.

---

## 🙏 Penghargaan

| 🏷️ Atribusi | 🔗 Referensi |
| :--- | :--- |
| **Pengembang Asli** | Fran Máñez — [fran.upc@gmail.com](mailto:fran.upc@gmail.com) |
| **Fork Maintainer** | [Rochmady (mokesano)](https://github.com/mokesano) |
| **Forum Asli** | [PKP Support Forum (2013)](https://pkp.sfu.ca/support/forum/viewtopic.php?f=28&t=10962) |
| **PKP Statistics Framework** | [pkp.sfu.ca](https://pkp.sfu.ca/wiki/index.php?title=PKP_Statistics_Framework) |

---

<p align="center">
  <br>
  <sub>Diarsipkan dengan ❤️ sebagai bagian dari sejarah pengembangan OJS</sub>
  <br><br>
  <sub>© 2016 Fran Máñez & Rochmady. Dilisensikan di bawah GPL‑2.0.</sub>
</p>