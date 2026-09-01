---
title: BarcodeWake uppdrag och uppdragskedjor
lang: sv
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

# BarcodeWake uppdrag och uppdragskedjor

Ett BarcodeWake-uppdrag är det villkor som används för att stänga av ett larm. Den nuvarande källan stöder streckkod, QR-kod, matematik, skrivning, skakning och steg-uppgifter, där registrerad NFC hanteras via kodskanningsvägen. Uppdrag kan köras ensamma, i följd eller genom slumpmässigt urval.

## Skanningsuppdrag skapar fysiskt avstånd

En streckkod- eller QR-uppdrag jämför en levande kamerabild med en kod som registrerades under installationen. Koden kan placeras på ett föremål utom räckhåll: toalettartiklar i ett badrum, en frukostartikel i ett kök eller ett annat stabilt föremål i ett väl upplyst område. NFC följer samma allmänna idé med en kompatibel tagg och enhet. Appen lagrar en hashrepresentation i aktuella sökvägar snarare än att behöva den råa koden för vanlig jämförelse.

Välj ett föremål som fortfarande kommer att vara tillgängligt när larmet ljuder. Förpackningar kasseras, etiketter bleknar och resor förändrar miljön. Att registrera en kod på den enda medicinlådan som du kan behöva byta ut är mindre robust än att använda en varaktig etikett. [Guiden för att ställa in ett larm](../guides/set-up-an-alarm.md) täcker placering och testning.

## Utmaningsuppdrag byter rörelse mot ansträngning

Matematik och skrivning kräver fokuserad inmatning. Skakning och steg kräver fysisk rörelse och stödda sensorer. Svårighets- och målinställningar ändrar hur mycket arbete som förväntas, men ett svårare uppdrag är inte automatiskt bättre. Överdriven friktion kan uppmuntra att larmet stängs av helt, medan en enkel uppgift kan bli automatisk efter upprepning.

Anpassa uppgiften till feltypen. Om du stänger av larm halvsova, kan skanning i ett annat rum skapa användbart avstånd. Om kameraåtkomst är obekvämt kan en kort skriv- eller matteuppgift vara mer praktisk. Om mobilitet, balans eller tillgänglighet är ett problem, undvik rörelsebaserade uppdrag och välj en uppgift som kan utföras säkert.

## Enkelt, kedjande och slumpmässigt läge

Enkelt läge begär ett konfigurerat uppdrag. Kedjande läge kör flera konfigurerade uppdrag i ordning. Slumpmässigt läge väljer från en konfigurerad uppsättning, vilket minskar risken för att en inlärd interaktion blir automatisk. Dessa lägen finns i den nyare kontrollerade källan; [tillgänglighet](../availability.md) förklarar varför detta inte bevisar att de redan finns i varje offentlig version.

Kör alltid ett kortfristigt test efter att ha ändrat läge, behörigheter eller registrerade objekt. Håll det valda objektet nåbart och ge en säker återhämtningsväg. För leveransproblem som inte är relaterade till uppdragets slutförande, använd [Tillförlitlighetskontroll](../help/alarm-delivery.md).

