---
title: BarcodeWake privacy en betrouwbaarheid van alarmen
lang: nl
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake privacy en betrouwbaarheid van alarmen

BarcodeWake bewaart gedocumenteerde alarmconfiguratie en missiegegevens op het apparaat en vereist geen app-account. Huidige codepaden hashen geregistreerde codewaarden. Optionele telemetrie wordt beschreven als standaard uitgeschakeld, terwijl alarmbezorging nog steeds afhangt van systeemmachtigingen en leverancierscontroles.

## Lokale gegevens verwijderen geen systeemafhankelijkheden

Lokale opslag betekent dat gewone alarmconfiguratie geen BarcodeWake-cloudaccount vereist. Alarmrecords, geschiedenis en voorkeuren worden verwerkt via de lokale gegevenslaag van de app. Geregistreerde barcode-, QR- en NFC-waarden worden weergegeven met SHA-256-hashes in huidige opslag- en importpaden, wat voorkomt dat de gewone onbewerkte waarde wordt bewaard voor matching.

Hashing is niet hetzelfde als encryptie van elk app-record, en lokale opslag is geen back-up. Iemand met toegang tot een ontgrendeld apparaat kan nog steeds alarmnamen, schema's of geschiedenis zien via de app. Een verloren of gereset telefoon kan ook lokale gegevens verliezen tenzij de gebruiker een export heeft gemaakt. Zie [back-up en delen](../guides/backup-and-sharing.md) voor de formaten en hun verschillende doeleinden.

Het privacybeleid zegt dat optionele telemetrie standaard uit is en beschrijft geaggregeerde verwerking indien ingeschakeld. Deze documentatie doet daarom niet de bredere bewering dat de app nooit over een netwerk kan communiceren. Het stelt de smallere geverifieerde feiten: kernoperatie en gegevens zijn lokaal, geen productaccount is vereist, en geen advertentie-SDK-afhankelijkheid verschijnt in het gecontroleerde project.

## Betrouwbaarheid is een gedeelde verantwoordelijkheid

BarcodeWake kan een alarm plannen en presenteren, maar het besturingssysteem beslist wanneer achtergrondwerk mag worden uitgevoerd en welke onderbrekingen zijn toegestaan. Meldingstoestemming, toegang tot exact-alarm, stille of focusmodi, batterijoptimalisatie, automatische app-onderbreking en fabrikantstaakkillers kunnen allemaal van belang zijn. De betrouwbaarheidstools in de app kunnen configuratierisico's identificeren en gebruikers naar instellingen leiden; ze kunnen het systeembeleid niet overschrijven.

Na installatie testen met het scherm vergrendeld en de telefoon in dezelfde stroommodus die 's nachts wordt gebruikt. Herhaal die test na een systeemupdate, batterijbesparingswijziging of app-herinstallatie. Houd het apparaat opgeladen, het volume apropraat en de gekozen missie fysiek beschikbaar. Volg [probleemoplossing voor alarmbezorging](../help/alarm-delivery.md) wanneer een test mislukt.

## Waar privacy en betrouwbaarheid geen beloften over doen

BarcodeWake is geen medisch hulpmiddel, noodwaarschuwingsservice of slaapfasetracker. Geen alarmapp kan garanderen dat je wakker wordt of kan compenseren voor een niet-beschikbaar apparaat. De [feiten en limieten pagina](../facts.md) vermeldt deze grenzen, terwijl [beschikbaarheid](../availability.md) openbaar bewijs van winkels scheidt van nieuwere bronmogelijkheden.

