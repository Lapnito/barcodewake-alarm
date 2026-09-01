---
title: Faceți backup și partajați alarmele BarcodeWake în siguranță
lang: or
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Faceți backup și partajați alarmele BarcodeWake în siguranță

Folosiți o exportare JSON când păstrați sau mutați propriile date din aplicație, un cod de bare PDF imprimabil pentru backup pentru recuperare și partajare QR de configurare când altă persoană are nevoie doar de structura alarmei. Partajarea omite în mod intenționat secretele înregistrate și istoricul.

## Alegeți formatul potrivit pentru sarcină

Sursa curentă oferă căi de schimb diferite deoarece backup-ul și partajarea nu sunt aceeași operațiune. Un backup JSON este destinat transferului structurat de date și restaurării. Un backup PDF transformă materialul de recuperare într-un document cu cod de bare imprimabil. Un QR de configurare este deliberat mai îngust: poate transmite o configurație limitată de alarmă fără a purta valori de cod de bare înregistrate, identificatori NFC, PIN-uri sau istoric.

Nu tratați un QR de configurare ca pe un backup complet al dispozitivului. Destinatarul trebuie să-și înregistreze propriile coduri fizice și să revizuiască permisiunile local. Partajarea curentă a configurării limitează și câte alarme transportă, așa că verificați rezultatul importat în loc să presupuneți că fiecare program s-a mutat. [Faptele despre produs](../facts.md) înregistrează aceste limite.

## Creați și protejați un backup personal

Folosiți acțiunea de exportare disponibilă în build-ul instalat, alegeți JSON sau backup-ul imprimabil conform planului de recuperare și salvați rezultatul undeva sub controlul dumneavoastră. Un backup poate dezvălui numele alarmelor, programele și alte configurații chiar dacă valorile brute de cod înregistrate sunt protejate sau omise. Gestionați-l ca pe date personale de rutină: evitați linkurile publice, imprimantele partajate și canalele de mesagerie neverificate.

După exportare, confirmați că fișierul poate fi găsit și că timestamp-ul său corespunde backup-ului prevăzut. Nu ștergeți datele originale ale aplicației doar pentru că o comandă de exportare a raportat succes. Testarea restaurării este singura verificare de încredere, dar efectuați-o pe un dispozitiv sigur sau după ce faceți o a doua copie, astfel încât testul însuși să nu devină un eveniment de pierdere.

## Partajați configurarea fără a partaja secrete

Generați un QR de configurare doar pentru alarmele pe care destinatarul ar trebui să le primească. Destinatarul îl scanează, verifică programul importat și furnizează propriul cod, etichetă NFC sau detalii de recuperare. Acest design previne transferarea în tăcere a cheii fizice care respinge alarma altcuiva printr-o configurație partajată.

După import, fiecare persoană ar trebui să ruleze [testul complet de configurare a alarmei](set-up-an-alarm.md). Permisiunile, senzorii și restricțiile sistemului de operare nu se transferă în QR. Dacă o alarmă importată nu apare în timp ce este blocată, urmați [depanarea livrării alarmelor](../help/alarm-delivery.md).

Versiunile sursă și magazin au diferit în timpul acestui audit, deci un build public instalat poate să nu expună fiecare opțiune de schimb descrisă aici. [Disponibilitatea](../availability.md) explică cum să interpretați capabilitățile disponibile doar în sursă.

