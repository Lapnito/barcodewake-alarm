---
title: BarcodeWaken tietosuoja ja hälytyksen luotettavuus
lang: fi
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
# BarcodeWaken tietosuoja ja hälytyksen luotettavuus

BarcodeWake säilyttää dokumentoidut hälytysasetukset ja tehtävä tiedot laitteella, eikä vaadi sovellustiliä. Nykyiset koodipolut hash-merkitsevät rekisteröidyt koodiarvot. Valinnainen telemetria on kuvattu oletuksena poistetuksi käytöstä, kun taas hälytysten toimittaminen riippuu edelleen järjestelmän käyttöoikeuksista ja valmistajan hallinnasta.

## Paikallinen data ei poista järjestelmäriippuvuuksia

Paikallinen tallennus tarkoittaa, että tavallinen hälytysasetus ei vaadi BarcodeWaken pilvitiliä. Hälytystietueet, historia ja asetukset käsitellään sovelluksen paikallisen datakerroksen kautta. Rekisteröidyt viivakoodi-, QR- ja NFC-arvot esitetään SHA-256 hash-arvoina nykyisissä tallennus- ja tuontireiteissä, mikä välttää tavallisen raak值 säilyttämisen yhteensovittamista varten.

Hash-merkintä ei ole sama kuin jokaisen sovellustietueen salaus, eikä paikallinen tallennus ole varmuuskopio. Joku, jolla on pääsy lukitsemattomaan laitteeseen, voi silti nähdä hälytysten nimet, aikataulut tai historian sovelluksen kautta. Kadonnut tai nollattu puhelin voi myös menettää paikalliset tiedot, ellei käyttäjä ole tehnyt vientiä. Katso [varmuuskopiointi ja jakaminen](../guides/backup-and-sharing.md) muotojen ja niiden eri tarkoitusten osalta.

Tietosuojakäytäntö sanoo, että valinnainen telemetria on oletuksena poissa käytöstä, ja se kuvaa koostettua käsittelyä, jos se on käytössä. Tämä dokumentaatio ei siksi esitä laajempaa väitettä, että sovellus ei koskaan voisi viestiä verkon kautta. Se esittää kapeammat vahvistetut faktat: ydintoiminta ja data ovat paikallisia, tuotetiliä ei vaadita, eikä mainonta-SDK-riippuvuutta näy tarkistetussa projektissa.

## Luotettavuus on yhteinen vastuu

BarcodeWake voi ajastaa ja esittää hälytyksen, mutta käyttöjärjestelmä päättää, milloin taustatyö saa suorittaa ja mitkä keskeytykset sallitaan. Ilmoitusoikeus, täsmällisen hälytyksen käyttö, hiljaiset tai keskitystilat, akun optimointi, automaattinen sovelluksen keskeytys ja valmistajan tehtävänhallinta voivat kaikki vaikuttaa. Sovelluksen sisäinen luotettavuustyökalu voi tunnistaa määritysriskit ja ohjata käyttäjiä asetuksiin; se ei voi ohittaa järjestelmäkäytäntöä.

Asennuksen jälkeen testaa näytön ollessa lukittuna ja puhelimen samassa virtatilassa, jota käytetään yön yli. Toista testi järjestelmäpäivityksen, akun säästötilan muutoksen tai sovelluksen uudelleenasennuksen jälkeen. Pidä laite ladattuna, äänenvoimakkuus sopivana ja valittu tehtävä fyysisesti saatavilla. Noudata [hälytyksen toimittamisen vianmääritystä](../help/alarm-delivery.md), kun testi epäonnistuu.

## Mitä tietosuoja ja luotettavuus eivät takaa

BarcodeWake ei ole lääkinnällinen laite, hätähälytyspalvelu tai univaiheiden seuranta. Mikään hälytyssovellus ei voi taata heräämistä tai korvata käytettävissä olevan laitteen puuttumista. [Faktat ja rajoitukset -sivu](../facts.md) luetellaan nämä rajat, kun taas [saatavuus](../availability.md) erottaa julkisen kaupan todisteet uudemman lähdekoodin ominaisuuksista.

