---
title: Com configurar una alarma BarcodeWake
lang: ca
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---
# Com configurar una alarma BarcodeWake

Creeu primer la programació, trieu una missió que sigui segura i pràctica, concediu els permisos necessaris i, tot seguit, feu una prova a curt termini amb la pantalla bloquejada. Per a les missions d'escaneig, registreu un objecte durador que estarà disponible i llegible quan soni l'alarma.

## Trieu la missió abans de l'objecte

Decidiu quina acció ha de separar el despertar del descart. Un codi de barres a una altra habitació crea distància física. Les matemàtiques o escriure afegeixen concentració sense necessitat de càmera. Agitar o fer passos afegeix moviment però depèn dels sensors i pot no ser adequat per a totes les persones o entorns. La [referència de la missió](../features/missions.md) explica els compromisos entre els modes individual, encadenat i aleatori.

Si feu servir un codi de barres, codi QR o etiqueta NFC, trieu alguna cosa duradora. Eviteu l'embalatge d'un sol ús, un objecte que un altre membre de la llar pugui moure o un codi que serà inaccessible mentre viatgeu. Comproveu que la càmera pot enfocar amb la llum esperada. NFC necessita un telèfon i una etiqueta compatibles.

## Configureu la programació i la regla de descart

Obriu l'editor d'alarmes, configureu l'hora desitjada i els dies actius i, tot seguit, seleccioneu la missió mostrada per la versió instal·lada. Configureu-ne la dificultat o l'objectiu de manera conservadora per a la primera prova. Si la versió instal·lada admet cadenes, organitzeu les missions en un ordre que es pugui completar de manera segura sense córrer per les escales ni sortir d'una àrea segura.

Registreu el codi física des del flux de configuració de la missió. Doneu a l'alarma una etiqueta que identifiqui la rutina prevista en lloc d'exposar informació sensible. Reviseu el volum, la vibració i qualsevol opció de seguiment posterior al despertar que es mostri a la versió instal·lada. Els controls disponibles poden diferir perquè les [versions pública i del codi font](../availability.md) no eren idèntiques en la data de l'auditoria.

## Concediu permisos amb un propòsit

Permeteu les notificacions i l'accés relacionat amb l'alarma necessari per al lliurament. Concediu accés a la càmera només quan feu servir una missió d'escaneig i accés als sensors quan la missió escollida ho necessiti. A Android, reviseu la configuració d'alarma exacta i de bateria si la verificació de fiabilitat de l'app ho indica. No suposeu que desar una alarma provingui que el lliurament en segon pla està permès.

## Proveu el recorregut complet durant la nit

Programeu una prova uns minuts endavant. Bloquegeu la pantalla, deixeu BarcodeWake en segon pla i poseu el telèfon en el mateix estat de so i d'energia previst per a la nit. Confirmeu que l'alarma apareix, que l'àudio és audible i que la missió exacta seleccionada es pot completar. Tot seguit repetiu-ho després de moure l'objecte registrat a la seva ubicació real.

Si el lliurament falla, feu servir la [llista de verificació del lliurament d'alarma](../help/alarm-delivery.md). Si té èxit, penseu a fer una [còpia de seguretat local](backup-and-sharing.md) un cop la configuració estigui estable.

