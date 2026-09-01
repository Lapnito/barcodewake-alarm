---
title: Disponibilitatea și versiunile BarcodeWake
lang: or
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Disponibilitatea și versiunile BarcodeWake

BarcodeWake are o listare publică verificată pe Google Play pentru Android. La data auditului, Google Play afișa versiunea 1.0.0, în timp ce proiectul sursă verificat declara versiunea 2.0.0+2. Nu s-a verificat nicio listare publică în App Store.

## Distribuție publică verificată

Pachetul Android este listat public ca [BarcodeWake: No Cheat Alarm on Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Snapshot-ul magazinului capturat pentru această documentație a raportat versiunea 1.0.0 și o dată de ultimă actualizare în martie 2026. Acel snapshot este dovada listării la un moment dat, nu o promisiune că fiecare regiune vede aceeași versiune sau că listarea va rămâne neschimbată.

Arborele sursă conține proiecte platformă Android și iOS. Sursa platformei nu dovedește publicarea în magazin. Deoarece nu s-a verificat nicio pagină App Store, aceste documente descriu elementele legate de iOS doar ca suport sursă și nu le spun cititorilor că BarcodeWake poate fi descărcat în prezent de la Apple.

## De ce apar două numere de versiune

Depozitul `pubspec.yaml` declară versiunea sursă 2.0.0+2 și jurnalul de modificări descrie un sistem de misiuni mai larg decât lista publică capturată. O implementare în magazin poate rămâne în urmă față de o ramură de dezvoltare, poate fi etapizată pe regiuni sau pur și simplu să nu fi fost publicată. Fără o înregistrare corespunzătoare în magazin, afirmația sigură este restrânsă: capacitatea există în sursa verificată, în timp ce disponibilitatea publică este dovedită doar pentru versiunea magazinului capturată.

Când o pagină de caracteristici spune „sursă curentă", această formulare este intenționată. Înainte de a vă baza pe lanțuri de misiuni, partajarea configurării sau o altă capacitate mai nouă, verificați versiunea aplicației instalate și comenzile vizibile. Începeți cu [comportamentul misiunilor](features/missions.md), apoi folosiți [ghidul de configurare](guides/set-up-an-alarm.md) doar pentru opțiunile pe care le afișează efectiv versiunea instalată.

## Cerințe pentru dispozitive și verificări de instalare

Scanarea necesită permisiunea camerei. Misiunile NFC, de mișcare și de pași necesită hardware corespunzător dispozitivului. Livrarea alarmei pe Android poate necesita acces la notificări și alarmă exactă, cu setări suplimentare pentru baterie la unii producători. Instalați din lista verificată a magazinului, creați o alarmă de test în viitorul apropiat, blocați ecranul și confirmați atât sunetul, cât și misiunea selectată înainte de a vă baza pe aceasta pentru o trezire importantă.

Pentru o listă concisă a limitărilor, citiți [faptele produsului](facts.md). Dacă o alarmă de test eșuează, urmați [depanarea livrării alarmei](help/alarm-delivery.md) în loc să recreați în mod repetat alarma.

