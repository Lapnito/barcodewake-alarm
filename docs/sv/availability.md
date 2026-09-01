---
title: BarcodeWake tillgänglighet och versioner
lang: sv
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake tillgänglighet och versioner

BarcodeWake har en verifierad offentlig Google Play-lista för Android. Vid granskningsdatumet visade Google Play version 1.0.0, medan det kontrollerade källprojektet deklarerade version 2.0.0+2. Ingen offentlig App Store-lista verifierades.

## Verifierad offentlig distribution

Android-paketet är offentligt listat som [BarcodeWake: No Cheat Alarm på Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Ögonblicksbilden av butiken som fångades för denna dokumentation rapporterade version 1.0.0 och ett senast uppdaterat datum i mars 2026. Den ögonblicksbilden är bevis på listningen vid en viss tidpunkt, inte ett löfte om att varje region ser samma utrullning eller att listningen förblir oförändrad.

Källträdet innehåller Android- och iOS-plattformsprojekt. Plattformskälla bevisar inte butikpublicering. Eftersom ingen App Store-sida verifierades, beskriver dessa dokument iOS-relaterade objekt som endast källstöd och informerar inte läsarna om att BarcodeWake för närvarande kan laddas ner från Apple.

## Varför två versionsnummer visas

Förvarets `pubspec.yaml` deklarerar källversion 2.0.0+2 och dess changelog beskriver ett bredare missionssystem än den fångade offentliga listningen. En butikutrullning kan ligga efter en utvecklingsgren, vara stegvis per region, eller helt enkelt inte ha publicerats. Utan en matchande butikspost är det säkra uttalandet snävt: funktionen finns i den kontrollerade källan, medan den offentliga tillgängligheten endast är bevisad för den fångade butiksversionen.

När en funktionssida säger "nuvarande källa" är det ordvalet avsiktligt. Innan du förlitar dig på missionskedjor, delningsinställningar eller en annan nyare funktion, kontrollera den installerade appens version och synliga kontroller. Börja med [missionsbeteende](features/missions.md), använd sedan [konfigurationsguiden](guides/set-up-an-alarm.md) endast för alternativ som din installerade version faktiskt visar.

## Enhetskrav och installationskontroller

Scanning kräver kamratillstånd. NFC-, rörelse- och stegmissioner behöver motsvarande enhetshårdvara. Android-alarmleverans kan kräva avisering och exakt alarmåtkomst, med ytterligare batteriinställningar hos vissa tillverkare. Installera från den verifierade butikslistningen, skapa ett närtids-testalarm, lås skärmen och bekräfta både ljud och den valda missionen innan du förlitar dig på det för ett viktigt uppvaknande.

För en koncis gränsliste, läs [produktfakta](facts.md). Om ett testalarm misslyckas, följ [felsökning av alarmleverans](help/alarm-delivery.md) snarare än att upprepade gånger återskapa alarmet.

