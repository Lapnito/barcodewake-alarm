---
title: Waarom een BarcodeWake-alarm mogelijk niet afgaat
lang: nl
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
# Waarom een BarcodeWake-alarm mogelijk niet afgaat

Een opgeslagen alarm kan nog steeds worden geblokkeerd door meldingsinstellingen, toegang tot exacte alarmen, focus- of stille modi, laag volume, batterijbeperkingen, opschorting van apps of achtergrondbediening van de fabrikant. Controleer de aflevering apart van missiescanning en voer vervolgens een test op het vergrendelscherm uit.

## Isoleer eerst de aflevering van het negeren

Maak een testalarm voor de korte termijn met een eenvoudige missie en laat de app op de achtergrond draaien. Vergrendel het scherm. Als er geen alarmscherm of geluid verschijnt, ligt het probleem bij de aflevering; het wijzigen van de geregistreerde streepjescode zal dit niet oplossen. Als het alarm wel verschijnt maar de missie niet kan worden voltooid, werkt de aflevering en ligt het probleem bij de camera, sensor, codematching of missieconfiguratie.

Controleer of het alarm is ingeschakeld, of de geplande dag correct is en of de tijdzone van de telefoon overeenkomt met het beoogde schema. Controleer het media- en alarmvolume in plaats van alleen af te gaan op de status van de zijknop. Bekijk de niet-storen- of focusregels, verbonden audioapparaten en of de telefoon opnieuw is opgestart nadat het alarm werd gemaakt.

## Bekijk de machtigingspoorten van het besturingssysteem

 Sta meldingen en alle toegang tot exacte alarmen of alarmen in volledig scherm toe die worden gevraagd door de geïnstalleerde build. Verwijder BarcodeWake uit agressieve batterijoptimalisatie of automatische slaaplijsten wanneer de apparaatleverancier die bedieningselementen biedt. Open de betrouwbaarheidsdiagnostiek in de app en volg de apparaatspecifieke instellingen die deze identificeert. De pagina [privacy en betrouwbaarheid](../features/privacy-and-reliability.md) legt uit waarom deze systeemafhankelijkheden blijven bestaan, zelfs wanneer app-gegevens lokaal zijn.

Nadat u één instelling hebt gewijzigd, herhaalt u de test op het vergrendelscherm. Het wijzigen van verschillende bedieningselementen tegelijk maakt het moeilijker om de oorzaak te identificeren. Systeemupdates kunnen machtigingen opnieuw instellen of opnieuw interpreteren, dus test opnieuw na een grote update of herinstallatie van de app.

## Diagnosticeer de missievoltooiing apart

Voor streepjescode- en QR-missies reinigt u de cameralens, verbetert u de verlichting en bevestigt u dat het geregistreerde object ongewijzigd is. Verleen cameratoegang. Voor NFC verifieert u de apparaatondersteuning en houdt u de tag nabij de juiste antennepositie. Schud- en stapmissies zijn afhankelijk van bewegings- of stapsensoren en kunnen anders werken wanneer energiebesparingsmodi de sensortoelevering beperken.

Als een missie is geconfigureerd als onderdeel van een keten, moet elke vereiste stap worden voltooid. Bekijk [missiegedrag](../features/missions.md) en maak indien nodig een nieuwe test met de [installatieprocedure](../guides/set-up-an-alarm.md).

## Weet wanneer de telefoon de grens is

BarcodeWake kan een uitgeschakeld apparaat, een lege batterij, kapotte audiohardware of elke fabrikantstaakdoder niet overschrijven. Het is geen noodsituatie-notificatiedienst. Houd een andere alarmmethode aan voor situaties met hoge gevolgen en meld reproduceerbare storingen met apparaatmodel, systeemversie, app-versie en de exacte testomstandigheden.

