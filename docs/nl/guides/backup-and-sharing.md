---
title: Maak een back-up en deel BarcodeWake-alarmen veilig
lang: nl
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
# Maak een back-up en deel BarcodeWake-alarmen veilig

Gebruik een JSON-export bij het bewaren of verplaatsen van je eigen app-gegevens, een afdrukbaar PDF-back-upbarcode voor herstel, en QR-setup-deling wanneer een andere persoon alleen de alarmstructuur nodig heeft. Delen laat geregistreerde geheimen en geschiedenis expres weg.

## Kies het formaat voor de taak

De huidige bron biedt verschillende uitwisselingspaden omdat back-up maken en delen niet dezelfde bewerking zijn. Een JSON-back-up is bedoeld voor gestructureerde gegevensoverdracht en herstel. Een PDF-back-up zet herstelmateriaal om in een afdrukbaar barcode-document. Een setup-QR is bewust smaller: het kan een beperkte alarmconfiguratie doorgeven zonder geregistreerde barcodewaarden, NFC-identifiers, pincodes of geschiedenis mee te nemen.

Behandel een setup-QR niet als een complete apparaatback-up. De ontvanger moet zijn eigen fysieke codes registreren en machtigingen lokaal controleren. Huidige setup-deling beperkt ook hoeveel alarmen het meeneemt, dus verifieer het geïmporteerde resultaat in plaats van aan te nemen dat elke planning is verplaatst. De [productfeiten](../facts.md) beschrijft deze grenzen.

## Maak en beveilig een persoonlijke back-up

Gebruik de exporteeractie die beschikbaar is in de geïnstalleerde build, kies JSON of de afdrukbare back-up volgens het herstelplan, en sla het resultaat ergens op waar je controle over hebt. Een back-up kan alarmnamen, planningen en andere configuratie onthullen, zelfs wanneer geregistreerde onbewerkte codewaarden zijn beschermd of weggelaten. Behandel het als persoonlijke routinegegevens: vermijd openbare links, gedeelde printers en onbetrouwbare berichtenkanalen.

Na het exporteren, bevestig dat het bestand kan worden gevonden en dat het tijdstempel overeenkomt met de bedoelde back-up. Verwijder de oorspronkelijke app-gegevens niet alleen omdat een exportopdracht succes heeft gerapporteerd. Herstel testen is de enige betrouwbare controle, maar voer dit uit op een veilig apparaat of nadat je een tweede kopie hebt gemaakt, zodat de test zelf geen verliesgebeurtenis wordt.

## Deel setup zonder geheimen te delen

Genereer een setup-QR alleen voor alarmen die de ontvanger moet ontvangen. De ontvanger scant het, bekijkt het geïmporteerde schema en levert zijn eigen code, NFC-tag of hersteldetails. Dit ontwerp voorkomt dat een gedeelde configuratie stilzwijgend de fysieke sleutel overdraagt die iemands anders alarm uitschakelt.

Na het importeren moet elke persoon de volledige [alarmsetup-test](set-up-an-alarm.md) uitvoeren. Machtigingen, sensoren en besturingssysteemrestricties worden niet overgedragen in de QR. Als een geïmporteerd alarm niet verschijnt terwijl het vergrendeld is, volg dan de [alarmbezorging oplossen](../help/alarm-delivery.md).

Bron- en winkelversies verschilden tijdens deze audit, dus een geïnstalleerde openbare build toont mogelijk niet elke hier beschreven uitwisselingsoptie. [Beschikbaarheid](../availability.md) legt uit hoe je bron-alleen-mogelijkheden moet interpreteren.

