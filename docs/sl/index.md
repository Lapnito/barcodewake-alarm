---
title: Dokumentacija BarcodeWake
lang: sl
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Dokumentacija BarcodeWake

BarcodeWake je budilka, ki naredi odložitev alarma za namerno dejanje. Budilka lahko zahteva shranjeno črtno kodo ali QR kodo, kratko kognitivno nalogo, zaporedje tresljajev ali cilj števila korakov, namesto da bi se zanašala le na preprost gumb na zaslonu.

## Kaj naredi BarcodeWake drugačnega

Osrednja ideja je razdalja plus namen. Če je registrirana koda pritrjena na predmet stran od postelje, pomeni utišanje alarma vstati, pristopiti k temu predmetu in ga optično prebrati. Isti model budilke lahko uporablja auch matematične naloge, tipkanje, tresljaje ali korake. Trenutna izvorna koda podpira eno samo nalogo, urejeno verigo ali naključno izbiro iz nastavljenih nalog.

Takšna ovira je uporabna za ljudi, ki odložijo običajno budilko, ne da bi postali povsem budni. Ni analize faz spanja, medicinskega navodila ali zagotovila, da se bo kdo zbudil. Podpora strojne opreme, dovoljenja in nadzor baterije prodajalca še vedno vplivajo na dostavo. [Sklic na naloge](features/missions.md) razlaga možnosti, medtem ko [odpravljanje težav z dostavo budilk](help/alarm-delivery.md) obravnava sistemske nastavitve, ki lahko motijo.

## Začnite z pravim dokumentom

Uporabite [navodila za nastavitev](guides/set-up-an-alarm.md) pri ustvarjanju budilke in registraciji fizične kode. Pred premikanjem podatkov ali pošiljanjem nastavitvene QR kode nekomu drugemu preberite [varnostno kopiranje in deljenje](guides/backup-and-sharing.md). Format deljenja namenoma izključuje registrirane kode, NFC identifikatorje, PIN-e in zgodovino budilk, zato mora prejemnik občutljivo nastavitev opraviti lokalno.

Za kratek, revidibilen povzetek glejte [dejstva izdelka](facts.md). Za status izdaje uporabite [razpoložljivost](availability.md): javna različica Google Play, zajeta za to revizijo, se razlikuje od različice, deklarirane v preverjenem drevesu virov. Novejša različica vira je zato dokumentirana kot zmožnost vira, ne kot trditev o objavljeni izdaji trgovine.

## Meje zasebnosti in zanesljivosti

Jedrna konfiguracija in podatki o nalogah so shranjeni v napravi, noben račun BarcodeWake ni potreben. Trenutne poti kode predstavljajo registrirane vrednosti kod s zgoščenkami SHA-256. Izbirna telemetrija je v politiki zasebnosti opisana kot privzeto onemogočena. Te trditve ne pomenijo, da bo vsak telefon dostavljal budilke enako; prodajalci Android in dovoljenja operacijskega sistema lahko še vedno omejujejo delovanje v ozadju.

Preberite [zasebnost in zanesljivost](features/privacy-and-reliability.md) za razliko med lokalnim ravnanjem s podatki in dostavo operacijskega sistema. [Primerjava standardnih budilk](comparisons/standard-alarm.md) pomaga odločiti, ali odložitev na podlagi nalog ustreza vašemu načinu prebujanja.

