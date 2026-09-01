---
title: BarcodeWake dokumentation
lang: da
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake dokumentation

BarcodeWake er en alarmklokke, der gør afvisning til en bevidst handling. En alarm kan kræve en gemt stregkode eller QR-kode, en kort kognitiv opgave, en rystesekvens eller et skridtmål i stedet for udelukkende at stole på en nem på-skærm-knap.

## Hvad gør BarcodeWake anderledes

Den centrale idé er afstand plus hensigt. Hvis den registrerede kode er knyttet til en genstand væk fra sengen, betyder at slukke for alarmen at rejse sig, nå den genstand og scanne den. Samme alarmmodel kan også bruge matematik, indtastning, rystelse eller skridtmissioner. Den aktuelle kildekode understøtter en enkelt mission, en ordnet kæde eller tilfældig valg fra konfigurerede missioner.

Denne friktion er nyttig for personer, der afviser en almindelig alarm uden at blive fuldt vågen. Det er ikke søvnstadieanalyse, medicinsk vejledning eller en garanti for, at nogen vil vågne. Hardwareunderstøttelse, tilladelser og leverandørers batteristyring påvirker stadig leveringen. [Missionsreferencen](features/missions.md) forklarer valgmulighederne, mens [fejlfinding af alarmlevering](help/alarm-delivery.md) dækker systemindstillinger, der kan forstyrre.

## Start med det rigtige dokument

Brug [opsætningsguiden](guides/set-up-an-alarm.md) ved oprettelse af en alarm og registrering af en fysisk kode. Læs [sikkerhedskopiering og deling](guides/backup-and-sharing.md) før flytning af data eller afsendelse af en opsætnings-QR til en anden. Delingsformatet udelader bevidst registrerede koder, NFC-identifikatorer, PIN-koder og alarmhistorik, så en modtager skal fuldføre følsom opsætning lokalt.

For et kort, reviderbart resumé, se [produktfakta](facts.md). For udgivelsesstatus, brug [tilgængelighed](availability.md): den offentlige Google Play-version, der er indfanget til denne revision, afviger fra den version, der er erklæret af den kontrollerede kilde-træ. Den nyere kildeversion er derfor dokumenteret som kildekapacitet, ikke hævdet som en udgivet butiksudgivelse.

## Grænser for privatlivets fred og pålidelighed

Kernekonfiguration og missionsdata er gemt på enheden, og der kræves ingen BarcodeWake-konto. Aktuelle kodeveje repræsenterer registrerede kodeværdier med SHA-256-hash. Valgfri telemetri er beskrevet af privatlivspolitikken som deaktiveret som standard. Disse udsagn betyder ikke, at alle telefoner vil levere alarmer identisk; Android-leverandører og operativsystemtilladelser kan stadig begrænse baggrundsadfærd.

Læs [privatliv og pålidelighed](features/privacy-and-reliability.md) for at skelne mellem lokal datahåndtering og operativsystemlevering. [Standard alarm sammenligningen](comparisons/standard-alarm.md) hjælper med at beslutte, om missionsbaseret afvisning matcher den måde, du vågner på.

