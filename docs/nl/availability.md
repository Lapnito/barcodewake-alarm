---
title: BarcodeWake-beschikbaarheid en versies
lang: nl
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake-beschikbaarheid en versies

BarcodeWake heeft een geverifieerde openbare vermelding op Google Play voor Android. Op de auditdatum toonde Google Play versie 1.0.0, terwijl het gecontroleerde bronproject versie 2.0.0+2 verklaarde. Er is geen openbare App Store-vermelding geverifieerd.

## Geverifieerde openbare distributie

Het Android-pakket is openbaar vermeld als [BarcodeWake: Geen valsspeler-alarm op Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). De winkelsnapshot vastgelegd voor deze documentatie rapporteerde versie 1.0.0 en een laatst-bijgewerkt datum in maart 2026. Die snapshot is bewijs van de vermelding op een bepaald moment, geen belofte dat elke regio dezelfde uitrol ziet of dat de vermelding ongewijzigd zal blijven.

De bronboom bevat Android- en iOS-platformprojecten. Platformbron bewijst geen winkelpublicatie. Omdat er geen App Store-pagina is geverifieerd, beschrijven deze docs iOS-gerelateerde items alleen als bronondersteuning en vertellen ze lezers niet dat BarcodeWake momenteel downloadbaar is van Apple.

## Waarom twee versienummers verschijnen

Het repository `pubspec.yaml` verklaart bronversie 2.0.0+2 en de changelog beschrijft een breder missiesysteem dan de vastgelegde openbare vermelding. Een winkelimplementatie kan achterlopen op een ontwikkelingstak, per regio worden gefaseerd, of gewoon niet zijn gepubliceerd. Zonder een overeenkomend winkeliercord is de veilige verklaring beperkt: de mogelijkheid bestaat in de gecontroleerde bron, terwijl openbare beschikbaarheid alleen bewezen is voor de vastgelegde winkelversie.

Wanneer een featurepagina "huidige bron" zegt, is die formulering bewust. Voordat u vertrouwt op missieketens, setup-delen of een andere nieuwere mogelijkheid, controleer de versie van de geïnstalleerde app en zichtbare bedieningselementen. Begin met [missiegedrag](features/missions.md), gebruik dan de [installatiegids](guides/set-up-an-alarm.md) alleen voor opties die uw geïnstalleerde build daadwerkelijk toont.

## Apparaatvereisten en installatiecontroles

Scannen vereist cameramachtiging. NFC-, bewegings- en stapmissies hebben overeenkomstige apparaathardware nodig. Android-alarmbezorging kan meldings- en exacte-alarmtoegang vereisen, met extra batterij-instellingen bij sommige fabrikanten. Installeer vanaf de geverifieerde winkelvermelding, maak een nabije testalarm, vergrendel het scherm en bevestig zowel geluid als de geselecteerde missie voordat u ervan afhankelijk bent voor een belangrijk wekken.

Voor een beknopte grenslijst, lees [productfeiten](facts.md). Als een testalarm mislukt, volg dan [alarmbezorging probleemoplossing](help/alarm-delivery.md) in plaats van de alarm herhaaldelijk opnieuw te maken.

