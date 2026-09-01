---
title: BarcodeWake görevleri ve görev zincirleri
lang: tr
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
# BarcodeWake görevleri ve görev zincirleri

Bir BarcodeWake görevi, bir alarmı kapatmak için kullanılan koşuldur. Mevcut kaynak kod, QR, matematik, yazma, sallama ve adım görevlerini destekler; kayıtlı NFC kod tarama yoluyla işlenir. Görevler tek başına, sıralı veya rastgele seçim ile çalışabilir.

## Tarama görevleri fiziksel mesafe oluşturur

Barkod veya QR görevi, canlı kamera taramasını kurulum sırasında kayıtlı bir kodla karşılaştırır. Kod, kol erişiminin dışındaki bir nesneye yerleştirilebilir: banyoda tuvalet malzemeleri, mutfakta kahvaltılık bir öğe veya iyi aydınlatılmış bir alanda başka stabil bir nesne. NFC uyumlu bir etiket ve cihazla aynı genel fikri takip eder. Uygulama, normal karşılaştırma için ham koda ihtiyaç duymak yerine mevcut yollarda bir karma temsilini saklar.

Alarm çaldığında hâlâ kullanılabilir olacak bir nesne seçin. Ambalajlar atılır, etiketler soluklaşır ve seyahat ortamı değiştirir. Değiştirmeniz gerekebilecek tek ilaç kutusuna bir kod kaydetmek, dayanıklı bir etiket kullanmaktan daha az sağlamdır. [Alarm kurulum rehberi](../guides/set-up-an-alarm.md) yerleştirme ve testi kapsar.

## Zorluk görevleri hareket karşılığında çaba ister

Matematik ve yazma dikkatli giriş gerektirir. Sallama ve adımlar fiziksel hareket ve desteklenen sensörler gerektirir. Zorluk ve hedef ayarları ne kadar çaba beklendiğini değiştirir, ancak daha zor bir görev otomatik olarak daha iyi değildir. Aşırı sürtünme alarmı tamamen devre dışı bırakmayı teşvik edebilirken, kolay bir görev tekrarlamadan sonra otomatik hale gelebilir.

Görevi hata moduna uygun hale getirin. Alarmları yarı uyurken kapatıyorsanız, başka bir odada tarama faydalı mesafe oluşturur. Kamera erişimi uygun değilse, kısa bir yazma veya matematik görevi daha pratik olabilir. Hareketlilik, denge veya erişilebilirlik endişesi varsa, hareket tabanlı görevlerden kaçının ve güvenli bir şekilde tamamlanabilecek bir görev seçin.

## Tek, zincir ve rastgele modlar

Tek mod bir yapılandırılmış görev ister. Zincir modu birkaç yapılandırılmış görevi sırayla çalıştırır. Rastgele mod yapılandırılmış bir setten seçim yapar ve bir memorized etkileşimin otomatik hale gelme şansını azaltır. Bu modlar daha yeni kontrol edilen kaynakta mevcuttur; [kullanılabilirlik](../availability.md) bunun neden her kamu yapısında zaten bulunduğunu kanıtlamadığını açıklar.

Mod, izinler veya kayıtlı nesneler değiştirildikten sonra her zaman yakın vadeli bir test çalıştırın. Seçilen nesneyi erişilebilir tutun ve güvenli bir kurtarma yolu sağlayın. Görev tamamlamayla ilgisi olmayan teslimat sorunları için [güvenilirlik kontrol listesi](../help/alarm-delivery.md) kullanın.

