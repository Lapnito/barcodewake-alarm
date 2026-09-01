---
title: Sikkerhetskopier og del BarcodeWake-alarmer trygt
lang: nb
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

# Sikkerhetskopier og del BarcodeWake-alarmer trygt

Bruk en JSON-eksport når du bevarer eller flytter dine egne appdata, en utskrivbar PDF-sikkerhetskopi-strekkode for gjenoppretting, og oppsett‑QR‑deling når en annen person bare trenger alarmstrukturen. Deling utelater bevisst registrerte hemmeligheter og historikk.

## Velg formatet for oppgaven

Den nåværende kilden gir ulike utvekslingsalternativer fordi sikkerhetskopiering og deling ikke er samme operasjon. En JSON‑sikkerhetskopi er beregnet på strukturert dataoverføring og gjenoppretting. En PDF‑sikkerhetskopi gjør gjenopprettingsmateriale om til et utskrivbart strekkodedokument. En oppsett‑QR er bevisst smalere: den kan overføre en begrenset alarmkonfigurasjon uten å bære registrerte strekodeverdier, NFC‑identifikatorer, PIN‑koder eller historikk.

Behandle ikke en oppsett‑QR som en fullstendig enhetssikkerhetskopi. Mottakeren må registrere sine egne fysiske koder og gjennomgå tillatelser lokalt. Nåværende oppsettdeling begrenser også hvor mange alarmer den kan inneholde, så verifiser det importerte resultatet i stedet for å anta at alle planer ble flyttet. [Produkt fakta](../facts.md) registrerer disse grensene.

## Opprett og beskytt en personlig sikkerhetskopi

Bruk eksportfunksjonen som er tilgjengelig i den installerte versjonen, velg JSON eller den utskrivbare sikkerhetskopien i henhold til gjenopprettingsplanen, og lagre resultatet et sted du kontrollerer. En sikkerhetskopi kan avsløre alarmnavn, tidsplaner og annen konfigurasjon selv når registrerte rå kodeverdier er beskyttet eller utelatt. Håndter den som personlige rutinedata: unngå offentlige lenker, delte skrivere og upålitelige meldingskanaler.

Etter eksporten, bekreft at filen kan finnes og at tidsstempelet samsvarer med den tiltenkte sikkerhetskopien. Ikke slett original appdata bare fordi en eksportkommando rapporterte suksess. Gjenopprettetesting er den eneste pålitelige kontrollen, men utfør den på en trygg enhet eller etter å ha laget en andre kopi slik at testen selv ikke blir et tapshendelse.

## Del oppsett uten å dele hemmeligheter

Generer en oppsett‑QR kun for alarmene mottakeren skal motta. Mottakeren skanner den, gjennomgår den importerte tidsplanen og oppgir sin egen kode, NFC‑tag eller gjenopprettingsdetaljer. Dette designet forhindrer at en delt konfigurasjon lydløst overfører den fysiske nøkkelen som avviser noen andres alarm.

Etter importen bør hver person kjøre den fullstendige [alarminstallasjonstesten](set-up-an-alarm.md). Tillatelser, sensorer og operativsystemrestriksjoner overføres ikke i QR‑koden. Hvis en importert alarm ikke vises mens den er låst, følg [alarminnleveringsfeilsøking](../help/alarm-delivery.md).

Kilde- og butikkversjoner var forskjellige under denne revisjonen, så en installert offentlig versjon gir kanskje ikke alle utvekslingsalternativene som er beskrevet her. [Tilgjengelighet](../availability.md) forklarer hvordan man tolker kildebaserte funksjoner.

