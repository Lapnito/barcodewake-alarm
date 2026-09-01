---
title: Hvorfor en BarcodeWake-alarm muligvis ikke ringer
lang: da
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Hvorfor en BarcodeWake-alarm muligvis ikke ringer

En gemt alarm kan stadig blive blokeret af notifikationsindstillinger, adgang til præcis alarm, fokus- eller lydløs tilstand, lav lydstyrke, batteribegrænsninger, app-suspension eller leverandørens baggrundskontroller. Kontroller levering separat fra missionsscanning, og kør derefter en låst skærm-test.

## Først isolere levering fra afvisning

Opret en nærterm test-alarm med en simpel mission, og lad appen være i baggrunden. Lås skærmen. Hvis der ikke vises nogen alarm-skærm eller lyd, er problemet levering; at ændre den registrerede stregkode vil ikke rette det. Hvis alarmen vises, men missionen ikke kan fuldføres, fungerer levering, og problemet er kamera, sensor, kode-matchning eller mission-konfiguration.

Bekræft, at alarmen er aktiveret, den planlagte dag er korrekt, og telefonens tidszone matcher den tilsigtede tidsplan. Kontroller medie- og alarmlydstyrke i stedet for udelukkende at stole på sideknap-tilstanden. Gennemgå gener ikke-forstyrre- eller fokusregler, tilsluttede lydenheder, og om telefonen blev genstartet efter alarmen blev oprettet.

## Gennemgå operativsystemets tilladelsesporte

Tillad notifikationer og enhver præcis alarm- eller fuld skærm alarm-adgang, der anmodes om af den installerede build. Fjern BarcodeWake fra aggressiv batterioptimering eller automatiske sovende lister, når enhedsleverandøren tilbyder disse kontroller. Åbn appens diagnostik for pålidelighed, og følg de enhedsspecifikke indstillinger, den identificerer. [Privatlivets- og pålidelighedssiden](../features/privacy-and-reliability.md) forklarer, hvorfor disse systemafhængigheder forbliver, selv når appdata er lokale.

Efter at have ændret en indstilling, gentag låst skærm-testen. Hvis du ændrer flere kontroller på én gang, bliver årsagen sværere at identificere. Systemopdateringer kan nulstille eller genfortolke tilladelser, så test igen efter en større opdatering eller app-geninstallation.

## Diagnosticer missionsfuldførelse separat

For stregkode- og QR-missioner skal du rengøre kameraobjektivet, forbedre belysningen og bekræfte, at det registrerede objekt er uændret. Giv kamera-tilladelse. For NFC skal du verificere enhedsunderstøttelse og holde mærket nær den korrekte antenneposition. Ryst- og skridtmissioner afhænger af bevægelses- eller skridtsensorer og kan opføre sig forskelligt, når strømbesparende tilstande begrænser sensordata.

Hvis en mission blev konfigureret som en del af en kæde, skal hvert krævet trin fuldføres. Gennemgå [missionsadfærd](../features/missions.md), og opret om nødvendigt en ny test ved hjælp af [opsætningsproceduren](../guides/set-up-an-alarm.md).

## Ved, hvornår telefonen er grænsen

BarcodeWake kan ikke tilsidesætte en slukket enhed, et udtømt batteri, ødelagt lydhardware eller enhver producents opgavedræber. Det er ikke en nødblivstyringstjeneste. Bevar en anden alarmmetode til situationer med høje konsekvenser, og rapporter reproducerbare fejl med enhedsmodel, systemversion, appversion og de nøjagtige testforhold.

