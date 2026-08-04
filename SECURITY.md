# Kebijakan Keamanan

## Melaporkan Kerentanan

Jika kamu menemukan kerentanan keamanan di proyek ini (misalnya XSS lewat input pada fitur GitHub Live Lookup, atau eksposur data sensitif), silakan laporkan melalui:

- Buka [issue baru](../../issues/new) dengan label `security`, **tanpa** menyertakan detail eksploitasi secara publik jika kerentanannya kritis.
- Atau hubungi maintainer langsung lewat profil GitHub [@Jouqio](https://github.com/Jouqio).

## Cakupan

Proyek ini adalah situs statis (HTML/CSS/JS) tanpa backend sendiri. Satu-satunya komunikasi jaringan yang dilakukan adalah permintaan `fetch()` langsung dari browser pengguna ke `api.github.com` (data publik, tanpa autentikasi, tanpa menyimpan data pengguna di server mana pun).

## Praktik yang Diterapkan

- Semua input pengguna (username GitHub di fitur Live Lookup) di-escape otomatis lewat `textContent`/atribut DOM standar, bukan `innerHTML` langsung dari input pengguna.
- Tidak ada API key atau kredensial yang disimpan di kode sisi klien.
- Tautan eksternal menggunakan `rel="noopener noreferrer"`.
