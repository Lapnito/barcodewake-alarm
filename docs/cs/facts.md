---
title: Fakta a omezení BarcodeWake
lang: cs
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
# Fakta a omezení BarcodeWake

BarcodeWake plánuje budíky a ověřuje zvolenou odkládací misi. Může využívat skenování, kognitivní výzvy nebo pohyb, ukládá dokumentovaná základní data lokálně, nevyžaduje produkt účet a neprovádí analýzu fází spánku.

## Přehled faktů o produktu

| Otázka | Ověřená odpověď |
|---|---|
| Co to je? | Budík s fyzickými a kognitivními úkoly k odložení. |
| Jaké úkoly existují v aktuálním zdrojovém kódu? | Čárový kód, QR, matematika, psaní, třesení a kroky. NFC je zpracován jako registrovaná cesta kódu. |
| Je vyžadován účet? | Pro dokumentované funkce není přítomen žádný účet ani přihlašovací proces. |
| Kde jsou data uchovávána? | Konfigurace budíků, historie a předvolby využívají lokální úložiště. Aktuální cesty kódu hašují hodnoty registrovaných kódů. |
| Je to sledovač spánku? | Ne. Plánuje budíky a ověřuje úkoly; nezařazuje fáze spánku. |
| Je každá funkce zdrojového kódu veřejně vydána? | Není stanoveno. Verze obchodu a zdroje se lišily k datu auditu. |

## Omezení, která jsou důležitá v praxi

Aplikace budíku funguje v rámci omezení na úrovni telefonu. Oprávnění k oznámením, přístup k přesným budíkům, nastavení fokusu, optimalizace baterie a vendor-specifické ovládání na pozadí mohou ovlivnit, zda budík dorazí podle očekávání. BarcodeWake obsahuje kontroly spolehlivosti a pokyny, ale aplikace nemůže přepsat každé omezení operačního systému nebo výrobce. Otestujte budík po instalaci a po významných změnách systému; [kontrolní seznam doručení](help/alarm-delivery.md) vysvětluje jak.

Hardware mise také záleží. Skenování vyžaduje přístup k fotoaparátu a čitelný fyzický kód. Mise třesení a kroků závisí na příslušných senzorech. NFC potřebuje kompatibilní hardware. Zkopírovaný nebo poškozený štítek může zabránit shodě, takže si udržte záložní cestu a nedělejte jediný registrovaný objekt nepřístupným.

## Záměrně neuváděné tvrzení

Tyto stránky neuvádějí lékařský přínos, zaručené probuzení, načasování spánkového cyklu, cloudovou synchronizaci ani ověřené veřejné vydání pro iOS. Také nelikvidují zdrojovou verzi jako živou obchodní verzi. Viz [dostupnost](availability.md) pro toto rozlišení a [soukromí a spolehlivost](features/privacy-and-reliability.md) pro důkazy za lokálním úložištěm a formulací telemetrie.

