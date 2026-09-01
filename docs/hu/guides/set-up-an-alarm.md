---
title: Hogyan állítsunk be BarcodeWake riasztást
lang: hu
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---

# Hogyan állítsunk be BarcodeWake riasztást

Először hozza létre az ütemezést, válasszon biztonságos és praktikus küldetést, adja meg a szükséges engedélyeket, majd futtasson egy közelgő zároltképernyős tesztet. A szkennelési küldetések esetén regisztráljon egy tartós objektumot, amely elérhető és olvasható lesz, amikor a riasztás megszólal.

## Válassza ki a küldetést az objektum előtt

Döntse el, mely művelet válassza el az ébredést a elutasítástól. Egy vonalkód egy másik szobában fizikai távolságot teremt. Matek vagy gépelés koncentrációt ad hozzá, kamera nélkül. Rázás vagy lépések mozgást adnak, de érzékelőktől függnek, és nem feltétlenül alkalmasak minden személyre vagy környezetre. A [küldetési referencia](../features/missions.md) elmagyarázza az egyéni, lánc és véletlenszerű módok közötti kompromisszumokat.

Ha vonalkódot, QR-kódot vagy NFC-címkét használ, válasszon tartós tárgyat. Kerülje az eldobható csomagolást, olyan objektumot, amelyet más háztartási tag elmozdíthat, vagy olyan kódot, amely utazás közben nem lesz elérhető. Ellenőrizze, hogy a kamera tud-e fókuszálni a várt fényviszonyok között. Az NFC-hez kompatibilis telefon és címke szükséges.

## Állítsa be az ütemezést és az elutasítási szabályt

Nyissa meg a riasztásszerkesztőt, állítsa be a kívánt időt és az aktív napokat, majd válassza ki a telepített build által mutatott küldetést. Az első teszthez konzervatívan állítsa be a nehézséget vagy a célt. Ha a telepített verzió támogatja a láncokat, úgy rendezze a küldetéseket, hogy azok biztonságosan, sietés nélkül, lépcsőkön át vagy biztonságos terület elhagyása nélkül teljesíthetők legyenek.

Regisztrálja a fizikai kódot a küldetés beállítási folyamatából. Adja a riasztásnak olyan címkét, amely a szándékolt rutint azonosítja, ne pedig érzékeny információt tegyen közzé. Tekintse át a hangerőt, a rezgést és az ébresztési utáni opciókat, amelyek a telepített buildben láthatók. Az elérhető vezérlők eltérhetnek, mert a [nyilvános és forrásverziók](../availability.md) az audit dátumán nem voltak azonosak.

## Adjon engedélyeket céllal

Engedélyezze az értesítéseket és a riasztáshoz szükséges hozzáférést a kézbesítéshez. Csak szkennelési küldetés esetén adjon kamera-hozzáférést, és érzékelő-hozzáférést, ha a választott küldetés ezt igényli. Androidon tekintse át a pontos riasztás és akkumulátor beállításait, ha az alkalmazás megbízhatósági ellenőrzése jelzi azokat. Ne feltételezze, hogy a riasztás mentése bizonyítja a háttérbeli kézbesítés engedélyezettségét.

## Tesztelje a teljes éjszakai útvonalat

Állítson be egy tesztet néhány perccel előre. Zárja le a képernyőt, hagyja a BarcodeWake-et a háttérben, és helyezze a telefont ugyanabba a hang- és energiaállapotba, amelyet az éjszakára tervezett. Erősítse meg, hogy a riasztás megjelenik, a hang hallható, és a pontosan kiválasztott küldetés elvégezhető. Ezután ismételje meg a regisztrált objektum tényleges helyére való áthelyezése után.

Ha a kézbesítés sikertelen, használja a [riasztáskézbesítési ellenőrzőlistát](../help/alarm-delivery.md). Ha sikeres, fontolja meg a [helyi biztonsági mentés](backup-and-sharing.md) elkészítését, miután a beállítás stabil.

