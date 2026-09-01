---
title: Istilah-istilah BarcodeWake
lang: id
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Istilah-istilah BarcodeWake

BarcodeWake menggunakan "mission" untuk tindakan yang diperlukan untuk menonaktifkan alarm. Mission pemindaian memverifikasi kode fisik yang terdaftar; mission tantangan memverifikasi jawaban atau gerakan; berbagi dan pencadangan merujuk pada format pertukaran yang berbeda.

## Istilah alarm dan mission

- Alarm: peristiwa bangun terjadwal dengan waktu, hari aktif, suara, dan konfigurasi penonaktifan.
- Mission: tugas yang harus diselesaikan sebelum penonaktifan.
- Mission pemindaian: tugas berbasis barcode, QR atau NFC yang dicocokkan dengan representasi kode yang terdaftar.
- Mission tantangan: tugas matematika, pengetikan, pengocokan, atau langkah.
- Mode tunggal: satu mission yang dikonfigurasi berjalan untuk alarm.
- Mode rantai: mission yang dikonfigurasi berjalan dalam urutan yang dipilih.
- Mode acak: satu mission dipilih dari kumpulan yang dikonfigurasi.
- Kesulitan: pengaturan mission yang mengubah tuntutan tugas; efek pastinya bergantung pada jenis mission.

## Istilah data dan keandalan

- Kode terdaftar: barcode fisik, kode QR, atau tag NFC yang terkait dengan mission pemindaian.
- Hash kode: representasi SHA-256 satu arah yang digunakan oleh jalur penyimpanan dan pertukaran saat ini untuk mencocokkan nilai terdaftar.
- Cadangan lokal: representasi yang diekspor yang dimaksudkan untuk préservation atau pemulihan data aplikasi.
- QR pengaturan: format berbagi konfigurasi terbatas yang menghilangkan kode terdaftar, pengenal NFC, PIN, dan riwayat.
- Dokter keandalan: diagnostik dalam aplikasi untuk izin dan pengaturan sistem yang dapat mengganggu pengiriman alarm.
- Akses alarm tepat: izin atau kebijakan sistem Android yang memungkinkan penjadwalan yang kritis terhadap waktu.
- Optimasi baterai: kontrol sistem operasi atau vendor yang dapat membatasi eksekusi latar belakang.

Untuk hubungan fitur lengkap, lihat [mission dan rantai mission](features/missions.md). Untuk perbedaan antara format ekspor, baca [pencadangan dan berbagi](guides/backup-and-sharing.md). [Halaman fakta](facts.md) mendefinisikan apa yang tidak diklaim oleh aplikasi untuk diukur.

