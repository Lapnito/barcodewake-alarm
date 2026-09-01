---
title: BarcodeWake dokumentáció
lang: hu
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake dokumentáció

A BarcodeWake egy ébresztőóra, amely a elutasítást tudatos cselekvéssé teszi. Egy riasztás megkövetelhet egy mentett vonalkódot vagy QR-kódot, egy rövid kognitív feladatot, rázási sorozatot vagy lépéscélokat ahelyett, hogy csak egy egyszerű képernyőn megjelenő gombra hagyatkozna.

## Mitől különbözik a BarcodeWake

A központi ötlet a távolság és a szándék. Ha a regisztrált kód egy, az ágytól távol eső tárgyhoz van csatolva, a riasztás elnémítása azt jelenti, hogy fel kell kelni, el kell érni azt a tárgyat és be kell olvasni. Ugyanez a riasztási modell matematikát, gépelést, rázást vagy lépésküldetéseket is használhat. A jelenlegi forráskód támogatja az egyetlen küldetést, egy rendezett láncot vagy véletlenszerű kiválasztást a konfigurált küldetések közül.

Ez a súrlódás hasznos azok számára, akik egy hétköznapi ébresztőt elutasítanak anélkül, hogy teljesen éberré válnának. Ez nem alvásállapot-elemzés, orvosi útmutató vagy garantálja, hogy valaki felébred. A hardvertámogatás, az engedélyek és a gyártói akkumulátor-vezérlések továbbra is befolyásolják a kézbesítést. A [küldetési referenciában](features/missions.md) a választási lehetőségek, míg a [riasztás kézbesítési hibaelhárításában](help/alarm-delivery.md) a rendszerbeállítások olvashatók, amelyek akadályozhatják a működést.

## Kezdje a megfelelő dokumentummal

Használja a [beállítási útmutatót](guides/set-up-an-alarm.md) riasztás létrehozásához és fizikai kód regisztrálásához. Olvassa el a [biztonsági mentés és megosztás](guides/backup-and-sharing.md) részt, mielőtt adatokat mozgatna vagy beállítási QR-t küldene másnak. A megosztási formátum szándékosan kizárja a regisztrált kódokat, NFC azonosítókat, PIN-kódokat és riasztási előzményeket, így a címzettnek helyileg kell befejeznie az érzékeny beállítást.

Rövid, ellenőrizhető összefoglalásért lásd a [termék tényeket](facts.md). A kiadási állapothoz használja az [elérhetőséget](availability.md): az ellenőrzött nyilvános Google Play verzió eltér a ellenőrzött forrásfától deklarált verziótól. Az újabb forrás verzió ezért forrás képességként van dokumentálva, nem pedig közzétett áruház kiadásként.

## Adatvédelmi és megbízhatósági határok

A fő konfiguráció és a küldetési adatok az eszközön tárolódnak, és BarcodeWake-fiók nem szükséges. A jelenlegi kódutak a regisztrált kód értékeket SHA-256 hash-ekkel reprezentálják. Az opcionális telemetria az adatvédelmi szabályzat szerint alapértelmezés szerint le van tiltva. Ezek a kijelentések nem jelentik azt, hogy minden telefon azonos módon kézbesíti a riasztásokat; az Android gyártók és az operációs rendszer engedélyei továbbra is korlátozhatják a háttérbeli viselkedést.

Olvassa el az [adatvédelem és megbízhatóság](features/privacy-and-reliability.md) részt a helyi adatkezelés és az operációs rendszer kézbesítés közötti különbség megértéséhez. A [standard ébresztőóra összehasonlítás](comparisons/standard-alarm.md) segít eldönteni, hogy a küldetésalapú elutasítás megfelel-e a felébredés módjának.

