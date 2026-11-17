# 🎬 AI Creative Studio

Buat video Shorts vertikal **9:16 (720×1280)** dari gambar + teks + narasi — langsung di browser, gratis, tanpa install, tanpa daftar.

👉 **Coba langsung:** https://malik2112.github.io/ai-creative-studio/

## Apa itu?

AI Creative Studio adalah studio mini untuk kreator video pendek:

1. **Proyek** — satu proyek = satu video. Kelola ide sampai video selesai.
2. **Bengkel AI** — 5 alat bantu: cari **Ide**, tulis **Naskah** per adegan, buat **Judul**, susun **Prompt Gambar**, dan **Prompt Video** (untuk Veo / Flow / Hailuo / Seedance / DomoAI).
3. **Galeri** — simpan gambar-gambarmu (hasil generate dari AI apa pun) di browser.
4. **Video** — rakit video 9:16 dari gambar + teks tiap adegan + narasi (unggah audio atau rekam dari mic), lengkap dengan efek zoom/pan halus. Hasilnya bisa diunduh (MP4/WebM).
5. **Panduan** — tutorial 7 langkah dari nol sampai video jadi.

## Cara memakai

**Paling gampang:** buka link GitHub Pages di atas dari HP atau laptop. Tidak perlu install apa pun.

**Atau dari source:**
```bash
git clone https://github.com/malik2112/ai-creative-studio.git
# buka file index.html di browser — selesai, tidak ada build step.
```

**Alur cepat (5 menit):**
1. Tab **Proyek** → buat proyek baru (atau "Muat proyek contoh" untuk coba-coba).
2. Tab **Bengkel AI** → pilih alat, isi topik, jalankan, salin hasilnya.
3. Generate gambar di alat AI favoritmu (Gemini, ChatGPT, Leonardo, dll.), lalu unggah ke tab **Galeri**.
4. Tab **Video** → klik gambar sesuai urutan adegan, isi teks tiap adegan, tambah narasi kalau mau, tekan **Rakit Video 9:16**.
5. Tonton preview, lalu **Download**.

## Yang jalan di sini vs versi asli

Versi ini adalah **versi publik mandiri** (satu file `index.html`, tanpa server). Dibangun ulang sebagai aplikasi statis dari AI Creative Studio asli yang berjalan di dalam Muse.

| Fitur | Di sini (GitHub Pages) | Di versi asli (Muse) |
|---|---|---|
| Manajemen proyek (buat/ubah/hapus) | ✅ Jalan penuh (localStorage) | ✅ |
| Bengkel AI: ide, naskah, judul, prompt gambar & video | ⚠️ Template pintar offline di browser — hasil disalin ke ChatGPT/Gemini/Claude | ✅ AI langsung di dalam aplikasi |
| Generate gambar AI di dalam aplikasi | ❌ Tidak ada — unggah gambarmu sendiri ke Galeri | ✅ Generate gratis di dalam aplikasi |
| Galeri gambar | ✅ Jalan penuh (IndexedDB) | ✅ |
| Rakit video 9:16 (gambar + teks + narasi) | ✅ Jalan penuh (canvas + MediaRecorder) | ✅ |
| Klip gerak AI sungguhan (Veo/Hailuo/dll.) | ❌ Dibuat di luar (prompt-nya dibantu Bengkel AI) | ❌ Sama — dibuat di luar via prompt-video |

**Kenapa begitu?** Generate gambar dan pemanggilan AI langsung memakai API runtime khusus Muse yang tidak tersedia di luar Muse. Semua yang murni browser (proyek, galeri, rakit video) jalan penuh di sini.

## Privasi

- Semua data (proyek, riwayat Bengkel AI, gambar galeri) tersimpan **hanya di browser perangkatmu** (localStorage + IndexedDB).
- Tidak ada server, tidak ada pelacakan, tidak ada API key, tidak ada data yang dikirim ke mana pun.
- Hapus data browser = data studio ikut terhapus. Ekspor penting? Simpan hasil (teks/naskah/video) dengan tombol Salin / Download.

## Tips

- **Satu adegan, satu subjek.** Jangan masukkan dua tokoh atau dua aksi dalam satu prompt gambar/video — hasilnya sering berantakan.
- **Cek preview sebelum download.** Pastikan teks tidak terpotong dan urutan gambar sudah benar.
- Video di dalam studio adalah gambar diam dengan efek zoom/pan — bukan gerak AI sungguhan. Untuk gerak beneran, buat klipnya di Flow/Hailuo/DomoAI, lalu gabungkan dengan hasil rakitan di sini (mis. di CapCut).

## Lisensi

MIT — bebas dipakai, diubah, dan dibagikan.
