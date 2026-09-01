---
title: Missions i cadenes de missions de BarcodeWake
lang: ca
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

# Missions i cadenes de missions de BarcodeWake

Una missió de BarcodeWake és la condició utilitzada per desactivar una alarma. La font actual admet tasques de codi de barres, QR, matemàtiques, escriptura, sacseig i passos, i el NFC registrat es gestiona a través del camí d'escaneig de codi. Les missions poden executar-se soles, en seqüència o per selecció aleatòria.

## Les missions d'escaneig creen distància física

Una missió de codi de barres o QR compara un escaneig de càmera en temps real amb un codi registrat durant la configuració. El codi es pot col·locar en un objecte fora de l'abast del braç: articles de toilet a un bany, un article d'esmorzar a una cuina, o un altre objecte estable en una zona ben il·luminada. El NFC segueix la mateixa idea general amb una etiqueta i un dispositiu compatibles. L'aplicació emmagatzema una representació hash en les rutes actuals en lloc de necessitar el codi cru per a la comparació ordinària.

Trieu un objecte que encara estarà disponible quan soni l'alarma. L'embalatge es llença, les etiquetes s'esvaeixen i els viatges canvien l'entorn. Registrar un codi a la capsa de medicines que potser haureu de substituir és menys robust que fer servir una etiqueta duradora. La [guia de configuració d'alarma](../guides/set-up-an-alarm.md) tracta la col·locació i les proves.

## Les missions de repte intercanvien moviment per esforç

Les matemàtiques i l'escriptura requereixen entrada concentrada. El sacseig i els passos requereixen moviment física i sensors compatibles. La configuració de dificultat i objectiu canvia quant de treball s'espera, però una missió més difícil no és automàticament millor. Una fricció excessiva pot induir a desactivar l'alarma completament, mentre que una tasca fàcil pot fer-se automàtica després de la repetició.

Adequeu la tasca al mode de fallada. Si apagueu les alarmes mig adormits, escanejar en una altra habitació crea una distància útil. Si l'accés a la càmera és inconvenient, una tasca curta d'escriptura o de matemàtiques pot ser més pràctica. Si la mobilitat, l'equilibri o l'accessibilitat és una preocupació, eviteu les missions basades en moviment i trieu una tasca que es pugui completar de manera segura.

## Modes individual, encadenat i aleatori

El mode individual demana una missió configurada. El mode encadenat executa diverses missions configurades en ordre. El mode aleatori selecciona d'un conjunt configurat, reduint la probabilitat que una interacció memoritzada es faci automàtica. Aquests modes estan presents al codi font més recent verificat; la [disponibilitat](../availability.md) explica per què això no demostra que ja estiguin a cada versió pública.

Executeu sempre una prova a curt termini després de canviar el mode, els permisos o els objectes registrats. Mantingueu l'objecte seleccionat a l'abast i proporcioneu una ruta de recuperació segura. Per a problemes de lliurament no relacionats amb la finalització de la missió, feu servir la [llista de verificació de fiabilitat](../help/alarm-delivery.md).

