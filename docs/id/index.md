---
title: Dokumentasi BarcodeWake
lang: id
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---

# Dokumentasi BarcodeWake

BarcodeWake adalah jam alarm yang membuat pembatalan menjadi tindakan yang disengaja. Alarm dapat memerlukan barcode atau kode QR yang tersimpan, tugas kognitif singkat, urutan gelengan, atau target langkah, bukan hanya bergantung pada tombol di layar yang mudah.

## Apa yang membuat BarcodeWake berbeda

Ide utamanya adalah jarak ditambah niat. Jika kode yang terdaftar melekat pada objek yang jauh dari tempat tidur, membungkam alarm berarti bangun, menjangkau objek tersebut dan memindainya. Model alarm yang sama juga dapat menggunakan misi matematika, pengetikan, gelengan, atau langkah. Kode sumber saat ini mendukung satu misi, rantai berurutan, atau pemilihan acak dari misi yang dikonfigurasi.

Hambatan ini berguna bagi orang yang membatalkan alarm biasa tanpa menjadi sepenuhnya sadar. Ini bukan analisis tahap tidur, panduan medis, atau jaminan bahwa seseorang akan bangun. Dukungan perangkat keras, izin, dan kontrol baterai vendor masih mempengaruhi pengiriman. [referensi misi](features/missions.md) menjelaskan pilihan tersebut, sementara [pemecahan masalah pengiriman alarm](help/alarm-delivery.md) mencakup pengaturan sistem yang dapat mengganggu.

## Mulai dengan dokumen yang tepat

Gunakan [panduan pengaturan](guides/set-up-an-alarm.md) saat membuat alarm dan mendaftarkan kode fisik. Bacalah [cadangan dan berbagi](guides/backup-and-sharing.md) sebelum memindahkan data atau mengirim QR pengaturan ke orang lain. Format berbagi secara sengaja mengecualikan kode terdaftar, pengenal NFC, PIN, dan riwayat alarm, sehingga penerima harus menyelesaikan penyiapan sensitif secara lokal.

Untuk ringkasan singkat yang dapat diaudit, lihat [fakta produk](facts.md). Untuk status rilis, gunakan [ketersediaan](availability.md): versi Google Play publik yang ditangkap untuk audit ini berbeda dari versi yang dinyatakan oleh pohon sumber yang diperiksa. Oleh karena itu, versi sumber yang lebih baru didokumentasikan sebagai kemampuan sumber, bukan dinyatakan sebagai rilis toko yang dipublikasikan.

## Batasan privasi dan keandalan

Konfigurasi inti dan data misi disimpan di perangkat, dan tidak diperlukan akun BarcodeWake. Jalur kode saat ini mewakili nilai kode terdaftar dengan hash SHA-256. Telemetri opsional dijelaskan oleh kebijakan privasi sebagai dinonaktifkan secara default. Pernyataan tersebut tidak berarti setiap telepon akan mengirimkan alarm dengan cara yang sama; vendor Android dan izin sistem operasi masih dapat membatasi perilaku latar belakang.

Baca [privasi dan keandalan](features/privacy-and-reliability.md) untuk membedakan antara penanganan data lokal dan pengiriman oleh sistem operasi. [Perbandingan alarm standar](comparisons/standard-alarm.md) membantu memutuskan apakah pembatalan berbasis misi sesuai dengan cara Anda bangun.

