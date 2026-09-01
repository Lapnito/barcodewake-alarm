---
title: Soukromí a spolehlivost alarmů aplikace BarcodeWake
lang: cs
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
# Soukromí a spolehlivost alarmů aplikace BarcodeWake

BarcodeWake uchovává zdokumentovanou konfiguraci alarmů a data mise na zařízení a nevyžaduje žádný účet aplikace. Současné cesty kódu hashují registrované hodnoty kódů. Volitelná telemetrie je popsána jako ve výchozím nastavení zakázaná, zatímco doručování alarmů stále závisí na systémových oprávněních a ovládacích prvcích dodavatele.

## Lokální data neodstraňují závislosti na systému

Lokální úložiště znamená, že běžné nastavení alarmu nevyžaduje cloudový účet BarcodeWake. Záznamy alarmů, historie a preference jsou zpracovávány prostřednictvím lokální datové vrstvy aplikace. Registrované hodnoty čárových kódů, QR kódů a NFC jsou reprezentovány pomocí SHA-256 hashů v aktuálních cestách úložiště a importu, což se vyhýbá uchovávání běžné surové hodnoty pro porovnávání.

Hashování není totéž co šifrování každého záznamu aplikace a lokální úložiště není záloha. Někdo s přístupem k odemčenému zařízení může stále vidět názvy alarmů, plány nebo historii prostřednictvím aplikace. Ztracený nebo resetovaný telefon může také ztratit lokální data, pokud uživatel neprovedl export. Viz [zálohování a sdílení](../guides/backup-and-sharing.md) pro formáty a jejich různé účely.

Zásady ochrany osobních údajů uvádějí, že volitelná telemetrie je ve výchozím nastavení vypnutá a popisují agregované zpracování, pokud je povolena. Tato dokumentace proto nečiní širší tvrzení, že aplikace nemůže nikdy komunikovat přes síť. Uvádí užší ověřená fakta: základní operace a data jsou lokální, žádný produktový účet není vyžadován a v kontrolovaném projektu se neobjevuje žádná závislost na reklamním SDK.

## Spolehlivost je sdílená odpovědnost

BarcodeWake může naplánovat a prezentovat alarm, ale operační systém rozhoduje o tom, kdy může běžet práce na pozadí a jaká přerušení jsou povolena. Oprávnění k oznámením, přístup k přesným alarmům, tichému režimu nebo režimu soustředění, optimalizace baterie, automatické pozastavení aplikace a zabijáky úloh výrobce mohou všechny hrát roli. Nástroje spolehlivosti v aplikaci mohou identifikovat rizika konfigurace a nasměrovat uživatele k nastavení; nemohou přepsat systémové zásady.

Po instalaci otestujte se zamknutou obrazovkou a telefonem ve stejném režimu napájení, jaký se používá přes noc. Opakujte tento test po aktualizaci systému, změně úsporného režimu baterie nebo přeinstalaci aplikace. Udržujte zařízení nabité, hlasitost odpovídající a zvolenou misi fyzicky dostupnou. Postupujte podle [řešení problémů s doručováním alarmů](../help/alarm-delivery.md), když test selže.

## Co soukromí a spolehlivost neslibují

BarcodeWake není zdravotnickým prostředkem, službou nouzových upozornění ani sledovačem spánkových fází. Žádná aplikace pro alarmy nemůže zaručit probuzení nebo kompenzovat nedostupné zařízení. [Stránka s fakty a omezeními](../facts.md) uvádí tyto hranice, zatímco [dostupnost](../availability.md) odděluje důkazy z veřejných obchodů od schopností novějšího zdroje.

