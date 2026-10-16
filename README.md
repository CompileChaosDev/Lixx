# MALIX AUTO SCRAPER (frontend)

Satu file statis (`index.html`), tanpa build. Isi: halaman Generator, History, Contact Owner.
Backend scraper belum ada, jadi analisis dan tes nyata belum berjalan.

## Isi kontak owner
Di `index.html`, cari `const OWNER={wa:"",tg:""};` lalu isi
`wa:"628123456789"` dan `tg:"usernameowner"` (sudah diisi tg: malix_raw).

## Baterai HP
Memakai Battery Status API. Jalan di Chrome/Edge Android lewat HTTPS (Vercel sudah HTTPS).
Tidak didukung di Safari iOS dan Firefox, di sana tampil "--%". Buka link Vercel di Chrome Android, jangan dari browser dalam aplikasi lain.

## Upload ke GitHub
1. Buat repo baru di github.com (misal `malix-auto-scraper`).
2. Add file > Upload files, upload `index.html`, `README.md`, `.gitignore`, lalu Commit.

## Deploy ke Vercel
1. vercel.com > Add New > Project > Import repo tadi.
2. Framework: Other. Build command dan Output directory dikosongkan. Klik Deploy.

## Cara update
Edit atau upload ulang `index.html` di repo GitHub (Add file > Upload files, timpa nama yang sama), lalu Commit.
Vercel otomatis deploy ulang dalam sekitar satu menit.
