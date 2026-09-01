---
title: BarcodeWake-termistö
lang: fi
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# BarcodeWake-termistö

BarcodeWake käyttää termiä “tehtävä” toiminnosta, joka vaaditaan hälytyksen kumoamiseen. Skannaustehtävät vahvistavat rekisteröidyn fyysisen koodin; haastetehtävät vahvistavat vastauksen tai liikkeen; jakaminen ja varmuuskopiointi viittaavat eri vaihtomuotoihin.

## Hälytyksen ja tehtävän termit

- Hälytys: ajastettu herätystapahtuma, jossa on aika, aktiiviset päivät, ääni ja kumoamisasetukset.
- Tehtävä: tehtävä, joka on suoritettava ennen kumoamista.
- Skannaustehtävä: viivakoodi-, QR- tai NFC-pohjainen tehtävä, joka vastaa rekisteröityä koodiesitystä.
- Haastetehtävä: matemaattinen, kirjoitus-, ravistus- tai askelutehtävä.
- Yksittäinen tila: yksi määritetty tehtävä suoritetaan hälytykselle.
- Ketjutustila: määritetyt tehtävät suoritetaan valitussa järjestyksessä.
- Satunnainen tila: yksi tehtävä valitaan määritetystä joukosta.
- Vaikeustaso: tehtävän asetus, joka muuttaa tehtävän vaatimusta; sen tarkka vaikutus riippuu tehtävätyypistä.

## Tieto- ja luotettavuustermien määritelmät

- Rekisteröity koodi: fyysinen viivakoodi, QR-koodi tai NFC-tunniste, joka liittyy skannaustehtävään.
- Koodin tiiviste: yksisuuntainen SHA‑256-esitys, jota nykyiset tallennus- ja vaihtopolut käyttävät rekisteröityjen arvojen yhdistämiseen.
- Paikallinen varmuuskopio: viety esitys, joka on tarkoitettu säilyttämään tai palauttamaan sovellusdataa.
- Asetuksien QR‑koodi: rajoitettu konfiguraationjakomuoto, joka ei sisällä rekisteröityjä koodeja, NFC‑tunnuksia, PIN‑koodeja tai historiaa.
- Luotettavuuslääkäri: sovelluksen sisäinen diagnostiikka käyttöoikeuksille ja järjestelmäasetuksille, jotka voivat häiritä hälytyksen toimittamista.
- Tarkan hälytyksen käyttöoikeus: Android‑järjestelmän lupa tai käytäntö, joka sallii aikakriittisen aikataulutuksen.
- Akun optimointi: käyttöjärjestelmän tai laitetoimittajan hallintatoimet, jotka voivat rajoittaa taustasuoritusta.

Täydelliset ominaisuussuhteet löydät kohdasta [tehtävät ja tehtäväketjut](features/missions.md). Vientimuotojen erot löydät kohdasta [varmuuskopiointi ja jakaminen](guides/backup-and-sharing.md). [Tietosivu](facts.md) määrittelee, mitä sovellus ei väitä mittaavansa.

