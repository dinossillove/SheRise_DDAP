
```markdown
# 🚀 Panduan Kolaborasi Git & Struktur Proyek - SheRise

Halo Tim! Biar kodingan kita tetap rapi, sinkron, dan tidak ada duplikasi folder (terutama folder assets), yuk ikuti aturan main di bawah ini sebelum mulai ngoding halaman masing-masing.

---

## 📁 Struktur Folder Proyek
Semua file harus diletakkan sesuai strukturnya agar tidak merusak jalur (*path*) kodingan atau membuat gambar menjadi *broken link*:

```text
SheRise_DDAP/
├── assets/
│   └── images/          <-- 🔴 SEMUA FOTO/GAMBAR MASUK SINI! JANGAN BIKIN FOLDER BARU!
├── index.html           <-- Halaman Home
├── girls-spot.html      <-- Halaman Girls Spot
├── career-plan.html     <-- Halaman Career Plan
└── README.md            <-- Panduan ini

```

### 📸 Aturan Penamaan Aset Gambar

Biar rapi dan terstruktur, format penamaan file gambar disesuaikan dengan singkatan nama halaman:

* **Halaman Home:** `img_home_namagambar.png`
* **Halaman Girls Spot (GS):** `img_gs_namagambar.png`
* **Halaman Career Plan (CP):** `img_cp_namagambar.png`

---

## 🛠️ Alur Kerja Git (Wajib Diikuti!)

Setiap kali kamu mau mulai nambahin kodingan atau membuat halaman baru (Home, My Record, dll), ikuti 3 langkah wajib ini di terminal VS Code:

### 1. SEBELUM NGODING (Ambil Update Terbaru)

Pastikan laptop kamu mengambil kodingan paling baru yang sudah di-upload oleh anggota tim lain agar tidak terjadi *conflict*:

```bash
git pull origin main

```

*Setelah berhasil pull, baru silakan buat file HTML baru atau masukkan foto ke folder `assets/images/`.*

### 2. SETELAH SELESAI NGODING (Bungkus Perubahan)

Kalau halaman barumu sudah beres dan tampilannya sudah aman di browser lokal, bungkus perubahan tersebut:

```bash
git add .
git commit -m "feat: menambah halaman home dan aset gambarnya"

```

*(Silakan sesuaikan pesan di dalam tanda kutip dengan halaman atau fitur yang kamu kerjakan).*

### 3. TERBANGKAN KE GITHUB (Push)

Kirim hasil kerjamu ke repository GitHub agar anggota tim lain bisa mengambil update-nya:

```bash
git push origin main

```

---

## ⚠️ Aturan Emas (Golden Rules)

1. **Jangan membuat folder baru untuk aset.** Folder `assets/images/` sudah disiapkan untuk menampung seluruh gambar proyek kita.
2. **Gunakan FontAwesome.** Kita sudah memasang CDN FontAwesome di bagian `<head>` halaman, jadi kamu tinggal panggil class-nya saja jika butuh ikon (contoh: `<i class="fas fa-user"></i>`).
3. **Konfirmasi di grup.** Selalu kabari tim di grup chat setelah kamu melakukan `git push` agar yang lain bisa langsung melakukan `git pull`.

*Selamat ngoding, teman-teman! Mari kita selesaikan proyek SheRise ini dengan lancar dan kompak!* 🔥

```

---

### Cara Mengunggahnya ke GitHub lewat Terminal VS Code:
Setelah kamu *save* file `README.md` tersebut di VS Code, langsung jalankan perintah ini di terminalmu:

```bash
git add .
git commit -m "docs: menambahkan file README.md untuk panduan tim"
git push origin main

```

Begitu berhasil ter-*push*, coba buka halaman repository GitHub kalian di browser. Panduan di atas otomatis akan langsung muncul dengan visual yang rapi dan profesional di halaman utama bagian bawah! 🚀
