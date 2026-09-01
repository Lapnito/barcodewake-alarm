---
title: Disponibilitat i versions de BarcodeWake
lang: ca
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilitat i versions de BarcodeWake

BarcodeWake té una fitxa pública verificada a Google Play per a Android. En la data de l'auditoria, Google Play mostrava la versió 1.0.0, mentre que el projecte font verificat declarava la versió 2.0.0+2. No es va verificar cap fitxa pública a l'App Store.

## Distribució pública verificada

El paquet Android apareix publicament com a [BarcodeWake: No Cheat Alarm a Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). L'instantània de la botiga capturada per a aquesta documentació reportava la versió 1.0.0 i una data d'última actualització al març de 2026. Aquesta instantània és evidència de la fitxa en un moment determinat, no una promesa que cada regió vegi el mateix llançament o que la fitxa romandrà sense canvis.

L'arbre font conté projectes de plataforma Android i iOS. El codi font de la plataforma no prova la publicació a la botiga. Com que no es va verificar cap pàgina a l'App Store, aquests documents descriuen els elements relacionats amb iOS com a suport de codi font únicament i no indiquen als lectors que BarcodeWake actualment es pugui descarregar des d'Apple.

## Per què apareixen dos números de versió

El fitxer `pubspec.yaml` del repositori declara la versió font 2.0.0+2 i el seu registre de canvis descriu un sistema de missions més ampli que la fitxa pública capturada. És possible que el llançament a la botiga vagi darrere d'una branca de desenvolupament, s'estigui implementant per regions, o senzillament no s'hagi publicat. Sense un registre coincident a la botiga, l'afirmació segura és restrictiva: la funcionalitat existeix al codi font verificat, mentre que la disponibilitat pública només està provada per a la versió de la botiga capturada.

Quan una pàgina de funcionalitats diu "font actual", aquesta formulació és deliberada. Abans de dependre de cadenes de missions, compartició de configuració o una altra funcionalitat més recent, comproveu la versió de l'aplicació instal·lada i els controls visibles. Comenceu amb [comportament de les missions](features/missions.md), després useu la [guia de configuració](guides/set-up-an-alarm.md) només per a les opcions que la vostra versió instal·lada realment mostra.

## Requisits del dispositiu i comprovacions d'instal·lació

L'escaneig requereix permís de càmera. Les missions NFC, de moviment i de passos necessiten el maquinari corresponent del dispositiu. El lliurament d'alarmes a Android pot requerir accés a notificacions i alarmes exactes, amb configuracions addicionals de bateria en alguns fabricants. Instal·leu des de la fitxa verificada de la botiga, creeu una alarma de prova a curt termini, bloquegeu la pantalla i confirmeu tant el so com la missió seleccionada abans de dependre'n per a un despertar important.

Per a una llista concisa de limitacions, llegiu [fets del producte](facts.md). Si una alarma de prova falla, seguiu la [solució de problemes de lliurament d'alarmes](help/alarm-delivery.md) en lloc de tornar a crear l'alarma repetidament.

