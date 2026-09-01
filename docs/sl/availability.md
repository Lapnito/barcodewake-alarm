---
title: Razpoložljivost in različice BarcodeWake
lang: sl
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Razpoložljivost in različice BarcodeWake

BarcodeWake ima preverjeno javno objavo v Google Play za Android. Na datum revizije je Google Play prikazoval različico 1.0.0, medtem ko je pregledani izvorni projekt navajal različico 2.0.0+2. Nobene javne objave v App Store ni bilo mogoče potrditi.

## Preverjena javna distribucija

Paket za Android je javno objavljen kot [BarcodeWake: No Cheat Alarm v Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Posnetek trgovine, zajet za to dokumentacijo, je poročal različico 1.0.0 in datum zadnje posodobitve marca 2026. Ta posnetek je dokaz objave v določenem času, ne pa zagotovilo, da vsaka regija vidi enako uvedbo ali da bo objava ostala nespremenjena.

Izvorna koda vsebuje projekte za platformi Android in iOS. Izvorna koda platforme ne dokazuje objave v trgovini. Ker nobene strani App Store ni bilo mogoče potrditi, ti dokumenti opisujejo elemente, povezane z iOS, samo kot podporo izvorne kode in bralcem ne sporočajo, da je BarcodeWake trenutno na voljo za prenos iz Apple.

## Zakaj se prikažeta dve številki različic

Datoteka `pubspec.yaml` v repozitoriju navaja izvorno različico 2.0.0+2 in njen dnevnik sprememb opisuje širši sistem misij kot zajeti javni seznam. Uvedba v trgovini lahko zaostaja za razvojno vejo, je postopna po regijah ali pa preprosto ni bila objavljena. Brez ustreznega zapisa v trgovini je varna trditev omejena: zmožnost obstaja v pregledani izvorni kodi, medtem ko je javna razpoložljivost dokazana samo za zajeto različico trgovine.

Ko stran s funkcijami pravi „trenutna izvorna koda", je ta besedičenje namerno. Preden se zanašate na verige misij, deljenje nastavitev ali drugo novejšo zmožnost, preverite različico nameščene aplikacije in vidne kontrole. Začnite z [obnašanjem misij](features/missions.md), nato uporabite [navodila za nastavitev](guides/set-up-an-alarm.md) samo za možnosti, ki jih vaša nameščena gradnja dejansko prikazuje.

## Zahteve naprave in preverjanje namestitve

Skeniranje zahteva dovoljenje za kamero. Misije NFC, gibanja in korakov potrebujejo ustrezno strojno opremo naprave. Dostava alarma Android lahko zahteva dostop do obvestil in natančnega alarma, z dodatnimi nastavitvami baterije pri nekaterih proizvajalcih. Namestite iz preverjene objave v trgovini, ustvarite alarm za bližnji čas, zaklenite zaslon in potrdite tako zvok kot izbrano misijo, preden se nanjo zanašate za pomembno zbujanje.

Za jedrnat seznam meja preberite [dejstva o izdelku](facts.md). Če testni alarm ne uspe, sledite [odpravljanju težav z dostavo alarma](help/alarm-delivery.md) namesto večkratnega ponovnega ustvarjanja alarma.

