---
title: Misi dan rantai misi BarcodeWake
lang: id
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---

# Misi dan rantai misi BarcodeWake

Misi BarcodeWake adalah kondisi yang digunakan untuk membatalkan alarm. Sumber saat ini mendukung tugas barcode, QR, matematika, pengetikan, goyangan, dan langkah, dengan NFC yang terdaftar ditangani melalui jalur pemindaian kode. Misi dapat dijalankan sendiri, secara berurutan, atau dengan pemilihan acak.

## Misi pindaian menciptakan jarak fisik

Misi barcode atau QR membandingkan pemindaian kamera langsung dengan kode yang terdaftar saat pengaturan. Kode dapat ditempatkan pada objek di luar jangkauan tangan: kebutuhan kamar mandi di kamar mandi, item sarapan di dapur, atau objek stabil lainnya di area yang terang. NFC mengikuti ide umum yang sama dengan tag dan perangkat yang kompatibel. Aplikasi menyimpan representasi hash di jalur saat ini alih-alih memerlukan kode mentah untuk perbandingan biasa.

Pilih objek yang akan tetap tersedia saat alarm berbunyi. Kemasan dibuang, label pudar, dan perjalanan mengubah lingkungan. Mendaftarkan kode pada kotak obat satu-satunya yang mungkin perlu Anda ganti kurang kuat dibandingkan menggunakan label yang tahan lama. [Panduan pengaturan alarm](../guides/set-up-an-alarm.md) mencakup penempatan dan pengujian.

## Misi tantangan menukar gerakan untuk usaha

Matematika dan pengetikan memerlukan input yang terfokus. Goyangan dan langkah memerlukan gerakan fisik serta sensor yang didukung. Pengaturan kesulitan dan target mengubah seberapa banyak pekerjaan yang diharapkan, tetapi misi yang lebih sulit tidak secara otomatis lebih baik. Gesekan berlebihan dapat mendorong untuk menonaktifkan alarm sepenuhnya, sementara tugas yang mudah dapat menjadi otomatis setelah pengulangan.

Sesuaikan tugas dengan mode kegagalan. Jika Anda mematikan alarm dalam keadaan setengah sadar, memindai di ruangan lain menciptakan jarak yang berguna. Jika akses kamera tidak nyaman, tugas pengetikan atau matematika singkat mungkin lebih praktis. Jika mobilitas, keseimbangan, atau aksesibilitas menjadi perhatian, hindari misi berbasis gerakan dan pilih tugas yang dapat diselesaikan dengan aman.

## Mode tunggal, rantai, dan acak

Mode tunggal meminta satu misi yang dikonfigurasi. Mode rantai menjalankan beberapa misi yang dikonfigurasi secara berurutan. Mode acak memilih dari kumpulan yang dikonfigurasi, mengurangi kemungkinan bahwa satu interaksi yang dihafalkan menjadi otomatis. Mode-mode ini ada di sumber yang lebih baru yang telah diperiksa; [ketersediaan](../availability.md) menjelaskan mengapa hal itu tidak membuktikan bahwa mereka sudah ada di setiap build publik.

Selalu jalankan tes jangka pendek setelah mengganti mode, izin, atau objek terdaftar. Jaga agar objek yang dipilih tetap dapat dijangkau dan sediakan rute pemulihan yang aman. Untuk masalah pengiriman yang tidak terkait dengan penyelesaian misi, gunakan [daftar periksa keandalan](../help/alarm-delivery.md).

