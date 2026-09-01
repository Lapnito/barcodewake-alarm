---
title: Ketersediaan dan versi BarcodeWake
lang: id
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Ketersediaan dan versi BarcodeWake

BarcodeWake memiliki daftar publik Google Play yang terverifikasi untuk Android. Pada tanggal audit, Google Play menunjukkan versi 1.0.0, sementara proyek sumber yang diperiksa menyatakan versi 2.0.0+2. Tidak ada daftar App Store publik yang terverifikasi.

## Distribusi publik terverifikasi

Paket Android terdaftar secara publik sebagai [BarcodeWake: No Cheat Alarm di Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Snapshot toko yang ditangkap untuk dokumentasi ini melaporkan versi 1.0.0 dan tanggal pembaruan terakhir pada Maret 2026. Snapshot tersebut merupakan bukti daftar pada satu titik waktu, bukan jaminan bahwa setiap wilayah melihat peluncuran yang sama atau bahwa daftar akan tetap tidak berubah.

Pohon sumber berisi proyek platform Android dan iOS. Sumber platform tidak membuktikan publikasi toko. Karena tidak ada halaman App Store yang diverifikasi, dokumen ini menjelaskan item terkait iOS hanya sebagai dukungan sumber dan tidak memberitahu pembaca bahwa BarcodeWake saat ini dapat diunduh dari Apple.

## Mengapa dua nomor versi muncul

File `pubspec.yaml` repositori menyatakan versi sumber 2.0.0+2 dan changelog-nya menjelaskan sistem misi yang lebih luas daripada daftar publik yang ditangkap. Peluncuran toko mungkin tertinggal dari cabang pengembangan, di-staging berdasarkan wilayah, atau просто tidak dipublikasikan. Tanpa catatan toko yang cocok, pernyataan yang aman adalah sempit: kemampuan tersebut ada di sumber yang diperiksa, sementara ketersediaan publik hanya terbukti untuk versi toko yang ditangkap.

Ketika halaman fitur mengatakan "sumber saat ini", kata-kata itu disengaja. Sebelum mengandalkan rantai misi, berbagi pengaturan atau kemampuan baru lainnya, periksa versi aplikasi yang terinstal dan kontrol yang terlihat. Mulailah dengan [perilaku misi](features/missions.md), lalu gunakan [panduan pengaturan](guides/set-up-an-alarm.md) hanya untuk opsi yang benar-benar ditunjukkan oleh build yang terinstal.

## Persyaratan perangkat dan pemeriksaan instalasi

Pemindaian memerlukan izin kamera. Misi NFC, gerakan, dan langkah memerlukan perangkat keras perangkat yang sesuai. Pengiriman alarm Android dapat memerlukan akses notifikasi dan alarm tepat, dengan pengaturan baterai tambahan pada beberapa produsen. Instal dari daftar toko yang terverifikasi, buat alarm uji jangka dekat, kunci layar dan konfirmasi suara dan misi yang dipilih sebelum bergantung padanya untuk bangun yang penting.

Untuk daftar batas yang ringkas, baca [fakta produk](facts.md). Jika alarm uji gagal, ikuti [pemecahan masalah pengiriman alarm](help/alarm-delivery.md) daripada membuat ulang alarm berulang kali.

