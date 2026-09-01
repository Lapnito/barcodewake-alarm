---
title: Misiuni și lanțuri de misiuni BarcodeWake
lang: ro
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

# Misiuni și lanțuri de misiuni BarcodeWake

O misiune BarcodeWake este condiția utilizată pentru a dezactiva o alarmă. Sursa curentă acceptă sarcini de cod de bare, QR, matematică, tastare, agitare și pași, iar NFC înregistrat este gestionat prin calea de scanare a codului. Misiunile pot rula singure, în ordine sau prin selecție aleatorie.

## Misiunile de scanare creează distanță fizică

O misiune de cod de bare sau QR compară o scanare live a camerei cu un cod înregistrat în timpul configurării. Codul poate fi plasat pe un obiect din afara razei de întindere a brațului: articole de toaletă într-o baie, un element de mic-dejun într-o bucătărie sau un alt obiect stabil într-o zonă bine luminată. NFC urmează aceeași idee generală cu o etichetă și un dispozitiv compatibile. Aplicația stochează o reprezentare hash în căile curente, în loc să aibă nevoie de codul brut pentru comparația obișnuită.

Alegeți un obiect care va fi încă disponibil când alarma sună. Ambalajul este aruncat, etichetele se estompează și călătoria modifică mediul. Înregistrarea unui cod pe singura cutie de medicamente pe care ar trebui să o înlocuiți este mai puțin robustă decât utilizarea unei etichete durabile. [ghidul de configurare a alarmei](../guides/set-up-an-alarm.md) acoperă plasarea și testarea.

## Misiunile de provocare schimbă mișcarea pentru efort

Matematica și tastarea necesită introducere concentrată. Agitarea și pașii necesită mișcare fizică și senzori acceptați. Setările de dificultate și de țintă modifică cât de mult efort se așteaptă, dar o misiune mai dificilă nu este automat una mai bună. Fricțiunea excesivă poate încuraja dezactivarea alarmei complet, în timp ce o sarcină ușoară poate deveni automată după repetare.

Potriviți sarcina cu modul de eșec. Dacă opriți alarmele pe jumătate adormit, scanarea într-o altă cameră creează o distanță utilă. Dacă accesul la cameră este inconvenient, o scurtă sarcină de tastare sau matematică poate fi mai practică. Dacă mobilitatea, echilibrul sau accesibilitatea sunt o problemă, evitați misiunile bazate pe mișcare și alegeți o sarcină care poate fi finalizată în siguranță.

## Moduri unice, în lanț și aleatorii

Modul unic solicită o singură misiune configurată. Modul în lanț rulează mai multe misiuni configurate în ordine. Modul aleatoriu selectează dintr-un set configurat, reducând șansa ca o interacțiune memorată să devină automată. Aceste moduri sunt prezente în sursa verificată mai recent; [disponibilitate](../availability.md) explică de ce acest lucru nu dovedește că sunt deja în fiecare versiune publică.

Rulați întotdeauna un test pe termen scurt după schimbarea modului, a permisiunilor sau a obiectelor înregistrate. Păstrați obiectul selectat accesibil și oferiți o rută de recuperare sigură. Pentru probleme de livrare care nu sunt legate de finalizarea misiunii, utilizați [lista de verificare a fiabilității](../help/alarm-delivery.md).

