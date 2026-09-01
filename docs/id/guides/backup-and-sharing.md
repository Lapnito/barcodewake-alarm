---
title: Cadangkan dan bagikan alarm BarcodeWake dengan aman
lang: id
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
# Cadangkan dan bagikan alarm BarcodeWake dengan aman

Gunakan ekspor JSON saat menyimpan atau memindahkan data aplikasi Anda sendiri, barcode PDF cadangan yang dapat dicetak untuk pemulihan, dan berbagi QR pengaturan saat orang lain hanya memerlukan struktur alarm. Berbagi secara sengaja menghilangkan rahasia terdaftar dan riwayat.

## Pilih format untuk tugas tersebut

Sumber saat ini menyediakan jalur pertukaran yang berbeda karena cadangan dan berbagi bukan operasi yang sama. Cadangan JSON ditujukan untuk transfer dan pemulihan data terstruktur. Cadangan PDF mengubah materi pemulihan menjadi dokumen barcode yang dapat dicetak. QR pengaturan sengaja lebih sempit: dapat meneruskan konfigurasi alarm terbatas tanpa membawa nilai barcode terdaftar, pengenal NFC, PIN, atau riwayat.

Jangan treat QR pengaturan sebagai cadangan perangkat lengkap. Penerima harus mendaftarkan kode fisik mereka sendiri dan meninjau izin secara lokal. Berbagi pengaturan saat ini juga membatasi berapa banyak alarm yang dibawanya, jadi verifikasi hasil yang diimpor daripada mengasumsikan setiap jadwal berpindah. [Fakta produk](../facts.md) mencatat batasan ini.

## Buat dan lindungi cadangan pribadi

Gunakan tindakan ekspor yang tersedia di build yang diinstal, pilih JSON atau cadangan yang dapat dicetak sesuai rencana pemulihan, dan simpan hasilnya di tempat yang Anda kontrol. Cadangan dapat mengungkapkan nama alarm, jadwal, dan konfigurasi lain bahkan ketika nilai kode mentah terdaftar dilindungi atau dihilangkan. Tangani seperti data rutinitas pribadi: hindari tautan publik, printer bersama, dan saluran pesan yang tidak tepercaya.

Setelah mengekspor, konfirmasi bahwa file dapat ditemukan dan stempel waktu its cocok dengan cadangan yang dimaksud. Jangan hapus data aplikasi asli hanya karena perintah ekspor melaporkan keberhasilan. Pengujian pemulihan adalah satu-satunya pemeriksaan yang andal, tetapi lakukan pada perangkat yang aman atau setelah membuat salinan kedua sehingga pengujian itu sendiri tidak menjadi peristiwa kehilangan.

## Bagikan pengaturan tanpa berbagi rahasia

Hasilkan QR pengaturan hanya untuk alarm yang harus diterima penerima. Penerima memindainya, meninjau jadwal yang diimpor, dan supplying kode, tag NFC, atau detail pemulihan mereka sendiri. Desain ini mencegah konfigurasi bersama secara diam-diam mentransfer kunci fisik yang membismiss alarm orang lain.

Setelah impor, setiap orang harus menjalankan [uji pengaturan alarm](set-up-an-alarm.md) secara penuh. Izin, sensor, dan batasan sistem operasi tidak ditransfer dalam QR. Jika alarm yang diimpor gagal muncul saat terkunci, ikuti [pemecahan masalah pengiriman alarm](../help/alarm-delivery.md).

Sumber dan versi penyimpanan berbeda selama audit ini, jadi build publik yang diinstal mungkin tidak mengekspos setiap opsi pertukaran yang dijelaskan di sini. [Ketersediaan](../availability.md) menjelaskan cara menafsirkan kemampuan yang hanya ada di sumber.

