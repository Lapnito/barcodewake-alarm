---
title: Varför en BarcodeWake-alarm kanske inte ringer
lang: sv
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
# Varför en BarcodeWake-alarm kanske inte ringer

En sparad alarm kan fortfarande blockeras av aviseringsinställningar, exakt alarmåtkomst, fokus- eller ljudlöslägen, låg volym, batteribegränsningar, appupphängning eller leverantörens bakgrundskontroller. Kontrollera leveransen separat från uppdragsskanning och kör sedan ett test med låst skärm.

## Isolera först leveransen från avvisningen

Skapa ett alarm inom kort med ett enkelt uppdrag och lämna appen i bakgrunden. Lås skärmen. Om ingen alarmskärm eller ljud visas är problemet leveransen; att ändra den registrerade streckkoden kommer inte att lösa det. Om larmet visas men uppdraget inte kan slutföras fungerar leveransen och problemet är kameran, sensorn, kodmatchningen eller uppdragskonfigurationen.

Bekräfta att larmet är aktiverat, den schemalagda dagen är korrekt och telefonens tidszon matchar det avsedda schemat. Kontrollera media- och alarmvolymen snarare än att endast förlita dig på sidoknappens status. Granska disturbansregler eller fokusregler, anslutna ljudenheter och om telefonen startades om efter att larmet skapades.

## Granska operativsystemets behörighetsgrindar

Tillåt aviseringar och all exakt alarmåtkomst eller fullständig alarmåtkomst som begärts av den installerade versionen. Ta bort BarcodeWake från aggressiv batterioptimering eller automatiska sovlistor när enhetsleverantören erbjuder dessa kontroller. Öppna appens tillförlitlighetsdiagnostik och följ de enhetsspecifika inställningar som den identifierar. Sidan [sekretess och tillförlitlighet](../features/privacy-and-reliability.md) förklarar varför dessa systemberoenden kvarstår även när appdata är lokala.

Efter att ha ändrat en inställning upprepar du testet med låst skärm. Att ändra flera kontroller samtidigt gör orsaken svårare att identifiera. Systemuppdateringar kan återställa eller omforma behörigheter, så testa igen efter en stor uppdatering eller ominstallation av appen.

## Diagnostisera uppdragsslutförande separat

För streckkod- och QR-uppdrag rengör du kameralinsen, förbättrar belysningen och bekräftar att det registrerade objektet är oförändrat. Ge kamerabehörighet. För NFC verifierar du enhetsstödet och håller taggen nära rätt antennposition. Skak- och steguppdrag är beroende av rörelse- eller stegsensorer och kan bete sig annorlunda när energisparlägen begränsar sensorleveransen.

Om ett uppdrag konfigurerades som en del av en kedja måste varje nödvändigt steg slutföras. Granska [uppdragsbeteende](../features/missions.md) och skapa vid behöv ett nytt test med [konfigurationsproceduren](../guides/set-up-an-alarm.md).

## Vet när telefonen är gränsen

BarcodeWake kan inte åsidosätta en avstängd enhet, ett urladdat batteri, trasig ljudhårdvara eller varje tillverkares aktivitetsdödare. Det är inte en tjänst för nödmeddelanden. Behåll en annan alarmmetod för situationer med höga konsekvenser och rapportera reproducerbara fel med enhetsmodell, systemversion, appversion och de exakta testförhållandena.

