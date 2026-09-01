---
title: Fakta dan batasan BarcodeWake
lang: id
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Fakta dan batasan BarcodeWake

BarcodeWake menjadwalkan alarm dan memverifikasi misi dismissal yang dipilih. Aplikasi ini dapat menggunakan pemindaian, tantangan kognitif atau gerakan, menyimpan data inti yang didokumentasikan secara lokal, tidak memerlukan akun produk, dan tidak melakukan analisis tahap tidur.

## Fakta produk dalam sekilas

| Pertanyaan | Jawaban terverifikasi |
|---|---|
| Apa ini? | Jam alarm dengan misi dismissal fisik dan kognitif. |
| Misi apa yang ada di sumber saat ini? | Barcode, QR, matematika, mengetik, menggoyangkan dan langkah. NFC ditangani sebagai jalur kode terdaftar. |
| Apakah akun diperlukan? | Tidak ada akun atau alur masuk yang hadir untuk fitur yang didokumentasikan. |
| Di mana data disimpan? | Konfigurasi alarm, riwayat dan preferensi menggunakan penyimpanan lokal. Jalur kode saat ini menggunakan hash untuk nilai kode terdaftar. |
| Apakah ini pelacak tidur? | Tidak. Aplikasi ini menjadwalkan alarm dan memverifikasi misi; tidak mengklasifikasikan tahap tidur. |
| Apakah setiap fitur sumber dirilis secara publik? | Tidak didirikan. Versi toko dan sumber berbeda pada tanggal audit. |

## Batasan yang penting dalam praktik

Aplikasi alarm beroperasi di dalam batasan tingkat telepon. Izin notifikasi, akses alarm tepat waktu, pengaturan fokus, optimalisasi baterai dan kontrol latar belakang khusus vendor dapat memengaruhi apakah alarm tiba seperti yang diharapkan. BarcodeWake menyertakan pemeriksaan reliabilitas dan panduan, tetapi aplikasi tidak dapat mengabaikan setiap batasan sistem operasi atau produsen. Uji alarm setelah instalasi dan setelah perubahan sistem utama; [daftar periksa pengiriman](help/alarm-delivery.md) menjelaskan caranya.

Hardware misi juga penting. Pemindaian memerlukan akses kamera dan kode fisik yang dapat dibaca. Misi goyangan dan langkah bergantung pada sensor yang relevan. NFC memerlukan hardware yang kompatibel. Label yang disalin atau rusak dapat mencegah pencocokan, jadi jaga jalur pemulihan dan jangan buat objek terdaftar satu-satunya tidak dapat diakses.

## Klaim yang secara sengaja tidak dibuat

Halaman-halaman ini tidak mengklaim manfaat medis, bangun terjamin, waktu siklus tidur, sinkronisasi cloud atau rilis iOS publik yang terverifikasi. Halaman-halaman ini juga tidak memperlakukan versi sumber sebagai versi toko langsung. Lihat [ketersediaan](availability.md) untuk perbedaan tersebut dan [privasi dan reliabilitas](features/privacy-and-reliability.md) untuk bukti di balik penyimpanan lokal dan wording telemetri.

