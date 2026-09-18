# Happy Birthday — Website (versi single-file)

Ini versi anti-gagal-deploy: seluruh CSS, JavaScript, dan foto sudah
digabung jadi **satu file** — `index.html`. Tidak ada lagi file `style.css`,
`script.js`, atau folder `photos/` yang terpisah, jadi tidak ada risiko
file "hilang" atau salah path waktu di-upload ke hosting.

## Kenapa ini dibuat

Kalau sebelumnya website tampil tanpa gaya sama sekali (font default,
semua bagian numpuk jadi satu, tidak ada kartu hitam) — itu karena file
`style.css` / `script.js` gagal termuat waktu di-deploy. Versi single-file
ini menghilangkan kemungkinan itu terjadi lagi.

## Cara deploy ulang (GitHub / Vercel / Netlify)

1. **Hapus dulu** file `index.html`, `style.css`, `script.js`, dan folder
   `photos/` yang lama dari repository/hosting kamu.
2. Upload file `index.html` yang baru ini (dan folder `music/` kalau kamu
   pakai musik latar) ke tempat yang sama.
3. Selesai — tidak perlu pengaturan tambahan apa pun.

## Kalau mau edit teks lagi

Karena sekarang semuanya ada di satu file, caranya sama seperti sebelumnya:
buka `index.html` di VS Code, cari kata **"Edit"** untuk placeholder yang
masih perlu diisi.

**Catatan:** karena foto sudah "ditanam" langsung ke dalam file HTML
(bukan file terpisah), kalau suatu saat mau ganti foto, kirim foto barunya
ke Claude lagi supaya bisa ditanam ulang — tidak bisa cuma diganti nama
filenya seperti versi sebelumnya.

## Musik latar

Tetap sama seperti sebelumnya: taruh file MP3 di folder `music/`, rename
jadi `song.mp3`.
