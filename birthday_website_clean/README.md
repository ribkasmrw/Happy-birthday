# 🎂 Birthday Website — Cara Menjalankan

## Struktur Folder
```
birthday_website/
├── app.py               ← Backend Python (Flask)
├── requirements.txt     ← Daftar library
├── templates/
│   └── index.html       ← Tampilan website
└── static/
    └── uploads/         ← Folder untuk foto & video (otomatis dibuat)
```

---

## 🛠️ Langkah-langkah

### 1. Install Python
Pastikan Python 3.8+ sudah terinstall.  
Download: https://www.python.org/downloads/

### 2. Buka folder di VS Code
```
File → Open Folder → pilih folder birthday_website
```

### 3. Buka Terminal di VS Code
```
Terminal → New Terminal   (atau Ctrl+`)
```

### 4. Install library yang dibutuhkan
```bash
pip install -r requirements.txt
```

### 5. Jalankan website
```bash
python app.py
```

### 6. Buka di browser
```
http://localhost:5000
```

---

## ✏️ Cara Kustomisasi

Buka file `app.py`, cari bagian `CONFIG` di baris atas:

```python
CONFIG = {
    "nama_pacar": "Cinta",       # ← Ganti nama pacarmu
    "nama_pengirim": "Sayangmu", # ← Ganti namamu
    "tanggal_ultah": "12 Mei",   # ← Ganti tanggal ultahnya
    "pesan_utama": "...",        # ← Pesan singkat di hero
    "pesan_panjang": "...",      # ← Pesan panjang/surat cinta
}
```

Simpan → refresh browser → selesai! 🎉

---

## 🌐 Biar Bisa Diakses Pacar dari HP/Laptop Lain

1. Pastikan HP/laptop pacar dan laptopmu terhubung **WiFi yang sama**
2. Cari IP laptopmu:
   - Windows: buka CMD → ketik `ipconfig` → lihat "IPv4 Address" (contoh: 192.168.1.5)
   - Mac/Linux: `ifconfig` atau `ip addr`
3. Pacarmu buka browser dan ketik:
   ```
   http://192.168.1.5:5000
   ```
   (ganti dengan IP laptopmu)

---

## 🖼️ Cara Menambahkan Foto & Video

Taruh file foto/video langsung ke folder `static/uploads/`:
```
birthday_website/
└── static/
    └── uploads/
        ├── foto1.jpg
        ├── foto2.png
        └── video1.mp4
```
Refresh browser → foto/video langsung tampil di gallery! 🎉

Format yang didukung: PNG, JPG, JPEG, GIF, WEBP, MP4, MOV, AVI, MKV, WEBM

---

## 💡 Tips
- Klik foto/video untuk memperbesar (lightbox)
- Urutkan foto sesuai urutan nama file (contoh: `01_foto.jpg`, `02_foto.jpg`)
