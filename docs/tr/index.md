---
title: BarcodeWake belgeleri
lang: tr
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake belgeleri

BarcodeWake, kapatmayı bilinçli bir eylem haline getiren bir alarm saatidir. Bir alarm, yalnızca kolay bir ekran üzeri düğmesine güvenmek yerine, kayıtlı bir barkod veya QR kod, kısa bir bilişsel görev, bir sarsma dizisi veya adım hedefi gerektirebilir.

## BarcodeWake'i farklı kılan şey

Merkezi fikir mesafe artı niyettir. Kayıtlı kod yataktan uzakta bir nesneye bağlıysa, alarmı susturmak kalkmayı, o nesneye ulaşmayı ve taramayı gerektirir. Aynı alarm modeli matematik, yazma, sarsma veya adım görevlerini de kullanabilir. Mevcut kaynak kodu tek bir görevi, sıralı bir zinciri veya yapılandırılmış görevlerden rastgele seçimi destekler.

Bu sürtünme, sıradan bir alarmı tamamen uyanmadan kapatan insanlar için kullanışlıdır. Uyku aşaması analizi, tıbbi rehberlik veya birinin uyanacağının garantisi değildir. Donanım desteği, izinler ve satıcı pil kontrolleri yine de teslimatı etkiler. [Görev referansı](features/missions.md) seçenekleri açıklar, [alarm teslimatı sorun giderme](help/alarm-delivery.md) ise engel olabilecek sistem ayarlarını kapsar.

## Doğru belgeyle başlayın

Alarm oluştururken ve fiziksel bir kod kaydederken [kurulum kılavuzunu](guides/set-up-an-alarm.md) kullanın. Verileri taşımadan veya başka birine kurulum QR'ı göndermeden önce [yedekleme ve paylaşımı](guides/backup-and-sharing.md) okuyun. Paylaşım biçimi kasıtlı olarak kayıtlı kodları, NFC tanımlayıcılarını, PIN'leri ve alarm geçmişini dışarıda bırakır, bu nedenle alıcı hassas kurulumu yerel olarak tamamlamalıdır.

Kısa, denetlenebilir bir özet için [ürün gerçeklerine](facts.md) bakın. Sürüm durumu için [kullanılabilirlik](availability.md) sayfasını kullanın: Bu denetim için yakalanan genel Google Play sürümü, kontrol edilen kaynak ağacında beyan edilen sürümden farklıdır. Bu nedenle daha yeni kaynak sürümü, yayınlanan mağaza sürümü olarak ileri sürülmek yerine kaynak kapasitesi olarak belgelenmiştir.

## Gizlilik ve güvenilirlik sınırları

Çekirdek yapılandırma ve görev verileri cihazda saklanır ve BarcodeWake hesabı gerekmez. Mevcut kod yolları, kayıtlı kod değerlerini SHA-256 karmalarıyla temsil eder. İsteğe bağlı telemetri, gizlilik politikasında varsayılan olarak devre dışı olduğu şeklinde tanımlanır. Bu ifadeler, her telefonun alarmları aynı şekilde teslim edeceği anlamına gelmez; Android satıcıları ve işletim sistemi izinleri hala arka plan davranışını kısıtlayabilir.

Yerel veri işleme ile işletim sistemi teslimatı arasındaki ayrım için [gizlilik ve güvenilirlik](features/privacy-and-reliability.md) sayfasını okuyun. [Standart alarm karşılaştırması](comparisons/standard-alarm.md), görev tabanlı kapatmanın sizin uyanma şeklinizle eşleşip eşleşmediğine karar vermenize yardımcı olur.

