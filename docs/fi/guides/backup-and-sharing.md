---
title: Varmuuskopioi ja jaa BarcodeWake-herätykset turvallisesti
lang: fi
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
# Varmuuskopioi ja jaa BarcodeWake-herätykset turvallisesti

Käytä JSON-vientiä, kun haluat säilyttää tai siirtää omia sovellustietojasi, tulostettavaa PDF-varmuuskopiointia viivakoodina palautusta varten, ja asennuksen QR-koodin jakamista, kun toinen henkilö tarvitsee vain herätysrakenteen. Jakaminen jättää tarkoituksella pois rekisteröidyt salaisuudet ja historian.

## Valitse työhön sopiva muoto

Nykyinen lähde tarjoaa erilaisia vaihtoehtoja, koska varmuuskopiointi ja jakaminen eivät ole sama toimenpide. JSON-varmuuskopio on tarkoitettu rakenteelliseen tiedonsiirtoon ja palauttamiseen. PDF-varmuuskopio muuttaa palautusmateriaalin tulostettavaksi viivakoodidokumentiksi. Asennuksen QR-koodi on tarkoituksella suppeampi: se voi välittää rajallisen herätyskokoonpanon ilman rekisteröityjä viivakoodiarvoja, NFC-tunnuksia, PIN-koodeja tai historiaa.

Älä kohtele asennuksen QR-koodia täydellisenä laitteistovarmuuskopiona. Vastaanottajan on rekisteröitävä omat fyysiset koodinsa ja tarkistettava käyttöoikeudet paikallisesti. Nykyinen asennuksen jakaminen rajoittaa myös sitä, kuinka monta herätystä se voi sisältää, joten varmista tuotu tulos sen sijaan, että olettaisit jokaisen aikataulun siirtyneen. [Tuotetiedot](../facts.md) tallentaa nämä rajat.

## Luo ja suojaa henkilökohtainen varmuuskopio

Käytä vientitoimintoa, joka on käytettävissä asennetussa versiossa, valitse JSON tai tulostettava varmuuskopio palautussuunnitelmasi mukaan ja tallenna tulos johonkin hallitsemaasi paikkaan. Varmuuskopio voi paljastaa herätysten nimet, aikataulut ja muun kokoonpanon, vaikka rekisteröidyt raakakoodiarvot on suojattu tai jätetty pois. Käsittele sitä henkilökohtaisten rutiinitietojen tapaan: vältä julkisia linkkejä, jaettuja tulostimia ja luottamattomia viestikanavia.

Viennin jälkeen varmista, että tiedosto löytyy ja että sen aikaleima vastaa tarkoitettua varmuuskopiota. Älä poista alkuperäisiä sovellustietoja vain siksi, että vientikomento ilmoitti onnistumisesta. Palautustestaus on ainoa luotettava tarkistus, mutta suorita se turvallisella laitteella tai toisen kopion tekemisen jälkeen, jotta testaus itsessään ei muutu tietojen menetykseksi.

## Jaa asennus jakamatta salaisuuksia

Luo asennuksen QR-koodi vain niille herätyksille, jotka vastaanottajan tulisi saada. Vastaanottaja skannaa sen, tarkistaa tuodun aikataulun ja toimittaa omat koodinsa, NFC-tunnisteensa tai palautustietonsa. Tämä suunnittelu estää jaetun kokoonpanon hiljaisesti siirtämästä fyysistä avainta, joka kumoaa jonkun toisen herätyksen.

Tuonnin jälkeen jokaisen henkilön tulisi suorittaa täydellinen [herätyksen asennustesti](set-up-an-alarm.md). Käyttöoikeudet, anturit ja käyttöjärjestelmän rajoitukset eivät siirry QR-koodissa. Jos tuotu herätys ei ilmesty lukituksen aikana, noudata [herätyksen toimituksen vianmääritystä](../help/alarm-delivery.md).

Lähde- ja tallennusversiot poikkesivat toisistaan tämän tarkastuksen aikana, joten asennettu julkinen versio ei välttämättä näytä kaikkia tässä kuvattuja vaihtoehtoja. [Saatavuus](../availability.md) selittää, miten tulkita vain lähdekoodissa olevia ominaisuuksia.

