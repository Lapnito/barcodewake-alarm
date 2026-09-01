---
title: BarcodeWake terminológia
lang: hu
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---
# BarcodeWake terminológia

A BarcodeWake a „küldetés" kifejezést használja az ébresztő elhallgattatásához szükséges műveletre. A szkennelési küldetések egy regisztrált fizikai kódot ellenőriznek; a kihívás küldetések egy válasz vagy mozgás ellenőrzését végzik; a megosztás és a biztonsági mentés különböző csereformátumokat jelentenek.

## Ébresztő és küldetés kifejezések

- Ébresztő: egy ütemezett ébresztési esemény időponttal, aktív napokkal, hanggal és elutasítási beállításokkal.
- Küldetés: a feladat, amelyet az elutasítás előtt el kell végezni.
- Szkennelési küldetés: egy vonalkód, QR vagy NFC alapú feladat, amelyet egy regisztrált kódábrázoláshoz illesztenek.
- Kihívás küldetés: egy matematikai, gépelési, rázás vagy lépés feladat.
- Egyszerű mód: egy beállított küldetés fut az ébresztőhöz.
- Lánc mód: a beállított küldetések kiválasztott sorrendben futnak.
- Véletlen mód: egy küldetést választanak ki a beállított halmazból.
- Nehézség: egy küldetés beállítás, amely megváltoztatja a feladat igényességét; pontos hatása a küldetés típusától függ.

## Adat- és megbízhatósági kifejezések

- Regisztrált kód: a fizikai vonalkód, QR kód vagy NFC címke, amely egy szkennelési küldetéshez van társítva.
- Kód hash: egy egyirányú SHA-256 ábrázolás, amelyet a jelenlegi tárolási és csereutak a regisztrált értékek összehasonlításához használnak.
- Helyi biztonsági mentés: egy exportált ábrázolás, amely az alkalmazás adatainak megőrzésére vagy visszaállítására szolgál.
- Beállítási QR: egy korlátozott konfiguráció-megosztási formátum, amely kihagyja a regisztrált kódokat, NFC azonosítókat, PIN-eket és előzményeket.
- Megbízhatósági doktor: alkalmazáson belüli diagnosztika az engedélyekhez és rendszerbeállításokhoz, amelyek befolyásolhatják az ébresztés kézbesítését.
- Pontos ébresztés hozzáférés: Android rendszer engedély vagy házirend, amely időkritikus ütemezést tesz lehetővé.
- Akkumulátor optimalizálás: operációs rendszer vagy gyártó általi vezérlések, amelyek korlátozhatják a háttérbeli végrehajtást.

A teljes funkciókapcsolatért lásd a [küldetések és küldetési láncok](features/missions.md) oldalt. Az export formátumok közötti különbségekért olvassa el a [biztonsági mentés és megosztás](guides/backup-and-sharing.md) útmutatót. A [tények oldal](facts.md) meghatározza, hogy az alkalmazás mit nem állít mérni.

