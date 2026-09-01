---
title: Terminologi BarcodeWake
lang: ms
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
# Terminologi BarcodeWake

BarcodeWake menggunakan “misi” untuk tindakan yang diperlukan untuk menutup alarm. Misi imbasan mengesahkan kod fizikal berdaftar; misi cabaran mengesahkan jawapan atau gerakan; perkongsian dan sandaran merujuk kepada format pertukaran yang berbeza.

## Istilah alarm dan misi

- Alarm: acara bangun terjadual yang termasuk masa, hari aktif, bunyi dan tetapan untuk menutup alarm.
- Misi: tugas yang perlu diselesaikan sebelum alarm boleh ditutup.
- Misi imbasan: tugas berdasarkan barcode, QR atau NFC yang sepadan dengan perwakilan kod berdaftar.
- Misi cabaran: tugas matematik, menaip, goncang atau langkah.
- Mod tunggal: satu misi yang dikonfigurasi dijalankan untuk alarm.
- Mod rantaian: misi yang dikonfigurasi dijalankan mengikut urutan yang dipilih.
- Mod rawak: satu misi dipilih daripada set yang dikonfigurasi.
- Kesukaran: tetapan misi yang mengubah keperluan tugas; kesannya yang tepat bergantung pada jenis misi.

## Istilah data dan kebolehpercayaan

- Kod berdaftar: barcode, kod QR atau tag NFC fizikal yang berkaitan dengan misi imbasan.
- Hash kod: perwakilan SHA-256 sehala yang digunakan oleh laluan penyimpanan dan pertukaran semasa untuk memadankan nilai berdaftar.
- Sandaran setempat: perwakilan yang dieksport bertujuan untuk mengekalkan atau memulihkan data aplikasi.
- QR persediaan: format perkongsian konfigurasi terhad yang tidak merangkumi kod berdaftar, pengenal NFC, PIN dan sejarah.
- Doktor Kebolehpercayaan: diagnostik dalam aplikasi untuk kebenaran dan tetapan sistem yang mungkin mengganggu penghantaran alarm.
- Akses alarm tepat: kebenaran atau dasar sistem Android yang membolehkan penjadualan yang kritikal masa.
- Pengoptimuman bateri: kawalan sistem operasi atau vendor yang mungkin menyekat pelaksanaan latar belakang.

Untuk hubungan ciri penuh, lihat [misi dan rentetan misi](features/missions.md). Untuk perbezaan antara format eksport, baca [sandaran dan perkongsian](guides/backup-and-sharing.md). Halaman [halaman fakta](facts.md) mentakrifkan apa yang aplikasi tidak mendakwa untuk mengukur.

