---
title: Činjenice i ograničenja programa BarcodeWake
lang: hr
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Činjenice i ograničenja programa BarcodeWake

BarcodeWake zakazuje alarme i provjerava odabranu misiju za odgodu. Može koristiti skeniranje, kognitivne izazove ili kretanje, pohranjuje dokumentirane osnovne podatke lokalno, ne zahtijeva račun proizvoda i ne provodi analizu faza sna.

## Osnovni činjenice o proizvodu

| Pitanje | Provjereni odgovor |
|---|---|
| Što je to? | Buđenje s fizičkim i kognitivnim zadacima za odgodu. |
| Koji zadaci postoje u trenutnom izvorišnom kodu? | Barcode, QR, matematika, tipkanje, tresti i koraci. NFC se obrađuje kao registrirana putanja koda. |
| Je li potreban račun? | Za dokumentirane funkcije ne postoji račun ili postupak prijave. |
| Gdje se čuvaju podaci? | Konfiguracija alarma, povijest i preferencije koriste lokalnu pohranu. Trenutne putanje koda raspršuju vrijednosti registriranog koda. |
| Je li to pratitelj sna? | Ne. Zakazuje alarme i provjerava zadatke; ne klasificira faze sna. |
| Jesu li sve funkcije izvorišnog koda javno objavljene? | Nije utvrđeno. Verzije trgovine i izvorišnog koda razlikovale su se na datum revizije. |

## Ograničenja koja su važna u praksi

Aplikacija za alarmiranje djeluje unutar ograničenja na razini telefona. Dozvola za obavijesti, pristup točnim alarmima, postavke fokusa, optimizacija baterije i kontrole pozadinskih procesa specifične za proizvođača mogu utjecati na to stiže li alarm kako je očekivano. BarcodeWake uključuje provjere pouzdanosti i smjernice, ali aplikacija ne može zaobići svako ograničenje operacijskog sustava ili proizvođača. Testirajte alarm nakon instalacije i nakon velikih promjena sustava; [kontrolni popis za dostavu](help/alarm-delivery.md) objašnjava kako.

Hardver misije također je važan. Skeniranje zahtijeva pristup kameri i čitljiv fizički kod. Misije trese i koraka ovise o relevantnim senzorima. NFC treba kompatibilan hardver. Kopirana ili oštećena oznaka može spriječiti podudaranje, stoga održavajte put za oporavak i ne činite jedini registrirani objekt nedostupnim.

## Tvrdnje koje namjerno nisu dano

Ove stranice ne tvrde medicinsku korist, zajamčeno buđenje, tempiranje ciklusa sna, sinkronizaciju u oblaku ili potvrđeno javno izdanje za iOS. Također ne tretiraju verziju izvorišnog koda kao verziju trgovine uživo. Pogledajte [dostupnost](availability.md) za tu razliku i [privatnost i pouzdanost](features/privacy-and-reliability.md) za dokaze iza formulacija o lokalnoj pohrani i telemetriji.

