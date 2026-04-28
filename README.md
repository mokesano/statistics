# 📊 Statistics Plugin for OJS — *Archived Edition*

**A graph-based statistics visualization plugin for Open Journal Systems (OJS) version 2.4.3 to 2.4.8-1. It reads data from the `METRICS` table and presents interactive charts directly on the editor's dashboard.**

---

<p align="center">
  <img src="https://img.shields.io/badge/OJS-2.4.3%20--%202.4.8--1-21759B?style=for-the-badge&logo=open-access&logoColor=white" alt="OJS Version">
  <img src="https://img.shields.io/badge/PHP-5.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP Version">
  <img src="https://img.shields.io/badge/status-archived-inactive?style=for-the-badge&logo=github" alt="Status">
  <img src="https://img.shields.io/badge/license-GPL%202.0-blue?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/badge/last%20commit-2016-lightgrey?style=for-the-badge" alt="Last Commit">
</p>

<br>

> ⚠️ **This repository has been archived.** There will be no further development, updates, or support. This plugin is only compatible with **OJS 2.4.x** and will not work on OJS 3.x or later.

---

## 📖 Background

This plugin is an updated version of an older statistics plugin first published in 2013 on the PKP forum. Its goal is simple: to visualize the statistical data stored in the OJS `METRICS` table directly within the editor interface, without requiring external analytics tools.

**This fork** is maintained by [mokesano](https://github.com/mokesano) as a backup and historical reference. The original version was developed by **Fran Máñez** (Universitat Politècnica de Catalunya · BarcelonaTech).

---

## ⚙️ Compatibility

| Component | Version |
| :--- | :--- |
| **OJS** | 2.4.3, 2.4.4-0, 2.4.4-1, 2.4.5, 2.4.6, 2.4.7, 2.4.7-1, 2.4.8, 2.4.8-1 |
| **PHP** | 5.x |
| **Database** | MySQL (table `METRICS`) |

> ❌ **Not compatible with OJS 3.x** — the plugin architecture and database structure have completely changed.

---

## 📦 Installation

1. Download the code from [this repository](https://github.com/mokesano/statistics).
2. Rename the folder to `statistics/`.
3. Compress the folder into `statistics.tar.gz`:
   ```bash
   tar -pczf statistics.tar.gz statistics/
   ```
4. Go to OJS: **Home → User → Journal Management → Plugin Management → Install A New Plugin**.
5. Upload the `statistics.tar.gz` file.

---

## 🧩 Plugin Structure

| File | Function |
| :--- | :--- |
| `index.php` | Plugin entry point |
| `StatisticsPlugin.inc.php` | Plugin registration to OJS |
| `StatisticsHandler.inc.php` | Handles statistics data requests |
| `StatisticsChartsDAO.inc.php` | Data access to `METRICS` table |
| `index.tpl` | Main template (Smarty) |
| `css/` | Stylesheets |
| `js/` | Interactive charts |
| `locale/` | Translations |
| `version.xml` | Plugin metadata (v1.0.0.0) |

---

## 📄 License

**GNU General Public License v2.0** — same as the OJS license.

---

## 🙏 Acknowledgments

| 🏷️ Attribution | 🔗 Reference |
| :--- | :--- |
| **Original Developer** | Fran Máñez — [fran.upc@gmail.com](mailto:fran.upc@gmail.com) |
| **Fork Maintainer** | [Rochmady (mokesano)](https://github.com/mokesano) |
| **Original Forum** | [PKP Support Forum (2013)](https://pkp.sfu.ca/support/forum/viewtopic.php?f=28&t=10962) |
| **PKP Statistics Framework** | [pkp.sfu.ca](https://pkp.sfu.ca/wiki/index.php?title=PKP_Statistics_Framework) |

---

<p align="center">
  <br>
  <sub>Archived with ❤️ as part of OJS development history</sub>
  <br><br>
  <sub>© 2016 Fran Máñez & Rochmady. Licensed under GPL‑2.0.</sub>
</p>