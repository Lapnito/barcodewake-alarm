---
title: BarcodeWake alarmlarını güvenli bir şekilde yedekleyin ve paylaşın
lang: tr
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
# BarcodeWake alarmlarını güvenli bir şekilde yedekleyin ve paylaşın

Kendi uygulama verilerinizi korumak veya taşımak için bir JSON dışa aktarması, kurtarma için yazdırılabilir bir PDF yedekleme barkodu ve başka bir kişi yalnızca alarm yapısına ihtiyaç duyduğunda kurulum QR paylaşımı kullanın. Paylaşım, kayıtlı sırları ve geçmişi kasıtlı olarak hariç tutar.

## İş için formatı seçin

Mevcut kaynak, yedekleme ve paylaşmanın aynı işlem olmaması nedeniyle farklı değişim yolları sağlar. Bir JSON yedeği, yapılandırılmış veri aktarımı ve geri yükleme için tasarlanmıştır. Bir PDF yedeği, kurtarma materyalini yazdırılabilir bir barkod belge haline getirir. Bir kurulum QR'ı kasıtlı olarak daha dardır: kayıtlı barkod değerlerini, NFC tanımlayıcılarını, PIN'leri veya geçmişi taşımadan sınırlı bir alarm yapılandırmasını iletebilir.

Bir kurulum QR'ını tam bir cihaz yedeklemesi olarak ele almayın. Alıcı, kendi fiziksel kodlarını kaydetmeli ve izinleri yerel olarak gözden geçirmelidir. Mevcut kurulum paylaşımı ayrıca taşıdığı alarm sayısını sınırlar, bu nedenle her çizelgenin taşındığını varsaymak yerine içe aktarılan sonucu doğrulayın. [Ürün gerçekleri](../facts.md) bu sınırları kaydeder.

## Kişisel bir yedek oluşturun ve koruyun

Kurulu derlemede bulunan dışa aktarma eylemini kullanın, kurtarma planına göre JSON veya yazdırılabilir yedeklemeyi seçin ve sonucu kontrol ettiğiniz bir yere kaydedin. Bir yedekleme, kayıtlı ham kod değerleri korunsa veya atlanmış olsa bile alarm adlarını, çizelgeleri ve diğer yapılandırmaları ortaya çıkarabilir. Kişisel rutin verileri gibi ele alın: genel bağlantılardan, paylaşılan yazıcılardan ve güvenilmez mesajlaşma kanallarından kaçının.

Dışa aktardıktan sonra, dosyanın bulunabildiğini ve zaman damgasının amaçlanan yedeklemeyle eşleştiğini onaylayın. Bir dışa aktarma komutu başarılı olduğu bildirdi diye orijinal uygulama verilerini silmeyin. Geri yükleme testi, tek güvenilir kontroldür, ancak bunu güvenli bir cihazda veya testin kendisinin bir kayıp olayına dönüşmemesi için ikinci bir kopya oluşturduktan sonra gerçekleştirin.

## Sırları paylaşmadan kurulumu paylaşın

Yalnızca alıcının alması gereken alarmlar için bir kurulum QR'ı oluşturun. Alıcı bunu tarar, içe aktarılan çizelgeyi gözden geçirir ve kendi kodunu, NFC etiketini veya kurtarma ayrıntılarını sağlar. Bu tasarım, paylaşılan bir yapılandırmanın başkasının alarmını kapatmak için kullandığı fiziksel anahtarı sessizce aktarmasını önler.

İçe aktardıktan sonra, her kişi tam [alarm kurulum testini](set-up-an-alarm.md) çalıştırmalıdır. İzinler, sensörler ve işletim sistemi kısıtlamaları QR'da aktarılmaz. Kilitliyken içe aktarılan bir alarm görünmüyorsa, [alarm teslimat sorunlarını giderme](../help/alarm-delivery.md) bölümünü izleyin.

Bu denetim sırasında kaynak ve depo sürümleri farklıydı, bu nedenle yüklenen genel derleme burada açıklanan her değişim seçeneğini ortaya çıkarmayabilir. [Kullanılabilirlik](../availability.md), yalnızca kaynakta bulunan yeteneklerin nasıl yorumlanacağını açıklar.

