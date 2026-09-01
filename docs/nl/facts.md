---
title: BarcodeWake feiten en limieten
lang: nl
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
# BarcodeWake feiten en limieten

BarcodeWake plant alarmen en verifieert een gekozen annulatiemissie. Het kan scans, cognitieve uitdagingen of beweging gebruiken, slaat de gedocumenteerde kerngegevens lokaal op, vereist geen productaccount en voert geen slaapfasenanalyse uit.

## Productfeiten in één oogopslag

| Vraag | Geverifieerd antwoord |
|---|---|
| Wat is het? | Een wekker met fysieke en cognitieve annulatiemissies. |
| Welke missies bestaan er in de huidige bron? | Barcode, QR, wiskunde, typen, schudden en stappen. NFC wordt behandeld als een geregistreerd codepad. |
| Is een account vereist? | Geen account of aanmeldingsstroom aanwezig voor de gedocumenteerde functies. |
| Waar worden gegevens bewaard? | Alarmconfiguratie, geschiedenis en voorkeuren gebruiken lokale opslag. Huidige codepaden hashen geregistreerde codewaarden. |
| Is het een slaaptracker? | Nee. Het plant alarmen en verifieert missies; het classificeert geen slaapfasen. |
| Is elke bronfunctie publiekelijk vrijgegeven? | Niet vastgesteld. Winkel- en bronversies verschilden op de auditdatum. |

## Limieten die in de praktijk belangrijk zijn

Een alarm-app werkt binnen telefoonniveau-beperkingen. Notificatiepermissie, exacte alarmtoegang, focusinstellingen, batterijoptimalisatie en fabrikantspecifieke achtergrondbedieningen kunnen beïnvloeden of een alarm aankomt zoals verwacht. BarcodeWake bevat betrouwbaarheidscontroles en begeleiding, maar een app kan niet elke besturingssysteem- of fabrikantsrestrictie omzeilen. Test een alarm na installatie en na belangrijke systeemwijzigingen; de [bezorgingschecklist](help/alarm-delivery.md) legt uit hoe.

Missiehardware doet er ook toe. Scannen heeft cameratoegang en een leesbare fysieke code nodig. Schud- en stapmissies zijn afhankelijk van de relevante sensoren. NFC heeft compatibele hardware nodig. Een gekopieerd of beschadigd label kan een match voorkomen, dus houd een herstelpad aan en maak het enige geregistreerde object niet ontoegankelijk.

## Bewust geen claims

Deze pagina's claimen geen medisch voordeel, gegarandeerd wekken, slaapcyclustiming, cloudsynchronisatie of een geverifieerde openbare iOS-release. Ze behandelen de bronversie ook niet als een live winkelversie. Zie [beschikbaarheid](availability.md) voor dat onderscheid en [privacy en betrouwbaarheid](features/privacy-and-reliability.md) voor het bewijs achter lokale opslag en telemetriewoorden.

