---
title: Terminologie BarcodeWake
lang: cs
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Terminologie BarcodeWake

BarcodeWake používá termín „mise“ pro akci požadovanou k odklepnutí alarmu. Skenovací mise ověřují registrovaný fyzický kód; výzvové mise ověřují odpověď nebo pohyb; sdílení a záloha označují různé formáty výměny.

## Termíny alarmu a misí

- Alarm: naplánovaná událost probuzení s časem, aktivními dny, zvukem a konfigurací odklepnutí.
- Mise: úkol, který musí být splněn před odklepnutím.
- Skenovací mise: úkol založený na čárovém kódu, QR nebo NFC, který je porovnán s registrovanou reprezentací kódu.
- Výzvová mise: matematický, psací, třesací nebo krokový úkol.
- Jednotlivý režim: pro alarm běží jedna nakonfigurovaná mise.
- Řetězcový režim: nakonfigurované mise běží v zvoleném pořadí.
- Náhodný režim: jedna mise je vybrána z nakonfigurované sady.
- Obtížnost: nastavení mise, které mění náročnost úkolu; jeho přesný účinek závisí na typu mise.

## Termíny dat a spolehlivosti

- Registrovaný kód: fyzický čárový kód, QR kód nebo NFC štítek přidružený ke skenovací misi.
- Kódový hash: jednosměrná SHA-256 reprezentace používaná aktuálními cestami ukládání a výměny pro porovnávání registrovaných hodnot.
- Lokální záloha: exportovaná reprezentace určená k uchování nebo obnovení dat aplikace.
- Nastavovací QR: omezený formát sdílení konfigurace, který vynechává registrované kódy, NFC identifikátory, PINy a historii.
- Spolehlivostní lékař: diagnostika v aplikaci pro oprávnění a systémová nastavení, která mohou narušovat doručení alarmu.
- Přístup k přesnému alarmu: systémové oprávnění nebo zásada Androidu umožňující časově kritické plánování.
- Optimalizace baterie: ovládací prvky operačního systému nebo dodavatele, které mohou omezovat běh na pozadí.

Úplný vztah funkcí naleznete v [mise a řetězce misí](features/missions.md). Rozdíly mezi exportními formáty si přečtěte v [záloha a sdílení](guides/backup-and-sharing.md). [Stránka faktů](facts.md) definuje, co aplikace netvrdí, že měří.

