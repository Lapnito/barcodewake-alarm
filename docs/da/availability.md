---
title: BarcodeWake tilgængelighed og versioner
lang: da
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---

# BarcodeWake tilgængelighed og versioner

BarcodeWake har en bekræftet offentlig Google Play-listing for Android. På revisionsdatoen viste Google Play version 1.0.0, mens det kontrollerede kildeprojekt erklærede version 2.0.0+2. Ingen offentlig App Store-listing blev bekræftet.

## Bekræftet offentlig distribution

Android-pakken er offentligt listet som [BarcodeWake: No Cheat Alarm på Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Butikssnapshotet, der blev registreret til denne dokumentation, rapporterede version 1.0.0 og en sidst-opdateret dato i marts 2026. Dette snapshot er bevis for listingen på et tidspunkt, ikke en løfte om, at alle regioner ser den samme udrulning, eller at listingen forbliver uændret.

Kildeträet indeholder Android- og iOS-platformprojekter. Platforms kildekode beviser ikke butikspublikation. Da ingen App Store-side blev bekræftet, beskriver disse docs iOS-relaterede elementer som kun kildeunderstøttelse og fortæller ikke læserne, at BarcodeWake aktuelt kan downloades fra Apple.

## Hvorfor to versionsnumre vises

Repositoryen `pubspec.yaml` erklærer kildeversion 2.0.0+2, og dens changelog beskriver et bredere missionssystem end den fangede offentlige listing. En butiksrulning kan være bagud i forhold til en udviklingsgren, være faset efter region eller blot ikke være udgivet. Uden en matchende butiksregistrering er det sikre udsagn snævert: funktionaliteten findes i den kontrollerede kilde, mens offentlig tilgængelighed kun er bevist for den fangede butiksversion.

Når en funktionsside siger „aktuel kilde”, er den formulering med vilje. Før du stoler på missionskæder, deling af opsætning eller en anden nyere funktion, skal du kontrollere den installerede apps version og synlige kontrolelementer. Start med [missionsadfærd](features/missions.md), og brug derefter [opsætningsguiden](guides/set-up-an-alarm.md) kun for de indstillinger, din installerede build faktisk viser.

## Enheds‑krav og installationskontrol

Scanning kræver kameratilladelse. NFC-, bevægelses- og skridtmissioner kræver tilsvarende enhedshardware. Android-alarmlevering kan kræve notifikation og præcis-alarm-adgang, med ekstra batteriindstillinger hos nogle producenter. Installer fra den bekræftede butikslisting, opret en testalarm på kort sigt, lås skærmen og bekræft både lyd og den valgte mission, før du stoler på den til en vigtig opvågning.

For en kort afgrænsningsliste, læs [produktoplysninger](facts.md). Hvis en testalarm fejler, skal du følge [alarmleveringsfejlfinding](help/alarm-delivery.md) i stedet for gentagne gange at genskabe alarmen.

