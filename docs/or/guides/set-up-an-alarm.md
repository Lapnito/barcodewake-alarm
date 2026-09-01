---
title: Cum să configurați o alarmă BarcodeWake
lang: or
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
# Cum să configurați o alarmă BarcodeWake

Creează mai întâi programul, alege o misiune care este sigură și practică, acordă permisiunile necesare, apoi efectuează un test pe termen scurt cu ecranul blocat. Pentru misiunile de scanare, înregistrează un obiect durabil care va fi disponibil și lizibil când alarma sună.

## Alege misiunea înainte de obiect

Decide ce acțiune ar trebui să separe trezirea de respingere. Un cod de bare din altă cameră creează distanță fizică. Matematica sau tastarea adaugă concentrare fără a necesita o cameră. Agitarea sau pașii adaugă mișcare, dar depind de senzori și pot să nu se potrivească pentru fiecare persoană sau mediu. [Referința misiunii](../features/missions.md) explică compromisurile dintre modurile single, chain și random.

Dacă folosești un cod de bare, cod QR sau etichetă NFC, alege ceva durabil. Evită ambalajele de unică folosință, un obiect pe care alt membru al gospodăriei l-ar putea muta sau un cod care va fi inaccesibil în timpul călătoriei. Verifică că camera poate focaliza în lumina așteptată. NFC necesită un telefon și o etichetă compatibile.

## Configurează programul și regula de respingere

Deschide editorul de alarme, setează ora dorită și zilele active, apoi selectează misiunea afișată de build-ul instalat. Configurează-i dificultatea sau ținta conservator pentru primul test. Dacă versiunea instalată acceptă lanțuri, aranjează misiunile într-o ordine care poate fi completată în siguranță fără a te grăbi pe scări sau a părăsi o zonă sigură.

Înregistrează codul fizic din fluxul de configurare a misiunii. Dă alarmei o etichetă care identifică rutina dorită în loc să expui informații sensibile. Verifică volumul, vibrațiile și orice opțiuni de urmărire a trezirii vizibile în build-ul instalat. Controalele disponibile pot diferi deoarece [versiunea publică și cea sursă](../availability.md) nu erau identice la data auditului.

## Acordă permisiunile cu un scop

Permite notificările și accesul legat de alarme necesare pentru livrare. Acordă accesul la cameră doar când folosești o misiune de scanare și accesul la senzori când misiunea aleasă are nevoie de aceasta. Pe Android, verifică setările de alarmă exactă și baterie dacă verificarea fiabilității aplicației le semnalează. Nu presupune că salvarea unei alarme dovedește că livrare în fundal este permisă.

## Testează întreaga cale overnight

Programează un test cu câteva minute înainte. Blochează ecranul, lasă BarcodeWake în fundal și pune telefonul în același stare de sunet și alimentare planificată pentru overnight. Confirmă că alarma apare, audio este audibil și misiunea selectată poate fi completată. Apoi repetă după mutarea obiectului înregistrat în locația sa reală.

Dacă livrarea eșuează, folosește [lista de verificare pentru livrare alarme](../help/alarm-delivery.md). Dacă reușește, ia în considerare crearea unei [copii de siguranță locale](backup-and-sharing.md) după ce configurația este stabilă.

