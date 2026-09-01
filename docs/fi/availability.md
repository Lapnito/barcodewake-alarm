---
title: BarcodeWaken saatavuus ja versiot
lang: fi
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWaken saatavuus ja versiot

BarcodeWakella on vahvistettu julkinen Google Play -listaus Androidille. Tarkastuspäivänä Google Play näytti versiota 1.0.0, kun tarkistettu lähdeprojekti ilmoitti version 2.0.0+2. Yhtään julkista App Store -listausta ei vahvistettu.

## Vahvistettu julkinen jakelu

Android-paketti on julkisesti listattu nimellä [BarcodeWake: No Cheat Alarm Google Playssa](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Tämän dokumentaation yhteydessä tallennettu kauppasnapshot raportoi version 1.0.0 ja viimeisimmän päivityksen päivämääräksi maaliskuun 2026. Tämä snapshot on todiste listauksesta tietyssä ajankohdassa, ei lupaus siitä, että jokainen alue näkee saman julkaisun tai että listaus pysyy muuttumattomana.

Lähdekoodipuu sisältää Android- ja iOS-alustaprojektit. Alustan lähdekoodi ei todista kauppajulkaisua. Koska yhtään App Store -sivua ei vahvistettu, nämä dokumentit kuvaavat iOS:ään liittyvät kohteet vain lähdetukena, eikä niissä kerrota lukijoille, että BarcodeWake on tällä hetkellä ladattavissa Applelta.

## Miksi näkyy kaksi versionumeroa

Varastot `pubspec.yaml` ilmoittaa lähdeversion 2.0.0+2 ja sen muutoshistoria kuvaa laajempaa tehtäväjärjestelmää kuin kaapattu julkinen listaus. Kauppajulkaisu voi jäädä jälkeen kehityshaarasta, vaiheittain alueittain, tai sitä ei yksinkertaisesti ole julkaistu. Ilman vastaavaa kauppatietuetta turvallinen väite on suppea: kyky on olemassa tarkistetussa lähdekoodissa, kun taas julkinen saatavuus on todistettu vain kaapatulle kauppaversiolle.

Kun ominaisuussivu sanoo "nykyinen lähde", tuo sanamuoto on tarkoituksellinen. Ennen kuin luotat tehtäväketjuihin, asetusjakoon tai muuhun uudempaan ominaisuuteen, tarkista asennetun sovelluksen versio ja näkyvät säätimet. Aloita [tehtäväkäyttäytymisestä](features/missions.md) ja käytä sitten [asetusten opasta](guides/set-up-an-alarm.md) vain niihin vaihtoehtoihin, jotka asennettu koontiversiosi todella näyttää.

## Laitteistovaatimukset ja asennustarkistukset

Skannaaminen vaatii kameran käyttöoikeuden. NFC-, liike- ja askelmäärätehtävät vaativat vastaavaa laitteistoa. Android-herätysjakelu voi vaatia ilmoitus- ja tarkan herätyksen käyttöoikeuden, lisäksi akun asetuksia joillakin valmistajilla. Asenna vahvistetusta kauppalistauksesta, luo lähiaikainen testiherätys, lukitse näyttö ja vahvista sekä ääni että valittu tehtävä ennen kuin luotat siihen tärkeässä heräämisessä.

Tietoa selkeästä rajalistauksesta on kohdassa [tuotetiedot](facts.md). Jos testiherätys epäonnistuu, noudata [herätyksen jakelun vianmääritystä](help/alarm-delivery.md) äläkä toista herätyksen uudelleenluomista.

