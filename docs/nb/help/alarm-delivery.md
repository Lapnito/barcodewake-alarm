---
title: Hvorfor en BarcodeWake-alarm kanskje ikke ringer
lang: nb
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
# Hvorfor en BarcodeWake-alarm kanskje ikke ringer

En lagret alarm kan fortsatt blokkeres av varslingsinnstillinger, eksakt alarmtilgang, fokus- eller lydløse moduser, lavt volum, batteribegrensninger, appopphenging eller leverandørens bakgrunnskontroller. Sjekk levering separat fra oppdragsskanning, og kjør deretter en låst skjerm-test.

## Først isoler levering fra avvisning

Opprett en nærforestående testalarm med et enkelt oppdrag og la appen være i bakgrunnen. Lås skjermen. Hvis ingen alarmskjerm eller lyd vises, er problemet levering; å endre den registrerte strekkoden vil ikke fikse det. Hvis alarmen vises men oppdraget ikke kan fullføres, fungerer levering og problemet er kamera, sensor, kode-matching eller oppdragskonfigurasjon.

Bekreft at alarmen er aktivert, den planlagte dagen er korrekt og telefonens tidssone samsvarer med den tiltenkte tidsplanen. Sjekk media- og alarmvolum i stedet for kun å stole på sideknappens tilstand. Gå gjennom ikke-forstyrr- eller fokusregler, tilkoblede lydenheter og om telefonen ble startet på nytt etter at alarmen ble opprettet.

## Gå gjennom operativsystemets tillatelsesporter

Tillat varsler og all eksakt alarm- eller fullskjermsalarmtilgang som er forespurt av den installerte versjonen. Fjern BarcodeWake fra aggressiv batteroptimalisering eller automatiske sovende lister når enhetsleverandøren tilbyr disse kontrollene. Åpne pålitelighetsdiagnostikken i appen og følg de enhetsspesifikke innstillingene den identifiserer. [Personvern og pålitelighetssiden](../features/privacy-and-reliability.md) forklarer hvorfor disse systemavhengighetene forblir selv når appdata er lokale.

Etter å ha endret én innstilling, gjenta låst skjerm-testen. Å endre flere kontroller samtidig gjør årsaken vanskeligere å identifisere. Systemoppdateringer kan tilbakestille eller omfortolke tillatelser, så test på nytt etter en større oppdatering eller reinstallering av appen.

## Diagnostiser oppdragsgjennomføring separat

For strekkode- og QR-oppdrag, rengjør kameralinsen, forbedre belysningen og bekreft at det registrerte objektet er uendret. Gi kameratillatelse. For NFC, verifiser enhetsstøtte og hold taggen nær den korrekte antenneplasseringen. Rist- og stegoppdrag avhenger av bevegelses- eller stegsensorer og kan oppføre seg annerledes når strømsparingsmoduser begrenser sensorlevering.

Hvis et oppdrag ble konfigurert som en del av en kjede, må hvert nødvendig trinn fullføres. Gå gjennom [oppdragsatferd](../features/missions.md) og, om nødvendig, opprett en ny test ved hjelp av [oppsettsprosedyren](../guides/set-up-an-alarm.md).

## Vet når telefonen er grensen

BarcodeWake kan ikke overstyre en avslått enhet, et utladet batteri, ødelagt lydmaskinvare eller alle produsentens oppgavedrepere. Det er ikke en nødmeldingstjeneste. Ha en annen alarmmetode for situasjoner med høye konsekvenser og rapporter reproduserbare feil med enhetsmodell, systemversjon, appversjon og de eksakte testforholdene.

