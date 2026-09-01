---
title: BarcodeWake zasebnost in zanesljivost alarmov
lang: sl
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
# BarcodeWake zasebnost in zanesljivost alarmov

BarcodeWake hrani dokumentirano konfiguracijo alarmov in podatke o misijah v napravi ter ne zahteva računa aplikacije. Trenutne poti kode izračunavajo zgoščenke registriranih vrednosti kod. Izbirna telemetrija je opisana kot privzeto onemogočena, medtem ko dostava alarmov še vedno temelji na sistemskih dovoljenjih in nadzoru proizvajalca.

## Lokalni podatki ne odpravljajo odvisnosti od sistema

Lokalno shranjevanje pomeni, da običajna nastavitev alarma ne zahteva računa BarcodeWake v oblaku. Zapisi alarmov, zgodovina in preference se obravnavajo prek lokalne podatkovne plasti aplikacije. Registrirane vrednosti črtne kode, QR in NFC so predstavljene z zgoščenke SHA-256 v trenutnih poti shranjevanja in uvoza, kar se izogne ohranjanju običajne surove vrednosti za ujemanje.

Razprševanje ni enako šifriranju vsakega zapisa aplikacije, lokalno shranjevanje pa ni varnostna kopija. Nekdo z dostopom do odklenjene naprave lahko še vedno vidi imena alarmov, urnike ali zgodovino prek aplikacije. Izgubljen ali ponastavljen telefon lahko prav tako izgubi lokalne podatke, razen če je uporabnik izvozil varnostno kopijo. Glejte [varnostno kopiranje in souporabo](../guides/backup-and-sharing.md) za formate in njihove različne namene.

Pravilnik o zasebnosti navaja, da je izbirna telemetrija privzeto izklopljena in opisuje ravnanje z združenimi podatki, če je omogočena. Ta dokumentacija zato ne podaja širše trditve, da aplikacija nikoli ne more komunicirati prek omrežja. Navaja ožja preverljiva dejstva: jedro delovanja in podatki so lokalni, račun izdelka ni potreben in v preverjenem projektu se ne pojavi odvisnost oglaševalskega SDK-ja.

## Zanesljivost je skupna odgovornost

BarcodeWake lahko načrtuje in prikaže alarm, vendar operacijski sistem odloča, kdaj lahko delajo opravila v ozadju in katere prekinitve so dovoljene. Dovoljenje za obvestila, natančen dostop do alarmov, tihi ali fokus načini, optimizacija baterije, samodejna suspenzija aplikacije in orodja za končevanje opravil proizvajalca lahko vsi vplivajo. Orodje za zanesljivost v aplikaciji lahko prepozna tveganja konfiguracije in usmeri uporabnike k nastavitvam; ne more prezreti sistemske politike.

Po namestitvi testirajte s zaklenjenim zaslonom in telefonom v istem načinu napajanja, ki se uporablja čez noč. Ponovite ta test po posodobitvi sistema, spremembi varčevalnika baterije ali ponovni namestitvi aplikacije. Napravo imejte napolnjeno, glasnost primerno in izbrano misijo fizično dostopno. Sledite [odpravljanju težav z dostavo alarmov](../help/alarm-delivery.md), če test ne uspe.

## Kaj zasebnost in zanesljivost ne zagotavljata

BarcodeWake ni medicinski pripomoček, storitev za nujne primere ali sledilnik stopenj spanja. Nobena aplikacija za alarme ne more zagarantirati zbujanja ali nadomestiti nedostopne naprave. Stran [dejstva in omejitve](../facts.md) navaja te meje, medtem ko [razpoložljivost](../availability.md) ločuje dokaze iz javnih trgovin od zmogljivosti novejše kode.

