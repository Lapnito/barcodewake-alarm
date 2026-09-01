---
title: Misija in verige misij BarcodeWake
lang: sl
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
# Misija in verige misij BarcodeWake

Misija BarcodeWake je pogoj, ki se uporablja za izklop alarma. Trenutni vir podpira naloge črtne kode, QR kode, matematike, tipkanja, tresenja in korakov, pri čemer se registrirani NFC obravnava prek poti skeniranja kode. Misije lahko delujejo posamezno, zaporedno ali z naključno izbiro.

## Pregledovalne misije ustvarjajo fizično razdaljo

Misija črtne kode ali QR kode primerja dejansko skeniranje kamere s kodo, registrirano med nastavitvijo. Kodo je mogoče namestiti na predmetu zunaj dosega roke: izdelki za osebno nego v kopalnici, artikel za zajtrk v kuhinji ali drug stabilen predmet na dobro osvetljenem območju. NFC sledi istemu splošnemu konceptu s kompatibilno oznako in napravo. Aplikacija shrani hash predstavitev v trenutne poti, namesto da bi potrebovala surovno kodo za običajno primerjavo.

Izberite predmet, ki bo še vedno na voljo, ko zazvoni alarm. Embalaža se zavrže, nalepke zbledijo in potovanje spremeni okolje. Registracija kode na edini škatli za zdravila, ki jo boste morda morali zamenjati, je manj robustna kot uporaba trajne nalepke. [Navodila za nastavitev alarma](../guides/set-up-an-alarm.md) zajemajo namestitev in testiranje.

## Misije izzivov menjujejo gibanje za trud

Matematika in tipkanje zahtevata osredotočen vnos. Tresenje in koraki zahtevajo fizično gibanje in podprte senzorje. Nastavitve težavnosti in cilja spreminjajo pričakovano količino dela, vendar težja misija ni samodejno boljša. Preveliko trenje lahko spodbudi popolno onemogočanje alarma, medtem ko lahko enostavna naloga po ponavljanju postane samodejna.

Prilagodite nalogo načinu napake. Če izklopite alarme polspanja, skeniranje v drugem prostoru ustvari uporabno razdaljo. Če je dostop do kamere nepriročen, je lahko kratka naloga tipkanja ali matematike bolj praktična. Če gre za mobilnost, ravnotežje ali dostopnost, se izogibajte misijam, ki temeljijo na gibanju, in izberite nalogo, ki jo je mogoče varno opraviti.

## Posamezni, verižni in naključni načini

Posamezni način zahteva eno konfigurirano misijo. Verižni način izvaja več konfiguriranih misij zaporedno. Naključni način izbira iz konfiguriranega nabora in zmanjšuje verjetnost, da ena zapomnjena interakcija postane samodejna. Ti načini so prisotni v novejšem preverjenem viru; [razpoložljivost](../availability.md) pojasnjuje, zakaj to ne dokazuje, da so že v vsaki javni gradnji.

Po spremembi načina, dovoljenj ali registriranih predmetov vedno izvedite kratkoročni test. Ohranite izbrani predmet dosegljiv in zagotovite varno pot okrevanja. Za težave z dostavo, ki niso povezane z dokončanjem misije, uporabite [kontrolni seznam zanesljivosti](../help/alarm-delivery.md).

