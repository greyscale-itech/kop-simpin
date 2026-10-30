# Koperasi Kosfa

Aplikasi web untuk memantau debitur, kreditur, dan cash flow koperasi simpan pinjam. Tampilan mobile-first dengan tema biru-hijau.

## Fitur

- Login dengan email dan kata sandi, plus biometrik (sidik jari / Face ID)
- **Home:** ringkasan piutang, status debitur, grafik cash flow
- **Debitur:** daftar peminjam, pencarian, filter status, detail pinjaman
- **Cash flow:** kas masuk dan keluar per bulan, tambah dana masuk manual
- **Admin:** tambah debitur, dashboard kreditur, pengaturan akun

## Cara pakai

Tinggal buka `index.html` di browser. Nggak perlu install apa pun.

## Upload ke GitHub

**Lewat website (paling gampang)**
1. Buat repository baru di github.com.
2. Klik **Add file > Upload files**, lalu tarik semua isi folder ini.
3. Klik **Commit changes**.

**Lewat terminal**
```bash
cd koperasi-kosfa
git init
git add .
git commit -m "Versi pertama Koperasi Kosfa"
git branch -M main
git remote add origin https://github.com/USERNAME/NAMA-REPO.git
git push -u origin main
```

## Aktifkan GitHub Pages (biar online)

1. Buka repo, lalu **Settings > Pages**.
2. Di bagian **Source**, pilih **Deploy from a branch**.
3. Pilih branch `main` dan folder `/ (root)`, lalu **Save**.
4. Tunggu 1 sampai 2 menit. Alamatnya jadi `https://USERNAME.github.io/NAMA-REPO/`.

Biometrik butuh HTTPS, jadi aktifkan dari alamat GitHub Pages tadi, bukan dari file yang dibuka langsung.

## Catatan penting

- Login dan semua data **tersimpan di browser** (localStorage) masing-masing perangkat. Belum ada server atau database, jadi data nggak otomatis sinkron antar perangkat.
- Akun di sini hanya pengaman tampilan. Untuk dipakai bersama dengan data anggota yang sungguhan, sambungkan ke backend dengan autentikasi, misalnya Supabase atau Firebase.
- Lupa kata sandi: pakai tautan "Reset akun" di halaman login (hanya menghapus akun di perangkat itu).

## Struktur folder

```
koperasi-kosfa/
├── index.html   # seluruh aplikasi (satu file)
├── README.md
├── .gitignore
└── .nojekyll
```

Developed by Fajar Q.
