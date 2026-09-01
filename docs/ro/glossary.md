---
title: Terminologia BarcodeWake
lang: ro
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
# Terminologia BarcodeWake

BarcodeWake folosește „misiune” pentru acțiunea necesară pentru a dezactiva o alarmă. Misiunile de scanare verifică un cod fizic înregistrat; misiunile de provocare verifică un răspuns sau o mișcare; partajarea și backup‑ul se referă la diferite formate de schimb.

## Termeni privind alarmele și misiunile

- Alarmă: un eveniment de trezire programat, cu ora, zilele active, sunetul și configurarea pentru a fi dezactivată.
- Misiune: sarcina care trebuie finalizată înainte de dezactivare.
- Misiune de scanare: o sarcină bazată pe cod de bare, QR sau NFC care corespunde unei reprezentări a codului înregistrat.
- Misiune de provocare: o sarcină de matematică, tastare, scuturare sau pas.
- Modul unic: o singură misiune configurată se execută pentru alarmă.
- Modul lanț: misiunile configurate se execută în ordinea aleasă.
- Modul aleator: o misiune este selectată dintr-un set configurat.
- Dificultate: o setare a misiunii care modifică cerința sarcinii; efectul exact depinde de tipul misiunii.

## Termeni privind datele și fiabilitatea

- Cod înregistrat: codul de bare, codul QR sau eticheta NFC fizică asociată cu o misiune de scanare.
- Hash de cod: o reprezentare SHA-256 unidirecțională folosită de căile actuale de stocare și schimb pentru a potrivi valorile înregistrate.
- Backup local: o reprezentare exportată destinată păstrării sau restaurării datelor aplicației.
- QR de configurare: un format limitat de partajare a configurației care omite codurile înregistrate, identificatorii NFC, PIN‑urile și istoricul.
- Doctor de fiabilitate: diagnostice integrate pentru permisiuni și setări de sistem care pot perturba funcționarea alarmei.
- Acces la alarmă exactă: permisiune sau politică a sistemului Android care permite programarea în timp real.
- Optimizare baterie: comenzi ale sistemului de operare sau ale producătorului care pot restricționa execuția în fundal.

Pentru relația completă a funcționalităților, consultați [misiuni și lanțuri de misiuni](features/missions.md). Pentru diferențele dintre formatele de export, citiți [backup și partajare](guides/backup-and-sharing.md). Pagina [fapte](facts.md) definește ce nu pretinde aplicația că măsoară.

