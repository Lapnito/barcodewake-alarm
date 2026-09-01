---
title: Zakaj se alarm BarcodeWake morda ne oglasi
lang: sl
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---
# Zakaj se alarm BarcodeWake morda ne oglasi

Shranjeni alarm lahko še vedno blokirajo nastavitve obvestil, dostop do natančnega alarma, načini osredotočenosti ali tihega načina, nizka glasnost, omejitve baterije, suspendiranje aplikacije ali nadzor ozadja ponudnika. Preverite dostavo ločeno od skeniranja misije, nato izvedite test z zaklenjenim zaslonom.

## Najprej ločite dostavo od zavrnitve

Ustvarite kratkoročen testni alarm preproste misije in pustite aplikacijo v ozadju. Zaklenite zaslon. Če se ne prikaže noben alarm zaslona ali zvok, je težava v dostavi; sprememba registrirane črtne kode ne bo pomagala. Če se alarm prikaže, vendar misija ne more biti dokončana, dostava deluje, težava pa je v kameri, senzorju, ujemanju kode ali konfiguraciji misije.

## Preglejte dovoljenja operacijskega sistema

Dovolite obvestila in kakršen koli dostop do natančnega alarma ali celozaslonskega alarma, ki ga zahteva nameščena različica. Odstranite BarcodeWake iz agresivne optimizacije baterije ali samodejnih seznamov spanja, če naprava ponuja te nadzore. Odprite diagnostiko zanesljivosti v aplikaciji in sledite nastavitvam, ki jih določi za posamezno napravo. Stran [zasebnost in zanesljivost](../features/privacy-and-reliability.md) razlaga, zakaj te sistemske odvisnosti ostajajo, četudi so podatki aplikacije lokalni.

## Diagnosticirajte izpolnitev misije ločeno

Za črtne kode in QR misije očistite lečo kamere, izboljšajte osvetljenost in potrdite, da registrirani predmet ni spremenjen. Podelite dovoljenje za kamero. Pri NFC preverite podporo naprave in držite oznako blizu pravilne antenske pozicije. Misije tresenja in korakov so odvisne od gibalnih ali korakovnih senzorjev in se lahko obnašajo drugače, ko načini varčevanja z energijo omejujejo dostavo senzorjev.

Če je bila misija konfigurirana kot del verige, mora biti vsak zahtevan korak dokončan. Preglejte [obnašanje misije](../features/missions.md) in, če je potrebno, ustvarite nov test z uporabo [postopka nastavitve](../guides/set-up-an-alarm.md).

## Vedite, kdaj je telefon meja

BarcodeWake ne more preglasiti izklopljene naprave, izpraznjene baterije, okvarjene strojne opreme za zvok ali katerega koli proizvajalčevega opravila za ubijanje procesov. Ni storitev za nujna obvestila. Ohranite drugo metodo alarma za situacije z visokimi posledicami in poročajte o ponovljivih napakah z modelom naprave, različico sistema, različico aplikacije in natančnimi pogoji testa.

