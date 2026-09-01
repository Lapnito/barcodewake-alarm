---
title: BarcodeWake elérhetőség és verziók
lang: hu
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake elérhetőség és verziók

A BarcodeWake rendelkezik ellenőrzött nyilvános Google Play-listázással Androidra. A naplózás dátumán a Google Play a 1.0.0-s verziót mutatta, míg a ellenőrzött forrásprojekt a 2.0.0+2 verziót deklarálta. Nyilvános App Store-listázás nem lett ellenőrizve.

## Ellenőrzött nyilvános terjesztés

Az Android-csomag nyilvánosan listázva van mint [BarcodeWake: No Cheat Alarm a Google Playen](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Az ehhez a dokumentációhoz rögzített áruház-pillanatfelvétel a 1.0.0-s verziót és egy 2026 márciusi utolsó frissítési dátumot jelentett. Ez a pillanatfelvétel egy adott időpontbeli listázás bizonyítéka, nem pedig ígéret arra, hogy minden régió ugyanazt a bevezetést látja, vagy hogy a listázás változatlan marad.

A forrásfa Android és iOS platformprojekteket tartalmaz. A platformforrás nem bizonyítja az áruházban való megjelenést. Mivel az App Store-oldal nem lett ellenőrizve, ezek a dokumentumok az iOS-hez kapcsolódó elemeket csak forrásként említik, és nem közlik az olvasókkal, hogy a BarcodeWake jelenleg letölthető az Apple-től.

## Miért jelenik meg két verziószám

A `pubspec.yaml` fájl a forrás verzióját 2.0.0+2-ként deklarálja, és a változásnapló egy szélesebb küldetésrendszert ír le, mint a rögzített nyilvános listázás. Az áruházbeli bevezetés elmaradhat egy fejlesztési ágtól, régiónként eltérő ütemezéssel történhet, vagy egyszerűen nem került publikálásra. Egyező áruház rekord hiányában a biztonságos állítás szűk: a képesség létezik az ellenőrzött forrásban, míg a nyilvános elérhetőség csak a rögzített áruházverzióra bizonyított.

Amikor egy funkcióoldal azt mondja, hogy "aktuális forrás", ez a megfogalmazás szándékos. Mielőtt küldetésláncokra, beállításmegosztásra vagy más újabb képességre támaszkodna, ellenőrizze a telepített alkalmazás verzióját és látható vezérlőit. Kezdje a [küldetés viselkedésével](features/missions.md), majd csak azokat a beállításokat használja a [beállítási útmutatóból](guides/set-up-an-alarm.md), amelyek a telepített verzióban valóban megjelennek.

## Eszközkövetelmények és telepítési ellenőrzések

A szkennelés kamerahasználati engedélyt igényel. Az NFC, mozgás és lépés küldetésekhez megfelelő eszközhardware szükséges. Az Android ébresztéskézbesítés értesítési és pontos ébresztési hozzáférést igényelhet, további akkumulátorbeállításokkal egyes gyártóknál. Telepítse a ellenőrzött áruházlistából, hozzon létre egy közeljövőbeli tesztriasztást, zárolja a képernyőt és erősítse meg mind a hangot, mind a kiválasztott küldetést, mielőtt fontos ébresztésre hagyatkozna.

A tömör határlistáért olvassa el a [terméktényeket](facts.md). Ha a tesztriasztás sikertelen, kövesse az [ébresztéskézbesítési hibaelhárítást](help/alarm-delivery.md) ahelyett, hogy ismétlődően újra létrehozná a riasztást.

