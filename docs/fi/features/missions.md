---
title: BarcodeWake-tehtävät ja tehtäväketjut
lang: fi
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
# BarcodeWake-tehtävät ja tehtäväketjut

BarcodeWake-tehtävä on ehto, jota käytetään herätyksen lopettamiseen. Nykyinen lähde tukee viivakoodi-, QR-koodi-, matematiikka-, kirjoitus-, ravistus- ja askelutehtäviä, ja rekisteröity NFC käsitellään koodinlukutien kautta. Tehtäviä voi suorittaa yksin, peräkkäin tai satunnaisessa järjestyksessä.

## Skannaustehtävät luovat fyysistä etäisyyttä

Viivakoodi- tai QR-kooditehtävä vertaa suoraa kameraskannausta asennuksen aikana rekisteröityyn koodiin. Koodin voi sijoittaa esineeseen käsivarren ulottumattomiin: kylpyhuoneen hygieniatarvikkeisiin, keittiön aamupalakohtaan tai toiseen vakaaseen esineeseen hyvin valaistussa tilassa. NFC noudattaa samaa yleiskonseptia yhteensopivalla tarralla ja laitteella. Sovellus tallentaa hajautusesityksen nykyisiin polkuihin tavallisen vertailun sijaan ilman että raakakoodia tarvitaan.

Valitse esine, joka on edelleen saatavilla kun herätys soi. Pakkaukset heitetään pois, tarrat haalistuvat ja matkustaminen muuttaa ympäristöä. Koodin rekisteröinti ainoaan lääkelaatikkoon, jonka saatat joutua vaihtamaan, on vähemmän vankkaa kuin kestävän tarran käyttäminen. [Herätyksen asetusten oppaassa](../guides/set-up-an-alarm.md) käsitellään sijoittelua ja testaamista.

## Haastetehtävät vaihtavat liikettä työn muotoon

Matematiikka ja kirjoittaminen vaativat keskittynyttä syöttöä. Ravistus ja askeleet vaativat fyysistä liikettä ja tuettuja antureita. Vaikeus- ja tavoiteasetukset muuttavat sitä, kuinka paljon työtä odotetaan, mutta vaikeampi tehtävä ei automaattisesti ole parempi. Liiallinen kitka voi kannustaa herätyksen poiskytkemiseen kokonaan, kun taas helppo tehtävä voi muuttua automaattiseksi toiston jälkeen.

Yhdistä tehtävä epäonnistumistilaan. Jos sammutat herätykset puoliunessa, skannaaminen toisessa huoneessa luo hyödyllistä etäisyyttä. Jos kameran käyttö on hankalaa, lyhyt kirjoitus- tai matematiikkatehtävä voi olla käytännöllisempi. Jos liikkuvuus, tasapaino tai esteettömyys on huolenaihe, vältä liikkeeseen perustuvia tehtäviä ja valitse tehtävä, joka voidaan suorittaa turvallisesti.

## Yksittäinen-, ketju- ja satunnaisila

Yksittäistilassa pyydetään yhtä määritettyä tehtävää. Ketjutilassa suoritetaan useita määritettyjä tehtäviä järjestyksessä. Satunnaisessa tilassa valitaan määritetystä joukosta, mikä vähentää todennäköisyyttä että yksi opittu vuorovaikutus muuttuu automaattiseksi. Nämä tilat ovat läsnä uudemmassa tarkistetussa lähteessä; [saatavuus](../availability.md) selittää miksi se ei todista niiden olevan jo jokaisessa julkisessa versiossa.

Suorita aina lähiterminaalinen testi tilan, käyttöoikeuksien tai rekisteröityjen objektien muuttamisen jälkeen. Pidä valittu esine saavutettavissa ja tarjoa turvallinen palautumisreitti. Toimitusongelmiin, jotka eivät liity tehtävän suorittamiseen, käytä [luotettavuuden tarkistuslistaa](../help/alarm-delivery.md).

