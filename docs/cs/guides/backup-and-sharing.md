---
title: Zálohujte a sdílejte alarmy BarcodeWake bezpečně
lang: cs
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
# Zálohujte a sdílejte alarmy BarcodeWake bezpečně

Použijte export JSON při zachování nebo přesunu vlastních dat aplikace, tištitelný záložní čárový kód PDF pro obnovení a sdílení nastavení QR, když jiná osoba potřebuje pouze strukturu alarmu. Sdílení záměrně vynechává registrovaná tajemství a historii.

## Vyberte formát pro danou úlohu

Aktuální zdroj poskytuje různé cesty pro výměnu, protože zálohování a sdílení nejsou stejná operace. Záloha JSON je určena pro strukturovaný přenos dat a obnovení. Záloha PDF převádí materiál pro obnovení na tištitelný dokument s čárovým kódem. Nastavení QR je záměrně užší: může předat omezenou konfiguraci alarmu bez přenosu registrovaných hodnot čárového kódu, identifikátorů NFC, kódů PIN nebo historie.

Nepovažujte nastavení QR za úplnou zálohu zařízení. Příjemce musí zaregistrovat vlastní fyzické kódy a lokálně zkontrolovat oprávnění. Aktuální sdílení nastavení také omezuje, kolik alarmů přenáší, proto ověřte importovaný výsledek místo předpokladu, že se přesunul každý plán. [Fakta o produktu](../facts.md) zaznamenávají tato omezení.

## Vytvořte a chraňte osobní zálohu

Použijte akci exportu dostupnou v nainstalovaném buildu, zvolte JSON nebo tištitelnou zálohu podle plánu obnovení a uložte výsledek někam, kde máte kontrolu. Záloha může odhalit názvy alarmů, plány a další konfiguraci, i když jsou registrované surové hodnoty kódu chráněny nebo vynechány. Zacházejte s ní jako s osobními běžnými daty: vyhněte se veřejným odkazům, sdíleným tiskárnám a nedůvěryhodným komunikačním kanálům.

Po exportu potvrďte, že soubor lze najít a že jeho časové razítko odpovídá zamýšlené záloze. Neodstraňujte původní data aplikace pouze proto, že příkaz exportu ohlásil úspěch. Test obnovení je jedinou spolehlivou kontrolou, ale proveďte ho na bezpečném zařízení nebo po vytvoření druhé kopie, aby se samotný test nestal událostí ztráty.

## Sdílejte nastavení bez sdílení tajemství

Generujte nastavení QR pouze pro alarmy, které by měl příjemce obdržet. Příjemce ho naskenuje, zkontroluje importovaný plán a poskytne vlastní kód, NFC tag nebo detaily pro obnovení. Tento návrh zabraňuje tomu, aby sdílená konfigurace tiše nepřenesla fyzický klíč, který odmítne alarm někoho jiného.

Po importu by každá osoba měla spustit úplný [test nastavení alarmu](set-up-an-alarm.md). Oprávnění, senzory a omezení operačního systému se v QR nepřenášejí. Pokud importovaný alarm selže při zobrazení během uzamčení, postupujte podle [řešení problémů s doručením alarmu](../help/alarm-delivery.md).

Zdrojová a obchodní verze se během tohoto auditu lišily, takže nainstalovaný veřejný build nemusí zpřístupňovat každou možnost výměny zde popsanou. [Dostupnost](../availability.md) vysvětluje, jak interpretovat schopnosti dostupné pouze ve zdroji.

