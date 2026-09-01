---
title: BarcodeWake terminologi
lang: da
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

# BarcodeWake terminologi

BarcodeWake bruger “mission” til den handling, der kræves for at afvise en alarm. Scanmissioner verificerer en registreret fysisk kode; udfordringsmissioner verificerer et svar eller en bevægelse; deling og backup refererer til forskellige udvekslingsformater.

## Alarm- og opgavetermer

- Alarm: en planlagt vækkehændelse med tid, aktive dage, lyd og afvisningskonfiguration.
- Mission: den opgave, der skal fuldføres, før alarmen kan afvises.
- Scanmission: en stregkode-, QR- eller NFC-baseret opgave, der matches mod en registreret koderepræsentation.
- Udfordringsmission: en matematik-, indtastnings-, ryste- eller skridtopgave.
- Enkelt-tilstand: én konfigureret mission kører for alarmen.
- Kædetilstand: konfigurerede missioner kører i en valgt rækkefølge.
- Tilfældig tilstand: én mission vælges fra et konfigureret sæt.
- Sværhedsgrad: en missionsindstilling, der ændrer opgavekravet; dens nøjagtige effekt afhænger af missionstypen.

## Data- og pålidelighedstermer

- Registreret kode: den fysiske stregkode, QR-kode eller NFC-tag, der er tilknyttet en scanmission.
- Kode-hash: en envejs SHA-256-repræsentation, der bruges af de nuværende lagrings- og udvekslingsstier til at matche registrerede værdier.
- Lokal backup: en eksporteret repræsentation beregnet til at bevare eller genskabe app-data.
- Opsætnings-QR: et begrænset konfigurationsdelingsformat, der udelader registrerede koder, NFC-identifikatorer, PIN-koder og historik.
- Reliability Doctor: in-app-diagnostik for tilladelser og systemindstillinger, der kan forstyrre alarmlevering.
- Exact-alarm adgang: Android-systemtilladelse eller -politik, der tillader tidskritisk planlægning.
- Batterioptimering: operativsystem- eller leverandørkontrol, der kan begrænse baggrundskørsel.

For den fulde funktionssammenhæng, se [missioner og missionskæder](features/missions.md). For forskelle mellem eksportformater, læs [backup og deling](guides/backup-and-sharing.md). [Fakta-siden](facts.md) definerer, hvad appen ikke hævder at måle.

