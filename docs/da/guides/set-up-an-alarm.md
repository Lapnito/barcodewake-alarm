---
title: Sådan opsætter du en BarcodeWake-alarm
lang: da
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---
# Sådan opsætter du en BarcodeWake-alarm

Opret først tidsplanen, vælg en mission, der er sikker og praktisk, giv de nødvendige tilladelser, og kør derefter en låst skærm-test i den nærmeste fremtid. For scanmissioner skal du registrere et holdbart objekt, der vil være tilgængeligt og læsbart, når alarmen ringer.

## Vælg missionen før objektet

Beslut, hvilken handling der skal adskille vågning fra afvisning. En stregkode i et andet rum skaber fysisk afstand. Matematik eller indtasting tilføjer koncentration uden at kræve et kamera. Rystelse eller skridt tilføjer bevægelse, men afhænger af sensorer og passer muligvis ikke til enhver person eller ethvert miljø. [Mission reference](../features/missions.md) forklarer afvejningerne mellem enkelt-, kæde- og tilfældige tilstande.

Hvis du bruger en stregkode, QR-kode eller NFC-mærkat, skal du vælge noget holdbart. Undgå engangsemballage, et objekt som et andet husstandsmedlem kan flytte, eller en kode, der vil være utilgængelig under rejser. Kontroller, at kameraet kan fokusere i det forventede lys. NFC kræver en kompatibel telefon og et mærkat.

## Konfigurer tidsplanen og afvisningsreglen

Åbn alarmeditoren, indstil det ønskede tidspunkt og aktive dage, og vælg derefter den mission, der vises af den installerede build. Konfigurer dens sværhedsgrad eller mål konservativt til den første test. Hvis den installerede version understøtter kæder, skal du arrangere missioner i en rækkefølge, der trygt kan fuldføres uden at haste over trapper eller forlade et sikkert område.

Registrer den fysiske kode fra missionsopsætningsflowet. Giv alarmen et label, der identificerer den tilsigtede rutine, i stedet for at eksponere følsomme oplysninger. Gennemgå lydstyrke, vibration og eventuelle opfølgningsindstillinger for opvækning, der er synlige i den installerede build. Tilgængelige kontroller kan afvige, fordi [den offentlige og kildeversionerne](../availability.md) ikke var identiske på auditdatoen.

## Giv tilladelser med et formål

Tillad notifikationer og alarmrelateret adgang, der er nødvendig for levering. Giv kun kameraadgang, når du bruger en scanmission, og sensoradgang, når den valgte mission kræver det. På Android skal du gennemgå indstillinger for præcise alarmer og batteri, hvis appens pålidelighedskontrol markerer dem. Antag ikke, at det at gemme en alarm bevises, at baggrundslevering er tilladt.

## Test den komplette overnatningssti

Indstil en test et par minutter frem. Lås skærmen, lad BarcodeWake være i baggrunden, og læg telefonen i samme lyd- og strømtilstand, som er planlagt til overnatning. Bekræft, at alarmen vises, lyden er hørbar, og den præcist valgte mission kan fuldføres. Gentag derefter efter at have flyttet det registrerede objekt til dets virkelige placering.

Hvis levering mislykkes, skal du bruge [alarmleveringschecklisten](../help/alarm-delivery.md). Hvis det lykkes, bør du overveje at lave en [lokal sikkerhedskopi](backup-and-sharing.md), efter opsætningen er stabil.

