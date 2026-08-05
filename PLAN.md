# AchievementForge — Rencana Pengembangan

> Catatan: versi PLAN.md ini sudah direvisi. Bagian sebelumnya berisi strategi "farming" achievement pakai dua akun (PR tanpa review sungguhan, merge tanpa proses review, dsb) sengaja dihapus — praktik itu berisiko dianggap manipulasi sistem GitHub dan bisa merugikan kredibilitas repo di mata recruiter atau kontributor lain. Fokus rencana ini sekarang murni pada pengembangan produk dan kontribusi yang genuine.

---

##  Struktur Repository

```
Try-git/
├── indeks.html
├── Pelajaran_manipulasi_dom_js.html
├── .github/
│   ├── ISSUE_TEMPLATE/bug_report.md
│   ├── PULL_REQUEST_TEMPLATE.md
│   └── workflows/deploy.yml
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── KEAMANAN.md
├── LISENSI
└── PLAN.md
```

---

## 🗺️ Roadmap

### Fase 1 — Foundation ✅
- Struktur repo, README, lisensi MIT, template issue/PR.

### Fase 2 — Dashboard ✅
- Hero + animasi partikel, grid achievement, filter tab, dark/light mode, timeline, roadmap.

### Fase 2.5 — GitHub Live Lookup ✅
- Integrasi GitHub REST API: cari username, tampilkan repos/followers/following/total star secara real-time.

### Fase 3 — Community 🔄
- [ ] Aktifkan GitHub Discussions
- [ ] Tambah label `good first issue` untuk kontributor baru
- [ ] Contributor spotlight di README

### Fase 4 — Analytics 📅
- [ ] Contribution calendar widget (data dari GitHub API)
- [ ] Export data achievement ke JSON
- [ ] Kalkulasi persentase completion

### Fase 5 — Explorer 
- [ ] Hub strategi achievement (artikel per achievement)
- [ ] Quiz "achievement apa yang cocok untukmu"
- [ ] Public REST API untuk data achievement

---

##  Prinsip Kontribusi

Setiap PR harus berisi perubahan **nyata** perbaikan bug, fitur baru yang berguna, perbaikan dokumentasi, atau peningkatan aksesibilitas. Review dilakukan sungguh-sungguh sebelum merge. Ini menjaga riwayat commit tetap kredibel dan benar-benar mencerminkan kemampuan development.

##  Konvensi Commit
Proyek ini mengikuti [Conventional Commits](https://www.conventionalcommits.org/):

```
feat:     fitur baru
fix:      perbaikan bug
docs:     perubahan dokumentasi
style:    perubahan format/CSS (tanpa perubahan logika)
refactor: restrukturisasi kode (tanpa fitur/fix baru)
chore:    proses build, update dependency
perf:     peningkatan performa
ci:       perubahan konfigurasi CI/CD
```

---

*AchievementForge dibangun untuk belajar Git dan web development secara nyata.*
