---
title: BarcodeWake tilgjengelighet og versjoner
lang: nb
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake tilgjengelighet og versjoner

BarcodeWake har en verifisert offentlig Google Play-oppføring for Android. På revisjonsdatoen viste Google Play versjon 1.0.0, mens det kontrollerte kildeprosjektet erklærte versjon 2.0.0+2. Ingen offentlig App Store-oppføring ble verifisert.

## Verifisert offentlig distribusjon

Android-pakken er offentlig oppført som [BarcodeWake: No Cheat Alarm on Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Øyeblikksbildet av butikken som ble tatt for denne dokumentasjonen rapporterte versjon 1.0.0 og en sist oppdateringsdato i mars 2026. Dette øyeblikksbildet er bevis på oppføringen på et tidspunkt, ikke en forsikring om at alle regioner ser samme utrulling eller at oppføringen forblir uendret.

Kildekoden inneholder Android- og iOS-plattformprosjekter. Plattformkilde beviser ikke butikkpublisering. Fordi ingen App Store-side ble verifisert, beskriver disse dokumentene iOS-relaterte elementer kun som kildebasert støtte og forteller ikke leserne at BarcodeWake for øyeblikket kan lastes ned fra Apple.

## Hvorfor to versjonsnumre vises

Repositoryen `pubspec.yaml` erklærer kildeversjon 2.0.0+2 og dens changelog beskriver et bredere oppdragssystem enn den fangede offentlige oppføringen. En butikkutrulling kan ligge etter en utviklingsgren, være trinnvis fordelt etter region, eller rett og slett ikke ha blitt publisert. Uten en samsvarende butikkpost er det trygge utsagnet snevert: funksjonaliteten eksisterer i den kontrollerte koden, mens offentlig tilgjengelighet kun er bevist for den fangede butikkversjonen.

Når en funksjonsside sier «current source», er ordvalget med vilje. Før du stole på oppdragskjeder, oppsettsdeling eller en annen nyere funksjon, sjekk den installerte appens versjon og synlige kontroller. Start med [oppdragsatferd](features/missions.md), og bruk deretter [oppsettsguiden](guides/set-up-an-alarm.md) kun for alternativer som din installerte versjon faktisk viser.

## Enhetskrav og installasjonskontroller

Skanning krever kameratillatelse. NFC-, bevegelses- og skrittoppdrag trenger tilsvarende maskinvare på enheten. Android alarmlevering kan kreve varsel- og eksakt-alarm-tilgang, med ekstra batteriinnstillinger på enkelte produsenter. Installer fra den verifiserte butikkoppføringen, opprett en nærterminal testalarm, lås skjermen og bekreft både lyd og det valgte oppdraget før du stoler på det for en viktig vekking.

For en konsis grenseliste, les [produkt fakta](facts.md). Hvis en testalarm feiler, følg [alarmleveringsfeilsøking](help/alarm-delivery.md) i stedet for å gjentatte ganger opprette alarmen på nytt.

