---
title: BarcodeWake fakta og begrensninger
lang: nb
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
# BarcodeWake fakta og begrensninger

BarcodeWake planlegger alarmer og bekrefter en valgt avvisningsoppgave. Den kan bruke skanninger, kognitive utfordringer eller bevegelse, lagrer den dokumenterte kjerneinformasjonen lokalt, krever ingen produktkonto, og utfører ikke søvnfaseanalyse.

## Produktfakta på et øyeblikk

| Spørsmål | Verifisert svar |
|---|---|
| Hva er det? | En vekkerklokke med fysiske og kognitive avvisningsoppgaver. |
| Hvilke oppgaver finnes i gjeldende kilde? | Strekkode, QR, matematikk, skriving, risting og steg. NFC håndteres som en registrert kodevei. |
| Er en konto nødvendig? | Ingen konto eller påloggingsflyt er til stede for de dokumenterte funksjonene. |
| Hvor lagres data? | Alarmkonfigurasjon, historikk og preferanser bruker lokal lagring. Gjeldende kodeveier hasher registrerte kodeverdier. |
| Er det en søvnfølger? | Nei. Den planlegger alarmer og bekrefter oppgaver; den klassifiserer ikke søvnfaser. |
| Er hver kildefunksjon offentlig utgitt? | Ikke fastslått. Butikk- og kildeversjoner varierte på revisjonsdatoen. |

## Begrensninger som betyr noe i praksis

En alarmapp opererer innenfor telefonnivå-begrensninger. Tillatelse for varsler, tilgang til eksakte alarmer, fokusinnstillinger, batterioptimalisering og leverandørspesifikke bakgrunnskontroller kan påvirke om en alarm kommer som forventet. BarcodeWake inkluderer pålitelighetskontroller og veiledning, men en app kan ikke overstyre alle operativsystem- eller produsentbegrensninger. Test en alarm etter installasjon og etter store systemendringer; [leveringssjekklisten](help/alarm-delivery.md) forklarer hvordan.

Oppgaverelert maskinvare betyr også noe. Skanning krever kameratilgang og en lesbar fysisk kode. Riste- og stegoppgaver avhenger av de relevante sensorene. NFC trenger kompatibel maskinvare. En kopiert eller skadet etikett kan forhindre en match, så ha en gjenopprettingsvei og gjør ikke det eneste registrerte objektet utilgjengelig.

## Påstander som bevisst ikke er fremsatt

Disse sidene fremsetter ingen påstander om medisinsk nytte, garantert vekking, søvnsirkeltiming, skylagring eller en verifisert offentlig iOS-utgivelse. De behandler heller ikke kildeversjonen som en live butikkversjon. Se [tilgjengelighet](availability.md) for den distinksjonen og [personvern og pålitelighet](features/privacy-and-reliability.md) for bevisene bak lokale lagrings- og telemetriotale.

