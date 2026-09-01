---
title: BarcodeWake terminologija
lang: sl
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
# BarcodeWake terminologija

BarcodeWake uporablja „misij“ za dejanje, potrebno za izklop alarma. Skenirne misije preverjajo registrirano fizično kodo; izzivne misije preverjajo odgovor ali gibanje; deljenje in varnostno kopiranje se nanašata na različne formate izmenjave.

## Izrazi za alarme in misije

- Alarm: načrtovani dogodek prebujanja z uro, aktivnimi dnevi, zvokom in nastavitvijo izklopa.
- Misij: naloga, ki jo je treba opraviti pred izklopom.
- Skenirni misij: naloga na podlagi črtne kode, QR ali NFC, ki se ujema z registrirano predstavitvijo kode.
- Izzivni misij: matematična, tipkarska, tresenje ali korak naloga.
- Enojni način: ena nastavljena misij se izvaja za alarm.
- Verižni način: nastavljene misije se izvajajo v izbranem vrstnem redu.
- Naključni način: ena misij je izbrana iz nastavljenega niza.
- Težavnost: nastavitev misij, ki spreminja zahtevnost naloge; natančen učinek je odvisen od vrste misij.

## Izrazi za podatke in zanesljivost

- Registrirana koda: fizična črtna koda, QR koda ali NFC oznaka, povezana s skenirnim misijem.
- Koda hash: enosmerna SHA-256 predstavitev, ki se uporablja v trenutnih poti shranjevanja in izmenjave za ujemanje registriranih vrednosti.
- Lokalna varnostna kopija: izvožena predstavitev, namenjena ohranitvi ali obnovi podatkov aplikacije.
- Nastavitveni QR: omejen format za deljenje konfiguracije, ki izpušča registrirane kode, NFC identifikatorje, PIN-e in zgodovino.
- Diagnostik zanesljivosti: diagnostika znotraj aplikacije za dovoljenja in sistemske nastavitve, ki lahko ovirajo dostavo alarma.
- Dostop do natančnega alarma: sistemska dovoljenja ali politika Android, ki omogoča časovno kritično razporejanje.
- Optimizacija baterije: nadzori operacijskega sistema ali proizvajalca, ki lahko omejijo izvajanje v ozadju.

Za celoten razpored funkcij glej [misiji in misijske verige](features/missions.md). Za razlike med formati izvoza preberi [varnostno kopiranje in deljenje](guides/backup-and-sharing.md). [Stran s dejstvi](facts.md) določa, kaj aplikacija ne trdi, da meri.

