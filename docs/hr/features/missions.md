---
title: BarcodeWake misije i lanci misija
lang: hr
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# BarcodeWake misije i lanci misija

BarcodeWake misija je uvjet koji se koristi za odbacivanje alarma. Trenutni izvor podržava barkod, QR, matematičke zadatke, tipkanje, tresenje i korake, pri čemu se registrirani NFC obrađuje kroz putanju skeniranja koda. Misije se mogu izvoditi samostalno, u nizu ili nasumičnim odabirom.

## Misija skeniranja stvara fizičku udaljenost

Misija barkoda ili QR koda uspoređuje živo skeniranje kamerom s kodom registriranim tijekom postavljanja. Kod se može staviti na objekt izvan dosega ruke: kozmetika u kupaonici, namirnica za doručak u kuhinji ili drugi stabilan objekt na dobro osvijetljenom području. NFC prati istu opću ideju s kompatibilnom oznakom i uređajem. Aplikacija pohranjuje hash reprezentaciju u trenutnim putanjama umjesto da treba sirov kod za uobičajenu usporedbu.

Odaberite objekt koji će još uvijek biti dostupan kada se alarm oglasi. Pakovanja se bacaju, oznake blijede, a putovanja mijenjaju okruženje. Registracija koda na jedinoj kutiji lijekova koju možda trebate zamijeniti manje je robusna od korištenja trajne oznake. [Vodič za postavljanje alarma](../guides/set-up-an-alarm.md) pokriva postavljanje i testiranje.

## Misija izazova razmjenjuje kretanje za napor

Matematika i tipkanje zahtijevaju usredotočen unos. Tresenje i koraci zahtijevaju fizičko kretanje i podržane senzore. Postavke težine i cilja mijenjaju koliko se rada očekuje, ali teža misija nije automatski i bolja. Preveliko trenje može poticati potpuno isključivanje alarma, dok laki zadatak može postati automatski nakon ponavljanja.

Prilagodite zadatak načinu kvara. Ako isključujete alarme polusanjivo, skeniranje u drugoj sobi stvara korisnu udaljenost. Ako je pristup kameri nezgodan, kratki zadatak tipkanja ili matematike može biti praktičniji. Ako su mobilnost, ravnoteža ili pristupačnost problem, izbjegavajte misije temeljene na kretanju i odaberite zadatak koji se može sigurno izvršiti.

## Pojedinačni, lanac i nasumični načini rada

Pojedinačni način traži jednu konfiguriranu misiju. Način rada lanca pokreće nekoliko konfiguriranih misija redom. Nasumični način bira iz konfiguriranog skupa, smanjujući vjerojatnost da jedna memorirana interakcija postane automatska. Ovi načini postoje u novijem provjerenom izvorištu; [dostupnost](../availability.md) objašnjava zašto to ne dokazuje da su već u svakoj javnoj verziji.

Uvijek pokrenite kratkoročni test nakon promjene načina, dozvola ili registriranih objekata. Držite odabrani objekt dostupnim i osigurajte sigurnu rutu oporavka. Za probleme s isporukom koji nisu povezani s dovršetkom misije, koristite [kontrolni popis pouzdanosti](../help/alarm-delivery.md).

