---
title: Misiie BarcodeWake a reťaze misií
lang: sk
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
# Misiie BarcodeWake a reťaze misií

Misia BarcodeWake je podmienka použitá na odpovedanie budíka. Aktuálny zdroj podporuje úlohy s čiarovým kódom, QR kódom, matematikou, písaním, potrasením a krokmi, pričom registrované NFC je spracované cez cestu skenovania kódu. Misie môžu bežať samostatne, v poradí alebo náhodným výberom.

## Scanovacie misie vytvárajú fyzickú vzdialenosť

Misia s čiarovým kódom alebo QR kódom porovnáva živé skenovanie fotoaparátom s kódom registrovaným počas nastavenia. Kód je možné umiestniť na objekt mimo dosahu ruky: hygienické potreby v kúpeľni, položku na raňajky v kuchyni alebo iný stabilný objekt na dobre osvetlenom mieste. NFC sa riadi rovnakou všeobecnou myšlienkou s kompatibilnou značkou a zariadením. Aplikácia ukladá hašovú reprezentáciu v aktuálnych cestách namiesto potreby surového kódu na bežné porovnanie.

Vyberte objekt, ktorý bude stále dostupný, keď budík zaznie. Obaly sa vyhodia, štítky vyblednú a cestovanie mení prostredie. Registrácia kódu na jedinej škatuli s liekmi, ktorú môže byť potrebné vymeniť, je menej spoľahlivá ako použitie trvanlivého štítka. [Príručka nastavenia budíka](../guides/set-up-an-alarm.md) pokrýva umiestnenie a testovanie.

## Výzvové misie vymieňajú pohyb za úsilie

Matematika a písanie vyžadujú sústredený vstup. Potrasenie a kroky vyžadujú fyzický pohyb a podporované senzory. Nastavenie obtiažnosti a cieľa mení, koľko práce sa očakáva, ale ťažšia misia automaticky nie je lepšia. Nadmerné trenie môže podporiť úplné vypnutie budíka, zatiaľ čo jednoduchá úloha sa môže stať automatickou po opakovaní.

Prispôsobte úlohu režimu zlyhania. Ak vypínate budíky napoly spa, skenovanie v inej miestnosti vytvára užitočnú vzdialenosť. Ak je prístup ku kamere nepraktický, krátka úloha písania alebo matematiky môže byť praktickejšia. Ak máte obavy z mobility, rovnováhy alebo prístupnosti, vyhnite sa misiam založeným na pohybe a vyberte úlohu, ktorú je možné bezpečne dokončiť.

## Jednoduchý, reťazový a náhodný režim

Jednoduchý režim vyžaduje jednu nakonfigurovanú misiu. Reťazový režim spúšťa niekoľko nakonfigurovaných misií v poradí. Náhodný režim vyberá z nakonfigurovanej sady, čím znižuje pravdepodobnosť, že jedna zapamätaná interakcia sa stane automatickou. Tieto režimy sú prítomné v novšom kontrolovanom zdroji; [dostupnosť](../availability.md) vysvetľuje, prečo to nepreukazuje, že sú už v každej verejnej zostave.

Po zmene režimu, povolení alebo registrovaných objektov vždy spustite krátkodobý test. Uchovajte vybraný objekt dosiahnuteľný a poskytnite bezpečnú cestu obnovy. Pre problémy s doručením nesúvisiace s dokončením misie použite [kontrolný zoznam spoľahlivosti](../help/alarm-delivery.md).

