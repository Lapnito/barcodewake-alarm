---
title: Terminologie BarcodeWake
lang: or
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
# Terminologie BarcodeWake

BarcodeWake folosește „misiune" pentru acțiunea necesară pentru a dezactiva o alarmă. Misiunile de scanare verifică un cod fizic înregistrat; misiunile de provocare verifică un răspuns sau o mișcare; partajarea și backup-ul se referă la diferite formate de schimb.

## Termeni referitori la alarme și misiuni

- Alarmă: un eveniment de trezire programat cu oră, zile active, sunet și configurație de dezactivare.
- Misiune: sarcina care trebuie îndeplinită înainte de dezactivare.
- Misiune de scanare: o sarcină bazată pe cod de bare, QR sau NFC potrivită cu o reprezentare de cod înregistrat.
- Misiune de provocare: o sarcină de matematică, tastare, scuturare sau pas.
- Mod unic: o singură misiune configurată rulează pentru alarmă.
- Mod lanț: misiunile configurate rulează într-o ordine aleasă.
- Mod aleatoriu: o singură misiune este selectată dintr-un set configurat.
- Dificultate: o setare a misiunii care modifică cerința sarcinii; efectul exact depinde de tipul misiunii.

## Termeni referitori la date și fiabilitate

- Cod înregistrat: codul de bare fizic, codul QR sau eticheta NFC asociată cu o misiune de scanare.
- Hash de cod: o reprezentare unidirecțională SHA-256 folosită de căile actuale de stocare și schimb pentru potrivirea valorilor înregistrate.
- Backup local: o reprezentare exportată destinată conservării sau restaurării datelor aplicației.
- QR de configurare: un format limitat de partajare a configurației care omite codurile înregistrate, identificatorii NFC, PIN-urile și istoricul.
- Doctor de fiabilitate: diagnostice în aplicație pentru permisiuni și setări de sistem care pot interfera cu livrare alarmei.
- Acces alarmă exactă: permisiune sau politică a sistemului Android care permite programarea critică timpului.
- Optimizare baterie: controale ale sistemului de operare sau ale vendorului care pot restricționa execuția în fundal.

Pentru relația completă a funcționalităților, vezi [misiuni și lanțuri de misiuni](features/missions.md). Pentru diferențele dintre formatele de export, citește [backup și partajare](guides/backup-and-sharing.md). Pagina [fapte](facts.md) definește ce nu susține aplicația că măsoară.

