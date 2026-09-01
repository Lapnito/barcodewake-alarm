---
title: Dejstva in omejitve BarcodeWake
lang: sl
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
# Dejstva in omejitve BarcodeWake

BarcodeWake načrtuje budilke in preverja izbrano nalogo odprave. Uporablja lahko skeniranje, kognitivne izzive ali gibanje, shranjuje dokumentirane jedrne podatke lokalno, ne zahteva računa izdelka in ne izvaja analize stopenj spanja.

## Ključna dejstva o izdelku

| Vprašanje | Preverjen odgovor |
|---|---|
| Kaj je to? | Budilka s fizičnimi in kognitivnimi nalogami za odpravo. |
| Katere naloge obstajajo v trenutni kodi? | Črtna koda, QR, matematika, tipkanje, tresenje in koraki. NFC se obravnava kot registrirana pot kode. |
| Ali je račun obvezen? | Za dokumentirane funkcije račun ali postopek prijave ni prisoten. |
| Kje se hranijo podatki? | Konfiguracija budilke, zgodovina in nastavitve uporabljajo lokalno shrambo. Trenutne poti kode zgoščujejo vrednosti registrirane kode. |
| Ali je to sledilnik spanja? | Ne. Načrtuje budilke in preverja naloge; ne razvršča stopenj spanja. |
| Ali je vsaka funkcija v kodi javno izdana? | Ni ugotovljeno. Različici trgovine in izvorne kode sta se na datum revizije razlikovali. |

## Omejitve, ki so pomembne v praksi

Aplikacija za budilko deluje znotraj omejitev na ravni telefona. Dovoljenje za obvestila, dostop do natančnih budilk, nastavitve osredotočenosti, optimizacija baterije in nadzor ozadja, ki je značilen za posameznega proizvajalca, lahko vplivajo na to, ali budilka pride, kot je pričakovano. BarcodeWake vključuje preverjanje zanesljivosti in navodila, vendar aplikacija ne more prepisati vsake omejitve operacijskega sistema ali proizvajalca. Preizkusite budilko po namestitvi in po večjih sistemskih spremembah; [kontrolni seznam dostave](help/alarm-delivery.md) razloži, kako.

Strojna oprema naloge je prav tako pomembna. Skeniranje zahteva dostop do kamere in čitljivo fizično kodo. Naloge tresenja in korakov so odvisne od ustreznih senzorjev. NFC potrebuje združljivo strojno opremo. Kopija ali poškodovana oznaka lahko prepreči ujemanje, zato ohranite pot obnovitve in ne naredite edinega registriranega predmeta nedostopnega.

## Trditve, ki namerno niso podane

Na teh straneh ni trditve o medicinski koristi, zagotovljenem prebujanju, časovnem razporejanju ciklov spanja, sinhronizaciji v oblaku ali preverjeni javni izdaji za iOS. Prav tako ne obravnavajo različice izvorne kode kot različice v trgovini. Glejte [razpoložljivost](availability.md) za to razlikovanje in [zasebnost in zanesljivost](features/privacy-and-reliability.md) za dokaze za formulacije o lokalni shrambi in telemetriji.

