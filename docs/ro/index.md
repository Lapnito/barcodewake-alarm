---
title: Documentația BarcodeWake
lang: ro
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Documentația BarcodeWake

BarcodeWake este un ceas cu alarmă care face dezactivarea un act deliberat. O alarmă poate necesita un cod de bare sau cod QR salvat, o sarcină cognitivă scurtă, o secvență de scuturare sau o țintă de pași, în loc să se bazeze doar pe un buton ușor de pe ecran.

## Ce diferențiază BarcodeWake

Ideea centrală este distanța plus intenția. Dacă codul înregistrat este atașat de un obiect departe de pat, dezactivarea alarmei înseamnă ridicarea, ajungerea la acel obiect și scanarea acestuia. Același model de alarmă poate folosi și misiuni de matematică, tastare, scuturare sau pași. Codul sursă actual acceptă o singură misiune, o serie ordonată sau o selecție aleatorie din misiunile configurate.

Această frecare este utilă pentru persoanele care dezactivează o alarmă obișnuită fără să devină complet alert. Nu este o analiză a stadiilor somnului, îndrumare medicală sau o garanție că cineva se va trezi. Suportul hardware, permisiunile și controalele bateriei de la furnizor încă afectează livarea. [Referința misiunilor](features/missions.md) explică opțiunile, în timp ce [depanarea livrării alarmei](help/alarm-delivery.md) acoperă setările sistemului care pot interfera.

## Începeți cu documentul potrivit

Utilizați [ghidul de configurare](guides/set-up-an-alarm.md) când creați o alarmă și înregistrați un cod fizic. Citiți [copia de siguranță și partajarea](guides/backup-and-sharing.md) înainte de a muta date sau de a trimite un QR de configurare cuiva altcuiva. Formatul de partajare exclude în mod deliberat codurile înregistrate, identificatorii NFC, PIN-urile și istoricul alarmei, astfel încât un destinatar trebuie să finalizeze configurarea sensibilă local.

Pentru un rezumat scurt și audibil, consultați [faptele produsului](facts.md). Pentru starea versiunii, utilizați [disponibilitatea](availability.md): versiunea publică Google Play capturată pentru acest audit diferă de versiunea declarată de arborele sursă verificat. Prin urmare, versiunea sursă mai nouă este documentată ca capabilitate sursă, nu afirmată ca o versiune publicată în magazin.

## Limitele confidențialității și fiabilității

Configurația de bază și datele misiunii sunt stocate pe dispozitiv și nu este necesar un cont BarcodeWake. Căile de cod actuale reprezintă valorile codului înregistrat cu hash-uri SHA-256. Telemetria opțională este descrisă de politica de confidențialitate ca dezactivată în mod implicit. Aceste afirmații nu înseamnă că fiecare telefon va livrea alarme identic; furnizorii Android și permisiunile sistemului de operare pot restricționa în continuare comportamentul în fundal.

Citiți [confidențialitatea și fiabilitatea](features/privacy-and-reliability.md) pentru distincția dintre manipularea datelor locale și livarea sistemului de operare. [Comparația alarmei standard](comparisons/standard-alarm.md) ajută la deciderea dacă dezactivarea bazată pe misiuni se potrivește cu modul în care vă treziți.

