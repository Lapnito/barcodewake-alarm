---
title: Confidențialitatea și fiabilitatea alarmelor BarcodeWake
lang: or
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
# Confidențialitatea și fiabilitatea alarmelor BarcodeWake

BarcodeWake păstrează configurația documentată a alarmei și datele misiunii pe dispozitiv și nu necesită un cont de aplicație. Căile curente ale codului folosesc funcții de hash pentru valorile codurilor înregistrate. Telemetria opțională este descrisă ca fiind dezactivată în mod implicit, în timp ce livrarea alarmei depinde în continuare de permisiunile sistemului și de controalele furnizorului.

## Datele locale nu elimină dependențele de sistem

Stocarea locală înseamnă că configurarea obișnuită a alarmei nu necesită un cont cloud BarcodeWake. Înregistrările alarmei, istoricul și preferințele sunt gestionate prin stratul de date local al aplicației. Valorile înregistrate ale codurilor de bare, QR și NFC sunt reprezentate cu hash-uri SHA-256 în stocarea curentă și în căile de import, ceea ce evită păstrarea valorii brute obișnuite pentru potrivire.

Hashing-ul nu este același lucru cu criptarea fiecărei înregistrări a aplicației, iar stocarea locală nu este o copie de siguranță. Cineva cu acces la un dispozitiv deblocat poate vedea în continuare numele alarmelor, programările sau istoricul prin aplicație. Un telefon pierdut sau resetat poate, de asemenea, să piardă datele locale, cu excepția cazului în care utilizatorul a făcut o exportare. Consultați [copie de siguranță și partajare](../guides/backup-and-sharing.md) pentru formatele și scopurile lor diferite.

Politica de confidențialitate spune că telemetria opțională este dezactivată în mod implicit și descrie gestionarea agregată dacă este activată. Prin urmare, această documentație nu face afirmația mai largă că aplicația nu poate comunica niciodată într-o rețea. Aceasta afirmă faptele verificate mai înguste: funcționarea de bază și datele sunt locale, nu este necesar niciun cont de produs și nu apare nicio dependență de SDK de publicitate în proiectul verificat.

## Fiabilitatea este o responsabilitate partajată

BarcodeWake poate programa și prezenta o alarmă, dar sistemul de operare decide când poate rula munca în fundal și ce întreruperi sunt permise. Permisiunea de notificare, accesul la alarme exacte, modurile silențioase sau de concentrare, optimizarea bateriei, suspendarea automată a aplicației și instrumentele de ucidere a sarcinilor ale producătorului pot conta toate. Instrumentul de fiabilitate din aplicație poate identifica riscurile de configurare și direcționa utilizatorii către setări; nu poate ignora politica sistemului.

După instalare, testați cu ecranul blocat și telefonul în același mod de alimentare folosit peste noapte. Repetați acest test după o actualizare de sistem, o modificare a economizorului de baterie sau o reinstalare a aplicației. Mențineți dispozitivul încărcat, volumul adecvat și misiunea aleasă fizic disponibilă. Urmați [depanarea livrării alarmelor](../help/alarm-delivery.md) când un test eșuează.

## Ce nu promit confidențialitatea și fiabilitatea

BarcodeWake nu este un dispozitiv medical, serviciu de alertă de urgență sau urmăritor de stagii de somn. Nicio aplicație de alarmă nu poate garanta trezirea sau compensa un dispozitiv indisponibil. Pagina [fapte și limite](../facts.md) enumeră aceste limite, în timp ce [disponibilitatea](../availability.md) separă dovezile din magazinele publice de capabilitățile sursei mai noi.

