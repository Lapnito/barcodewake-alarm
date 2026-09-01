---
title: Privasi dan kebolehpercayaan penggera BarcodeWake
lang: ms
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# Privasi dan kebolehpercayaan penggera BarcodeWake

BarcodeWake menyimpan konfigurasi penggera yang didokumenkan dan data misi pada peranti dan tidak memerlukan akaun aplikasi. Laluan kod semasa mencincang nilai kod berdaftar. Telemetri pilihan diterangkan sebagai dilumpuhkan secara lalai, sementara penghantaran penggera masih bergantung kepada kebenaran sistem dan kawalan vendor.

## Data setempat tidak menghapuskan kebergantungan sistem

Storan setempat bermakna tetapan penggera biasa tidak memerlukan akaun awan BarcodeWake. Rekod penggera, sejarah dan keutamaan dikendalikan melalui lapisan data setempat aplikasi. Nilai barkod berdaftar, QR dan NFC diwakili dengan cincangan SHA-256 dalam storan semasa dan laluan import, yang mengelakkan penyimpanan nilai mentah biasa untuk pemadanan.

Pemprosesan cincangan bukan sama dengan penyulitan bagi setiap rekod aplikasi, dan storan setempat bukan sandaran. Seseorang yang mempunyai akses kepada peranti yang tidak dikunci mungkin masih dapat melihat nama penggera, jadual atau sejarah melalui aplikasi. Telefon yang hilang atau direset juga boleh kehilangan data setempat kecuali pengguna membuat eksport. Lihat [sandaran dan perkongsian](../guides/backup-and-sharing.md) untuk format dan tujuan masing-masing.

Dasar privasi berkata telemetri pilihan dilumpuhkan secara lalai dan menghuraikan pengendalian agregat jika diaktifkan. Oleh itu, dokumentasi ini tidak membuat tuntutan yang lebih luas bahawa aplikasi tidak boleh berkomunikasi melalui rangkaian. Ia menyatakan fakta yang lebih sempit dan disahkan: operasi dan data teras adalah setempat, tiada akaun produk diperlukan, dan tiada kebergantungan SDK pengiklanan muncul dalam projek yang diperiksa.

## Kebolehpercayaan adalah tanggungjawab bersama

BarcodeWake boleh menjadualkan dan membentangkan penggera, tetapi sistem operasi memutuskan bila kerja latar belakang boleh berjalan dan gangguan mana yang dibenarkan. Kebenaran pemberitahuan, akses penggera tepat, mod senyap atau fokus, pengoptimalan bateri, penggantungan aplikasi automatik dan pembunuh tugas pengeluar semua boleh memberi kesan. Alat kebolehpercayaan dalam aplikasi boleh mengenal pasti risiko konfigurasi dan mengarahkan pengguna ke tetapan; ia tidak boleh mengatasi dasar sistem.

Selepas pemasangan, uji dengan skrin dikunci dan telefon dalam mod kuasa yang sama digunakan semalaman. Ulangi ujian itu selepas kemas kini sistem, perubahan penjimat bateri atau pasang semula aplikasi. Pastikan peranti dicas, kelantangan sesuai dan misi yang dipilih tersedia secara fizikal. Ikuti [penyelesaian masalah penghantaran penggera](../help/alarm-delivery.md) apabila ujian gagal.

## Apa yang privasi dan kebolehpercayaan tidak janjikan

BarcodeWake bukan peranti perubatan, perkhidmatan amaran kecemasan atau penjejak peringkat tidur. Tiada aplikasi penggera boleh menjamin anda bangun atau memberi pampasan untuk peranti yang tidak tersedia. Halaman [fakta dan had](../facts.md) menyenaraikan sempadan ini, sementara [ketersediaan](../availability.md) memisahkan bukti kedai awam daripada keupayaan sumber baharu.

