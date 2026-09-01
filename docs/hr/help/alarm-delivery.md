---
title: Zašto se alarm BarcodeWake možda ne oglašava
lang: hr
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
# Zašto se alarm BarcodeWake možda ne oglašava

Spremljeni alarm može i dalje biti blokiran postavkama obavijesti, pristupom točnom alarmu, fokusom ili tihim načinom rada, niskom glasnoćom, ograničenjima baterije, obustavom aplikacije ili kontrolama pozadine dobavljača. Provjerite isporuku zasebno od skeniranja misije, a zatim pokrenite test na zaključanom zaslonu.

## Najprije izolirajte isporuku od odbacivanja

Stvorite testni alarm kratkoročno s jednostavnom misijom i ostavite aplikaciju u pozadini. Zaključajte zaslon. Ako se ne pojavi zaslon alarma ili zvuk, problem je isporuka; promjena registrirane barkode neće to popraviti. Ako se alarm pojavi, ali misija ne može završiti, isporuka funkcionira i problem je kamera, senzor, podudaranje koda ili konfiguracija misije.

Potvrdite da je alarm omogućen, da je zakazani dan ispravan i da vremenska zona telefona odgovara namjeravanom rasporedu. Provjerite glasnoću medija i alarma umjesto da se oslanjate samo na stanje bočne tipke. Pregledajte pravila ne ometanja ili fokusa, povezane audio uređaje i je li telefon ponovno pokrenut nakon stvaranja alarma.

## Pregledajte vrata dozvola operacijskog sustava

Dopustite obavijesti i bilo koji točan alarm ili pristup alarmu preko cijelog zaslona koje zahtijeva instalirana verzija. Uklonite BarcodeWake iz agresivne optimizacije baterije ili automatskih popisa za spavanje kada dobavljač uređaja nudi te kontrole. Otvorite dijagnostiku pouzdanosti u aplikaciji i slijedite postavke specifične za uređaj koje identificira. [Stranica o privatnosti i pouzdanosti](../features/privacy-and-reliability.md) objašnjava zašto ove sistemske ovisnosti ostaju čak i kada su podaci aplikacije lokalni.

Nakon promjene jedne postavke, ponovite test na zaključanom zaslonu. Promjena nekoliko kontrola odjednom otežava identificiranje uzroka. Sistemska ažuriranja mogu resetirati ili reinterpretirati dozvole, stoga ponovno testirajte nakon velikog ažuriranja ili ponovne instalacije aplikacije.

## Dijagnosticirajte dovršetak misije zasebno

Za barkod i QR misije, očistite leću kamere, poboljšajte osvjetljenje i potvrdite da registrirani objekt nije promijenjen. Dodijelite dozvolu kamere. Za NFC, verificirajte podršku uređaja i držite oznaku blizu ispravnog položaja antene. Misije mahanja i koraka ovise o senzorima kretanja ili koraka i mogu se ponašati drugačije kada načini uštede energije ograničavaju isporuku senzora.

Ako je misija konfigurirana kao dio lanca, svaki zahtijevani korak mora biti dovršen. Pregledajte [ponašanje misija](../features/missions.md) i, ako je potrebno, stvorite novi test pomoću [postupka postavljanja](../guides/set-up-an-alarm.md).

## Znajte kada je telefon granica

BarcodeWake ne može nadjačati isključen uređaj, iscrpljenu bateriju, neispravan audio hardver ili svaki killer zadataka proizvođača. Nije usluga hitnih obavijesti. Držite drugu metodu alarma za situacije s visokim posljedicama i prijavite reproducirane greške s modelom uređaja, verzijom sustava, verzijom aplikacije i točnim testnim uvjetima.

