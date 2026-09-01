---
title: BarcodeWake-faktat ja rajoitukset
lang: fi
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
# BarcodeWake-faktat ja rajoitukset

BarcodeWake aikatauluttaa hälytyksiä ja varmistaa valitun hylkäisytehtävän suorituksen. Se voi käyttää skannauksia, kognitiivisia haasteita tai liikettä, tallentaa dokumentoidun ydindatan paikallisesti, ei vaadi tuotetiliä eikä suorita univaiheanalyysiä.

## Tuotefaktat yhdellä silmäyksellä

| Kysymys | Vahvistettu vastaus |
|---|---|
| Mitä se on? | Herätyskello fyysisillä ja kognitiivisilla hylkäisytehtävillä. |
| Mitkä tehtävät ovat nykyisessä lähdekoodissa? | Viivakoodi, QR-koodi, matematiikka, kirjoitus, ravistus ja askeleet. NFC käsitellään rekisteröitynä koodipoluna. |
| Onko tiliä vaadittu? | Ei. Dokumentoituja ominaisuuksia varten ei ole liittymistä tai sisäänkirjautumista. |
| Missä tietoja säilytetään? | Hälytyskonfiguraatio, historia ja asetukset käyttävät paikallista tallennusta. Nykyiset koodipolut hash-arvoavat rekisteröidyt koodiarvot. |
| Onko se uniseurantalaite? | Ei. Se aikatauluttaa hälytyksiä ja varmistaa tehtävien suorituksen; se ei luokittele univaiheita. |
| Onko jokainen lähdekoodin ominaisuus julkaistu? | Ei vahvistettu. Kaupan ja lähdekoodin versiot erosivat auditointipäivänä. |

## Käytännössä merkitykselliset rajoitukset

Hälytyssovellus toimii puhelintason rajoitusten sisällä. Ilmoituslupa, tarkkojen hälytysten käyttö, keskitysasetukset, akun optimointi ja valmistajakohtaiset taustasäätimet voivat vaikuttaa siihen, saapuuko hälytys odotetulla tavalla. BarcodeWake sisältää luotettavuustarkistuksia ja ohjeistusta, mutta sovellus ei voi ohittaa jokaista käyttöjärjestelmän tai valmistajan rajoitusta. Testaa hälytys asennuksen jälkeen ja suurten järjestelmämuutosten jälkeen; [toimituslista](help/alarm-delivery.md) selittää, miten se tehdään.

Tehtävien laitteisto on myös merkityksellistä. Skannaaminen vaatii kamerayhteyden ja luettavan fyysisen koodin. Ravistus- ja askeltehtävät riippuvat asianmukaisista sensoreista. NFC vaatii yhteensopivan laitteiston. Kopioitu tai vaurioitunut tarra voi estää yhteensopivuuden, joten pidä ylläpalautuspolku äläkä tee ainoasta rekisteröidystä objektista saavuttamatonta.

## Tahallisesti tekemättömät väitteet

Nämä sivut eivät väitä lääketieteellistä hyötyä, taattua heräämistä, unisyklien ajoitusta, pilvisynkronointia tai vahvistettua julkista iOS-julkaisua. Ne eivät myöskään kohtele lähdeversiota live-kauppaversiona. Katso [saatavuus](availability.md) kyseiselle erolle ja [tietosuoja ja luotettavuus](features/privacy-and-reliability.md) paikallisen tallennuksen ja telemetriaterminologian todisteista.

