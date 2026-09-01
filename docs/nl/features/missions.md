---
title: BarcodeWake-missies en missieketens
lang: nl
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
# BarcodeWake-missies en missieketens

Een BarcodeWake-missie is de voorwaarde die wordt gebruikt om een alarm uit te schakelen. De huidige bron ondersteunt barcode-, QR-, wiskunde-, typ-, schud- en stapactiviteiten, waarbij geregistreerde NFC wordt afgehandeld via het code-scanpad. Missies kunnen alleen worden uitgevoerd, opeenvolgend of door willekeurige selectie.

## Scanmissies creëren fysieke afstand

Een barcode- of QR-missie vergelijkt een live camerascan met een code die tijdens de installatie is geregistreerd. De code kan op een object buiten armsafstand worden geplaatst: toiletartikelen in een badkamer, een ontbijtartikel in een keuken, of een ander stabiel object in een goed verlichte ruimte. NFC volgt hetzelfde algemene idee met een compatibele tag en apparaat. De app slaat een hash-representatie op in de huidige paden in plaats van de ruwe code nodig te hebben voor gewone vergelijking.

Kies een object dat nog steeds beschikbaar zal zijn wanneer het alarm afgaat. Verpakking wordt weggegooid, labels vervagen en reizen verandert de omgeving. Een code registreren op de enige medicijndoos die u mogelijk moet vervangen is minder robuust dan het gebruik van een duurzaam label. De [alarminstallatiehandleiding](../guides/set-up-an-alarm.md) behandelt plaatsing en testen.

## Uitdagingsmissies ruilen beweging voor inspanning

Wiskunde en typen vereisen gerichte invoer. Schudden en stappen vereisen fysieke beweging en ondersteunde sensoren. Moeilijkheids- en doelinstellingen veranderen hoeveel werk er wordt verwacht, maar een moeilijkere missie is niet automatisch een betere. Overmatige wrijving kan ertoe aanzetten het alarm volledig uit te schakelen, terwijl een gemakkelijke taak na herhaling automatisch kan worden.

Pas de taak aan de faalmodus aan. Als je alarmen half in slaap uitzet, creëert scannen in een andere kamer nuttige afstand. Als camera-toegang onhandig is, kan een korte typ- of wiskundetaak praktischer zijn. Als mobiliteit, evenwicht of toegankelijkheid een zorg is, vermijd dan bewegingsgebaseerde missies en kies een taak die veilig kan worden voltooid.

## Enkelvoudige, keten- en willekeurige modi

Enkelvoudige modus vraagt om één geconfigureerde missie. Ketelmodus voert verschillende geconfigureerde missies opeenvolgend uit. Willekeurige modus selecteert uit een geconfigureerde set, waardoor de kans wordt verminderd dat één gememoriseerde interactie automatisch wordt. Deze modi zijn aanwezig in de nieuwere gecontroleerde bron; [beschikbaarheid](../availability.md) legt uit waarom dat niet bewijst dat ze al in elke openbare build zitten.

Voer altijd een test op korte termijn uit na het wijzigen van de modus, machtigingen of geregistreerde objecten. Houd het geselecteerde object bereikbaar en bied een veilige herstelroute. Gebruik voor leveringsproblemen die niet gerelateerd zijn aan missievoltooiing de [betrouwbaarheidschecklist](../help/alarm-delivery.md).

