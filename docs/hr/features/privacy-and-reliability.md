---
title: BarcodeWake privatnost i pouzdanost alarma
lang: hr
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
# BarcodeWake privatnost i pouzdanost alarma

BarcodeWake čuva dokumentiranu konfiguraciju alarma i podatke o misiji na uređaju i ne zahtijeva račun aplikacije. Trenutni putovi koda raspršuju registrirane vrijednosti kodova. Telemetrija koja je opcionalna opisana je kao isključena prema zadanim postavkama, dok dostava alarma još uvijek ovisi o sustavskim dopuštenjima i kontrolama proizvođača.

## Lokalni podaci ne uklanjaju ovisnosti o sustavu

Lokalna pohrana znači da obično postavljanje alarma ne zahtijeva BarcodeWake račun u oblaku. Zapisi alarma, povijest i preferencije obrađuju se putem lokalnog sloja podataka aplikacije. Registrirane vrijednosti barkoda, QR i NFC prikazane su SHA-256 raspršenicama u trenutnoj pohrani i putevima uvoza, čime se izbjegava zadržavanje obične sirove vrijednosti za podudaranje.

Raspršivanje (hashing) nije isto što i šifriranje svakog zapisa aplikacije, a lokalna pohrana nije sigurnosna kopija. Netko tko ima pristup otključanom uređaju i dalje može vidjeti nazive alarma, rasporede ili povijest kroz aplikaciju. Izgubljen ili resetiran telefon također može izgubiti lokalne podatke ako korisnik nije napravio izvoz. Pogledajte [sigurnosno kopiranje i dijeljenje](../guides/backup-and-sharing.md) za formate i njihove različite namjene.

Pravila o privatnosti navode da je opcionalna telemetrija prema zadanim postavkama isključena i opisuju agregatno rukovanje ako je omogućena. Stoga ova dokumentacija ne tvrdi širu tvrdnju da aplikacija nikada ne može komunicirati preko mreže. Navodi uže provjerene činjenice: osnovno djelovanje i podaci su lokalni, nije potreban račun proizvoda i u provjerenom projektu ne postoji ovisnost o SDK-u za oglašavanje.

## Pouzdanost je zajednička odgovornost

BarcodeWake može zakazati i prikazati alarm, ali operativni sustav odlučuje kada pozadinski rad smije raditi i koje prekide je dopušteno. Dopuštenje za obavijesti, pristup točnom alarmu, tihi ili fokus načini rada, optimizacija baterije, automatsko suspendiranje aplikacije i alati za ubijanje zadataka proizvođača mogu svi utjecati. Alat za pouzdanost unutar aplikacije može identificirati rizike konfiguracije i usmjeriti korisnike na postavke; ne može nadjačati sustavsku politiku.

Nakon instalacije, testirajte sa zaključanim zaslonom i telefonom u istom načinu rada napajanja koji se koristi preko noći. Ponovite taj test nakon ažuriranja sustava, promjene štednje baterije ili ponovne instalacije aplikacije. Držite uređaj napunjenim, glasnoću odgovarajućom i odabranu misiju fizički dostupnom. Slijedite [Rješavanje problema s dostavom alarma](../help/alarm-delivery.md) ako test ne uspije.

## Što privatnost i pouzdanost ne jamče

BarcodeWake nije medicinski uređaj, usluga hitnih upozorenja niti tracker faza sna. Nijedna aplikacija za alarm ne može jamčiti buđenje niti nadoknaditi nedostupnost uređaja. [Činjenice i ograničenja](../facts.md) navodi ta ograničenja, dok [Dostupnost](../availability.md) razdvaja dokaze iz javne trgovine od mogućnosti novijih izvora.

