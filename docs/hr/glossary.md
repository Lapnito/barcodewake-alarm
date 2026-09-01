---
title: BarcodeWake terminologija
lang: hr
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

# BarcodeWake terminologija

BarcodeWake koristi „misiju“ za radnju potrebnu za odbacivanje alarma. Skeniranje misija provjerava registrirani fizički kod; izazovne misije provjeravaju odgovor ili kretanje; dijeljenje i sigurnosna kopija odnose se na različite formate razmjene.

## Alarm i pojmovi o misijama

- Alarm: zakazani događaj buđenja s vremenom, aktivnim danima, zvukom i konfiguracijom odbacivanja.
- Misija: zadatak koji mora biti izvršen prije odbacivanja.
- Skeniranje misije: zadatak temeljen na barkodu, QR-u ili NFC-u koji se podudara s registriranom reprezentacijom koda.
- Izazovna misija: matematički, tipkarski, potresni ili korak zadatak.
- Pojedinačni način: za alarm se pokreće jedna konfigurirana misija.
- Lančani način: konfigurirane misije pokreću se u odabranom redoslijedu.
- Nasumični način: jedna misija odabire se iz skupa konfiguriranih misija.
- Težina: postavka misije koja mijenja zahtjevnost zadatka; njezin točan učinak ovisi o vrsti misije.

## Pojmovi o podacima i pouzdanosti

- Registrirani kod: fizički barkod, QR kod ili NFC oznaka pridružena skeniranju misije.
- Sažetak koda: jednosmjerna SHA-256 reprezentacija koju trenutni putevi pohrane i razmjene koriste za usklađivanje registriranih vrijednosti.
- Lokalna sigurnosna kopija: izvezena reprezentacija namijenjena očuvanju ili obnavljanju podataka aplikacije.
- Postavni QR: ograničeni format dijeljenja konfiguracije koji izostavlja registrirane kodove, NFC identifikatore, PIN-ove i povijest.
- Doktor pouzdanosti: dijagnostika unutar aplikacije za dozvole i sistemske postavke koje mogu ometati isporuku alarma.
- Pristup točnom alarmu: Android sistemska dozvola ili pravila koja omogućuju vremenski kritično raspoređivanje.
- Optimizacija baterije: kontrole operacijskog sustava ili dobavljača koje mogu ograničiti izvršavanje u pozadini.

Za potpuni odnos značajki pogledajte [misije i lanac misija](features/missions.md). Za razlike između formata izvoza pročitajte [sigurnosna kopija i dijeljenje](guides/backup-and-sharing.md). [Stranica s činjenicama](facts.md) definira što aplikacija ne tvrdi da mjeri.

