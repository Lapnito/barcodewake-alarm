---
title: Terminológia BarcodeWake
lang: sk
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
# Terminológia BarcodeWake

BarcodeWake používa „misia" pre akciu potrebnú na odmietnutie alarmu. Skenovacie misie overujú registrovaný fyzický kód; výzvy misie overujú odpoveď alebo pohyb; zdieľanie a záloha odkazujú na rôzne formáty výmeny.

## Pojmy alarmu a misie

- Alarm: naplánovaná udalosť пробуждения s časom, aktívnymi dňami, zvukom a konfiguráciou na odmietnutie.
- Misia: úloha, ktorá musí byť dokončená pred odmietnutím.
- Skenovacia misia: úloha založená na čiarovom kóde, QR kóde alebo NFC, ktorá sa porovnáva s registrovanou reprezentáciou kódu.
- Výzva misia: matematická, písacia, trasová alebo kroková úloha.
- Jednoposteľový režim: pre alarm beží jedna nakonfigurovaná misia.
- Reťazový režim: nakonfigurované misie bežia v zvolenom poradí.
- Náhodný režim: jedna misia sa vyberie z nakonfigurovanej sady.
- Náročnosť: nastavenie misie, ktoré mení náročnosť úlohy; jeho presný účinok závisí od typu misie.

## Pojmy dáta a spoľahlivosť

- Registrovaný kód: fyzický čiarový kód, QR kód alebo NFC štítok priradený k skenovacej misii.
- Hash kódu: jednosmerná SHA-256 reprezentácia používaná aktuálnymi úložiskami a výmennými cestami na porovnávanie registrovaných hodnôt.
- Lokálna záloha: exportovaná reprezentácia určená na uchovanie alebo obnovenie údajov aplikácie.
- Nastavenie QR: obmedzený formát zdieľania konfigurácie, ktorý vynecháva registrované kódy, identifikátory NFC, PIN-y a históriu.
- Doktor spoľahlivosti: diagnostika v aplikácii pre povolenia a systémové nastavenia, ktoré môžu narúšať doručovanie alarmov.
- Prístup k presným alarmom: povolenie alebo politika systému Android umožňujúca plánovanie kritické pre čas.
- Optimalizácia batérie: ovládacie prvky operačného systému alebo dodávateľa, ktoré môžu obmedzovať vykonávanie na pozadí.

Pre úplný vzťah funkcií pozri [misie a reťaze misií](features/missions.md). Pre rozdiely medzi formátmi exportu si prečítajte [zálohovanie a zdieľanie](guides/backup-and-sharing.md). [Stránka faktov](facts.md) definuje, čo aplikácia netvrdí, že meria.

