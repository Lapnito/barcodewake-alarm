---
title: Salvare și partajare în siguranță a alarmelor BarcodeWake
lang: ro
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
# Salvare și partajare în siguranță a alarmelor BarcodeWake

Folosește o exportare JSON când dorești să păstrezi sau să muți datele proprii ale aplicației, un cod de bare PDF imprimabil pentru backup în caz de recuperare și partajarea QR de configurare când altă persoană are nevoie doar de structura alarmei. Partajarea omite în mod deliberat secretele înregistrate și istoricul.

## Alegeți formatul potrivit pentru sarcină

Sursa curentă oferă diferite căi de schimb, deoarece backup-ul și partajarea nu sunt aceeași operație. Un backup JSON este destinat transferului structurat de date și restaurării. Un backup PDF transformă materialul de recuperare într-un document cod de bare imprimabil. Un QR de configurare este deliberat mai restrâns: poate transmite o configurație limitată a alarmei fără a transporta valorile de cod de bare înregistrate, identificatorii NFC, PIN-urile sau istoricul.

Nu trata un QR de configurare ca pe o copie de siguranță completă a dispozitivului. Destinatarul trebuie să-și înregistreze propriile coduri fizice și să verifice permisiunile local. Partajarea curentă de configurare limitează și câte alarme poate transporta, așadar verifică rezultatul importat în loc să presupui că fiecare program s-a mutat. [Faptele produsului](../facts.md) înregistrează aceste limite.

## Creați și protejați un backup personal

Folosește acțiunea de export disponibilă în build-ul instalat, alege JSON sau backup-ul imprimabil conform planului de recuperare și salvează rezultatul undeva sub controlul tău. Un backup poate dezvălui numele alarmelor, programările și alte configurații chiar dacă valorile brute de cod înregistrate sunt protejate sau omise. Tratează-l ca pe niște date personale de rutină: evită link-urile publice, imprimantele partajate și canalele de mesagerie neverificate.

După export, confirmă că fișierul poate fi găsit și că timestamp-ul său corespunde backup-ului dorit. Nu șterge datele originale ale aplicației doar pentru că o comandă de export a raportat succes. Testarea restaurării este singura verificare sigură, însă efectueaz-o pe un dispozitiv sigur sau după ce ai făcut o a doua copie, astfel încât testul în sine să nu devină un eveniment de pierdere.

## Partajați configurarea fără a partaja secrete

Generează un QR de configurare doar pentru alarmele pe care destinatarul ar trebui să le primească. Destinatarul îl scanează, verifică programul importat și furnizează propriul cod, etichetă NFC sau detalii de recuperare. Acest design previne transferarea silențioasă a cheii fizice care dezactivează alarma altcuiva printr-o configurație partajată.

După import, fiecare persoană ar trebui să ruleze testul complet de [test de configurare a alarmei](set-up-an-alarm.md). Permisiunile, senzorii și restricțiile sistemului de operare nu se transferă în QR. Dacă o alarmă importată nu apare când este blocată, urmează [depanarea livrării alarmei](../help/alarm-delivery.md).

Versiunile sursei și din magazin au diferit în timpul acestui audit, astfel încât o versiune publică instalată poate să nu expună fiecare opțiune de schimb descrisă aici. [Disponibilitate](../availability.md) explică cum să interpretezi capabilitățile disponibile doar în sursă.

