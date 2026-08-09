# Cara Pakai Paket Ini

Isi zip ini:

```
0001-feat-analytics-completion-export.patch   # patch git, bisa di-apply langsung
modified-files/                               # versi final 4 file yang berubah
  ├── index.html
  ├── README.md
  ├── CHANGELOG.md
  └── PLAN.md
PR_DESCRIPTION.md                             # teks siap-tempel buat form Pull Request
CARA_PAKAI.md                                 # file ini
```

## Opsi A — Pakai patch (direkomendasikan, paling rapi)

Di dalam folder hasil clone fork kamu:

```bash
git checkout main
git pull origin main          # pastikan up to date sama upstream ZakieMe/Try-git
git checkout -b feat/analytics-completion-export
git apply --stat 0001-feat-analytics-completion-export.patch   # cek dulu isinya
git am 0001-feat-analytics-completion-export.patch             # apply + auto-commit
git push origin feat/analytics-completion-export
```

`git am` bakal langsung bikin commit dengan pesan Conventional Commits yang
sudah disiapkan, jadi kamu nggak perlu commit manual lagi.

## Opsi B — Copy manual file yang sudah jadi

Kalau `git am` gagal (misal karena `main` di fork kamu udah beda dari yang
dipakai buat bikin patch ini):

```bash
git checkout main
git pull origin main
git checkout -b feat/analytics-completion-export
cp /path/ke/modified-files/index.html .
cp /path/ke/modified-files/README.md .
cp /path/ke/modified-files/CHANGELOG.md .
cp /path/ke/modified-files/PLAN.md .
git add index.html README.md CHANGELOG.md PLAN.md
git commit -m "feat: tambah analytics panel kalkulasi completion % dan export JSON"
git push origin feat/analytics-completion-export
```

## Buka Pull Request

1. Buka fork kamu di GitHub, klik banner **"Compare & pull request"**.
2. Pastikan base repository `ZakieMe/Try-git` branch `main`, compare dari
   branch `feat/analytics-completion-export` di fork kamu.
3. Copy-paste isi `PR_DESCRIPTION.md` ke form deskripsi PR.
4. Submit.

## Sebelum submit, cek dulu

- Buka `index.html` lokal (`python3 -m http.server 8080`) dan lihat section
  achievement — pastikan progress bar & tombol Export JSON muncul dan jalan.
- Baca ulang `CONTRIBUTING.md` di repo asli kalau ada aturan tambahan yang
  belum sempat berubah sejak paket ini dibuat.
