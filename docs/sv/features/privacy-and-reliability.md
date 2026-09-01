---
title: BarcodeWake integritets- och larmpålitlighet
lang: sv
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
# BarcodeWake integritets- och larmpålitlighet

BarcodeWake behåller dokumenterad larmkonfiguration och uppdragsdata på enheten och kräver inget appkonto. Befintliga kodvägar hash-värden för registrerade kodvärden. Valfri telemetri beskrivs som inaktiverad som standard, medan larmleverans fortfarande beror på systembehörigheter och leverantörskontroller.

## Lokal data tar inte bort systemberoenden

Lokal lagring innebär att vanlig larmkonfiguration inte kräver ett BarcodeWake-molnkonto. Larmposter, historik och inställningar hanteras genom appens lokala datalager. Registrerade streckkods-, QR- och NFC-värden representeras med SHA-256-hashvärden i nuvarande lagrings- och importvägar, vilket undviker att behålla det vanliga råvärdet för matchning.

Hashning är inte samma sak som kryptering av varje apppost, och lokal lagring är inte en säkerhetskopia. Någon med tillgång till en upplåst enhet kan fortfarande se larmnamn, scheman eller historik genom appen. En förlorad eller återställd telefon kan också förlora lokal data om inte användaren har gjort en export. Se [säkerhetskopiering och delning](../guides/backup-and-sharing.md) för formaten och deras olika syften.

Integritetspolicyn säger att valfri telemetri är av som standard och beskriver aggregerad hantering om den är aktiverad. Denna dokumentation gör därför inte det bredare påståendet att appen aldrig kan kommunicera över ett nätverk. Den anger de smalare verifierade fakta: kärnverksamhet och data är lokala, inget produktkonto krävs, och ingen annons-SDK-beroende framgår i den kontrollerade projektet.

## Tillförlitlighet är ett delat ansvar

BarcodeWake kan schemalägga och presentera ett larm, men operativsystemet avgör när bakgrundsarbete får köras och vilka avbrott som är tillåtna. Notifikationsbehörighet, exakt larmåtkomst, tysta eller fokuslägen, batterioptimering, automatisk appsuspension och tillverkares aktivitetshanterare kan alla ha betydelse. De interna tillförlitlighetsverktygen kan identifiera konfigurationsrisker och dirigera användare till inställningar; de kan inte åsidosätta systemprincipen.

Efter installation, testa med skärmen låst och telefonen i samma energiläge som används över natten. Upprepa det testet efter en systemuppdatering, batterispararändring eller appnyinstallation. Håll enheten laddad, volymen lämplig och det valda uppdraget fysiskt tillgängligt. Följ [felsökning av larmleverans](../help/alarm-delivery.md) när ett test misslyckas.

## Vad integritet och tillförlitlighet inte lovar

BarcodeWake är inte en medicinteknisk produkt, tjänst för nödmeddelanden eller sömndetekterare. Ingen larmapp kan garantera uppvaknandet eller kompensera för en otillgänglig enhet. [Sidan med fakta och begränsningar](../facts.md) listar dessa gränser, medan [tillgänglighet](../availability.md) separerar bevis från offentliga butiker från nyare källfunktionsmöjligheter.

