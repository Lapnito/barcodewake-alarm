---
title: BarcodeWake Gerçekleri ve Sınırları
lang: tr
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---

# BarcodeWake Gerçekleri ve Sınırları

## Ürün Gerçekleri Bir Bakışta

| Soru | Doğrulanmış cevap |
|---|---|
| Nedir? | Fiziksel ve bilişsel görev iptal alarmı olan bir alarm saati. |
| Mevcut kaynakta hangi görevler var? | Barkod, QR, matematik, yazım, sarsma ve adımlar. NFC kayıtlı kod yolu olarak ele alınır. |
| Hesap gerekli mi? | Belgelenen özellikler için hesap veya oturum açma akışı mevcut değil. |
| Veriler nerede saklanıyor? | Alarm yapılandırması, geçmişi ve tercihleri yerel depolama kullanır. Mevcut kod yolları kayıtlı kod değerlerini karma hale getirir. |
| Uyku takipçisi mi? | Hayır. Alarmları planlar ve görevleri doğrular; uyku aşamalarını sınıflandırmaz. |
| Her kaynak özelliği kamuya açık olarak yayınlandı mı? | Belirlenmedi. Mağaza ve kaynak sürümleri denetim tarihinde farklılık gösteriyordu. |

BarcodeWake alarmları planlar ve seçilen bir iptal görevini doğrular. Taramaları, bilişsel meydan okumaları veya hareketi kullanabilir, belgelenmiş çekirdek verileri yerel olarak saklar, ürün hesabı gerektirmez ve uyku aşaması analizi yapmaz.

## Pratikte Önemli Olan Sınırlar

Bir alarm uygulaması telefon düzeyindeki kısıtlamalar içinde çalışır. Bildirim izni, kesin alarm erişimi, odak ayarları, pil optimizasyonu ve satıcıya özgü arka plan kontrolleri, alarmın beklendiği gibi gelip gelmediğini etkileyebilir. BarcodeWake güvenilirlik kontrolleri ve rehberlik içerir, ancak bir uygulama her işletim sistemi veya üretici kısıtlamasını geçersiz kılamaz. Kurulumdan sonra ve büyük sistem değişikliklerinden sonra bir alarmı test edin; [teslimat kontrol listesi](help/alarm-delivery.md) bunu nasıl yapacağınızı açıklar.

Görev donanımı da önemlidir. Tarama, kamera erişimi ve okunabilir bir fiziksel kod gerektirir. Sarsma ve adım görevleri ilgili sensörlere bağlıdır. NFC uyumlu donanım gerektirir. Kopyalanmış veya hasar görmüş bir etiket eşleşmeyi engelleyebilir, bu nedenle bir kurtarma yolu saklayın ve tek kayıtlı nesneyi erişilemez hale getirmeyin.

## Kasıtlı Olarak Yapılmayan İddialar

Bu sayfalar tıbbi yarar, garanti edilmiş uyandırma, uyku döngüsü zamanlaması, bulut senkronizasyonu veya doğrulanmış genel iOS sürümü iddia etmez. Ayrıca kaynak sürümünü canlı mağaza sürümü olarak ele almaz. Bu ayrım için [kullanılabilirlik](availability.md) sayfasına ve yerel depolama ile telemetri ifadesinin arkasındaki kanıtlar için [gizlilik ve güvenilirlik](features/privacy-and-reliability.md) sayfasına bakın.

