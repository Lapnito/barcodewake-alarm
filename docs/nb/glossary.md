---
title: BarcodeWake-terminologi
lang: nb
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

BarcodeWake bruker «oppdrag» for handlingen som kreves for å avvise en alarm. Skanneoppdrag verifiserer en registrert fysisk kode; utfordringsoppdrag verifiserer et svar eller en bevegelse; deling og sikkerhetskopiering refererer til ulike utvekslingsformater.

## Alarm- og oppdragsbegreper

- Alarm: en planlagt vekkehendelse med tid, aktive dager, lyd og avvisningskonfigurasjon.
- Oppdrag: oppgaven som må fullføres før avvisning.
- Skanneoppdrag: en strekkode-, QR- eller NFC-basert oppgave som matches mot en registrert koderepresentasjon.
- Utfordringsoppdrag: en matematikk-, skrive-, riste- eller stegoppgave.
- Enkeltmodus: én konfigurert oppgave kjører for alarmen.
- Lenkemodus: konfigurerte oppdrag kjøres i valgt rekkefølge.
- Tilfeldig modus: én oppgave velges fra et konfigurert sett.
- Vanskelighetsgrad: en oppdragsinnstilling som endrer oppgavekrav; den nøyaktige effekten avhenger av oppdragstype.

## Data- og pålitelighetsbegreper

- Registrert kode: den fysiske strekkoden, QR-koden eller NFC-koden tilknyttet et skannoppdrag.
- Kodehash: en envegs SHA-256-representasjon brukt av gjeldende lagrings- og utvekslingsstier for matching av registrerte verdier.
- Lokal sikkerhetskopi: en eksportert representasjon ment for bevaring eller gjenoppretting av appdata.
- Oppsett-QR: et begrenset konfigurasjonsdelingsformat som utelater registrerte koder, NFC-identifikatorer, PIN-koder og historikk.
- Pålitelighetslege: innebygde diagnoser for tillatelser og systeminnstillinger som kan forstyrre alarmlevering.
- Eksakt alarm-tilgang: Android-systemtillatelse eller -policy som tillater tidskritisk planlegging.
- Batterioptimalisering: operativsystem- eller leverandørkontroller som kan begrense bakgrunnsutførelse.

For den fulle funksjonsrelasjonen, se [oppdrag og oppdragskjeder](features/missions.md). For forskjeller mellom eksportformater, les [sikkerhetskopiering og deling](guides/backup-and-sharing.md). [Fakta-siden](facts.md) definerer hva appen ikke påstår å måle.

