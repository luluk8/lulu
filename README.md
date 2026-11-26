# Portofolio Lu'lu' Isnaini — Graphic Design Student

Portofolio satu halaman berisi karya Nirmana, Desain Baju, After Effects, Fotografi, dan pengalaman PKL. Dibuat dengan HTML + Tailwind CDN, tanpa proses build.

## Isi folder

| File | Fungsi |
|---|---|
| `index.html` | Halaman utama (wajib untuk GitHub Pages) |
| `favicon.svg` | Ikon tab browser |
| `*.jpeg` | Seluruh foto/profil/logo/karya (nama sudah aman untuk URL) |
| `.nojekyll` | Memberitahu GitHub Pages agar tidak memproses file lewat Jekyll |
| `.gitignore` | Mengabaikan file sistem operasi/editor |
| `DESIGN.md` | Catatan desain/portofolio |

## Menjalankan di lokal

Buka `index.html` langsung di browser, atau jalankan server statis:

```bash
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Upload ke GitHub

1. Buka folder ini di terminal:
   ```bash
   cd "Folder_luluk"
   ```
2. Inisialisasi repo dan upload:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/USERNAME/NAMA_REPO.git
   git push -u origin main
   ```
   Ganti `USERNAME` dan `NAMA_REPO` sesuai akun/repo Anda.

## Mengaktifkan GitHub Pages

1. Di GitHub, buka repo → **Settings** → **Pages**.
2. **Build and deployment** → Source: **Deploy from a branch**.
3. Branch: **main**, folder: **/(root)** → **Save**.
4. Tunggu beberapa menit. Situs tampil di:
   ```
   https://USERNAME.github.io/NAMA_REPO/
   ```

## Catatan

- Semua gambar bersifat lokal dan memakai path relatif, sehingga tetap bekerja di `github.io/<nama-repo>/`.
- Tailwind, Google Fonts, dan Material Symbols dimuat dari CDN — koneksi internet diperlukan saat halaman dibuka.
- Bagian Karya Saya dan galeri PKL menggunakan carousel geser + tombol panah; tinggi foto mengikuti rasio aslinya.
- Untuk mengganti foto, cukup timpa file dengan nama yang sama di folder ini.
