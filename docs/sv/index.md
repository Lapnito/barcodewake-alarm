---
title: BarcodeWake-dokumentation
lang: sv
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake-dokumentation

BarcodeWake är en väckarklocka som gör avfärdandet till en medveten handling. En alarm kan kräva en sparad streckkod eller QR-kod, en kort kognitiv uppgift, en skakningssekvens eller ett stegmål istället för att endast förlita sig på en enkel på-skärmen-knapp.

## Vad som gör BarcodeWake annorlunda

Den centrala idén är avstånd plus avsikt. Om den registrerade koden är fäst vid ett objekt borta från sängen, innebär att stänga av larmet att man ställer sig upp, når det objektet och skannar det. Samma larmmodell kan också använda matte-, skriv-, skak- eller steguppdrag. Nuvarande källkod stöder ett enskilt uppdrag, en ordnad kedja eller slumpmässigt urval från konfigurerade uppdrag.

Den friktionen är användbar för personer som stänger av ett vanligt alarm utan att bli helt alerta. Det är inte sömnstadieanalys, medicinsk vägledning eller en garanti för att någon kommer att vakna. Hårdvarustöd, behörigheter och leverantörens batterikontroller påverkar fortfarande leveransen. [Uppdragsreferensen](features/missions.md) förklarar valen, medan [larmleverans felsökning](help/alarm-delivery.md) täcker systeminställningar som kan störa.

## Börja med rätt dokument

Använd [inställningsguiden](guides/set-up-an-alarm.md) när du skapar ett alarm och registrerar en fysisk kod. Läs [säkerhetskopiering och delning](guides/backup-and-sharing.md) innan du flyttar data eller skickar en inställnings-QR till någon annan. Delningsformatet utesluter medvetet registrerade koder, NFC-identifikatorer, PIN-koder och alarmhistorik, så en mottagare måste slutföra känslig inställning lokalt.

För en kort, granskbar sammanfattning, se [produktfakta](facts.md). För versionsstatus, använd [tillgänglighet](availability.md): den offentliga Google Play-versionen som fångades för denna granskning skiljer sig från versionen som deklareras av den kontrollerade källträdet. Den nyare källversionen dokumenteras därför som källkapacitet, inte påstås som en publicerad butiksrelease.

## Integritets- och tillförlitlighetsgränser

Kärnkonfiguration och uppdragsdata lagras på enheten, och inget BarcodeWake-konto krävs. Nuvarande kodvägar representerar registrerade kodvärden med SHA-256-hashvärden. Valfri telemetri beskrivs av integritetspolicyn som inaktiverad som standard. Dessa uttalanden betyder inte att varje telefon kommer att leverera larm identiskt; Android-leverantörer och operativsystembehörigheter kan fortfarande begränsa bakgrundsbeteende.

Läs [integritet och tillförlitlighet](features/privacy-and-reliability.md) för skillnaden mellan lokal datahantering och operativsystemleverans. [Standardlarmjämförelsen](comparisons/standard-alarm.md) hjälper dig att avgöra om uppdragsbaserat avfärdande matchar det sätt du vaknar på.

