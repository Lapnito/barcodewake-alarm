---
title: Sikkerhedskopier og del BarcodeWake-alarmer
lang: da
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Sikkerhedskopier og del BarcodeWake-alarmer

Brug en JSON-eksport, når du bevarer eller flytter dine egne appdata, en printbar PDF-sikkerhedskopi-stregkode til gendannelse, og QR-deling til opsætning, når en anden person kun har brug for alarmstrukturen. Deling udelader bevidst registrerede hemmeligheder og historik.

## Vælg formatet til opgaven

Den aktuelle kilde giver forskellige udvekslingsveje, fordi sikkerhedskopiering og deling ikke er den samme handling. En JSON-sikkerhedskopi er beregnet til struktureret dataoverførsel og gendannelse. En PDF-sikkerhedskopi gør gendannelsesmateriale til et printbart stregkodedokument. En opsætnings-QR er bevidst smallere: den kan videregive en begrænset alarmindstilling uden at medtage registrerede stregkodeværdier, NFC-identifikatorer, PIN-koder eller historik.

Behandl ikke en opsætnings-QR som en komplet enhedssikkerhedskopi. Modtageren skal registrere deres egne fysiske koder og gennemse tilladelser lokalt. Nuværende opsætningsdeling begrænser også, hvor mange alarmer den kan indeholde, så verificer det importerede resultat i stedet for at antage, at alle tidsplaner blev flyttet. [Produktfakta](../facts.md) registrerer disse grænser.

## Opret og beskyt en personlig sikkerhedskopi

Brug eksportfunktionen tilgængelig i den installerede version, vælg JSON eller den printbare sikkerhedskopi i henhold til gendannelsesplanen, og gem resultatet et sted, du styrer. En sikkerhedskopi kan afsløre alarmnavne, tidsplaner og anden konfiguration, selv når registrerede rå kodeværdier er beskyttet eller udeladt. Håndter det som personlige rutinedata: undgå offentlige links, delte printere og utroværdige beskedkanaler.

Efter eksporten skal du bekræfte, at filen kan findes, og at dens tidsstempel matcher den tilsigtede sikkerhedskopi. Slet ikke de originale appdata, bare fordi en eksportkommando rapporterede succes. Gendannelestestning er den eneste pålidelige kontrol, men udfør den på en sikker enhed eller efter at have lavet en anden kopi, så testen selv ikke bliver en tabshændelse.

## Del opsætning uden at dele hemmeligheder

Generer en opsætnings-QR kun for alarmer, som modtageren skal modtage. Modtageren scanner den, gennemser den importerede tidsplan og leverer deres egen kode, NFC-tag eller gendannelsesdetaljer. Dette design forhindrer en delt konfiguration i lydløst at overføre den fysiske nøgle, der afviser en andens alarm.

Efter importen bør hver person køre den fulde [alarminstallationstest](set-up-an-alarm.md). Tilladelser, sensorer og operativsystembegrænsninger overføres ikke i QR-koden. Hvis en importeret alarm ikke vises, mens den er låst, skal du følge [fejlfinding af alarminlevering](../help/alarm-delivery.md).

Kilde- og butiksversioner adskilte sig under denne revision, så en installeret offentlig version eksponerer muligvis ikke alle udvekslingsindstillinger, der er beskrevet her. [Tilgængelighed](../availability.md) forklarer, hvordan man fortolker kildebaserede funktioner.

