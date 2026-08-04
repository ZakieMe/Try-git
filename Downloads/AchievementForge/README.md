# ⚒️ AchievementForge

<div align="center">

![AchievementForge Banner](https://img.shields.io/badge/AchievementForge-GitHub%20Achievement%20Tracker-f59e0b?style=for-the-badge&logo=github&logoColor=white)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LISENSI)
[![GitHub Stars](https://img.shields.io/github/stars/Jouqio/Try-git?style=flat-square&color=f59e0b)](../../stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Jouqio/Try-git?style=flat-square&color=3fb950)](../../network/members)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)

**Dashboard pelacak achievement GitHub — dibangun dengan HTML, CSS, dan JavaScript murni, lengkap dengan pencarian statistik profil GitHub secara live.**

[🔥 Live Demo](https://jouqio.github.io/Try-git/indeks.html) · [📘 Belajar DOM](Pelajaran_manipulasi_dom_js.html) · [🐛 Lapor Bug](../../issues/new)

</div>

---

## 📋 Daftar Isi

- [Tentang](#-tentang)
- [Fitur](#-fitur)
- [Struktur Proyek](#-struktur-proyek)
- [Cara Menjalankan](#-cara-menjalankan)
- [Cara Berkontribusi (PR)](#-cara-berkontribusi-pr)
- [Deployment](#-deployment)
- [Roadmap](#-roadmap)
- [Lisensi](#-lisensi)

---

## 🔥 Tentang

**AchievementForge** adalah dashboard open source untuk melacak achievement GitHub, dibangun dengan HTML5, CSS3, dan Vanilla JavaScript — tanpa framework, tanpa dependency, tanpa build step.

Repo ini juga menjadi tempat latihan workflow Git & GitHub yang sesungguhnya: fork, branch, commit, dan pull request nyata dengan perubahan kode yang genuinely berguna.

---

## ✨ Fitur

- 🏆 **Achievement Showcase** — 11 achievement GitHub dengan strategi resmi untuk meraihnya
- 🔍 **GitHub Live Lookup** — cari username GitHub apa pun dan tarik data publik langsung dari GitHub REST API (repo, followers, following, total star)
- 🌙 **Dark / Light Mode** — transisi tema halus dengan persistensi `localStorage`
- ✨ **Animasi Partikel Canvas** — animasi hero interaktif
- 📱 **Fully Responsive** — mobile, tablet, dan desktop
- ⚡ **Zero Dependencies** — tidak butuh build tool
- 🔍 **Filter Achievement** — earned / in progress / available / legacy
- 📅 **Timeline & Roadmap** — riwayat dan rencana pengembangan
- 📘 **Modul Belajar DOM** — halaman interaktif belajar DOM manipulation, terintegrasi ke navigasi utama

---

## 📁 Struktur Proyek

```
Try-git/
├── indeks.html                         # Dashboard utama (self-contained)
├── Pelajaran_manipulasi_dom_js.html    # Modul belajar DOM manipulation
├── README.md                           # File ini
├── CONTRIBUTING.md                     # Panduan kontribusi
├── CHANGELOG.md                        # Riwayat versi
├── KEAMANAN.md                         # Kebijakan keamanan
├── LISENSI                             # Lisensi MIT
├── PLAN.md                             # Catatan rencana pengembangan
└── .github/
    ├── workflows/deploy.yml            # Auto-deploy ke GitHub Pages
    ├── ISSUE_TEMPLATE/
    │   └── bug_report.md
    └── PULL_REQUEST_TEMPLATE.md
```

---

## 🚀 Cara Menjalankan

Cukup browser modern — tidak perlu Node.js, npm, atau build tool.

```bash
git clone https://github.com/Jouqio/Try-git.git
cd Try-git
open indeks.html
# atau jalankan local server:
python3 -m http.server 8080
```

---

## 🤝 Cara Berkontribusi (PR)

```bash
# 1. Fork repo ini, lalu clone hasil fork kamu
git clone https://github.com/USERNAME_KAMU/Try-git.git
cd Try-git

# 2. Buat branch baru
git checkout -b feat/nama-fitur-kamu

# 3. Lakukan perubahan nyata di indeks.html / Pelajaran_manipulasi_dom_js.html

# 4. Commit pakai Conventional Commits
git commit -m "feat: tambah fitur X"

# 5. Push dan buka Pull Request
git push origin feat/nama-fitur-kamu
```

Lihat [CONTRIBUTING.md](CONTRIBUTING.md) untuk panduan lengkap.

---

## 🌐 Deployment

### GitHub Pages
1. Buka **Settings → Pages**
2. Source: **Deploy from a branch** → `main` / `(root)`
3. Situs otomatis live di `https://jouqio.github.io/Try-git/indeks.html`

Workflow otomatis di `.github/workflows/deploy.yml` sudah disediakan untuk deploy via GitHub Actions.

---

## 🗺️ Roadmap

| Fase | Judul | Status |
|------|-------|--------|
| 01 | Foundation — struktur repo & dokumentasi | ✅ Selesai |
| 02 | Dashboard — UI, dark mode, responsive | ✅ Selesai |
| 02.5 | GitHub Live Lookup — integrasi REST API | ✅ Selesai |
| 03 | Community — Discussions, kontributor | 🔄 Berjalan |
| 04 | Analytics — data live lanjutan | 📅 Rencana |
| 05 | Explorer — strategy hub, quiz | 📅 Rencana |

---

## 📄 Lisensi

Didistribusikan di bawah **Lisensi MIT**. Lihat [LISENSI](LISENSI) untuk detail.

---

<div align="center">

Dibuat untuk latihan Git & pengembangan web oleh **Jouqio**

**[⬆ Kembali ke atas](#️-achievementforge)**

</div>
