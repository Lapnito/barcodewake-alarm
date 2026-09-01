---
title: Dokumentace BarcodeWake
lang: cs
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Dokumentace BarcodeWake

BarcodeWake je budík, který proměňuje jeho zrušení v záměrný akt. Budík může vyžadovat uložený čárový kód nebo QR kód, krátký kognitivní úkol, sekvenci třesení nebo cíl kroků místo spoléhání pouze na snadné tlačítko na obrazovce.

## Co dělá BarcodeWake jiným

Centrální myšlenkou je vzdálenost a záměr. Pokud je registrovaný kód připojen k objektu daleko od postele, ztišení alarmu znamená vstát, dosáhnout tohoto objektu a naskenovat ho. Stejný model alarmu může také používat matematiku, psaní, třesení nebo krokové mise. Aktuální zdrojový kód podporuje jedinou misi, uspořádaný řetězec nebo náhodný výběr z nakonfigurovaných misí.

Toto tření je užitečné pro lidi, kteří zruší běžný budík, aniž by se plně probudili. Nejedná se o analýzu spánkových stadií, lékařské vedení ani záruku, že někdo vstane. Hardwarová podpora, oprávnění a bateriové ovládání od výrobce stále ovlivňují doručení. [Referenční dokumentace misí](features/missions.md) vysvětluje možnosti, zatímco [řešení problémů s doručením alarmů](help/alarm-delivery.md) pokrývá systémová nastavení, která mohou interferovat.

## Začněte správným dokumentem

Použijte [průvodce nastavením](guides/set-up-an-alarm.md) při vytváření alarmu a registraci fyzického kódu. Před přesunem dat nebo odesláním QR kódu pro nastavení někomu jinému si přečtěte [zálohování a sdílení](guides/backup-and-sharing.md). Formát sdílení záměrně vylučuje registrované kódy, NFC identifikátory, PINy a historii alarmů, takže příjemce musí citlivé nastavení dokončit lokálně.

Pro krátký auditable souhrn viz [fakta o produktu](facts.md). Pro stav vydání použijte [dostupnost](availability.md): veřejná verze Google Play zachycená pro tento audit se liší od verze deklarované kontrolovaným stromem zdrojového kódu. Novější verze zdrojového kódu je proto zdokumentována jako schopnost zdroje, nikoli tvrzena jako vydání publikovaného obchodu.

## Hranice soukromí a spolehlivosti

Základní konfigurace a data misí jsou uložena na zařízení a není vyžadován žádný účet BarcodeWake. Aktuální cesty kódu reprezentují hodnoty registrovaných kódů pomocí hashů SHA-256. Volitelná telemetrie je popsána zásadami ochrany osobních údajů jako ve výchozím nastavení zakázaná. Tyto výroky neznamenají, že každý telefon bude doručovat alarmy identicky; prodejci Android a oprávnění operačního systému stále mohou omezovat chování na pozadí.

Přečtěte si [soukromí a spolehlivost](features/privacy-and-reliability.md) pro rozlišení mezi lokálním zpracováním dat a doručením operačním systémem. [Srovnání se standardním budíkem](comparisons/standard-alarm.md) pomáhá rozhodnout, zda mission-based zrušení odpovídá způsobu, jakým se budíte.

