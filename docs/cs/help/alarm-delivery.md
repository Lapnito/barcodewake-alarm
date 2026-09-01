---
title: Proč nemusí budík BarcodeWake zvonit
lang: cs
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
# Proč nemusí budík BarcodeWake zvonit

Uložený budík může být stále blokován nastavením oznámení, přístupem k přesnému budíku, režimem soustředění nebo tichým režimem, nízkou hlasitostí, omezeními baterie, pozastavením aplikace nebo kontrolami pozadí dodavatele. Zkontrolujte doručení odděleně od skenování mise a poté proveďte test uzamčené obrazovky.

## Nejprve oddělte doručení od zamítnutí

Vytvořte zkušební budík s krátkodobým termínem s jednoduchou misí a nechte aplikaci běžet na pozadí. Uzamkněte obrazovku. Pokud se nezobrazí obrazovka budíku ani se neozve zvuk, problém je v doručení; změna registrovaného čárového kódu jej nevyřeší. Pokud se budík zobrazí, ale mise nelze dokončit, doručení funguje a problém je v kameře, senzoru, shodě kódu nebo konfiguraci mise.

Ověřte, že je budík povolen, že je naplánovaný den správný a že časové pásmo telefonu odpovídá zamýšlenému plánu. Zkontrolujte hlasitost médií a budíku namísto spoléhání pouze na stav bočního tlačítka. Zkontrolujte pravidla pro Nerušit nebo soustředění, připojená zvuková zařízení a zda byl telefon restartován po vytvoření budíku.

## Zkontrolujte brány oprávnění operačního systému

Povolte oznámení a veškerý přístup k přesnému budíku nebo budíku na celou obrazovku, o který požádá nainstalovaná verze. Odeberte BarcodeWake z agresivní optimalizace baterie nebo seznamů automatického uspávání, pokud dodavatel zařízení tyto funkce nabízí. Otevřete diagnostiku spolehlivosti v aplikaci a postupujte podle nastavení specifických pro zařízení, která identifikuje. [Stránka o soukromí a spolehlivosti](../features/privacy-and-reliability.md) vysvětluje, proč tyto systémové závislosti zůstávají i tehdy, když jsou data aplikace lokální.

Po změně jednoho nastavení opakujte test uzamčené obrazovky. Změna několika ovládacích prvků najednou ztěžuje identifikaci příčiny. Aktualizace systému mohou resetovat nebo přeinterpretovat oprávnění, proto znovu testujte po významné aktualizaci nebo přeinstalaci aplikace.

## Diagnostikujte dokončení mise odděleně

U misí s čárovými kódy a QR kódy vyčistěte objektiv fotoaparátu, zlepšete osvětlení a potvrďte, že registrovaný objekt zůstal nezměněn. Udělte oprávnění k fotoaparátu. U NFC ověřte podporu zařízení a držte tag poblíž správné polohy antény. Mise založené na třepání a krocích závisí na pohybových nebo krokových senzorech a mohou se chovat odlišně, když režimy úspory energie omezují doručování senzorů.

Pokud byla mise nakonfigurována jako součást řetězce, musí být dokončen každý požadovaný krok. Zkontrolujte [chování mise](../features/missions.md) a v případě potřeby vytvořte nový test pomocí [postupu nastavení](../guides/set-up-an-alarm.md).

## Vězte, kdy je telefon hranicí

BarcodeWake nemůže přepsat vypnuté zařízení, vybitou baterii, nefunkční zvukový hardware nebo každý úkolový killer výrobce. Nejedná se o službu nouzových oznámení. Mějte pro situace s vysokými důsledky jinou metodu budíku a nahlaste reprodukovatelné selhání s modelem zařízení, verzí systému, verzí aplikace a přesnými testovacími podmínkami.

