# 🍽️ RecipeMind AI

**RecipeMind AI** adalah aplikasi web berbasis kecerdasan buatan yang membantu pengguna menemukan resep makanan dan minuman secara interaktif melalui antarmuka chat. Aplikasi ini mendukung berbagai kategori resep — dari masakan nasional Indonesia, minuman tradisional, hidangan internasional, hingga dessert — lengkap dengan estimasi harga bahan-bahan dan fitur unduh PDF.

---

## 👥 Anggota Kelompok

| NIM | Nama |
|-----|------|
| 23051204325 | — |
| 23051204338 | — |
| 23051204349 | — |
| 23051204352 | — |

> **Kelompok 3 — TI J 2023**

---

## ✨ Fitur Utama

- 🔐 **Autentikasi Pengguna** — Sistem login & registrasi yang aman menggunakan Supabase sebagai backend, dengan password yang di-hash menggunakan SHA-256.
- 🤖 **AI Chatbot Resep** — Terhubung langsung ke OpenAI GPT-3.5-turbo untuk memberikan resep yang akurat dan terstruktur.
- 🗂️ **6 Mode Resep** — Pengguna dapat beralih antara mode:
  - Makanan Nasional (Indonesia)
  - Minuman Nasional (Indonesia)
  - Makanan Internasional
  - Minuman Internasional
  - Dessert
  - Mode General
- 💰 **Estimasi Harga Bahan** — Setiap resep disertai estimasi harga bahan-bahan secara otomatis sesuai harga pasar.
- 📥 **Download PDF** — Resep dan estimasi harga dapat diunduh dalam format PDF (powered by jsPDF).
- 💬 **Manajemen Riwayat Chat** — Pengguna dapat membuat sesi chat baru kapan saja.
- 🎨 **Loading Screen Animasi** — Tampilan loading screen yang menarik saat pertama kali membuka aplikasi.

---

## 🛠️ Teknologi yang Digunakan

| Teknologi | Kegunaan |
|-----------|----------|
| **HTML5** | Struktur halaman web |
| **CSS3** | Tampilan & animasi UI |
| **JavaScript (Vanilla)** | Logika aplikasi & interaksi |
| **[Supabase](https://supabase.com/)** | Backend autentikasi & database pengguna |
| **[OpenAI API](https://platform.openai.com/)** | Generasi resep oleh AI (GPT-3.5-turbo) |
| **[jsPDF](https://cdnjs.cloudflare.com/ajax/libs/jspdf/)** | Generate & download file PDF |
| **[Font Awesome 6](https://fontawesome.com/)** | Ikon UI |
| **[Google Fonts – Poppins](https://fonts.google.com/)** | Tipografi |

---

## 📁 Struktur Proyek

```
📦 RecipeMind/
├── Index.html          # Halaman login & registrasi
├── chat.html           # Halaman utama aplikasi chat AI
├── css/
│   ├── style.css       # Stylesheet untuk halaman login/register
│   └── chat.css        # Stylesheet untuk halaman chat
└── js/
    ├── script.js       # Logika autentikasi (login, register, loading screen)
    └── chatAI.js       # Logika AI chat, mode resep, PDF download
```

---

## 🚀 Cara Menjalankan

Karena proyek ini berbasis HTML/CSS/JS murni (tanpa framework), cara menjalankannya sangat sederhana:

### Persyaratan
- Browser modern (Chrome, Firefox, Edge, dll.)
- Koneksi internet (diperlukan untuk OpenAI API & Supabase)

### Langkah-langkah

1. **Clone atau unduh** repositori ini:
   ```bash
   git clone https://github.com/<username>/<repo-name>.git
   ```

2. **Buka file** `Index.html` langsung di browser, atau gunakan ekstensi **Live Server** di VS Code untuk hasil terbaik.

3. **Daftar akun** terlebih dahulu, lalu **login** untuk mengakses halaman chat.

> ⚠️ Jika ingin menggunakan API Key sendiri, ganti nilai `API_KEY` di `js/chatAI.js` dan konfigurasi Supabase di `js/script.js`.

---

## 🖥️ Tampilan Aplikasi

| Halaman | Deskripsi |
|---------|-----------|
| **Loading Screen** | Animasi loading bar sebelum masuk ke aplikasi |
| **Login / Register** | Form autentikasi dengan validasi real-time |
| **Chat AI** | Antarmuka chat dengan sidebar mode resep |

---

## ⚙️ Konfigurasi

### Supabase (Database & Auth)
Di file `js/script.js`, sesuaikan nilai berikut dengan project Supabase Anda:
```js
const supabaseUrl = 'YOUR_SUPABASE_URL';
const supabaseKey = 'YOUR_SUPABASE_ANON_KEY';
```

### OpenAI API
Di file `js/chatAI.js`, sesuaikan nilai berikut:
```js
const API_CONFIG = {
    API_KEY: 'YOUR_OPENAI_API_KEY',
    MODEL: 'gpt-3.5-turbo',
    API_URL: 'https://api.openai.com/v1/chat/completions'
};
```

---

## 📄 Dokumen

- 📎 [Spesifikasi Kebutuhan Perangkat Lunak (SKPL)](./Spesifikasi%20Kebutuhan%20Perangkat%20Lunak.pdf)

---

## 📝 Lisensi

Proyek ini dibuat untuk keperluan **tugas akademik** Semester 4 — Program Studi Teknik Informatika.

---

<p align="center">
  Made with ❤️ by Kelompok 3 TI J 2023
</p>
