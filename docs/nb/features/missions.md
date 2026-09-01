---
title: BarcodeWake oppdrag og oppdragskjeder
lang: nb
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
# BarcodeWake oppdrag og oppdragskjeder

Et BarcodeWake-oppdrag er betingelsen som brukes til å avslutte en alarm. Den nåværende kilden støtter strekkode, QR, matematikk, skriving, risting og skrittoppgaver, der registrert NFC håndteres gjennom kode-skanningsbanen. Oppdrag kan kjøres alene, i rekkefølge eller ved tilfeldig utvalg.

## Skanningsoppdrag skaper fysisk avstand

Et strekkode- eller QR-oppdrag sammenligner en direkte kameraskanning med en kode som ble registrert under oppsettet. Koden kan plasseres på en gjenstand utenfor arms rekkevidde: toalettartikler på badet, et frokostelement på kjøkkenet, eller en annen stabil gjenstand på et godt opplyst sted. NFC følger den samme generelle ideen med en kompatibel tagg og enhet. Appen lagrer en hash-representasjon i nåværende stier i stedet for å trenge rå kode for vanlig sammenligning.

Velg en gjenstand som fortsatt vil være tilgjengelig når alarmen ringer. Emballasje kastes, etiketter falmer og reiser endrer miljøet. Å registrere en kode på den eneste medisineskranken du kanskje trenger å bytte ut, er mindre robust enn å bruke en varig etikett. [Alarmoppsettsveiledningen](../guides/set-up-an-alarm.md) dekker plassering og testing.

## Utfordringsoppdrag bytter bevegelse mot innsats

Matematikk og skriving krever fokusert inndata. Risting og skritt krever fysisk bevegelse og støttede sensorer. Vanskelighets- og målinnstillinger endrer hvor mye arbeid som forventes, men et vanskeligere oppdrag er ikke automatisk et bedre. Overdreven friksjon kan oppmuntre til å deaktivere alarmen helt, mens en enkel oppgave kan bli automatisert etter repetisjon.

Tilpass oppgaven til feilmodusen. Hvis du slår av alarmer halvsovende, vil skanning i et annet rom skape nyttig avstand. Hvis kameraadgang er upraktisk, kan en kort skrive- eller matematikkoppgave være mer praktisk. Hvis mobilitet, balanse eller tilgjengelighet er en bekymring, unngå bevegelsesbaserte oppdrag og velg en oppgave som trygt kan utføres.

## Enkelt-, kjede- og tilfeldig-modus

Enkeltmodus ber om én konfigurert oppgave. Kjede modus kjører flere konfigurerte oppdrag i rekkefølge. Tilfeldig modus velger fra et konfigurert sett, og reduserer sjansen for at én memorert interaksjon blir automatisk. Disse modusene er til stede i den nyere kontrollerte kildekoden; [tilgjengelighet](../availability.md) forklarer hvorfor det ikke beviser at de allerede er i hver offentlig versjon.

Alltid kjør en nærliggende test etter å ha endret modus, tillatelser eller registrerte objekter. Hold det valgte objektet tilgjengelig og gi en trygg gjenopprettingsrute. For leveringsproblemer som ikke er relatert til oppdragsgjennomføring, bruk [pålitelighetssjekklisten](../help/alarm-delivery.md).

