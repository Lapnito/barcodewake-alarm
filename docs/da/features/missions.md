---
title: BarcodeWake missioner og missionskæder
lang: da
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# BarcodeWake missioner og missionskæder

En BarcodeWake mission er betingelsen, der bruges til at afvise en alarm. Den aktuelle kilde understøtter stregkode, QR, matematik, tastning, ryst og skridtopgaver, hvor registreret NFC håndteres via kode-scanningsvejen. Missioner kan køre alene, i rækkefølge eller ved tilfældig udvælgelse.

## Scanmissioner skaber fysisk afstand

En stregkode- eller QR-mission sammenligner en levende kamerascanning med en kode, der er registreret under opsætningen. Koden kan anbringes på en genstand uden for arms rækkevidde: toiletartikler på et badeværelse, et morgenmadselement i et køkken eller en anden stabil genstand på et godt oplyst sted. NFC følger den samme generelle idé med en kompatibel tag og enhed. Appen gemmer en hash-repræsentation i aktuelle stier i stedet for at have brug for den rå kode til normal sammenligning.

Vælg en genstand, der stadig vil være tilgængelig, når alarmen ringer. Emballage smides væk, etiketter falmer, og rejser ændrer miljøet. At registrere en kode på den eneste medicinæske, du muligvis skal erstatte, er mindre robust end at bruge en holdbar etiket. [alarm installationsguide](../guides/set-up-an-alarm.md) dækker placering og test.

## Udfordringsmissioner bytter bevægelse for indsats

Matematik og tastning kræver fokuseret input. Ryst og skridt kræver fysisk bevægelse og understøttede sensorer. Sværhedsgrad og målindstillinger ændrer, hvor meget arbejde der forventes, men en sværere mission er ikke automatisk en bedre. Overdreven friktion kan tilskynde til at deaktivere alarmen helt, mens en let opgave kan blive automatisk efter gentagelse.

Match opgaven til fejltilstanden. Hvis du slukker for alarmer halvt i søvne, skaber scanning i et andet rum nyttig afstand. Hvis kameraadgang er ubelejligt, kan en kort tastnings- eller matematikopgave være mere praktisk. Hvis mobilitet, balance eller tilgængelighed er en bekymring, undgå bevægelsesbaserede missioner og vælg en opgave, der kan udføres sikkert.

## Enkelt, kæde og tilfældig tilstand

Enkelt tilstand beder om én konfigureret mission. Kædetilstand kører flere konfigurerede missioner i rækkefølge. Tilfældig tilstand vælger fra et konfigureret sæt, hvilket reducerer sandsynligheden for, at én memoreret interaktion bliver automatisk. Disse tilstande er til stede i den nyere kontrollerede kilde; [tilgængelighed](../availability.md) forklarer, hvorfor det ikke beviser, at de allerede er i hver offentlig build.

Kør altid en nær-tid test efter at have ændret tilstand, tilladelser eller registrerede objekter. Hold det valgte objekt inden for rækkevidde og giv en sikker gendannelsesrute. For leveringsproblemer, der ikke er relateret til missionsfuldførelse, brug [pålidelighedstjekliste](../help/alarm-delivery.md).

