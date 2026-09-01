---
title: Mengapa Alarm BarcodeWake Mungkin Tidak Berbunyi
lang: id
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Mengapa Alarm BarcodeWake Mungkin Tidak Berbunyi

Alarm yang disimpan masih dapat diblokir oleh pengaturan notifikasi, akses alarm tepat waktu, mode fokus atau senyap, volume rendah, pembatasan baterai, penangguhan aplikasi, atau kontrol latar belakang vendor. Periksa pengiriman secara terpisah dari pemindaian misi, lalu jalankan tes layar terkunci.

## Pisahkan pengiriman dari pembatalan

Buat alarm uji coba jangka pendek dengan misi sederhana dan biarkan aplikasi tetap di latar belakang. Kunci layar. Jika tidak ada layar alarm atau suara yang muncul, masalahnya adalah pengiriman; mengubah barcode yang terdaftar tidak akan memperbaikinya. Jika alarm muncul tetapi misi tidak dapat diselesaikan, pengiriman berfungsi dan masalahnya adalah kamera, sensor, pencocokan kode, atau konfigurasi misi.

Pastikan alarm diaktifkan, hari yang dijadwalkan benar dan zona waktu telepon sesuai dengan jadwal yang dimaksud. Periksa volume media dan alarm alih-alih hanya mengandalkan status tombol samping. Tinjau aturan jangan ganggu atau fokus, perangkat audio yang terhubung, dan apakah telepon telah dimulai ulang setelah alarm dibuat.

## Tinjau izin sistem operasi

Izinkan notifikasi dan akses alarm tepat waktu atau alarm layar penuh apa pun yang diminta oleh build yang diinstal. Hapus BarcodeWake dari optimasi baterai yang agresif atau daftar tidur otomatis saat vendor perangkat menyediakan kontrol tersebut. Buka diagnostik keandalan dalam aplikasi dan ikuti pengaturan khusus perangkat yang diidentifikasinya. Halaman [halaman privasi dan keandalan](../features/privacy-and-reliability.md) menjelaskan mengapa ketergantungan sistem ini tetap ada meskipun data aplikasi bersifat lokal.

Setelah mengubah satu pengaturan, ulangi tes layar terkunci. Mengubah beberapa kontrol sekaligus membuat penyebab lebih sulit diidentifikasi. Pembaruan sistem dapat mereset atau menafsirkan ulang izin, jadi lakukan pengujian ulang setelah pembaruan besar atau instal ulang aplikasi.

## Diagnosa penyelesaian misi secara terpisah

Untuk misi barcode dan QR, bersihkan lensa kamera, perbaiki pencahayaan dan pastikan objek yang terdaftar tidak berubah. Berikan izin kamera. Untuk NFC, verifikasi dukungan perangkat dan tahan tag di dekat posisi antena yang benar. Misi goyang dan langkah bergantung pada sensor gerak atau langkah dan mungkin berperilaku berbeda ketika mode hemat daya membatasi pengiriman sensor.

Jika misi dikonfigurasi sebagai bagian dari rangkaian, setiap langkah yang diperlukan harus diselesaikan. Tinjau [perilaku misi](../features/missions.md) dan, jika perlu, buat tes baru menggunakan [prosedur pengaturan](../guides/set-up-an-alarm.md).

## Ketahui ketika telepon menjadi batas

BarcodeWake tidak dapat mengabaikan perangkat yang mati, baterai yang habis, perangkat keras audio yang rusak, atau setiap pembunuh tugas dari produsen. Ini bukan layanan notifikasi darurat. Pertahankan metode alarm lain untuk situasi dengan konsekuensi tinggi dan laporkan kegagalan yang dapat direproduksi dengan model perangkat, versi sistem, versi aplikasi, dan kondisi uji yang tepat.

