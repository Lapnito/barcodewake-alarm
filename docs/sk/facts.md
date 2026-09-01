---
title: Fakty a limity aplikácie BarcodeWake
lang: sk
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
# Fakty a limity aplikácie BarcodeWake

BarcodeWake plánuje budíky a overuje zvolenú úlohu na odloženie. Môže využívať skeny, kognitívne výzvy alebo pohyb, ukladá zdokumentované základné údaje lokálne, nevyžaduje produktový účet a nevykonáva analýzu fáz spánku.

## Zhrnutie faktov o produkte

| Otázka | Overená odpoveď |
|---|---|
| Čo to je? | Budík s fyzickými a kognitívnymi úlohami na odloženie. |
| Aké úlohy existujú v aktuálnom zdrojovom kóde? | Čiarový kód, QR kód, matematika, písanie, trasenie a kroky. NFC je spracovaný ako registrovaná cesta kódu. |
| Je potrebný účet? | Pre zdokumentované funkcie nie je prítomný žiadny účet ani prihlasovací postup. |
| Kde sa uchovávajú údaje? | Konfigurácia budíka, história a predvoľby využívajú lokálne úložisko. Aktuálne cesty kódu hashu registrované hodnoty kódu. |
| Je to sledovač spánku? | Nie. Plánuje budíky a overuje úlohy; neklasifikuje fázy spánku. |
| Je každá funkcia zo zdrojového kódu verejne vydaná? | Nie je stanovené. Verzie obchodu a zdrojového kódu sa pri audite líšili. |

## Limity, ktoré sú dôležité v praxi

Aplikácia budíka funguje v rámci obmedzení úrovne telefónu. Povolenie oznámení, prístup k presným budíkom, nastavenia zamerania, optimalizácia batérie a špecifické ovládacie prvky pozadia od výrobcu môžu ovplyvniť, či budík dorazí podľa očakávania. BarcodeWake obsahuje kontroly spoľahlivosti a usmernenia, ale aplikácia nemôže prepísať každé obmedzenie operačného systému alebo výrobcu. Otestujte budík po inštalácii a po veľkých systémových zmenách; [kontrolný zoznam doručenia](help/alarm-delivery.md) vysvetľuje, ako na to.

Hardvér úloh tiež zohráva úlohu. Skenovanie vyžaduje prístup k fotoaparátu a čitateľný fyzický kód. Úlohy trasenia a krokov závisia od príslušných senzorov. NFC potrebuje kompatibilný hardvér. Skopírovaný alebo poškodený štítok môže zabrániť zhode, preto si ponechajte cestu obnovenia a neurobte jediný registrovaný objekt neprístupným.

## Tvrdenia zámerne neuplatnené

Na týchto stránkach sa neuvádza medicínsky úžitok, zaručené zobudenie, načasovanie spánkového cyklu, cloudová synchronizácia ani overené verejné iOS vydanie. Nepovažujú ani zdrojovú verziu za živú verziu obchodu. Pozrite si [dostupnosť](availability.md) pre toto rozlíšenie a [súkromie a spoľahlivosť](features/privacy-and-reliability.md) pre dôkazy za formuláciami o lokálnom úložisku a telemetrii.

