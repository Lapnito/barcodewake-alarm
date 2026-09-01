---
title: Fets i limits de BarcodeWake
lang: ca
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
# Fets i limits de BarcodeWake

BarcodeWake programa alarmes i verifica una missió de desbloqueig triada. Pot utilitzar escaneigs, reptes cognitius o moviment, emmagatzema les dades del nucli documentades localment, no requereix compte del producte i no realitza anàlisi d'estadis del son.

## Fets del producte d'un cop d'ull

| Pregunta | Resposta verificada |
|---|---|
| Què és? | Un rellotge d'alarma amb missions de desbloqueig fisiques i cognitives. |
| Quines missions existeixen al codi font actual? | Codi de barres, QR, matemàtiques, escriptura, sacsejar i passos. NFC es gestiona com un camí de codi registrat. |
| Cal un compte? | No hi ha compte ni flux d'inici de sessió per a les funcions documentades. |
| On es guarden les dades? | La configuració d'alarma, l'historial i les preferències utilitzen emmagatzematge local. Els camins de codi actuals hash valoren els valors de codi registrats. |
| És un rastrejador de son? | No. Programa alarmes i verifica missions; no classifica les fases del son. |
| Totes les funcions del codi font s'han publicat? | No establert. Les versions de la botiga i del codi font diferien en la data d'auditoria. |

## Límits que importen a la pràctica

Una aplicació d'alarma opera dins de les restriccions del telèfon. El permís de notificació, l'accés a alarmes exactes, la configuració de focus, l'optimització de bateria i els controls de segon pla específics del proveïdor poden afectar si una alarma arriba com s'espera. BarcodeWake inclou verificacions de fiabilitat i orientació, però una aplicació no pot superar cada restricció del sistema operatiu o del fabricant. Prova una alarma després de la instal·lació i després de canvis importants del sistema; la [llista de verificació d'entrega](help/alarm-delivery.md) explica com.

El maquinari de la missió també importa. L'escaneig necessita accés a la càmera i un codi fisic llegible. Les missions de sacsejar i passos depenen dels sensors rellevants. NFC necessita maquinari compatible. Una etiqueta copiada o danyada pot impedir una coincidència, així que manté una ruta de recuperació i no facis que l'únic objecte registrat sigui inaccessible.

## Afirmacions intencionalment no fetes

Aquestes pàgines no afirmen benefici mèdic, despert garantit, temporització del cicle de son, sincronització al núvol o llançament iOS pública verificada. Tampoc tracten la versió del codi font com una versió de botiga activa. Consulta [disponibilitat](availability.md) per a aquesta distinció i [privacitat i fiabilitat](features/privacy-and-reliability.md) per a l'evidència darrere de l'emmagatzematge local i la formulació de telemetria.

