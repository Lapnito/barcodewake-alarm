---
title: Varno varnostno kopirajte in delite alarme BarcodeWake
lang: sl
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Varno varnostno kopirajte in delite alarme BarcodeWake

Uporabite izvoz JSON, ko želite ohraniti ali premakniti lastne podatke aplikacije, tiskalno varnostno kopijo PDF črtne kode za obnovitev, ter QR kodo za nastavitev, ko druga oseba potrebuje samo strukturo alarma. Deljenje namenoma izpusti registrirane skrivnosti in zgodovino.

## Izberite format za delo

Trenutni vir ponuja različne poti izmenjave, ker varnostno kopiranje in deljenje nista enaki operaciji. Varnostna kopija JSON je namenjena strukturiranemu prenosu podatkov in obnovitvi. Varnostna kopija PDF pretvori material za obnovitev v tiskalni dokument črtne kode. Nastavitvena QR koda je namenoma ožja: lahko posreduje omejeno konfiguracijo alarma, ne da bi nosila registrirane vrednosti črtne kode, identifikatorje NFC, PIN kode ali zgodovino.

Ne obravnavajte nastavitvene QR kode kot popolne varnostne kopije naprave. Prejemnik mora registrirati svoje fizične kode in lokalno pregledati dovoljenja. Trenutno deljenje nastavitev prav tako omejuje, koliko alarmov vsebuje, zato preverite uvoženi rezultat in ne predpostavljajte, da se je vsak urnik premaknil. [Dejstva o izdelku](../facts.md) beležijo te meje.

## Ustvarite in zaščitite osebno varnostno kopijo

Uporabite dejanje izvoza, ki je na voljo v nameščeni različici, izberite JSON ali tiskalno varnostno kopijo glede na načrt obnovitve in rezultat shranite nekje, kjer imate nadzor. Varnostna kopija lahko razkrije imena alarmov, urnike in drugo konfiguracijo, anche ko so registrirane surove vrednosti kode zaščitene ali izpuščene. Ravnajte z njo kot z osebnimi rutinskimi podatki: izogibajte se javnim povezavam, souporabi tiskalnikov in nezaupljivim komunikacijskim kanalom.

Po izvozu potrdite, da je datoteka mogoče najti in da njena časovna oznaka ustreza nameravani varnostni kopiji. Ne izbrišite izvirnih podatkov aplikacije samo zato, ker je ukaz za izvoz poročal o uspehu. Testiranje obnovitve je edini zanesljiv pregled, vendar ga izvedite na varni napravi ali po izdelavi druge kopije, da sam test ne postane dogodek izgube.

## Delite nastavitev brez deljenja skrivnosti

Ustvarite nastavitveno QR kodo samo za alarme, ki naj bi jih prejemnik prejel. Prejemnik jo skenira, pregleda uvoženi urnik in navede svojo kodo, oznako NFC ali podrobnosti za obnovitev. Ta zasnova preprečuje, da bi deljena konfiguracija tiho prenesla fizični ključ, ki odpravi tuji alarm.

Po uvozu bi moral vsakdo izvesti celoten [test nastavitve alarma](set-up-an-alarm.md). Dovoljenja, senzorji in omejitve operacijskega sistema se ne prenesejo v QR kodi. Če uvoženi alarm ne pride, medtem ko je zaklenjen, sledite [odpravljanju težav z dostavo alarma](../help/alarm-delivery.md).

Vir in shranjene različice so se med to revizijo razlikovale, zato nameščena javna različica morda ne razkriva vsake tukaj opisane možnosti izmenjave. [Razpoložljivost](../availability.md) razlaga, kako razlagati zmogljivosti, ki so na voljo samo v viru.

