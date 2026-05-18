# Fitur-Fitur Utama Aplikasi

**Halaman 8** | **Bagian I** | React ToDo App — Buku Analisa Teknis

---

## Task Creation (Pembuatan Tugas)

Fitur pembuatan tugas memungkinkan pengguna membuat tugas baru dengan informasi lengkap. Pengguna dapat mengisi judul tugas, memilih tanggal dan waktu, menulis deskripsi detail, memilih kategori (Personal, Work, School, Events), dan mengaktifkan atau menonaktifkan alert. Proses pembuatan tugas dilakukan melalui modal form yang muncul saat pengguna menekan tombol plus di pojok kanan bawah halaman Tasks.

## Task Editing (Pengeditan Tugas)

Fitur pengeditan memungkinkan modifikasi seluruh atribut tugas yang sudah ada. Pengguna dapat mengubah judul, tanggal, waktu, deskripsi, kategori, dan status alert melalui form EditBox yang mirip dengan form pembuatan tugas. Perubahan disimpan ke localStorage dan state aplikasi diperbarui secara real-time, termasuk pembaruan tampilan Description jika sedang terbuka.

## Task Deletion (Penghapusan Tugas)

Penghapusan tugas dapat dilakukan melalui dua cara: melalui icon trash pada setiap item tugas di daftar, atau melalui tombol Delete pada halaman Description. Setelah penghapusan, data di localStorage diperbarui, state aplikasi di-refresh, dan notifikasi sukses ditampilkan menggunakan React Toastify.

## Search dan Filter

Sistem pencarian menggunakan regex untuk mencocokkan keyword dengan judul tugas secara case-insensitive. Selain pencarian, pengguna dapat memfilter tugas berdasarkan status (All, Pending, Completed) dan kategori (All, Personal, Work, School, Events). Ketiga mekanisme filter ini saling eksklusif untuk menghindari konflik.

## Dashboard Analytics

Dashboard menampilkan tiga kartu statistik (Total Tasks, Pending Tasks, Completed Tasks) dan pie chart interaktif yang menunjukkan proporsi tugas yang sudah selesai versus yang masih pending. Visualisasi ini menggunakan amCharts 5 dengan animasi dan layout yang responsif.

## Sistem Notifikasi

Aplikasi menggunakan React Toastify untuk menampilkan notifikasi toast. Notifikasi ditampilkan untuk berbagai aksi: berhasil membuat tugas, berhasil mengedit tugas, berhasil menghapus tugas, dan error saat fetching data dari API. Notifikasi menggunakan dua tipe: success (hijau) dan error (merah).

---
*Halaman 8 dari 270 — Buku Analisa Komprehensif React ToDo App*
