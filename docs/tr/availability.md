---
title: BarcodeWake kullanılabilirlik ve sürümleri
lang: tr
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake kullanılabilirlik ve sürümleri

BarcodeWake, Android için doğrulanmış bir Google Play listesine sahiptir. Denetim tarihinde Google Play, sürüm 1.0.0 gösterirken, kontrol edilen kaynak proje sürüm 2.0.0+2 olarak beyan etti. Herhangi bir genel App Store listesi doğrulanmadı.

## Doğrulanmış genel dağıtım

Android paketi, [Google Play'de BarcodeWake: Hile Yapamazsın Alarmı](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us) olarak kamuya açıkça listelenmiştir. Bu belgeleme için yakalanan mağaza anlık görüntüsü, sürüm 1.0.0 ve Mart 2026'da son güncelleme tarihi bildirdi. Bu anlık görüntü, listelemenin belirli bir zamandaki kanıtıdır; her bölgenin aynı dağıtımı gördüğünü veya listenin değişmeden kalacağını garanti etmez.

Kaynak ağacı, Android ve iOS platform projelerini içerir. Platform kaynağı, mağaza yayınını kanıtlamaz. App Store sayfası doğrulanmadığından, bu belgeler iOS ile ilgili öğeleri yalnızca kaynak destek olarak açıklar ve okuyuculara BarcodeWake'in şu anda Apple'dan indirilebilir olduğunu söylemez.

## Neden iki sürüm numarası görünüyor

Depo `pubspec.yaml`, kaynak sürümü 2.0.0+2 olarak beyan eder ve değişiklik günlüğü, yakalanan genel listeden daha geniş bir görev sistemini tanımlar. Bir mağaza dağıtımı, bir geliştirme dalının gerisinde kalabilir, bölgeye göre aşamalı olabilir veya basitçe yayınlanmamış olabilir. Eşleşen bir mağaza kaydı olmadan, güvenli ifade dardır: yetenek, kontrol edilen kaynakta mevcuttur, genel kullanılabilirlik ise yalnızca yakalanan mağaza sürümü için kanıtlanmıştır.

Bir özellik sayfası "geçerli kaynak" dediğinde, bu ifade kasıtlıdır. Görev zincirlerine, kurulum paylaşımına veya başka bir yeni yeteneğe güvenmeden önce, yüklü uygulamanın sürümünü ve görünür kontrollerini kontrol edin. [Görev davranışıyla](features/missions.md) başlayın, ardından yüklü derlemenizin gerçekten gösterdiği seçenekler için yalnızca [kurulum kılavuzunu](guides/set-up-an-alarm.md) kullanın.

## Cihaz gereksinimleri ve kurulum kontrolleri

Tarama, kamera izni gerektirir. NFC, hareket ve adım görevleri, ilgili cihaz donanımını gerektirir. Android alarm teslimatı, bildirim ve tam-alarm erişimi gerektirebilir; bazı üreticilerde ek pil ayarları bulunur. Doğrulanmış mağaza listesinden kurun, yakın vadeli bir test alarmı oluşturun, ekranı kilitleyin ve önemli bir uyandırma için bağımlı kalmadan önce hem sesi hem de seçilen görevi onaylayın.

Kısa bir sınır listesi için [ürün gerçeklerini](facts.md) okuyun. Bir test alarmı başarısız olursa, alarmı tekrar tekrar yeniden oluşturmak yerine [alarm teslimat sorun giderme](help/alarm-delivery.md) kılavuzunu izleyin.

