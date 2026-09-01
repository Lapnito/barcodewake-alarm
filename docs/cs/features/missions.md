---
title: Mise a řetězce misí BarcodeWake
lang: cs
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
# Mise a řetězce misí BarcodeWake

BarcodeWake mise je podmínka použitá k vypnutí alarmu. Aktuální zdroj podporuje úlohy s čárovými kódy, QR kódy, matematikou, psaním, třesením a kroky, přičemž registrovaná NFC se zpracovává přes cestu skenování kódu. Mise mohou běžet samostatně, v pořadí nebo náhodným výběrem.

## Skenovací mise vytvářejí fyzickou vzdálenost

Mise s čárovým nebo QR kódem porovnává živý snímek z kamery s kódem registrovaným během nastavení. Kód lze umístit na objekt mimo dosah ruky: toaletní potřeby v koupelně, snídaňovou položku v kuchyni nebo jiný stabilní objekt v dobře osvětlené oblasti. NFC následuje stejnou obecnou myšlenku s kompatibilním tagem a zařízením. Aplikace ukládá hash reprezentaci v aktuálních cestách namísto potřeby surového kódu pro běžné porovnání.

Zvolte objekt, který bude k dispozici, když alarm zazní. Obaly se vyhazují, štítky blednou a cestování mění prostředí. Registrace kódu na jediné krabičce léků, kterou možná budete muset vyměnit, je méně robustní než použití trvanlivého štítku. [Průvodce nastavením alarmu](../guides/set-up-an-alarm.md) pokrývá umístění a testování.

## Náročné mise vyměňují pohyb za úsilí

Matematika a psaní vyžadují soustředěný vstup. Třesení a kroky vyžadují fyzický pohyb a podporované senzory. Nastavení obtížnosti a cíle mění, kolik práce se očekává, ale náročnější mise není automaticky lepší. Nadměrné tření může podporovat úplné deaktivování alarmu, zatímco snadný úkol se může po opakování stát automatickým.

Přizpůsobte úkol režimu selhání. Pokud vypínáte alarmy napůl spící, skenování v jiné místnosti vytváří užitečnou vzdálenost. Pokud je přístup ke kameře nepohodlný, krátký úkol psaní nebo matematiky může být praktičtější. Pokud jde o mobilitu, rovnováhu nebo přístupnost, vyhněte se misím založeným na pohybu a zvolte úkol, který lze bezpečně dokončit.

## Režimy Single, Chain a Random

Režim Single žádá o jednu nakonfigurovanou misi. Režim Chain spouští několik nakonfigurovaných misí v pořadí. Režim Random vybírá z nakonfigurované sady, čímž snižuje šanci, že se jedna zapamatovaná interakce stane automatickou. Tyto režimy jsou přítomny v novějším kontrolovaném zdroji; [dostupnost](../availability.md) vysvětluje, proč to neprokazuje, že jsou již v každé veřejné verzi.

Vždy spusťte test v blízkém časovém horizontu po změně režimu, oprávnění nebo registrovaných objektů. Udržujte vybraný objekt dosažitelný a poskytněte bezpečnou cestu obnovy. Pro problémy s doručením nesouvisející s dokončením mise použijte [kontrolní seznam spolehlivosti](../help/alarm-delivery.md).

