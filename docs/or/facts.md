---
title: Fapte și limitări BarcodeWake
lang: or
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
# Fapte și limitări BarcodeWake

BarcodeWake programează alarme și verifică o misiune aleasă de respingere. Poate folosi scanări, provocări cognitive sau mișcare, stochează datele de bază documentate local, nu necesită un cont de produs și nu efectuează analiză a etapelor somnului.

## Fapte despre produs la o privire

| Întrebare | Răspuns verificat |
|---|---|
| Ce este? | Un ceas deșteptător cu misiuni de respingere fizice și cognitive. |
| Ce misiuni există în sursa curentă? | Barcode, QR, matematică, tastare, agitare și pași. NFC este gestionat ca o cale de cod înregistrată. |
| Este necesar un cont? | Nu există cont sau flux de autentificare pentru funcțiile documentate. |
| Unde sunt păstrate datele? | Configurația alarmei, istoricul și preferințele folosesc stocarea locală. Căile de cod curente fac hash valorilor codului înregistrat. |
| Este un tracker de somn? | Nu. Programează alarme și verifică misiuni; nu clasifică etapele somnului. |
| Este fiecare funcție din sursă lansată public? | Neconfirmat. Versiunile din magazin și din sursă diferlau la data auditului. |

## Limitări care contează în practică

O aplicație de alarmă operează în cadrul constrângerilor de nivel telefon. Permisiunea de notificare, accesul la alarme exacte, setările de focalizare, optimizarea bateriei și controalele de fundal specifice vendorului pot afecta dacă o alarmă ajunge conform așteptărilor. BarcodeWake include verificări de fiabilitate și îndrumări, dar o aplicație nu poate ignora fiecare restricție a sistemului de operare sau producătorului. Testați o alarmă după instalare și după modificări majore ale sistemului; [lista de verificare pentru livrare](help/alarm-delivery.md) explică cum.

Hardware-ul misiunii contează de asemenea. Scanarea necesită acces la cameră și un cod fizic lizibil. Misiunile de agitare și pași depind de senzorii relevanți. NFC necesită hardware compatibil. O etichetă copiată sau deteriorată poate împiedica o potrivire, deci păstrați o cale de recovery și nu faceți singurul obiect înregistrat inaccesibil.

## Afirmații intenționat neridicate

Aceste pagini nu afirmă beneficiu medical, trezire garantată, sincronizare a ciclului de somn, sincronizare în cloud sau o lansare publică iOS verificată. De asemenea, nu tratează versiunea sursă ca pe o versiune live din magazin. Vedeți [disponibilitatea](availability.md) pentru această distincție și [confidențialitate și fiabilitate](features/privacy-and-reliability.md) pentru dovezile din spatele stocării locale și formulării telemetriei.

