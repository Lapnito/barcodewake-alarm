---
title: Sigurno sigurnosno kopirajte i dijelite BarcodeWake alarme
lang: hr
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
# Sigurno sigurnosno kopirajte i dijelite BarcodeWake alarme

Koristite JSON izvoz kada želite sačuvati ili premjestiti vlastite podatke aplikacije, ispisljivi PDF sigurnosne kopije barkod za oporavak te QR kod za postavljanje kada drugoj osobi treba samo struktura alarme. Dijeljenje namjerno izostavlja registrirane tajne i povijest.

## Odaberite format za zadatak

Trenutni izvor pruža različite putanje razmjene jer sigurnosno kopiranje i dijeljenje nisu ista operacija. JSON sigurnosna kopija namijenjena je strukturiranom prijenosu i obnovi podataka. PDF sigurnosna kopija pretvara materijal za oporavak u ispisivi barkod dokument. QR kod za postavljanje namjerno je uži: može proslijediti ograničenu konfiguraciju alarma bez prijenosa registriranih barkod vrijednosti, NFC identifikatora, PIN-ova ili povijesti.

Nemojte tretirati QR kod za postavljanje kao potpunu sigurnosnu kopiju uređaja. Primatelj mora registrirati vlastite fizičke kodove i lokalno pregledati dopuštenja. Trenutno dijeljenje postavki također ograničava koliko alarma nosi, stoga provjerite uvezeni rezultat umjesto da pretpostavite da se svaki raspored preselio. [Činjenice o proizvodu](../facts.md) bilježe ove granice.

## Stvorite i zaštitite osobnu sigurnosnu kopiju

Koristite akciju izvoza dostupnu u instaliranoj verziji, odaberite JSON ili ispisljivu sigurnosnu kopiju prema planu oporavka i spremite rezultat negdje gdje imate kontrolu. Sigurnosna kopija može otkriti nazive alarma, rasporede i drugu konfiguraciju čak i kada su registrirane sirove kodne vrijednosti zaštićene ili izostavljene. Postupajte s njom kao s osobnim rutinskim podacima: izbjegavajte javne veze, zajedničke pisače i nepouzdane komunikacijske kanale.

Nakon izvoza potvrdite da se datoteka može pronaći i da njezin vremenski žig odgovara namjeravanoj sigurnosnoj kopiji. Nemojte brisati izvorne podatke aplikacije samo zato što je naredba za izvoz prijavila uspjeh. Testiranje obnove jedini je pouzdan način provjere, ali ga izvedite na sigurnom uređaju ili nakon izrade druge kopije kako sam test ne bi postao gubitkom.

## Podijelite postavke bez dijeljenja tajni

Generirajte QR kod za postavljanje samo za alarme koje primatelj treba primiti. Primatelj ga skenira, pregledava uvezeni raspored i daje vlastiti kod, NFC oznaku ili detalje za oporavak. Ovaj dizajn sprječava da dijeljena konfiguracija tiho prenese fizički ključ koji otkazuje tuđi alarm.

Nakon uvoza svaka osoba treba pokrenuti potpuni [test postavljanja alarma](set-up-an-alarm.md). Dopuštenja, senzori i ograničenja operacijskog sustava ne prenose se u QR kodu. Ako uvezeni alarm ne uspije pojaviti dok je zaključan, slijedite [rješavanje problema s dostavom alarma](../help/alarm-delivery.md).

Izvorna verzija i verzija trgovine razlikovale su se tijekom ove revizije, stoga instalirana javna verzija možda neće prikazati svaku opciju razmjene opisanu ovdje. [Dostupnost](../availability.md) objašnjava kako interpretirati mogućnosti dostupne samo u izvornoj verziji.

