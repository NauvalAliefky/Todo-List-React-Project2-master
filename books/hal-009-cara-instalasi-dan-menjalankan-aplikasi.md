# Cara Instalasi dan Menjalankan Aplikasi

**Halaman 9** | **Bagian I** | React ToDo App — Buku Analisa Teknis

---

## Prasyarat Sistem

Sebelum menginstal React ToDo App, pastikan sistem Anda memenuhi prasyarat berikut. Node.js versi 14 atau lebih baru harus terinstal di komputer. NPM (Node Package Manager) yang biasanya sudah termasuk dalam instalasi Node.js juga diperlukan. Selain itu, koneksi internet diperlukan untuk mengunduh dependensi dan mengakses API dummy JSONPlaceholder pada penggunaan pertama.

## Langkah Instalasi

Proses instalasi dimulai dengan mengkloning repository dari GitHub menggunakan perintah git clone. Setelah repository berhasil di-clone, navigasikan ke direktori project dan jalankan perintah npm install untuk mengunduh seluruh dependensi yang terdaftar di package.json. Proses ini akan mengunduh React, React DOM, React Router DOM, amCharts, FontAwesome, React Toastify, dan dependensi lainnya.

## Menjalankan Aplikasi

Untuk menjalankan aplikasi dalam mode development, gunakan perintah npm start. Ini akan memulai development server pada port 3000 dan secara otomatis membuka browser di http://localhost:3000. Development server mendukung hot reloading, sehingga setiap perubahan kode akan langsung direfleksikan di browser tanpa perlu restart manual.

## Scripts yang Tersedia

Project ini menyediakan empat scripts utama melalui package.json. Script npm start untuk menjalankan development server. Script npm run build untuk membuat production build yang dioptimasi. Script npm test untuk menjalankan test runner. Script npm run eject untuk mengeluarkan konfigurasi Create React App (operasi satu arah yang tidak dapat dikembalikan).

## Build untuk Production

Untuk men-deploy aplikasi ke production, jalankan npm run build. Perintah ini akan menghasilkan folder build/ yang berisi file HTML, CSS, dan JavaScript yang sudah di-minify dan dioptimasi. Bundle production menggunakan hash pada filename untuk cache busting. Output build ini siap di-deploy ke platform hosting statis seperti Netlify, Vercel, atau GitHub Pages.

## Troubleshooting Umum

Beberapa masalah umum yang mungkin ditemui selama instalasi termasuk konflik versi Node.js, error npm install karena lockfile yang tidak kompatibel, dan masalah CORS saat mengakses API. Untuk mengatasi masalah versi Node.js, disarankan menggunakan nvm (Node Version Manager). Untuk masalah npm install, coba hapus node_modules dan package-lock.json lalu jalankan npm install kembali.

---
*Halaman 9 dari 270 — Buku Analisa Komprehensif React ToDo App*
