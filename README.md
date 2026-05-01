# 🏋️ U Gym Management System

Sistem manajemen gym berbasis web dengan arsitektur:
- **Front-end**: GitHub Pages (HTML/CSS/JS statis)
- **Back-end**: Google Apps Script (REST API)

## 📁 Struktur File

| File | Keterangan |
|------|------------|
| `index.html` | Dashboard utama & panel admin (login required) |
| `PublicRegistration.html` | Form pendaftaran member online (publik) |
| `PublicExtension.html` | Form perpanjangan membership (publik) |
| `code.gs` | Back-end Google Apps Script (tidak dihosting di sini) |

## 🔗 URL Penting

| Layanan | URL |
|---------|-----|
| 🌐 Website (GitHub Pages) | `https://[username].github.io/[repo-name]/` |
| 📝 Registrasi Member | `https://[username].github.io/[repo-name]/PublicRegistration.html` |
| 🔄 Perpanjangan | `https://[username].github.io/[repo-name]/PublicExtension.html?id=[MEMBER_ID]` |
| ⚙️ API Backend (GAS) | `https://script.google.com/macros/s/AKfycbzKWdekXY27eWx5h4CI7HvLxnTboVPryp_gTpqTtCNM-G7yqLe4m0owvj7YwGgTm8bv/exec` |

## 🚀 Cara Deploy

### Front-end (GitHub Pages)
1. Push semua file HTML ke repository ini
2. Pergi ke **Settings → Pages**
3. Pilih **Source: Deploy from a branch**
4. Pilih branch `main` dan folder `/` (root)
5. Klik **Save** — website akan aktif dalam beberapa menit

### Back-end (Google Apps Script)
1. Buka [script.google.com](https://script.google.com)
2. Buka project U Gym
3. Copy isi `code.gs` ke editor
4. Deploy: **Deploy → Manage Deployments → Edit → Deploy**

## 🏗️ Arsitektur

```
Browser (GitHub Pages)
    │
    │ fetch() POST request
    ▼
Google Apps Script (doPost)
    │
    │ SpreadsheetApp API
    ▼
Google Sheets (Database)
```

## 📞 Kontak

- **Email**: ugymindonesia@gmail.com
- **Telepon**: 08158905889
- **Alamat**: Jl. Imogiri Tim., Banguntapan, Bantul, DIY

---
© 2025 U Gym Management System
