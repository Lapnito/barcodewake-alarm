---
title: Terminologia de BarcodeWake
lang: ca
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# Terminologia de BarcodeWake

BarcodeWake utilitza “missió” per a l'acció requerida per silenciar una alarma. Les missions de lectura verifiquen un codi física registrat; les missions de repte verifiquen una resposta o moviment; compartir i fer còpia de seguretat fan referència a diferents formats d'intercanvi.

## Termes d'alarma i missió

- Alarma: un esdeveniment d'activació programat amb hora, dies actius, so i configuració de silenciament.
- Missió: la tasca que s'ha de completar abans de silenciar l'alarma.
- Missió de lectura: una tasca basada en codi de barres, QR o NFC que es compara amb una representació de codi registrat.
- Missió de repte: una tasca de matemàtiques, escriptura, agitació o passos.
- Mode únic: s'executa una única missió configurada per a l'alarma.
- Mode cadena: les missions configurades s'executen en un ordre triat.
- Mode aleatori: es selecciona una missió d'un conjunt configurat.
- Dificultat: una configuració de missió que canvia la demanda de la tasca; el seu efecte exacte depèn del tipus de missió.

## Termes de dades i fiabilitat

- Codi registrat: el codi de barres, codi QR o etiqueta NFC associat a una missió de lectura.
- Hash de codi: una representació SHA-256 unidireccional utilitzada per les rutes d'emmagatzematge i intercanvi actuals per fer coincidir valors registrats.
- Còpia de seguretat local: una representació exportada dissenyada per preservar o restaurar les dades de l'aplicació.
- QR de configuració: un format de compartició de configuració limitat que omet els codis registrats, identificadors NFC, PINs i historial.
- Doctor de fiabilitat: diagnòstics dins de l'aplicació per a permisos i configuracions del sistema que podrien interfere amb el lliurament de l'alarma.
- Accés a alarmes exactes: permís o política del sistema Android que permet la programació dependent del temps.
- Optimització de bateria: controls del sistema operatiu o del proveïdor que podrien restringir l'execució en segon pla.

Per a la relació completa de funcions, vegeu [missions i cadenes de missions](features/missions.md). Per a les diferències entre formats d'exportació, llegiu [còpia de seguretat i compartició](guides/backup-and-sharing.md). La [pàgina de fets](facts.md) defineix el que l'aplicació no afirma mesurar.

