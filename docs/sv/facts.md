---
title: BarcodeWake fakta och begränsningar
lang: sv
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# BarcodeWake fakta och begränsningar

BarcodeWake schemalägger alarm och verifierar en vald avfärdningsuppgift. Den kan använda skanningar, kognitiva utmaningar eller rörelse, lagrar den dokumenterade kärninformationen lokalt, kräver inget produktkonto och utför ingen sömnstadieanalys.

## Produktfakta i korthet

| Fråga | Verifierat svar |
|---|---|
| Vad är det? | En väckarklocka med fysiska och kognitiva avfärdningsuppgifter. |
| Vilka uppgifter finns i den aktuella källkoden? | Streckkod, QR, matematik, skrivning, skakning och steg. NFC hanteras som en registrerad kodväg. |
| Krävs ett konto? | Inget konto eller inloggningsflöde finns för de dokumenterade funktionerna. |
| Var lagras data? | Alarmkonfiguration, historik och inställningar använder lokal lagring. Aktuella kodvägar hashar registrerade kodvärden. |
| Är det en sömnspårare? | Nej. Den schemalägger alarm och verifierar uppgifter; den klassificerar inte sömnstadier. |
| Är varje källfunktion offentligt utgiven? | Ej fastställt. Butiks- och källversioner skilde sig åt vid granskningsdatumet. |

## Begränsningar som har betydelse i praktiken

En alarmapp arbetar inom telefonbaserade begränsningar. Meddelandetillstånd, exakt alarmåtkomst, fokusinställningar, batterioptimering och leverantörsspecifika bakgrundskontroller kan påverka om ett alarm kommer som förväntat. BarcodeWake inkluderar tillförlitlighetskontroller och vägledning, men en app kan inte åsidosätta varje operativsystems- eller tillverkarrestriktion. Testa ett alarm efter installation och efter stora systembyten; [leveranschecklistan](help/alarm-delivery.md) förklarar hur.

Uppgiftsmaskinvaran spelar också roll. Skanning kräver kameraåtkomst och en läsbar fysisk kod. Skak- och steguppgifter beror på relevanta sensorer. NFC behöver kompatibel maskinvara. En kopierad eller skadad etikett kan förhindra en matchning, så ha en återställningsväg och gör inte det enda registrerade objektet oåtkomligt.

## Påståenden som medvetet inte görs

Dessa sidor gör inga anspråk på medicinsk nytta, garanterad väckning, sömncykeltiming, molnsynkronisering eller en verifierad offentlig iOS-utgåva. De behandlar heller inte källversionen som en levande butiksversion. Se [tillgänglighet](availability.md) för den distinktionen och [sekretess och tillförlitlighet](features/privacy-and-reliability.md) för bevisen bakom lokal lagring och telemetriordval.

