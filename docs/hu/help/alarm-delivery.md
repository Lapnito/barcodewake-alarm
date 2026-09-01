---
title: Miért nem szólal meg a BarcodeWake riasztás
lang: hu
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
# Miért nem szólal meg a BarcodeWake riasztás

## Először különítsük el a kézbesítést a figyelmeztetéstől

Hozz létre egy közeljövőbeli tesztriasztást egy egyszerű küldetéssel, és hagyd az alkalmazást a háttérben. Zárd le a képernyőt. Ha nem jelenik meg riasztási képernyő vagy hang, akkor a probléma a kézbesítés; a regisztrált vonalkód megváltoztatása nem oldja meg. Ha a riasztás megjelenik, de a küldetés nem tud befejeződni, a kézbesítés működik, és a hiba a kamerában, szenzorban, kód-egyeztetésben vagy a küldetés beállításaiban van.

Erősítsd meg, hogy a riasztás be van kapcsolva, a beállított nap helyes, és a telefon időzónája megegyezik a tervezett ütemezéssel. Ellenőrizd a média és a riasztás hangerejét, ne csak az oldalsó gomb állapotára hagyatkozz. Vizsgáld meg a ne zavarjanak (Do Not Disturb) vagy a fókusz szabályokat, a csatlakoztatott audioeszközöket, valamint azt, hogy a telefont újraindították‑e a riasztás létrehozása után.

## Operációs rendszer engedélykapuinak áttekintése

Engedélyezd az értesítéseket és bármely pontos riasztási vagy teljes képernyős riasztási hozzáférést, amelyet a telepített build kér. Távolítsd el a BarcodeWake‑et az agresszív akkumulátor-optimalizálás vagy az automatikus alvólisták alól, ha az eszköz gyártója ezeket a vezérlőket kínálja. Nyisd meg az alkalmazáson belüli megbízhatósági diagnosztikát, és kövesd az általa azonosított eszközspecifikus beállításokat. A [adatvédelem és megbízhatóság oldal](../features/privacy-and-reliability.md) magyarázza, hogy ezek a rendszerfüggőségek miért maradnak fenn, még ha az alkalmazás adatai helyileg vannak tárolva.

Egy beállítás megváltoztatása után ismételd meg a lezárt képernyős tesztet. Több vezérlő egyszerre történő módosítása megnehezíti az ok azonosítását. A rendszerfrissítések visszaállíthatják vagy újraértelmezhetik az engedélyeket, ezért tesztelj újra egy nagyobb frissítés vagy az alkalmazás újratelepítése után.

## Küldetés-végrehajtás külön vizsgálata

Vonalkód- és QR‑küldetések esetén tisztítsd meg a kamera lencséjét, javítsd a megvilágítást, és erősítsd meg, hogy a regisztrált objektum változatlan. Adj kamera engedélyt. NFC esetén ellenőrizd az eszköz támogatását, és tartsd a címkét a megfelelő antennapozíció közelében. A rázás és lépés küldetések a mozgás- vagy lépésszenzoroktól függnek, és eltérően viselkedhetnek, ha az energiatakarékos módok korlátozzák a szenzor adatainak továbbítását.

Ha a küldetés egy lánc részeként lett beállítva, minden szükséges lépésnek be kell fejeződnie. Tekintsd át a [küldetés viselkedését](../features/missions.md), és szükség esetén hozz létre egy új tesztet a [beállítási eljárás](../guides/set-up-an-alarm.md) segítségével.

## Tudatosítsd, mikor a telefon korlátot jelent

A BarcodeWake nem tud felülírni egy kikapcsolt eszközt, lemerült akkumulátort, hibás audiohardvert vagy minden gyári feladatölő mechanizmust. Ez nem sürgősségi értesítési szolgáltatás. Tarts fenn egy másik riasztási módszert a nagy kockázatú helyzetekre, és jelentsd a reprodukálható hibákat az eszközmodell, a rendszerverzió, az alkalmazásverzió és a pontos tesztkörülmények megadásával.

