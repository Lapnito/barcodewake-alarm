---
title: Dostupnosť a verzie aplikácie BarcodeWake
lang: sk
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Dostupnosť a verzie aplikácie BarcodeWake

Aplikácia BarcodeWake má overený verejný záznam v obchode Google Play pre Android. V deň auditu Google Play zobrazoval verziu 1.0.0, zatiaľ čo kontrolovaný zdrojový projekt deklaroval verziu 2.0.0+2. Neboli overené žiadne verejné záznamy v App Store.

## Overená verejná distribúcia

Android balík je verejne uvedený ako [BarcodeWake: No Cheat Alarm na Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Snímka obchodu zachytená pre túto dokumentáciu hlásila verziu 1.0.0 a dátum poslednej aktualizácie v marci 2026. Táto snímka je dôkazom záznamu v danom čase, nie zárukou, že každý región vidí rovnaké zavedenie alebo že záznam zostane nezmenený.

Zdrojový strom obsahuje projekty platforiem Android a iOS. Zdroj platformy nepreukazuje publikáciu v obchode. Keďže žiadna stránka App Store nebola overená, tieto dokumenty popisujú položky súvisiace s iOS iba ako podporu zo zdroja a neinformujú čitateľov, že aplikácia BarcodeWake je momentálne stiahnuteľná od spoločnosti Apple.

## Prečo sa zobrazujú dve čísla verzií

Repositár `pubspec.yaml` deklaruje zdrojovú verziu 2.0.0+2 a jeho zoznam zmien popisuje širší systém misií ako zachytený verejný záznam. Zavedenie v obchode môže zaostať za vývojovou vetvou, byť fázované podľa regiónu, alebo jednoducho nebyť publikované. Bez zodpovedajúceho záznamu v obchode je bezpečné tvrdenie úzke: schopnosť existuje v kontrolovanom zdroji, zatiaľ čo verejná dostupnosť je preukázaná iba pre zachytenú verziu obchodu.

Keď stránka funkcií hovorí „aktuálny zdroj", toto formulovanie je úmyselné. Pred spoliehaním sa na reťazce misií, zdieľanie nastavení alebo inú novšiu schopnosť, skontrolujte verziu nainštalovanej aplikácie a viditeľné ovládacie prvky. Začnite so [správaním misií](features/missions.md), potom použite [príručku nastavenia](guides/set-up-an-alarm.md) iba pre možnosti, ktoré vaša nainštalovaná verzia skutočne zobrazuje.

## Požiadavky na zariadenie a kontroly inštalácie

Skenovanie vyžaduje povolenie fotoaparátu. NFC, pohybové a krokové misie vyžadujú zodpovedajúci hardvér zariadenia. Doručenie budíka v Android môže vyžadovať prístup k notifikáciám a presnému budíku, s ďalšími nastaveniami batérie u niektorých výrobcov. Inštalujte z overeného záznamu v obchode, vytvorte krátkodobý testovací budík, zamknite obrazovku a potvrďte zvuk aj vybranú misiu pred tým, ako sa na ňu budete spoliehať pri dôležitom budíku.

Pre stručný zoznam hraníc si prečítajte [fakty o produkte](facts.md). Ak testovací budík zlyhá, postupujte podľa [riešenia problémov s doručením budíka](help/alarm-delivery.md) namiesto opakovaného vytvárania budíka.

