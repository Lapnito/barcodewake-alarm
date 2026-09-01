---
title: Misi dan rantai misi BarcodeWake
lang: ml
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

Misi BarcodeWake ialah syarat yang digunakan untuk mengabaikan penggera. Sumber semasa menyokong tugas kod bar, QR, matematik, menaip, goncang dan langkah, dengan NFC berdaftar dikendalikan melalui laluan imbasan kod. Misi boleh berjalan sendiri, secara berjujukan atau melalui pemilihan rawak.

## Misi imbasan mewujudkan jarak fizikal

Misi kod bar atau QR membandingkan imbasan kamera langsung dengan kod yang berdaftar semasa persediaan. Kod boleh diletakkan pada objek di luar jangkauan tangan: alatsolek di bilik mandi, item sarapan pagi di dapur, atau objek stabil lain di kawasan yang terang. NFC mengikuti idea umum yang sama dengan tag dan peranti yang serasi. Apl menyimpan reprezentasi hash dalam laluan semasa berbanding memerlukan kod mentah untuk perbandingan biasa.

Pilih objek yang masih tersedia apabila penggera berbunyi. Pembungkusan dibuang, label pudar dan perjalanan mengubah persekitaran. Mendaftarkan kod pada kotak ubat唯一 yang mungkin anda perlukan untuk menggantikan adalah kurang teguh berbanding menggunakan label yang tahan lama. [Panduan persediaan penggera](../guides/set-up-an-alarm.md) merangkumi penempatan dan pengujian.

## Misi cabaran menukar gerakan untuk usaha

Matematik dan menaip memerlukan input yang fokus. Goncang dan langkah memerlukan pergerakan fizikal dan sensor yang disokong. Tetapan kesukaran dan sasaran mengubah berapa banyak kerja yang dijangkakan, tetapi misi yang lebih sukar bukan automaticamente lebih baik. Geseran yang keterlaluan boleh menggalakkan melumpuhkan penggera sepenuhnya, manakala tugas yang mudah boleh menjadi automatik selepas ulangan.

Sesuaikan tugas dengan mod kegagalan. Jika anda matikan penggera separuh tidur, mengimbas di bilik lain mewujudkan jarak yang berguna. Jika akses kamera tidak mudah, tugas menaip atau matematik yang pendek mungkin lebih praktikal. Jika mobiliti, keseimbangan atau kebolehcapaian menjadi kebimbangan, elakkan misi berdasarkan gerakan dan pilih tugas yang boleh disempurnakan dengan selamat.

## Mod tunggal, rantai dan rawak

Mod tunggal meminta satu misi yang dikonfigurasi. Mod rantai menjalankan beberapa misi yang dikonfigurasi secara berurutan. Mod rawak memilih dari set yang dikonfigurasi, mengurangkan kemungkinan satu interaksi yang dihafal menjadi automatik. Mod ini terdapat dalam sumber yang diperiksa yang lebih baharu; [ketersediaan](../availability.md) menjelaskan mengapa itu tidak membuktikan ia sudah berada dalam setiap versi awam.

Sentiasa jalankan ujian jangka pendek selepas menukar mod, kebenaran atau objek berdaftar. Pastikan objek yang dipilih mudah dicapai dan berikan laluan pemulihan yang selamat. Untuk masalah penghidraran yang tidak berkaitan dengan penyempurnaan misi, gunakan [senarai semak kebolehpercayaan](../help/alarm-delivery.md).

