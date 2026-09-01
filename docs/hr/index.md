---
title: BarcodeWake dokumentacija
lang: hr
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake dokumentacija

BarcodeWake je budilica koja onemogućuje slučajno isključivanje. Alarm može zahtijevati spremljeni barkod ili QR kod, kratki kognitivni zadatak, sekvencu trese ili cilj koraka umjesto oslanjanja samo na jednostavan gumb na zaslonu.

## Što čini BarcodeWake drugačijim

Središnja ideja je kombinacija udaljenosti i namjere. Ako je registrirani kod pričvršćen na objekt udaljen od kreveta, isključivanje alarma znači ustati, dohvatiti taj objekt i skenirati ga. Isti model alarma može također koristiti matematiku, tipkanje, tresenje ili korake kao zadatke. Trenutni izvorni kod podržava jedan zadatak, uređeni lanac ili nasumični odabir iz konfiguriranih zadataka.

Taj napor je koristan za ljude koji isključe obični alarm bez potpunog buđenja. To nije analiza faza sna, medicinski savjet niti jamstvo da će netko probuditi. Podrška hardvera, dopuštenja i kontrole baterije dobavljača i dalje utječu na isporuku. [Referenca za zadatke](features/missions.md) objašnjava izbore, dok [rješavanje problema s isporukom alarma](help/alarm-delivery.md) pokriva postavke sustava koje mogu ometati.

## Počnite s pravim dokumentom

Koristite [vodič za postavljanje](guides/set-up-an-alarm.md) prilikom stvaranja alarma i registracije fizičkog koda. Pročitajte [sigurnosnu kopiju i dijeljenje](guides/backup-and-sharing.md) prije premještanja podataka ili slanja QR koda za postavljanje nekome drugom. Format dijeljenja namjerno isključuje registrirane kodove, NFC identifikatore, PIN-ove i povijest alarma, tako da primatelj mora lokalno dovršiti osjetljivo postavljanje.

Za kratak sažetak koji se može provjeriti, pogledajte [činjenice o proizvodu](facts.md). Za status izdanja, koristite [dostupnost](availability.md): javna verzija s Google Playa uhvaćena za ovu reviziju razlikuje se od verzije deklarirane u provjerenom izvorničkom stablu. Nova verzija izvornog koda stoga je dokumentirana kao mogućnost izvora, a ne kao objavljeno izdanje u trgovini.

## Granice privatnosti i pouzdanosti

Osnovna konfiguracija i podaci o zadacima pohranjuju se na uređaju i nijedan BarcodeWake račun nije potreban. Trenutne putanje koda predstavljaju vrijednosti registriranih kodova s SHA-256 raspršivanjem. Neobavezna telemetrija opisana je politikom privatnosti kao onemogućena prema zadanim postavkama. Te izjave ne znače da će svaki telefon isporučivati alarme identično; Android dobavljači i dopuštenja operacijskog sustava i dalje mogu ograničiti ponašanje u pozadini.

Pročitajte [privatnost i pouzdanost](features/privacy-and-reliability.md) za razliku između lokalnog rukovanja podacima i isporuke operacijskog sustava. [Usporedba standardnih alarma](comparisons/standard-alarm.md) pomaže odlučiti odgovara li onemogućavanje temeljeno na zadacima načinu na koji se budite.

