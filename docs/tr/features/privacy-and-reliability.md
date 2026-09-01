---
title: BarcodeWake gizlilik ve alarm güvenilirliği
lang: tr
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

# BarcodeWake gizlilik ve alarm güvenilirliği

BarcodeWake, alarm yapılandırmasını ve görev verilerini cihazda belgelenmiş şekilde tutar ve uygulama hesabı gerektirmez. Mevcut kod yolları, kayıtlı kod değerlerini hash'ler. İsteğe bağlı telemetri varsayılan olarak devre dışı olarak tanımlanmıştır; alarm teslimatı yine de sistem izinlerine ve satıcı kontrollerine bağlıdır.

## Yerel veriler sistem bağımlılıklarını kaldırmaz

Yerel depolama, normal alarm kurulumunun BarcodeWake bulut hesabı gerektirmediği anlamına gelir. Alarm kayıtları, geçmişi ve tercihleri uygulamanın yerel veri katmanı üzerinden işlenir. Kayıtlı barkod, QR ve NFC değerleri mevcut depolama ve içe aktarma yollarında SHA‑256 hash'leri ile temsil edilir; bu, eşleştirme için normal ham değerin saklanmamasını sağlar.

Hashleme, her uygulama kaydının şifrelenmesiyle aynı değildir ve yerel depolama bir yedekleme değildir. Kilitli olmayan bir cihaza erişimi olan bir kişi yine de alarm adlarını, zamanlamalarını veya geçmişini uygulama üzerinden görebilir. Kayıp veya sıfırlanmış bir telefon da, kullanıcı bir dışa aktarma yapmadıysa yerel verileri kaybedebilir. Biçimler ve bunların farklı amaçları için [Yedekleme ve paylaşım](../guides/backup-and-sharing.md) bölümüne bakın.

Gizlilik politikası, isteğe bağlı telemetri'nin varsayılan olarak kapalı olduğunu ve etkinleştirildiğinde toplu işleme açıklamasını yapar. Bu belgeleme, uygulamanın hiçbir zaman ağ üzerinden iletişim kuramayacağı daha geniş bir iddia ileri sürmez. Daha dar, doğrulanmış gerçekleri belirtir: temel işlem ve veriler yereldir, ürün hesabı gerekmez ve kontrol edilen projede reklam SDK bağımlılığı görünmemektedir.

## Güvenilirlik paylaşılan bir sorumluluktur

BarcodeWake bir alarm planlayabilir ve sunabilir, ancak işletim sistemi arka plan çalışmasının ne zaman çalışabileceğini ve hangi kesintilere izin verildiğini belirler. Bildirim izni, kesin alarm erişimi, sessiz veya odak modları, pil optimizasyonu, otomatik uygulama askıya alma ve üretici görev kill'leri hepsi önemli olabilir. Uygulama içi güvenilirlik araçları yapılandırma risklerini belirleyebilir ve kullanıcıları ayarlara yönlendirebilir; sistem ilkesini geçersiz kılamaz.

Kurulumdan sonra, ekran kilitli ve telefon aynı gece kullanılan güç modunda test edin. Bir sistem güncellemesi, pil tasarrufu değişikliği veya uygulama yeniden kurulumundan sonra bu testi tekrarlayın. Cihazı şarjlı tutun, ses seviyesini uygun ayarlayın ve seçilen görevi fiziksel olarak erişilebilir kılın. Test başarısız olursa [Alarm teslimatı sorunlarını giderme](../help/alarm-delivery.md) bölümünü izleyin.

## Gizlilik ve güvenilirliğin vaat etmediği şeyler

BarcodeWake bir tıbbi cihaz, acil durum uyarı servisi veya uyku evresi takipçisi değildir. Hiçbir alarm uygulaması uyanmayı garanti edemez veya kullanılamaz durumdaki bir cihazın telafisini sağlayamaz. [Gerçekler ve sınırlar sayfası](../facts.md) bu sınırları listelerken, [Kullanılabilirlik](../availability.md) genel mağaza kanıtlarını daha yeni kaynak yeteneklerinden ayırır.

