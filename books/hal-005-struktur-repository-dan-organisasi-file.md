# Struktur Repository dan Organisasi File

**Halaman 5** | **Bagian I** | React ToDo App — Buku Analisa Teknis

---

## Overview Struktur

Repository React ToDo App mengikuti struktur standar Create React App dengan beberapa modifikasi dan penambahan. Root directory berisi file-file konfigurasi utama seperti package.json, .gitignore, dan _redirects untuk Netlify deployment. Source code aplikasi terorganisir dalam folder src/ dengan pemisahan yang jelas antara komponen, assets, dan konfigurasi global.

## Direktori Utama

Repository terdiri dari beberapa direktori utama. Folder public/ berisi file statis termasuk index.html, favicon.ico, manifest.json, dan robots.txt. Folder src/ berisi seluruh kode sumber aplikasi. Di dalam src/, terdapat folder components/ yang berisi semua komponen React, dan folder assets/ yang berisi gambar dan SVG icons yang digunakan dalam aplikasi.

## Hierarki Komponen

Folder src/components/ diorganisir berdasarkan fitur atau halaman. Terdapat empat folder utama: About/ untuk halaman tentang aplikasi, DashboardPage/ untuk halaman dashboard dan manajemen tugas, Footer/ untuk komponen footer, dan Home/ untuk halaman beranda. Setiap folder komponen mengikuti pola yang konsisten dengan file index.jsx sebagai komponen utama dan file .styles.css sebagai stylesheet terpisah.

## Organisasi DashboardPage

DashboardPage/ merupakan folder terbesar dan terkompleks, mencerminkan fakta bahwa dashboard adalah fitur utama aplikasi. Di dalamnya terdapat subfolder DashNav/ untuk navigation bar dashboard, DashboardContainer/ untuk konten dashboard dan pie chart, TasksContainer/ untuk manajemen tugas, dan UserAccount/ untuk profil pengguna. TasksContainer/ sendiri memiliki subfolder tambahan: AddTaskBox/, EditBox/, Description/, dan Task/.

## File Konfigurasi Root

Di root directory, package.json mendefinisikan metadata project, dependensi, dan scripts. File .gitignore mengecualikan node_modules, build output, dan file environment lokal. File _redirects berisi konfigurasi redirect untuk Netlify yang mengarahkan semua request ke index.html untuk mendukung client-side routing. File generate_docs.js merupakan script utilitas untuk generasi dokumentasi.

## Konvensi Penamaan

Project menggunakan konvensi penamaan yang konsisten: komponen React menggunakan PascalCase untuk nama folder dan file JSX, stylesheet menggunakan pola NamaKomponen.styles.css, dan file entry point setiap komponen diberi nama index.jsx. Konvensi ini memudahkan navigasi dan maintenance kode.

---
*Halaman 5 dari 270 — Buku Analisa Komprehensif React ToDo App*
