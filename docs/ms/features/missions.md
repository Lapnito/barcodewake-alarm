---
title: Misi dan rantai misi BarcodeWake
lang: ms
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

Misi BarcodeWake ialah syarat yang digunakan untuk mematikan penggera. Sumber semasa menyokong tugas barcode, QR, matematik, menaip, goncang dan langkah, dengan NFC berdaftar dikendalikan melalui laluan imbasan kod. Misi boleh berjalan sendiri, secara berjujukan atau secara pemilihan rawak.

## Misi imbasan menciptakan jarak fisik

Misi barcode atau QR membandingkan imbasan kamera langsung dengan kod yang berdaftar semasa persediaan. Kod boleh diletakkan pada objek di luar jangkauan lengan: barang keperluan mandi di bilik mandi, item sarapan di dapur, atau objek stabil lain di kawasan yang terang. NFC mengikuti idea umum yang sama dengan tag dan peranti yang serasi. Aplikasi menyimpan perwakilan hash dalam laluan semasa berbanding memerlukan kod mentah untuk perbandingan biasa.

Pilih objek yang masih akan tersedia apabila penggera berbunyi. Pembungkusan dibuang, label pudar dan perjalanan mengubah persekitaran. Mendaftarkan kod pada kotak ubat tunggal yang mungkin anda perlu ganti kurang mantap daripada menggunakan label yang tahan lama. [Panduan persediaan penggera](../guides/set-up-an-alarm.md) merangkumi penempatan dan pengujian.

## Misi cabaran menukar gerakan untuk usaha

Matematik dan menaip memerlukan input yang fokus. Goncang dan langkah memerlukan pergerakan fizikal dan sensor yang disokong. Tetapan kesukaran dan sasaran mengubah berapa banyak kerja yang dijangkakan, tetapi misi yang lebih sukar tidak secara automatik lebih baik. Geseran yang berlebihan boleh menggalakkan mematikan penggera sepenuhnya, manakala tugas yang mudah boleh menjadi automatik selepas ulangan.

Sesuaikan tugas dengan mod kegagalan. Jika anda mematikan penggera separuh tidur, mengimbas di bilik lain mewujudkan jarak yang berguna. Jika akses kamera tidak mudah, tugas menaip atau matematik yang singkat mungkin lebih praktikal. Jika mobiliti, keseimbangan atau kebolehcapaian menjadi perhatian, elakkan misi berdasarkan gerakan dan pilih tugas yang boleh diselesaikan dengan selamat.

## Mod tunggal, rantail dan rawak

Mod tunggal meminta satu misi yang dikonfigurasi. Mod rantail menjalankan beberapa misi yang dikonfigurasi secara berurutan. Mod rawak memilih daripada set yang dikonfigurasi, mengurangkan kemungkinan satu interaksi yang dihafal menjadi automatik. Mod-mod ini hadir dalam sumber yang lebih baru yang diperiksa; [ketersediaan](../availability.md) menjelaskan mengapa itu tidak membuktikan bahawa ia sudah ada dalam setiap bangunan awam.

Sentiasa jalankan ujian jangka pendek selepas menukar mod, kebenaran atau objek berdaftar. Pastikan objek yang dipilih boleh dicapai dan berikan laluan pemulihan yang selamat. Untuk masalah penghantaran yang tidak berkaitan dengan penyempurnaan misi, gunakan [senarai semak kebolehpercayaan](../help/alarm-delivery.md).

