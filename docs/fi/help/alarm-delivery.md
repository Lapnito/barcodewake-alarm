---
title: Miksi BarcodeWake-herätys ei välttämättä soi
lang: fi
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---

# Miksi BarcodeWake-herätys ei välttämättä soi

Tallennettu herätys voi silti estyä ilmoitusasetusten, tarkan herätyksen käyttöoikeuden, fokuksen tai hiljaisen tilan, matalan äänenvoimakkuuden, akkurajoitusten, sovelluksen keskeytyksen tai valmistajan taustasäätimien vuoksi. Tarkista toimitus erikseen tehtävän skannauksesta ja suorita sitten lukitun näytön testi.

## Erota ensin toimitus hylkäyksestä

Luo lähiajan testiherätys yksinkertaisella tehtävällä ja jätä sovellus taustalle. Lukitse näyttö. Jos herätysnäkymää tai ääntä ei tule, ongelma on toimituksessa; rekisteröidun viivakoodin muuttaminen ei korjaa sitä. Jos herätys tulee näkyviin, mutta tehtävä ei pysty suorittumaan, toimitus toimii ja ongelma on kamerassa, anturissa, koodin tunnistuksessa tai tehtäväkonfiguraatiossa.

Varmista, että herätys on käytössä, aikataulun päivä on oikea ja puhelimen aikavyöhyke vastaa aiottua aikataulua. Tarkista media- ja herätysääni eikä vain sivupainikkeen tilaa. Tarkista „Älä häiritse"‑ tai fokus‑säännöt, liitetyt äänilaitteet ja onko puhelinta käynnistetty uudelleen herätyksen luomisen jälkeen.

## Tarkista käyttöjärjestelmän käyttöoikeusportit

Salli ilmoitukset ja kaikki asennetun version pyytämät tarkan herätyksen tai täysruutuherätyksen käyttöoikeudet. Poista BarcodeWake aggressiivisesta akkujen optimoinnista tai automaattisesta lepotilalistasta, kun laitevalmistaja tarjoaa näitä hallintatoimintoja. Avaa sovelluksen luotettavuusdiagnostiikka ja noudata sen tunnistamia laitekohtaisia asetuksia. [tietosuoja- ja luotettavuussivu](../features/privacy-and-reliability.md) selittää, miksi nämä järjestelmäriippuvuudet pysyvät, vaikka sovelluksen tiedot ovat paikallisia.

Kun muutat yhtä asetusta, toista lukitun näytön testi. Usean säätimen muuttaminen kerralla vaikeuttaa syyn tunnistamista. Järjestelmäpäivitykset voivat nollata tai tulkita käyttöoikeuksia uudelleen, joten testaa uudelleen merkittävän päivityksen tai sovelluksen uudelleenasennuksen jälkeen.

## Diagnosoi tehtävän suoritus erikseen

Viivakoodi- ja QR‑tehtävissä puhdista kameran linssi, paranna valaistusta ja varmista, että rekisteröity kohde ei ole muuttunut. Myönnä kamerakäyttöoikeus. NFC‑tehtävissä varmista laitteen tuki ja pidä tunniste oikean antennin kohdalla. Ravista ja kävele -tehtävät riippuvat liike- tai askelsensorista ja voivat käyttäytyä eri tavalla, kun virransäästötilat rajoittavat sensorin toimintaa.

Jos tehtävä on määritetty osana ketjua, jokaisen vaaditun vaiheen on suorittauduttava. Tarkista [tehtävän käyttäytyminen](../features/missions.md) ja tarvittaessa luo uusi testi [asennusohjeen](../guides/set-up-an-alarm.md) mukaisesti.

## Tiedä, milloin puhelin on rajoitteena

BarcodeWake ei voi ohittaa sammutettua laitetta, tyhjentynyttä akkua, rikkoutunutta äänilaitteistoa tai jokaista valmistajan tehtävän tappajaa. Se ei ole hätäilmoituspalvelu. Pidä varasuunnitelma herätysmenetelmä korkean riskin tilanteisiin ja raportoi toistettavat virheetilanteet laitteen mallilla, järjestelmäversiolla, sovellusversiolla ja tarkoilla testiolosuhteilla.

