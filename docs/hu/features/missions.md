---
title: BarcodeWake küldetések és küldetésláncok
lang: hu
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
# BarcodeWake küldetések és küldetésláncok

A BarcodeWake küldetés az az állapot, amelyet az ébresztő elhallgattatásához használnak. A jelenlegi forrás támogatja a vonalkód, QR, matematikai, gépelés, rázás és lépés feladatokat, a regisztrált NFC-t pedig a kódolvasási útvonalon kezeli. A küldetések önállóan, sorban vagy véletlenszerű kiválasztással futtathatók.

## A szkennelési küldetések fizikai távolságot teremtenek

A vonalkód- vagy QR-küldetés az élő kamera szkennelését hasonlítja össze a beállítás során regisztrált kóddal. A kódot egy, a karoktól távol eső tárgyra helyezheted: fürdőszobai pipereszer, konyhai reggeli elem, vagy más stabil tárgy jól megvilágított helyen. Az NFC ugyanezt az általános ötletet követi kompatibilis címkével és eszközzel. Az alkalmazás hash ábrázolást tárol az aktuális útvonalakon, nem pedig a nyers kódot a normál összehasonlításhoz.

Válassz egy tárgyat, amely az ébresztéskor még rendelkezésre áll. A csomagolás eldobásra kerül, a címkék elhalványulnak, és az utazás megváltoztatja a környezetet. Ha egyetlen gyógyszeres dobozra regisztrálod a kódot, amelyet esetleg ki kell cserélned, az kevésbé robusztus, mint tartós címke használata. Az [ébresztő beállítási útmutató](../guides/set-up-an-alarm.md) a elhelyezést és a tesztelést ismerteti.

## A kihívás küldetések mozgást erőfeszítésre cserélik

A matek és a gépelés koncentrált beviteleket igényel. A rázás és a lépések fizikai mozgást igényelnek, valamint támogatott érzékelőket. A nehézség és a célbeállítások megváltoztatják, mennyi munkát várnak el, de a nehezebb küldetés nem automatikusan jobb. A túlzott súrlódás arra ösztönözhet, hogy teljesen kikapcsold az ébresztőt, míg egy könnyű feladat ismétlés után automatikussá válhat.

Igazítsd a feladatot a hibaüzemmódhoz. Ha félálomban kapcsolod ki az ébresztőket, egy másik szobában történő szkennelés hasznos távolságot teremt. Ha a kamera elérés nehézkes, egy rövid gépelési vagy matek feladat praktikusabb lehet. Ha a mobilitás, az egyensúly vagy a hozzáférhetőség aggodalom, kerüld a mozgásalapú küldetéseket, és válassz biztonságosan elvégezhető feladatot.

## Egyéni, lánc és véletlenszerű módok

Az egyéni mód egy konfigurált küldetést kér. A lánc mód a konfigurált küldetéseket sorrendben futtatja. A véletlenszerű mód a konfigurált halmazból választ, csökkentve annak esélyét, hogy egy memóriában rögzült interakció automatikussá váljon. Ezek a módok a newer ellenőrzött forrásban találhatók; a [elérhetőség](../availability.md) megmagyarázza, hogy ez miért nem bizonyítja, hogy már minden nyilvános buildben megtalálhatók.

Mindig végezz rövid távú tesztet a mód, az engedélyek vagy a regisztrált objektumok megváltoztatása után. Tartsd a kiválasztott objektumot elérhetően, és biztosíts biztonságos visszaállítási útvonalat. A küldetés teljesítésével nem összefüggő kézbesítési problémák esetén használd a [megbízhatósági ellenőrző listát](../help/alarm-delivery.md).

