---
title: Disponibilitate și versiuni BarcodeWake
lang: ro
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilitate și versiuni BarcodeWake

BarcodeWake are o listare publică verificată pe Google Play pentru Android. La data auditului, Google Play afișa versiunea 1.0.0, în timp ce proiectul sursă verificat declara versiunea 2.0.0+2. Nu s-a verificat nicio listare publică în App Store.

## Distribuție publică verificată

Pachetul Android este listat public ca [BarcodeWake: No Cheat Alarm pe Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Instantaneul magazinului capturat pentru această documentație raporta versiunea 1.0.0 și o dată ultimei actualizări în martie 2026. Acest instantaneu reprezintă dovezi ale listării la un moment dat, nu o promisiune că fiecare regiune vede aceeași versiune sau că listarea va rămâne neschimbată.

Structura sursă conține proiecte pentru platformele Android și iOS. Codul sursă al platformei nu demonstrează publicarea în magazin. Deoarece nicio pagină App Store nu a fost verificată, această documentație descrie elementele legate de iOS doar ca suport sursă și nu afirmă că BarcodeWake poate fi descărcat în prezent de pe Apple.

## De ce apar două numere de versiune

Fișierul `pubspec.yaml` din repository declară versiunea sursă 2.0.0+2, iar jurnalul modificărilor descrie un sistem de misiuni mai extins decât listarea publică captată. O lansare în magazin poate rămâne în urmă față de o ramură de dezvoltare, poate fi implementată pe regiuni sau pur și simplu să nu fi fost publicată. Fără o înregistrare corespunzătoare în magazin, afirmația sigură este restrânsă: capacitatea există în sursa verificată, în timp ce disponibilitatea publică este dovedită doar pentru versiunea magazinului captată.

Când o pagină de caracteristici menționează „sursa curentă", această formulare este intenționată. Înainte de a vă baza pe lanțuri de misiuni, partajarea configurației sau o altă funcție mai nouă, verificați versiunea instalată a aplicației și comenzile vizibile. Începeți cu [comportamentul misiunilor](features/missions.md), apoi folosiți [ghidul de configurare](guides/set-up-an-alarm.md) doar pentru opțiunile pe care build-ul instalat le afișează efectiv.

## Cerințe de dispozitiv și verificări de instalare

Scanarea necesită permisiunea camerei. Misiunile NFC, de mișcare și de pași necesită hardware corespunzător dispozitivului. Livrarea alarmelor pe Android poate necesita acces la notificări și alarme exacte, cu setări suplimentare de baterie la unii producători. Instalați din listarea verificată a magazinului, creați o alarmă de test în viitorul apropiat, blocați ecranul și confirmați atât sunetul, cât și misiunea selectată înainte de a vă baza pe aceasta pentru o trezire importantă.

Pentru o listă condensată a limitărilor, citiți [faptele produsului](facts.md). Dacă o alarmă de test eșuează, urmați [depanarea livrării alarmelor](help/alarm-delivery.md) în loc să recreați în mod repetat alarma.

