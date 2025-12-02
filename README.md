# 📊 Attendance Converter - Bank Sulselbar

Aplikasi web untuk mengkonversi data absensi detail harian menjadi laporan summary bulanan.

## 🚀 Demo

[Live Demo di Netlify](https://your-app-name.netlify.app)

## ✨ Fitur

- ✅ Upload file Excel (.xls/.xlsx) drag & drop
- ✅ Konversi otomatis detail → summary
- ✅ Preview hasil sebelum download
- ✅ Export ke Excel (.xlsx)
- ✅ Responsive design
- ✅ Tidak perlu backend/server

## 📋 Mapping Data

| Data Input (Detail) | Proses | Data Output (Summary) |
|---------------------|--------|----------------------|
| Attendance Code = "H" | COUNT | Hadir |
| Attendance Code = "A" | COUNT | Alpha |
| Attendance Code = "S" | COUNT | Sakit |
| Attendance Code = "C" | COUNT | Leave/Cuti |
| Attendance Code = "LIBUR" | COUNT | Libur |
| Late In > 0 | COUNT & SUM | Late In (number) & Late In (hours) |
| Fast Out > 0 | COUNT | Fast Out |
| Overtime Hour | SUM | Lembur |

## 🛠️ Cara Deploy

### Deploy ke Netlify

1. Fork/clone repository ini
2. Login ke [Netlify](https://netlify.com)
3. Klik "Add new site" → "Import an existing project"
4. Pilih repository dari GitHub
5. Settings:
   - Build command: (kosongkan)
   - Publish directory: `.` atau `/`
6. Klik "Deploy site"

### Deploy ke GitHub Pages

1. Fork repository ini
2. Pergi ke Settings → Pages
3. Source: Deploy from a branch
4. Branch: `main` / `master`, folder: `/ (root)`
5. Klik Save

## 📁 Struktur File

```
attendance-converter/
├── index.html      # Aplikasi utama (single file)
├── README.md       # Dokumentasi
└── netlify.toml    # Konfigurasi Netlify (opsional)
```

## 💻 Cara Penggunaan

1. Buka aplikasi di browser
2. Upload file Excel dari sistem attendance (format detail harian)
3. Klik tombol "Convert ke Summary"
4. Preview hasil konversi
5. Download file Excel hasil konversi

## 🔧 Teknologi

- HTML5 + CSS3 + JavaScript (Vanilla)
- [SheetJS](https://sheetjs.com/) - Library untuk membaca/menulis Excel

## 📝 Format Input yang Didukung

File Excel dengan kolom:
- Employee Code
- Employee Name
- Organization Unit Name
- Position Code
- Position Name
- Date
- Time In / Time Out
- Attendance Code (H, A, S, C, LIBUR, dll)
- Late In
- Fast Out
- Overtime Hour
- Is Holiday

## 👨‍💻 Developer

Strategic Initiative Management Office (SIMO)  
Change Management Office - Bank Sulselbar

---

© 2025 Bank Sulselbar
