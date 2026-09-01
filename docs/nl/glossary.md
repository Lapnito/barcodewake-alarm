---
title: BarcodeWake-terminologie
lang: nl
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
# BarcodeWake-terminologie

BarcodeWake gebruikt "missie" voor de actie die nodig is om een alarm uit te schakelen. Scanmissies verifiëren een geregistreerde fysieke code; uitdagingsmissies verifiëren een antwoord of beweging; delen en back-up verwijzen naar verschillende uitwisselingsformaten.

## Alarm- en missietermen

- Alarm: een gepland wekgebeurtenis met tijd, actieve dagen, geluid en uitschakelconfiguratie.
- Missie: de taak die moet worden voltooid voordat het alarm wordt uitgeschakeld.
- Scanmissie: een op barcode, QR of NFC gebaseerde taak die wordt afgezet tegen een geregistreerde coderepresentatie.
- Uitdagingsmissie: een wiskunde-, type-, schud- of staptaak.
- Enkele modus: één geconfigureerde missie wordt uitgevoerd voor het alarm.
- Kettingmodus: geconfigureerde missies worden in een gekozen volgorde uitgevoerd.
- Willekeurige modus: één missie wordt geselecteerd uit een geconfigureerde set.
- Moeilijkheidsgraad: een missie-instelling die de taakeisen wijzigt; het exacte effect is afhankelijk van het missietype.

## Gegevens- en betrouwbaarheidstermen

- Geregistreerde code: de fysieke streepjescode, QR-code of NFC-tag die aan een scanmissie is gekoppeld.
- Code-hash: een eenweg SHA-256-representatie die wordt gebruikt door huidige opslag- en uitwisselingspaden voor het afstemmen van geregistreerde waarden.
- Lokale back-up: een geëxporteerde representatie bedoeld om app-gegevens te bewaren of te herstellen.
- Setup QR: een beperkt configuratie-deelformaat dat geregistreerde codes, NFC-identificatoren, pincodes en geschiedenis weglaat.
- Betrouwbaarheidsdokter: in-app diagnostiek voor machtigingen en systeeminstellingen die alarmlevering kunnen verstoren.
- Exact-alarm toegang: Android-systeemmachtiging of -beleid voor tijd-kritische planning.
- Batterijoptimalisatie: besturingssysteem- of leverancierscontroles die achtergronduitvoering kunnen beperken.

Zie voor de volledige feature-relatie [missies en missieketens](features/missions.md). Voor verschillen tussen exportformaten lees [back-up en delen](guides/backup-and-sharing.md). Op de [feitenpagina](facts.md) wordt gedefinieerd wat de app niet beweert te meten.

