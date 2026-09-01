---
title: Confidențialitatea și fiabilitatea alarmei BarcodeWake
lang: ro
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# Confidențialitatea și fiabilitatea alarmei BarcodeWake

BarcodeWake păstrează configurația documentată a alarmei și datele misiunii pe dispozitiv și nu necesită un cont de aplicație. Căile curente ale codului hash valorile codurilor înregistrate. Telemetria opțională este descrisă ca dezactivată în mod implicit, în timp ce livrarea alarmei depinde în continuare de permisiunile sistemului și de controalele furnizorului.

## Datele locale nu elimină dependențele de sistem

Stocarea locală înseamnă că configurarea obișnuită a alarmei nu necesită un cont cloud BarcodeWake. Înregistrările alarmei, istoricul și preferințele sunt gestionate prin stratul de date local al aplicației. Valorile înregistrate ale codurilor de bare, QR și NFC sunt reprezentate cu hash-uri SHA-256 în căile curente de stocare și import, ceea ce evită păstrarea valorii brute obișnuite pentru potrivire.

Hashing-ul nu este același lucru cu criptarea fiecărei înregistrări a aplicației, iar stocarea locală nu este o copie de rezervă. Cineva cu acces la un dispozitiv deblocat poate vedea în continuare numele alarmelor, programele sau istoricul prin aplicație. Un telefon pierdut sau resetat poate pierde, de asemenea, datele locale, cu excepția cazului în care utilizatorul a făcut o exportare. Consultați [copia de rezervă și partajarea](../guides/backup-and-sharing.md) pentru formatele și scopurile lor diferite.

Politica de confidențialitate spune că telemetria opțională este dezactivată în mod implicit și descrie manipularea agregată dacă este activată. Prin urmare, această documentație nu face afirmația mai largă că aplicația nu poate comunica niciodată într-o rețea. Aceasta afirmă faptele verificate mai înguste: operațiunea de bază și datele sunt locale, nu este necesar un cont de produs și nu apare nicio dependență de SDK de publicitate în proiectul verificat.

## Fiabilitatea este o responsabilitate partajată

BarcodeWake poate programa și prezenta o alarmă, dar sistemul de operare decide când munca în fundal poate rula și care întreruperi sunt permise. Permisiunea de notificare, accesul la alarma exactă, modul silențios sau de concentrare, optimizarea bateriei, suspendarea automată a aplicației și ucigașii de sarcini ai producătorului pot conta cu toții. Instrumentul de fiabilitate din aplicație poate identifica riscurile de configurare și direcționa utilizatorii către setări; nu poate ignora politica sistemului.

După instalare, testați cu ecranul blocat și telefonul în același mod de alimentare folosit peste noapte. Repetați acel test după o actualizare a sistemului, o schimbare a economizorului de baterie sau o reinstalare a aplicației. Păstrați dispozitivul încărcat, volumul adecvat și misiunea aleasă disponibilă fizic. Urmați [depanarea livrării alarmei](../help/alarm-delivery.md) când un test eșuează.

## Ce nu promit confidențialitatea și fiabilitatea

BarcodeWake nu este un dispozitiv medical, serviciu de alertă de urgență sau tracker de fază a somnului. Nicio aplicație de alarmă nu poate garanta trezirea sau compensa un dispozitiv indisponibil. Pagina [fapte și limite](../facts.md) enumeră aceste granițe, în timp ce [disponibilitatea](../availability.md) separă dovezile din magazinul public de capabilitățile sursei mai noi.

