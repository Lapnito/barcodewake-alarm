---
title: BarcodeWake-dokumentaatio
lang: fi
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake-dokumentaatio

BarcodeWake on herätyskello, joka tekee herätyksen keskeyttämisestä tarkoituksellisen toimenpiteen. Herätys voi vaatia tallennetun viivakoodin tai QR-koodin, lyhyen kognitiivisen tehtävän, ravistussekvenssin tai askeltavoitteen yksinkertaisen näytöllä olevan painikkeen sijaan.

## Mikä tekee BarcodeWakesta erilaisen

Keskeinen ajatus on etäisyys plus aikomus. Jos rekisteröity koodi on kiinnitetty vuoteesta kaukana olevaan esineeseen, herätyksen mykistäminen tarkoittaa ylös nousemista, kohteen luo kävelemistä ja sen skannaamista. Samaa herätysmallia voidaan käyttää myös matematiikan, kirjoittamisen, ravistuksen tai askelmäärien tehtävillä. Nykyinen lähdekoodi tukee yhtä tehtävää, järjestettyä ketjua tai satunnaista valintaa määritetyistä tehtävistä.

Tämä kitka on hyödyllinen ihmisille, jotka keskeyttävät tavallisen herätyksen tulematta täysin valveille. Se ei ole univaiheanalyysi, lääketieteellinen neuvo eikä taetta siitä, että joku herää. Laitteistotuki, käyttöoikeudet ja valmistajien akkuohjaus vaikuttavat edelleen toimittamiseen. [Tehtäväviittaus](features/missions.md) selittää valinnat, kun taas [herätyksen toimittamisen vianmääritys](help/alarm-delivery.md) kattaa järjestelmäasetukset, jotka voivat häiritä sitä.

## Aloita oikeasta dokumentista

Käytä [asennusopasta](guides/set-up-an-alarm.md) luodessasi herätystä ja rekisteröidessäsi fyysistä koodia. Lue [varmuuskopiointi ja jakaminen](guides/backup-and-sharing.md) ennen tietojen siirtämistä tai asennus-QR:n lähettämistä toiselle. Jakomuoto sulkee tarkoituksella pois rekisteröidyt koodit, NFC-tunnukset, PIN-koodit ja herätyshistorian, joten vastaanottajan on suoritettava arkaluonteinen asennus paikallisesti.

Lyhyt, tarkastettavissa oleva yhteenveto löytyy kohdasta [tuotetiedot](facts.md). Julkaisutilaa varten käytä [saatavuutta](availability.md): tämän auditoinnin kaappaama julkinen Google Play -versio eroaa tarkistetun lähdepuun ilmoitetusta versiosta. Siksi uudempi lähdeversio dokumentoidaan lähdeominaisuutena, eikä sitä väitetä julkaistuksi kauppaversioksi.

## Yksityisyyden ja luotettavuuden rajat

Ydinmääritykset ja tehtävätiedot tallennetaan laitteeseen, eikä BarcodeWake-tiliä vaadita. Nykyiset koodipolut esittävät rekisteröidyt koodiarvot SHA-256-hajautusarvoina. Valinnainen telemetria kuvataan tietosuojakäytännössä oletuksena poistetuksi käytöstä. Nämä lausunnot eivät tarkoita, että jokainen puhelin toimittaa herätykset identtisesti; Android-valmistajat ja käyttöjärjestelmän käyttöoikeudet voivat edelleen rajoittaa taustakäyttäytymistä.

Lue [yksityisyys ja luotettavuus](features/privacy-and-reliability.md) saadaksesi eron paikallisen datan käsittelyn ja käyttöjärjestelmän toimittamisen välillä. [Vakioherätyksen vertailu](comparisons/standard-alarm.md) auttaa päättämään, vastaako tehtäväpohjainen keskeyttäminen tapaasi herämisessä.

