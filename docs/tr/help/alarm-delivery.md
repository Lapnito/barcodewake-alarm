---
title: BarcodeWake alarmı neden çalmayabilir
lang: tr
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# BarcodeWake alarmı neden çalmayabilir

Kaydedilen bir alarm, bildirim ayarları, kesin alarm erişimi, odak veya sessiz modlar, düşük ses, pil kısıtlamaları, uygulama askıya alma veya satıcı arka plan kontrolleri tarafından engellenebilir. Teslimatı görev taramadan ayrı olarak kontrol edin, ardından kilitli ekran testini çalıştırın.

## İlk olarak teslimatı reddetmeden ayırın

Kısa vadeli basit bir görevle test alarmı oluşturun ve uygulamayı arka planda bırakın. Ekranı kilitleyin. Alarm ekranı veya sesi görünmüyorsa, sorun teslimattadır; kayıtlı barkod değiştirmek bunu düzeltmeyecektir. Alarm görünüyor ancak görev tamamlanamıyorsa, teslimat çalışıyor ve sorun kamera, sensör, kod eşleştirme veya görev yapılandırmasıdır.

Alarmın etkinleştirildiğini, planlanan günün doğru olduğunu ve telefonun saat diliminin amaçlanan programa uygun olduğunu onaylayın. Yan düğme durumuna güvenmek yerine ortam ve alarm sesini kontrol edin. Rahatsız etmeyin veya odak kurallarını, bağlı ses cihazlarını ve alarm oluşturulduktan sonra telefonun yeniden başlatılıp başlatılmadığını gözden geçirin.

## İşletim sistemi izin kapılarını gözden geçirin

Kurulu derlemenin istediği bildirimlere ve herhangi bir kesin alarm veya tam ekran alarm erişimine izin verin. Cihaz satıcısı bu kontrolleri sunduğunda, BarcodeWake'i agresif pil optimizasyonundan veya otomatik uyku listelerinden kaldırın. Uygulama içi güvenilirlik tanılamalarını açın ve belirlediği cihaza özgü ayarları izleyin. [Gizlilik ve güvenilirlik sayfası](../features/privacy-and-reliability.md) bu sistem bağımlılıklarının uygulama verilerinin yerel olduğu durumlarda bile neden devam ettiğini açıklar.

Bir ayarı değiştirdikten sonra kilitli ekran testini tekrarlayın. Birkaç kontrolü aynı anda değiştirmek, nedeni belirlemeyi zorlaştırır. Sistem güncellemeleri izinleri sıfırlayabilir veya yeniden yorumlayabilir, bu nedenle büyük bir güncelleme veya uygulama yeniden yüklemesinden sonra yeniden test edin.

## Görev tamamlamayı ayrı ayrı tanılayın

Barkod ve QR görevleri için kamera lensini temizleyin, aydınlatmayı iyileştirin ve kayıtlı nesnenin değişmediğini onaylayın. Kamera izni verin. NFC için cihaz desteğini doğrulayın ve etiketi doğru anten konumuna yakın tutun. Salla ve adım görevleri, güç tasarrufu modları sensör teslimatını kısıtladığında hareket veya adım sensörlerine bağlıdır ve farklı davranabilir.

Bir görev bir zincirin parçası olarak yapılandırılmışsa, her gerekli adım tamamlanmalıdır. [Görev davranışını](../features/missions.md) gözden geçirin ve gerekirse [kurulum prosedürünü](../guides/set-up-an-alarm.md) kullanarak yeni bir test oluşturun.

## Telefonun sınır olduğu durumları bilin

BarcodeWake, kapatılmış bir cihazı, bitmiş pili, bozuk ses donanımını veya her üretici görev öldürücüsünü geçersiz kılamaz. Acil durum bildirim servisi değildir. Yüksek sonuçlu durumlar için başka bir alarm yöntemi kullanmaya devam edin ve cihaz modeli, sistem sürümü, uygulama sürümü ve tam test koşulları ile tekrarlanabilir hataları bildirin.

