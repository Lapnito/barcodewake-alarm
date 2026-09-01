---
title: Készítsen biztonsági másolatot és ossza meg a BarcodeWake riasztásokat biztonságosan
lang: hu
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# Készítsen biztonsági másolatot és ossza meg a BarcodeWake riasztásokat biztonságosan

Használjon JSON exportot a saját alkalmazásadatok megőrzésekor vagy áthelyezésekor, nyomtatható PDF biztonsági másolatot vonalkód formájában a helyreállításhoz, és beállítási QR megosztást, amikor egy másik személynek csak a riasztási struktúrára van szüksége. A megosztás szándékosan kihagyja a regisztrált titkokat és az előzményeket.

## Válassza ki a feladathoz megfelelő formátumot

A jelenlegi forrás különböző csereutakat biztosít, mert a biztonsági mentés és a megosztás nem ugyanaz a művelet. A JSON biztonsági másolat strukturált adatátvitelre és helyreállításra szolgál. A PDF biztonsági másolat a helyreállítási anyagot nyomtatható vonalkód dokumentummá alakítja. A beállítási QR szándékosan szűkebb: korlátozott riasztási konfigurációt tud átadni a regisztrált vonalkód értékek, NFC azonosítók, PIN-kódok vagy előzmények nélkül.

Ne kezelje a beállítási QR-t teljes eszköz biztonsági mentésként. A címzettnek regisztrálnia kell a saját fizikai kódjait és helyben felül kell vizsgálnia az engedélyeket. A jelenlegi beállítási megosztás korlátozza a hány riasztást tud hordozni, ezért ellenőrizze az importált eredményt ahelyett, hogy feltételezné, hogy minden ütemezés átkerült. A [termék tények](../facts.md) ezeket a határokat rögzíti.

## Hozza létre és védje meg a személyes biztonsági másolatot

Használja a telepített buildben elérhető export műveletet, válassza a JSON-t vagy a nyomtatható biztonsági mentést a helyreállítási terv szerint, és mentse az eredményt olyan helyre, amelyet Ön irányít. A biztonsági másolat felfedheti a riasztási neveket, ütemezéseket és egyéb konfigurációkat, még akkor is, ha a regisztrált nyers kód értékek védettek vagy kihagyásra kerülnek. Kezelje személyes rutin adatként: kerülje a nyilvános linkeket, megosztott nyomtatókat és nem megbízható üzenetküldő csatornákat.

Az exportálás után erősítse meg, hogy a fájl megtalálható és időbélyege megfelel a szándékolt biztonsági másolatnak. Ne törölje az eredeti alkalmazás adatokat csak azért, mert egy export parancs sikeresnek jelentette magát. A visszaállítási teszt az egyetlen megbízható ellenőrzés, de végezze el biztonságos eszközön vagy másolat készítése után, hogy a teszt maga ne váljon elvesztési eseménnyé.

## Ossza meg a beállítást titkok megosztása nélkül

Generáljon beállítási QR-t csak azokhoz a riasztásokhoz, amelyeket a címzett meg kell kapnia. A címzett beolvassa, áttekinti az importált ütemezést és megadja a saját kódját, NFC címkéjét vagy helyreállítási adatait. Ez a kialakítás megakadályozza, hogy egy megosztott konfiguráció csendben átvigye azt a fizikai kulcsot, amely elhallgattatja valaki más riasztását.

Az import után minden személynek futtatnia kell a teljes [riasztás beállítási tesztet](set-up-an-alarm.md). Az engedélyek, érzékelők és operációs rendszer korlátozások nem kerülnek át a QR-ben. Ha egy importált riasztás nem jelenik meg zárolás közben, kövesse a [riasztás kézbesítési hibaelhárítást](../help/alarm-delivery.md).

A forrás és a tárolt verziók eltértek ebben a felülvizsgálatban, ezért egy telepített nyilvános build nem biztos, hogy minden itt leírt csereopciót felfed. A [Elérhetőség](../availability.md) elmagyarázza, hogyan értelmezze a csak forrásban elérhető képességeket.

