---
title: Zálohujte a zdieľajte alarmy BarcodeWake bezpečne
lang: sk
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
# Zálohujte a zdieľajte alarmy BarcodeWake bezpečne

Použite JSON export, keď potrebujete zachovať alebo presunúť vlastné údaje aplikácie, tlačiteľný záložný čiarový kód PDF pre obnovu, a nastavovací QR kód na zdieľanie, keď iná osoba potrebuje iba štruktúru alarmu. Zdieľanie zámerne vynecháva registrované tajomstvá a históriu.

## Vyberte formát pre danú úlohu

Aktuálny zdroj poskytuje rôzne výmenné cesty, pretože zálohovanie a zdieľanie nie je tá istá operácia. JSON záloha je určená pre štruktúrovaný prenos údajov a obnovenie. PDF záloha premieňa materiál na obnovenie na tlačiteľný dokument s čiarovým kódom. Nastavovací QR kód je zámerne užší: môže odoslať obmedzenú konfiguráciu alarmu bez prenosu registrovaných hodnôt čiarových kódov, identifikátorov NFC, PIN kódov alebo histórie.

Nepovažujte nastavovací QR kód za úplnú zálohu zariadenia. Príjemca si musí zaregistrovať vlastné fyzické kódy a lokálne skontrolovať povolenia. Aktuálne zdieľanie nastavení tiež obmedzuje počet alarmov, ktoré môže obsahovať, preto overte importovaný výsledok namiesto toho, aby ste predpokladali, že sa presunul každý plán. [Fakty o produkte](../facts.md) zaznamenávajú tieto hranice.

## Vytvorte a chráňte osobnú zálohu

Použite akciu exportu dostupnú v nainštalovanej verzii, vyberte JSON alebo tlačiteľnú zálohu podľa plánu obnovy a uložte výsledok niekam, kde ho máte pod kontrolou. Záloha môže odhaliť názvy alarmov, plány a inú konfiguráciu, aj keď sú registrované nespracované hodnoty kódov chránené alebo vynechané. Zaobchádzajte s ňou ako s osobnými rutinnými údajmi: vyhnite sa verejným odkazom, zdieľaným tlačiarňam a nedôveryhodným kanálom zasielania správ.

Po exportovaní potvrďte, že súbor možno nájsť a že jeho časová značka zodpovedá zamýšľanej zálohe. Nemazte pôvodné údaje aplikácie len preto, že príkaz exportu hlásil úspech. Testovanie obnovenia je jediná spoľahlivá kontrola, ale vykonajte ho na bezpečnom zariadení alebo po vytvorení druhej kópie, aby samotný test nebol udalosťou straty.

## Zdieľajte nastavenie bez zdieľania tajomstiev

Generujte nastavovací QR kód iba pre alarmy, ktoré má príjemca prijať. Príjemca ho naskenuje, skontroluje importovaný plán a poskytne vlastný kód, NFC tag alebo podrobnosti na obnovenie. Tento dizajn zabraňuje tomu, aby zdieľaná konfigurácia ticho neprenosila fyzický kľúč, ktorý odomkne cudzí alarm.

Po importe by každá osoba mala spustiť úplný [test nastavenia alarmu](set-up-an-alarm.md). Povolenia, snímače a obmedzenia operačného systému sa v QR kóde neprenášajú. Ak sa importovaný alarm nezobrazuje počas uzamknutia, postupujte podľa [riešenia problémov s doručením alarmu](../help/alarm-delivery.md).

Zdrojová a uložená verzia sa počas tohto auditu líšili, takže nainštalovaná verejná verzia nemusí zobrazovať každú tu popísanú možnosť výmeny. [Dostupnosť](../availability.md) vysvetľuje, ako interpretovať schopnosti dostupné len vo zdrojovom kóde.

