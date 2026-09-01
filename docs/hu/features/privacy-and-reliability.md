---
title: BarcodeWake adatvédelem és riasztás megbízhatósága
lang: hu
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - is BarcodeWake private and reliable
facts_used:
  - offline
  - account_required
  - ads_tracking
  - data_storage
  - accuracy_limits
---
# BarcodeWake adatvédelem és riasztás megbízhatósága

A BarcodeWake a dokumentált riasztókonfigurációt és küldetésadatokat a készüléken tárolja, és nem igényel alkalmazásfiókot. A jelenlegi kódutak kivonatolják a regisztrált kódértékeket. A választható telemetria alapértelmezés szerint le van tiltva, míg a riasztás kézbesítése továbbra is a rendszerengedélyektől és a gyártói vezérlőktől függ.

## A helyi adatok nem szüntetik meg a rendszerfüggőségeket

A helyi tárolás azt jelenti, hogy a normál riasztóbeállítás nem igényel BarcodeWake felhőfiókot. A riasztási rekordok, előzmények és beállítások az alkalmazás helyi adatszintjén keresztül kezelődnek. A regisztrált vonalkód, QR és NFC értékek SHA-256 kivonatokként jelennek meg a jelenlegi tárolási és importálási útvonalakon, ami elkerüli az eredeti nyers érték megőrzését az egyeztetéshez.

A kivonatolás (hashing) nem ugyanaz, mint az alkalmazás minden rekordjának titkosítása, és a helyi tárolás nem backup. Egy feloldott készülékhez hozzáféréssel rendelkező személy továbbra is láthatja a riasztásneveket, ütemezéseket vagy előzményeket az alkalmazáson keresztül. Az elveszett vagy visszaállított telefon szintén elveszítheti a helyi adatokat, kivéve ha a felhasználó készített exportálást. Lásd a [backup és megosztás](../guides/backup-and-sharing.md) útmutatót a formátumokért és azok különböző céljaiért.

Az adatvédelmi szabályzat szerint a választható telemetria alapértelmezés szerint ki van kapcsolva, és leírja az összesített kezelést, ha engedélyezve van. Ez a dokumentáció ezért nem állítja azt a szélesebb állítást, hogy az alkalmazás soha nem kommunikálhat hálózaton keresztül. A szűkebb, ellenőrzött tényeket közli: a fő működés és az adatok helyiek, termékfiók nem szükséges, és a vizsgált projektben nem látható hirdetési SDK függőség.

## A megbízhatóság közös felelősség

A BarcodeWake képes riasztást ütemezni és bemutatni, de az operációs rendszer dönti el, hogy a háttérben végzett munka mikor futhat, és mely megszakítások engedélyezettek. Az értesítési engedély, a pontos riasztáshozzáférés, a csendes vagy fókusz módok, az akkumulátor-optimalizálás, az automatikus alkalmazás-felfüggesztés és a gyártói taskillerek mind számíthatnak. Az alkalmazáson belüli megbízhatósági eszközök azonosíthatják a konfigurációs kockázatokat és irányíthatják a felhasználókat a beállításokhoz; nem tudják felülbírálni a rendszerszabályzatot.

A telepítés után teszteljen lezárt képernyővel és a telefonnal ugyanabban az energiatakarékos módban, amelyet éjszakára használ. Ismételje meg a tesztet rendszerfrissítés, akkumulátortakarékos mód változtatás vagy alkalmazás-újratelepítés után. Tartsa a készüléket feltöltve, a hangerőt megfelelően, és a kiválasztott küldetést fizikailag elérhetően. Kövesse a [riasztás kézbesítésének hibaelhárítását](../help/alarm-delivery.md), ha a teszt sikertelen.

## Amit az adatvédelem és a megbízhatóság nem ígérnek

A BarcodeWake nem orvostechnikai eszköz, sürgősségi riasztószolgáltatás vagy alvási fázis-követő. Egyetlen riasztóalkalmazás sem garantálhatja a felébredést vagy nem kompenzálhat a nem elérhető készülékért. A [tények és korlátok oldal](../facts.md) felsorolja ezeket a határokat, míg a [rendelkezésre állás](../availability.md) elkülöníti a nyilvános áruház bizonyítékait az újabb forrásképességektől.

