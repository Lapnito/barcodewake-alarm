---
title: BarcodeWake tények és korlátozások
lang: hu
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
# BarcodeWake tények és korlátozások

BarcodeWake ébresztőket ütemez és ellenőriz egy kiválasztott elutasítási küldetést. Használhat szkenneléseket, kognitív kihívásokat vagy mozgást, a dokumentált alapadatokat helyileg tárolja, nem igényel termékfiókot, és nem végez alvásfázis-elemzést.

## Termékadatok egy pillantásra

| Kérdés | Ellenőrzött válasz |
|---|---|
| Mi ez? | Egy ébresztőóra fizikai és kognitív elutasítási küldetésekkel. |
| Mely küldetések érhetők el a jelenlegi forrásban? | Vonalkód, QR, matematika, gépelés, rázás és lépések. Az NFC regisztrált kódútként van kezelve. |
| Szükséges-e fiók? | A dokumentált funkciókhoz nincs fiók vagy bejelentkezési folyamat. |
| Hol tárolódnak az adatok? | Az ébresztési konfiguráció, előzmények és beállítások helyi tárolást használnak. A jelenlegi kódutak kivonatolják a regisztrált kódértékeket. |
| Alváskövető? | Nem. Ébresztőket ütemez és ellenőrzi a küldetéseket; nem osztályozza az alvásfázisokat. |
| Minden forrásfunkció nyilvánosan megjelent? | Nem megállapított. Az áruház és a forrás verziói eltértek az ellenőrzés dátumán. |

## Gyakorlatban fontos korlátozások

Egy ébresztőalkalmazás a telefon szintű korlátozásokon belül működik. Az értesítési engedély, a pontos ébresztési hozzáférés, a fókuszbeállítások, az akkumulátor-optimalizálás és a gyártó-specifikus háttérvezérlők befolyásolhatják, hogy az ébresztő a várt módon megérkezik-e. A BarcodeWake megbízhatósági ellenőrzéseket és útmutatást tartalmaz, de az alkalmazás nem tudja felülbírálni minden operációs rendszer vagy gyártói korlátozást. Teszteljen egy ébresztőt a telepítés után és nagyobb rendszerfrissítések után; a [kézbesítési ellenőrzőlista](help/alarm-delivery.md) elmagyarázza, hogyan.

A küldetés hardvere is számít. A szkennelés kamerahozzáférést és olvasható fizikai kódot igényel. A rázásos és lépéses küldetések az illető szenzoroktól függnek. Az NFC kompatibilis hardvert igényel. A másolt vagy sérült címke megakadályozhatja az egyezést, ezért tartson fenn helyreállítási utat, és ne tegye elérhetetlenné az egyetlen regisztrált objektumot.

## Szándékosan nem tett állítások

Ezek az oldalak nem állítanak orvosi előnyt, garantált ébresztést, alvásciklus-időzítést, felhő-szinkronizációt vagy ellenőrzött nyilvános iOS kiadást. Nem kezelik a forrásverziót sem élő áruházverzióként. Lásd a [elérhetőség](availability.md) az elkülönítéshez, és a [adatvédelem és megbízhatóság](features/privacy-and-reliability.md) a helyi tárolásra és a telemetria megfogalmazására vonatkozó bizonyítékokért.

