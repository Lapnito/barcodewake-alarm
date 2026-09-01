---
title: BarcodeWake terminolojisi
lang: tr
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
# BarcodeWake terminolojisi

BarcodeWake, bir alarmı kapatmak için gereken eylem için "görev" terimini kullanır. Tarama görevleri kayıtlı bir fiziksel kodu doğrular; meydan okuma görevleri bir yanıtı veya hareketi doğrular; paylaşım ve yedekleme farklı değişim formatlarını ifade eder.

## Alarm ve görev terimleri

- Alarm: Zaman, aktif günler, ses ve kapatma yapılandırması ile planlanmış bir uyanma olayı.
- Görev: Kapatılmadan önce tamamlanması gereken görev.
- Tarama görevi: Kayıtlı bir kod temsiliyle eşleştirilen barkod, QR veya NFC tabanlı görev.
- Meydan okuma görevi: Matematik, yazma, sallama veya adım görevi.
- Tek mod: Alarm için bir yapılandırılmış görev çalışır.
- Zincir mod: Yapılandırılmış görevler seçilen sırada çalışır.
- Rastgele mod: Yapılandırılmış bir setten bir görev seçilir.
- Zorluk: Görev talebini değiştiren bir görev ayarı; kesin etkisi görev türüne bağlıdır.

## Veri ve güvenilirlik terimleri

- Kayıtlı kod: Bir tarama göreviyle ilişkili fiziksel barkod, QR kodu veya NFC etiketi.
- Kod hash'i: Kayıtlı değerleri eşleştirmek için mevcut depolama ve değişim yollarında kullanılan tek yönlü SHA-256 temsili.
- Yerel yedekleme: Uygulama verilerini korumak veya geri yüklemek için tasarlanmış bir dışa aktarılmış temsil.
- Kurulum QR'ı: Kayıtlı kodları, NFC tanımlayıcılarını, PIN'leri ve geçmişi atlayan sınırlı bir yapılandırma paylaşım formatı.
- Güvenilirlik Doktoru: Alarm teslimatını engelleyebilecek izinler ve sistem ayarları için uygulama içi tanılamalar.
- Kesin alarm erişimi: Zamana duyarlı zamanlama sağlayan Android sistem izni veya politikası.
- Pil optimizasyonu: Arka plan yürütmeyi kısıtlayabilecek işletim sistemi veya satıcı kontrolleri.

Tam özellik ilişkisi için bkz. [görevler ve görev zincirleri](features/missions.md). Dışa aktarma formatları arasındaki farklar için [yedekleme ve paylaşım](guides/backup-and-sharing.md) bölümünü okuyun. [Gerçekler sayfası](facts.md), uygulamanın ölçmediğini iddia ettiği şeyleri tanımlar.

