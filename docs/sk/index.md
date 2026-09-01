---
title: BarcodeWake dokumentácia
lang: sk
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake dokumentácia

BarcodeWake je budík, ktorý premieňa odmietnutie na zámeraný úkon. Budík môže vyžadovať uložený čiarový kód alebo QR kód, krátku kognitívnu úlohu, sekvenciu potreskania alebo cieľ krokov namiesto toho, aby sa spoliehal len na jednoduché tlačidlo na obrazovke.

## Čo robí BarcodeWake iným

Centrálnym konceptom je vzdialenosť a úmysel. Ak je registrovaný kód pripojený k objektu ďaleko od postele, stíšenie budíka znamená vstať, dosiahnuť k tomuto objektu a naskenovať ho. Ten istý model budíka môže tiež využívať matematiku, písanie, trasenie alebo misie krokov. Aktuálny zdrojový kód podporuje jednu misiu, usporiadaný reťazec alebo náhodný výber z nakonfigurovaných misií.

Toto trenie je užitočné pre ľudí, ktorí odmietajú bežný budík bez toho, aby sa stali úplne bdelými. Nie je to analýza spánkových fáz, lekárske vedenie ani záruka, že niekto sa zobudí. Hardvérová podpora, povolenia a kontroly batérie od predajcov stále ovplyvňujú doručovanie. [Referencia misií](features/missions.md) vysvetľuje možnosti, zatiaľ čo [riešenie problémov s doručovaním budíka](help/alarm-delivery.md) pokrýva nastavenia systému, ktoré môžu zasahovať.

## Začnite správnym dokumentom

Použite [príručku nastavenia](guides/set-up-an-alarm.md) pri vytváraní budíka a registrácii fyzického kódu. Prečítajte si [zálohovanie a zdieľanie](guides/backup-and-sharing.md) pred presunom dát alebo odoslaním nastavovacieho QR kódu niekomu inému. Formát zdieľania zámerne vylučuje registrované kódy, identifikátory NFC, PINy a históriu budíkov, takže príjemca musí dokončiť citlivé nastavenie lokálne.

Pre krátky, auditeľný súhrn si pozrite [fakty o produkte](facts.md). Pre stav vydania použite [dostupnosť](availability.md): verejná verzia z Google Play zachytená pre tento audit sa líši od verzie deklarovanej kontrolovaným stromom zdrojového kódu. Novšia verzia zdroja je preto zdokumentovaná ako schopnosť zdroja, nie ako tvrdenie o vydaní v obchode.

## Hranice súkromia a spoľahlivosti

Jadro konfigurácie a údaje o misii sú uložené v zariadení a nie je potrebný žiadny účet BarcodeWake. Aktuálne cesty kódu reprezentujú hodnoty registrovaných kódov pomocou hashov SHA-256. Voliteľná telemetria je popísaná v zásadách ochrany osobných údajov ako predvolene zakázaná. Tieto vyhlásenia neznamenajú, že každý telefón bude doručovať budíky identicky; predajcovia Android a povolenia operačného systému môžu stále obmedzovať správanie na pozadí.

Prečítajte si [súkromie a spoľahlivosť](features/privacy-and-reliability.md) pre rozlíšenie medzi lokálnym spracovaním údajov a doručovaním operačným systémom. [Porovnanie so štandardným budíkom](comparisons/standard-alarm.md) pomáha rozhodnúť, či odmietnutie založené na misiách zodpovedá spôsobu, akým sa budíte.

