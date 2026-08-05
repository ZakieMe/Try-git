# Berkontribusi ke AchievementForge

Terima kasih sudah tertarik berkontribusi! Panduan ini menjelaskan cara berkontribusi secara nyata dan sehat ke repo ini.

## Alur Kerja

1. **Fork** repo ini ke akun GitHub kamu.
2. **Clone** hasil fork:
   ```bash
   git clone https://github.com/USERNAME_KAMU/Try-git.git
   cd Try-git
   ```
3. **Buat branch** baru dari `utama`/`main`:
   ```bash
   git checkout -b feat/deskripsi-singkat
   ```
4. **Lakukan perubahan.** Uji di browser lokal sebelum commit — buka `indeks.html` langsung atau jalankan `python3 -m http.server 8080`.
5. **Commit** menggunakan [Conventional Commits](https://www.conventionalcommits.org/):
   ```bash
   git commit -m "feat: tambah fitur pencarian repo di lookup"
   git commit -m "fix: perbaiki overflow canvas di layar kecil"
   git commit -m "docs: perbarui panduan instalasi"
   ```
6. **Push** dan buka **Pull Request** ke branch `utama`.

## Jenis Kontribusi yang Diterima

- Perbaikan bug nyata (layout rusak, fungsi error, dsb)
- Penambahan fitur yang benar-benar berguna bagi pengguna
- Perbaikan aksesibilitas (alt text, kontras warna, keyboard navigation)
- Perbaikan dokumentasi
- Optimasi performa

## Yang Tidak Diterima

- Perubahan kosmetik yang tidak jelas tujuannya semata untuk menambah jumlah commit/PR
- Kode yang menyalin tanpa modifikasi dari sumber lain tanpa atribusi
- Perubahan yang merusak fungsi yang sudah ada

## Standar Kode

- Vanilla HTML/CSS/JS saja jangan tambahkan framework atau dependency baru tanpa diskusi terlebih dahulu di issue.
- Gunakan custom property CSS yang sudah ada di `:root` (`--bg-0`, `--gold`, dst) daripada hardcode warna baru.
- Pastikan perubahan tetap responsif di mobile (breakpoint 768px dan 480px sudah ada).

Selamat berkontribusi! 
