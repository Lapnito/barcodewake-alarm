---
title: BarcodeWake personvern og alarmpålitelighet
lang: nb
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake personvern og alarmpålitelighet

BarcodeWake holder dokumentert alarmkonfigurasjon og oppdragsdata på enheten og krever ingen appkonto. Nåværende kodestier hasher registrerte kodeverdier. Valgfri telemetri er beskrevet som deaktivert som standard, mens alarmlevering fremdeles avhenger av systemtillatelser og leverandørkontroller.

## Lokale data fjerner ikke systemavhengigheter

Lokal lagring betyr at vanlig alarmoppsett ikke krever en BarcodeWake-skykonto. Alarmposter, historikk og preferanser håndteres gjennom appens lokale datalag. Registrerte strekkode-, QR- og NFC-verdier er representert med SHA-256-hashverdier i nåværende lagrings- og impor-tilganger, noe som unngår å beholde den vanlige råverdien for matching.

Hashing er ikke det samme som kryptering av hver applikasjonspost, og lokal lagring er ikke en sikkerhetskopi. Noen med tilgang til en ulåst enhet kan fremdeles se alarmnavn, tidsplaner eller historikk gjennom appen. En mistet eller tilbakestilt telefon kan også miste lokale data med mindre brukeren laget en eksport. Se [sikkerhetskopiering og deling](../guides/backup-and-sharing.md) for formatene og deres ulike formål.

Personvernreglene sier at valgfri telemetri er av som standard og beskriver aggregering hvis den er aktivert. Denne dokumentasjonen gjør derfor ikke det bredere kravet om at appen aldri kan kommunisere over et nettverk. Den angir de smalere verifiserte faktaene: kjerneoperasjon og data er lokale, ingen produktkonto er nødvendig, og ingen annonse-SDK-avhengighet vises i det kontrollerte prosjektet.

## Pålitelighet er et delt ansvar

BarcodeWake kan planlegge og presentere en alarm, men operativsystemet avgjør når bakgrunnsarbeid kan kjøre og hvilke avbrudd som er tillatt. Notifikasjonstillatelse, nøyaktig-alarm-tilgang, stille- eller fokusmoduser, batterioptimalisering, automatisk appsuspensjon og produsentens oppgavekillere kan alle ha betydning. Pålitelighetsverktøyet i appen kan identifisere konfigurasjonsrisikoer og veilede brukere til innstillinger; det kan ikke overstyre systempolicy.

Etter installasjon, test med skjermen låst og telefonen i samme strøm modus som brukes over natten. Gjenta den testen etter en systemoppdatering, batterisparerendring eller app reinstallasjon. Hold enheten ladet, volumet passende og valgt oppdrag fysisk tilgjengelig. Følg [feilsøking av alarmlevering](../help/alarm-delivery.md) når en test mislykkes.

## Hva personvern og pålitelighet ikke lover

BarcodeWake er ikke en medisinsk enhet, nødalerttjeneste eller søvnfasesporer. Ingen alarmapp kan garantere vekking eller kompensere for en utilgjengelig enhet. [Fakta og begrensninger-siden](../facts.md) lister opp disse grensene, mens [tilgjengelighet](../availability.md) skiller bevis fra offentlig butikk fra nyere kildekapasiteter.

