---
title: Privasi dan keandalan alarm BarcodeWake
lang: id
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# Privasi dan keandalan alarm BarcodeWake

BarcodeWake menyimpan konfigurasi alarm dan data misi yang terdokumentasi di perangkat dan tidak memerlukan akun aplikasi. Jalur kode saat ini melakukan hash nilai kode yang terdaftar. Telemetri opsional dijelaskan sebagai dinonaktifkan secara default, sementara pengiriman alarm masih bergantung pada izin sistem dan kontrol vendor.

## Data lokal tidak menghilangkan ketergantungan sistem

Penyimpanan lokal berarti pengaturan alarm biasa tidak memerlukan akun cloud BarcodeWake. Catatan alarm, riwayat, dan preferensi ditangani melalui lapisan data lokal aplikasi. Nilai barcode, QR, dan NFC yang terdaftar direpresentasikan dengan hash SHA-256 dalam penyimpanan dan jalur impor saat ini, yang menghindari penyimpanan nilai mentah biasa untuk pencocokan.

Hashing bukan sama dengan enkripsi setiap catatan aplikasi, dan penyimpanan lokal bukan merupakan cadangan. Seseorang yang memiliki akses ke perangkat yang tidak terkunci mungkin masih dapat melihat nama alarm, jadwal, atau riwayat melalui aplikasi. Ponsel yang hilang atau direset juga dapat kehilangan data lokal kecuali pengguna telah membuat ekspor. Lihat [cadangan dan berbagi](../guides/backup-and-sharing.md) untuk format dan tujuan masing‑masing.

Kebijakan privasi menyatakan bahwa telemetri opsional dimatikan secara default dan menjelaskan penanganan agregat jika diaktifkan. Oleh karena itu, dokumentasi ini tidak membuat klaim yang lebih luas bahwa aplikasi tidak dapat berkomunikasi melalui jaringan. Dokumen ini menyatakan fakta yang lebih sempit dan terverifikasi: operasi inti dan data bersifat lokal, tidak diperlukan akun produk, dan tidak ada ketergantungan SDK iklan yang muncul dalam proyek yang diperiksa.

## Keandalan adalah tanggung jawab bersama

BarcodeWake dapat menjadwalkan dan menampilkan alarm, tetapi sistem operasi memutuskan kapan pekerjaan latar belakang boleh berjalan dan gangguan mana yang diizinkan. Izin notifikasi, akses alarm tepat waktu, mode senyap atau fokus, optimalisasi baterai, penangguhan otomatis aplikasi, dan pembunuh tugas dari produsen semuanya dapat berpengaruh. Alat keandalan dalam aplikasi dapat mengidentifikasi risiko konfigurasi dan mengarahkan pengguna ke pengaturan; alat ini tidak dapat mengabaikan kebijakan sistem.

Setelah instalasi, uji dengan layar terkunci dan ponsel dalam mode daya yang sama dengan yang digunakan semalaman. Ulangi pengujian tersebut setelah pembaruan sistem, perubahan penghemat baterai, atau instalasi ulang aplikasi. Jaga perangkat tetap terisi daya, volume sesuai, dan misi yang dipilih tersedia secara fisik. Ikuti [pemecahan masalah pengiriman alarm](../help/alarm-delivery.md) ketika pengujian gagal.

## Apa yang tidak dijanjikan oleh privasi dan keandalan

BarcodeWake bukan perangkat medis, layanan peringatan darurat, atau pelacak tahap tidur. Tidak ada aplikasi alarm yang dapat menjamin bangun atau mengompensasi perangkat yang tidak tersedia. Halaman [fakta dan batasan](../facts.md) mencantumkan batasan‑batasan ini, sementara [ketersediaan](../availability.md) memisahkan bukti toko publik dari kemampuan sumber yang lebih baru.

