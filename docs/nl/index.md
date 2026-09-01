---
title: BarcodeWake-documentatie
lang: nl
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake-documentatie

BarcodeWake is een wekker die het uitzetten tot een bewuste handeling maakt. Een alarm kan een opgeslagen barcode of QR-code vereisen, een korte cognitieve taak, een schudsequentie of een stappendoel in plaats van alleen te vertrouwen op een eenvoudige knop op het scherm.

## Wat BarcodeWake anders maakt

Het centrale idee is afstand plus intentie. Als de geregistreerde code aan een object buiten het bed is bevestigd, betekent het uitzetten van het alarm opstaan, dat object pakken en het scannen. Hetzelfde alarmmodel kan ook wiskunde, typen, schudden of stapmissies gebruiken. De huidige broncode ondersteunt een enkele missie, een geordende keten of willekeurige selectie uit geconfigureerde missies.

Die wrijving is nuttig voor mensen die een gewoon alarm uitzetten zonder volledig alert te worden. Het is geen slaapfase-analyse, medische begeleiding of een garantie dat iemand wakker wordt. Hardwarondersteuning, machtigingen en batterijcontroles van leveranciers hebben nog steeds invloed op de bezorging. De [missiereferentie](features/missions.md) legt de keuzes uit, terwijl [probleemoplossing voor alarmbezorging](help/alarm-delivery.md) de systeeminstellingen behandelt die kunnen interfereren.

## Begin met het juiste document

Gebruik de [installatiehandleiding](guides/set-up-an-alarm.md) bij het maken van een alarm en het registreren van een fysieke code. Lees [back-up en delen](guides/backup-and-sharing.md) voordat u gegevens verplaatst of een installatie-QR naar iemand anders stuurt. Het deelformaat sluit opzettelijk geregistreerde codes, NFC-identificaties, pincodes en alarmgeschiedenis uit, dus een ontvanger moet gevoelige installatie lokaal voltooien.

Voor een korte, controleerbare samenvatting, zie [productfeiten](facts.md). Voor releasestatus, gebruik [beschikbaarheid](availability.md): de openbare Google Play-versie die voor deze audit is vastgelegd, verschilt van de versie die is gedeclareerd door de gecontroleerde bronboom. De nieuwere bronversie wordt daarom gedocumenteerd als broncapaciteit, niet beweerd als een gepubliceerde winkelrelease.

## Grenzen van privacy en betrouwbaarheid

Kernconfiguratie en missiegegevens worden op het apparaat opgeslagen en geen BarcodeWake-account is vereist. Huidige codepaden vertegenwoordigen geregistreerde codewaarden met SHA-256-hashes. Optionele telemetrie wordt in het privacybeleid beschreven als standaard uitgeschakeld. Deze verklaringen betekenen niet dat elke telefoon alarmen identiek zal bezorgen; Android-leveranciers en besturingssysteemmachtigingen kunnen nog steeds achtergrondgedrag beperken.

Lees [privacy en betrouwbaarheid](features/privacy-and-reliability.md) voor het onderscheid tussen lokale gegevensverwerking en besturingssysteembezorging. De [standaard alarmvergelijking](comparisons/standard-alarm.md) helpt bepalen of missiegebaseerd uitzetten past bij de manier waarop u wakker wordt.

