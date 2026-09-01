---
title: Dostupnost i verzije programa BarcodeWake
lang: hr
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Dostupnost i verzije programa BarcodeWake

BarcodeWake ima provjerenu javnu stranicu na Google Playu za Android. Na datum revizije, Google Play je pokazivao verziju 1.0.0, dok je provjereni izvorni projekt deklarirao verziju 2.0.0+2. Nije pronađena javna stranica na App Storeu.

## Provjerena javna distribucija

Android paket je javno naveden kao [BarcodeWake: Alarm bez varanja na Google Playu](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Snimka trgovine zabilježena za ovu dokumentaciju prijavila je verziju 1.0.0 i datum zadnjeg ažuriranja u ožujku 2026. Ta snimka je dokaz liste u određenom trenutku, a ne jamstvo da svaka regija vidi isto puštanje ili da će lista ostati nepromijenjena.

Izvorno stablo sadrži Android i iOS platformske projekte. Izvorni kod platforme ne dokazuje objavu u trgovini. Budući da nije potvrđena stranica App Storea, ovi dokumenti opisuju stavke vezane uz iOS samo kao podršku izvornog koda i ne govore čitateljima da je BarcodeWake trenutno dostupan za preuzimanje s Applea.

## Zašto se pojavljuju dva broja verzije

Repozitorij `pubspec.yaml` deklarira izvornu verziju 2.0.0+2, a njegov dnevnik promjena opisuje širi sustav misija od uhvaćene javne liste. Puštanje u trgovini može zaostajati za granom razvoja, biti postupno po regijama ili jednostavno nije objavljeno. Bez odgovarajućeg zapisa trgovine, siguran iskaz je uzak: sposobnost postoji u provjerenom izvornom kodu, dok je javna dostupnost dokazana samo za uhvaćenu verziju trgovine.

Kada stranica značajke kaže „trenutni izvor", ta formulacija je namjerna. Prije oslanjanja na lance misija, dijeljenje postavki ili drugu noviju sposobnost, provjerite verziju instalirane aplikacije i vidljive kontrole. Počnite s [ponašanjem misija](features/missions.md), zatim koristite [vodič za postavljanje](guides/set-up-an-alarm.md) samo za opcije koje vaša instalirana verzija zapravo pokazuje.

## Zahtjevi uređaja i provjere instalacije

Skeniranje zahtijeva dopuštenje za kameru. NFC, misije kretanja i koraka zahtijevaju odgovarajući hardver uređaja. Isporuka alarma na Androidu može zahtijevati pristup obavijestima i točnim alarmima, s dodatnim postavkama baterije kod nekih proizvođača. Instalirajte iz provjerene liste trgovine, stvorite kratkoročni testni alarm, zaključajte zaslon i potvrdite zvuk i odabranu misiju prije nego što se oslonite na njega za važno buđenje.

Za sažeti popis ograničenja, pročitajte [činjenice o proizvodu](facts.md). Ako testni alarm ne uspije, slijedite [rješavanje problema s isporukom alarma](help/alarm-delivery.md) umjesto da ponovno stvarate alarm.

