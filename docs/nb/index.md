---
title: BarcodeWake dokumentasjon
lang: nb
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake dokumentasjon

BarcodeWake er en vekkerklokke som gjør avvisning til en bevisst handling. En alarm kan kreve en lagret strekkode eller QR-kode, en kort kognitiv oppgave, en ristesekvens eller et skrittmål i stedet for kun å stole på en enkel på-skjermen-knapp.

## Hva som gjør BarcodeWake forskjellig

Den sentrale ideen er avstand pluss intensjon. Hvis den registrerte koden er festet til en gjenstand vekk fra sengen, betyr det å dempe alarmen at du reiser deg, når du den gjenstanden og skanner den. Samme alarmmodell kan også bruke matte-, skrive-, riste- eller skrittoppdrag. Nåværende kildekode støtter en enkelt oppgave, en ordnet kjede eller tilfeldig utvalg fra konfigurerte oppdrag.

Den friksjonen er nyttig for mennesker som avviser en vanlig alarm uten å bli fullt oppmerksom. Det er ikke søvnfaseanalyse, medisinsk veiledning eller en garanti for at noen vil våkne. Maskinvarestøtte, tillatelser og produsentens batterikontroller påvirker fortsatt levering. [Oppdragsreferansen](features/missions.md) forklarer valgmulighetene, mens [alarmeringsleveringsfeilsøking](help/alarm-delivery.md) dekker systeminnstillinger som kan forstyrre.

## Start med riktig dokument

Bruk [oppsettsveiledningen](guides/set-up-an-alarm.md) når du oppretter en alarm og registrerer en fysisk kode. Les [sikkerhetskopiering og deling](guides/backup-and-sharing.md) før du flytter data eller sender et oppsetts-QR til noen andre. Delingsformatet utelater bevisst registrerte koder, NFC-identifikatorer, PIN-koder og alarmhistorikk, så en mottaker må fullføre sensitivt oppsett lokalt.

For et kort, reviderbart sammendrag, se [produkt fakta](facts.md). For utgivelsesstatus, bruk [tilgjengelighet](availability.md): den offentlige Google Play-versjonen som ble tatt opp for denne revisjonen, avviker fra versjonen som er erklært av den kontrollerte kilde-treet. Den nyere kildeversjonen er derfor dokumentert som kildekapasitet, ikke bekreftet som en publisert butikkutgivelse.

## Personvern- og pålitelighetsgrenser

Kjernekonfigurasjon og oppdragsdata lagres på enheten, og ingen BarcodeWake-konto er nødvendig. Nåværende kodestier representerer registrerte kodeverdier med SHA-256-hash. Valgfri telemetri er beskrevet av personvernerklæringen som deaktivert som standard. Disse utsagnene betyr ikke at alle telefoner vil levere alarmer identisk; Android-leverandører og operativsystemtillatelser kan fortsatt begrense bakgrunnsatferd.

Les [personvern og pålitelighet](features/privacy-and-reliability.md) for skillet mellom lokal datahåndtering og operativsystemlevering. [Standard alarm sammenligning](comparisons/standard-alarm.md) hjelper deg med å avgjøre om oppdragsbasert avvisning matcher måten du våkner på.

