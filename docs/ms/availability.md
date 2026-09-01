---
title: Ketersediaan dan versi BarcodeWake
lang: ms
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

BarcodeWake mempunyai senarai awam Google Play yang disahkan untuk Android. Pada tarikh audit, Google Play menunjukkan versi 1.0.0, manakala projek sumber yang diperiksa mengisytiharkan versi 2.0.0+2. Tiada senarai App Store awam yang disahkan.

## Agihan awam yang disahkan

Pakej Android disenaraikan secara awam sebagai [BarcodeWake: No Cheat Alarm on Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Gambar skrin kedai yang ditangkap untuk dokumentasi ini melaporkan versi 1.0.0 dan tarikh kemas kini terakhir pada Mac 2026. Gambar skrin itu adalah bukti senarai pada satu masa, bukan janji bahawa setiap rantau melihat pengeluaran yang sama atau bahawa senarai akan kekal tidak berubah.

Pokok sumber mengandungi projek platform Android dan iOS. Sumber platform tidak membuktikan penerbitan kedai. Kerana tiada halaman App Store yang disahkan, dokumen ini menghuraikan item berkaitan iOS sebagai sokongan sumber sahaja dan tidak memberitahu pembaca bahawa BarcodeWake kini boleh dimuat turun dari Apple.

## Mengapa dua nombor versi muncul

Repositori `pubspec.yaml` mengisytiharkan versi sumber 2.0.0+2 dan log perubahannya menghuraikan sistem misi yang lebih luas daripada senarai awam yang ditangkap. Pelancaran kedai mungkin ketinggalan dari cawangan pembangunan, dilancarkan secara berperingkat mengikut rantau, atau sekadar tidak diterbitkan. Tanpa rekod kedai yang sepadan, kenyataan yang selamat adalah sempit: keupayaan itu wujud dalam sumber yang diperiksa, manakala ketersediaan awam dibuktikan hanya untuk versi kedai yang ditangkap.

Apabila halaman ciri mengatakan "sumber semasa", perkataan itu adalah disengajakan. Sebelum bergantung pada rantayan misi, perkongsian persediaan atau keupayaan baharu yang lain, semak versi apl yang dipasang dan kawalan yang terlihat. Mulakan dengan [tingkah laku misi](features/missions.md), kemudian gunakan [panduan persediaan](guides/set-up-an-alarm.md) hanya untuk pilihan yang dibina dipasang anda sebenarnya menunjukkan.

## Keperluan peranti dan semakan pemasangan

Pengimbasan memerlukan kebenaran kamera. Misi NFC, gerakan dan langkah memerlukan perkakasan peranti yang sepadan. Penghantaran alarm Android boleh memerlukan pemberitahuan dan akses alarm tepat, dengan tetapan bateri tambahan pada sesetengah pengeluar. Pasang dari senarai kedai yang disahkan, buat alarm ujian jangka dekat, kunci skrin dan sahkan kedua-dua bunyi dan misi yang dipilih sebelum bergantung padanya untuk bangun tidur yang penting.

Untuk senarai sempadan ringkas, baca [fakta produk](facts.md). Jika alarm ujian gagal, ikut [penyelesaian masalah penghantaran alarm](help/alarm-delivery.md) berbanding berulang kali menciptakan semula alarm itu.

