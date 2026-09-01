---
title: BarcodeWake fakta og begrænsninger
lang: da
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
# BarcodeWake fakta og begrænsninger

BarcodeWake planlægger alarmer og verificerer en valgt afvisningsopgave. Den kan bruge scanninger, kognitive udfordringer eller bevægelse, gemmer de dokumenterede kernedata lokalt, kræver ingen produktkonto og udfører ikke søvnstadieanalyse.

## Produktfakta på et øjeblik

| Spørgsmål | Verificeret svar |
|---|---|
| Hvad er det? | En alarmclock med fysiske og kognitive afvisningsopgaver. |
| Hvilke opgaver findes i den aktuelle kilde? | Stregkode, QR, matematik, tastning, ryst og skridt. NFC håndteres som en registreret kodesti. |
| Er en konto påkrævet? | Ingen konto eller loginflow er til stede for de dokumenterede funktioner. |
| Hvor opbevares data? | Alarmkonfiguration, historik og præferencer bruger lokal lagring. Aktuelle kodestier hash-er registrerede kodeværdier. |
| Er det en søvntracker? | Nej. Den planlægger alarmer og verificerer opgaver; den klassificerer ikke søvnstadier. |
| Er alle kildfunktioner offentligt udgivet? | Ikke fastslået. Butik- og kildeversioner var forskellige på auditdatoen. |

## Begrænsninger der betyder noget i praksis

En alarmapp opererer inden for telefon-niveau begrænsninger. Notifikationstilladelse, præcis alarm-adgang, fokusindstillinger, batterioptimering og producent-specifikke baggrundskontroller kan påvirke, om en alarm kommer som forventet. BarcodeWake inkluderer pålidelighedskontroller og vejledning, men en app kan ikke tilsidesætte alle operativsystem- eller producentbegrænsninger. Test en alarm efter installation og efter større systemændringer; [leveringschecklisten](help/alarm-delivery.md) forklarer hvordan.

Missionens hardware betyder også noget. Scanning kræver kameraadgang og en læsbar fysisk kode. Ryst- og skridtopgaver afhænger af de relevante sensorer. NFC kræver kompatibel hardware. En kopieret eller beskadiget etiket kan forhindre et match, så hold en gendannelsessti og gør ikke det eneste registrerede objekt utilgængeligt.

## Påstande der med vilje ikke fremsættes

Disse sider hævder ikke medicinsk fordel, garanteret vækning, søvncyklus-timing, cloudsynkronisering eller en verificeret offentlig iOS-udgivelse. De behandler heller ikke kildeversionen som en live butiksversion. Se [tilgængelighed](availability.md) for den distinktion og [privatliv og pålidelighed](features/privacy-and-reliability.md) for beviserne bag lokal lagring og telemetriordlyd.

