---
title: Sandaran dan kongsi penggera BarcodeWake dengan selamat
lang: ms
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Sandaran dan kongsi penggera BarcodeWake dengan selamat

Gunakan eksport JSON apabila menyimpan atau memindahkan data aplikasi anda sendiri, kod bar sandaran PDF yang boleh cetak untuk pemulihan, dan perkongsian QR persediaan apabila orang lain hanya memerlukan struktur penggera. Perkongsian sengaja tidak termasuk rahsia berdaftar dan sejarah.

## Pilih format untuk tugas

Sumber semasa menyediakan laluan pertukaran yang berbeza kerana sandaran dan perkongsian bukan operasi yang sama. Sandaran JSON bertujuan untuk pemindahan dan pemulihan data berstruktur. Sandaran PDF menukar bahan pemulihan kepada dokumen kod bar yang boleh dicetak. QR persediaan sengaja lebih sempit: ia boleh menghantar konfigurasi penggera terhad tanpa membawa nilai kod berdaftar, pengenalpasti NFC, PIN atau sejarah.

Jangan layan QR persediaan sebagai sandaran peranti lengkap. Penerima mesti mendaftar kod fizikal mereka sendiri dan menyemak kebenaran secara tempatan. Perkongsian persediaan semasa juga mengehadkan berapa banyak penggera yang dibawa, jadi sahkan hasil yang diimport dan jangan anggap setiap jadual berjaya dipindahkan. [Fakta produk](../facts.md) merekodkan sempadan ini.

## Buat dan lindungi sandaran peribadi

Gunakan tindakan eksport yang tersedia dalam bangunan pasang, pilih JSON atau sandaran yang boleh cetak mengikut pelan pemulihan, dan simpan hasilnya di tempat yang anda kawal. Sandaran mungkin mendedahkan nama penggera, jadual dan konfigurasi lain walaupun nilai kod mentah berdaftar dilindungi atau ditinggalkan. kendalnya seperti data rutin peribadi: elakkan pautan awam, pencetak berkongsi dan saluran pesanan yang tidak dipercayai.

Selepas mengeksport, sahkan bahawa fail boleh dijumpai dan cap masanya sepadan dengan sandaran yang dimaksudkan. Jangan padam data aplikasi asal semata-mata kerana perintah eksport melaporkan kejayaan. Ujian pemulihan adalah semakan tunggal yang dipercayai, tetapi lakukan pada peranti yang selamat atau selepas membuat salinan kedua supaya ujian itu sendiri tidak menjadi peristiwa kehilangan.

## Kongsi persediaan tanpa kongsi rahsia

Jana QR persediaan hanya untuk penggera yang perlu diterima penerima. Penerima mengimbasnya, menyemak jadual yang diimport dan menyediakan kod, tag NFC atau butiran pemulihan mereka sendiri. Reka bentuk ini mengelakkan konfigurasi berkongsi daripada senyap memindahkan kunci fizikal yang mengabaikan penggera orang lain.

Selepas import, setiap orang harus menjalankan [uji kaji persediaan penggera](set-up-an-alarm.md) penuh. Kebenaran, sensor dan sekatan sistem operasi tidak dipindahkan dalam QR. Jika penggera yang diimport gagal muncul semasa dikunci, ikut [hara pembrekak penggera](../help/alarm-delivery.md).

Sumber dan versi simpanan berbeza semasa audit ini, jadi bangunan awam yang dipasang mungkin tidak mendedahkan setiap pilihan pertukaran yang diterangkan di sini. [Ketersediaan](../availability.md) menjelaskan cara mentafsir keupayaan sumber sahaja.

