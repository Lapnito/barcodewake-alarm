---
title: BarcodeWake-terminologi
lang: sv
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
# BarcodeWake-terminologi

BarcodeWake använder “uppdrag” för den åtgärd som krävs för att avfärda ett alarm. Skanningsuppdrag verifierar en registrerad fysisk kod; utmaningsuppdrag verifierar ett svar eller en rörelse; delning och backup avser olika utbytesformat.

## Alarm- och uppdragstermer

- Alarm: ett schemalagt väckningstillfälle med tid, aktiva dagar, ljud och avfärdningskonfiguration.
- Uppdrag: uppgiften som måste utföras innan avfärdning.
- Skanningsuppdrag: en streckkod, QR- eller NFC-baserad uppgift som matchas mot en registrerad kodrepresentation.
- Utmaningsuppdrag: en matte-, skriv-, skak- eller steguppgift.
- Enkelläge: ett konfigurerat uppdrag körs för alarmet.
- Kedjeläge: konfigurerade uppdrag körs i en vald ordning.
- Slumpmässigt läge: ett uppdrag väljs från en konfigurerad uppsättning.
- Svårighetsgrad: en uppdragsinställning som ändrar uppgiftskrav; dess exakta effekt beror på uppdragstyp.

## Data- och tillförlitlighetstermer

- Registrerad kod: den fysiska streckkoden, QR-koden eller NFC-taggen som är kopplad till ett skanningsuppdrag.
- Kodhash: en envägs SHA-256-representation som används av aktuella lagrings- och utbytesvägar för att matcha registrerade värden.
- Lokal backup: en exporterad representation avsedd att bevara eller återställa appdata.
- Setup-QR: ett begränsat konfigurationsdelningsformat som utelämnar registrerade koder, NFC-identifikatorer, PIN-koder och historik.
- Tillförlitlighetsdoktorn: inbyggda diagnostik för behörigheter och systeminställningar som kan störa alarminleverans.
- Exakt alarm-åtkomst: Android-systembehörighet eller policy som tillåter tidskritiskt schemaläggande.
- Batterioptimering: operativsystem- eller leverantörskontroller som kan begränsa bakgrundskörning.

För fullständig funktionsrelation, se [uppdrag och uppdragskedjor](features/missions.md). För skillnader mellan exportformat, läs [backup och delning](guides/backup-and-sharing.md). [Faktasidan](facts.md) definierar vad appen inte påstår sig mäta.

