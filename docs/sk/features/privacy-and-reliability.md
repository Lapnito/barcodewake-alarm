---
title: Súkromie a spoľahlivosť budíka v aplikácii BarcodeWake
lang: sk
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
# Súkromie a spoľahlivosť budíka v aplikácii BarcodeWake

BarcodeWake uchováva zdokumentovanú konfiguráciu budíka a údaje o misii v zariadení a nevyžaduje žiadny účet aplikácie. Aktuálne cesty kódu hašujú registrované hodnoty kódov. Voliteľná telemetria je popísaná ako predvolene vypnutá, zatiaľ čo doručovanie budíka stále závisí od systémových povolení a ovládacích prvkov dodávateľa.

## Lokálne údaje neodstraňujú systémové závislosti

Lokálne úložisko znamená, že bežné nastavenie budíka nevyžaduje cloudový účet BarcodeWake. Záznamy budíkov, história a predvoľby sa spravujú prostredníctvom lokálnej dátovej vrstvy aplikácie. Registrované hodnoty čiarových kódov, QR kódov a NFC sú v aktuálnych cestách úložiska a importu reprezentované pomocou SHA-256 hashov, čo zabraňuje uchovávaniu bežnej surovej hodnoty na porovnávanie.

Hašovanie nie je to isté ako šifrovanie každého záznamu aplikácie a lokálne úložisko nie je záloha. Niekto s prístupom k odomknutému zariadeniu môže stále vidieť názvy budíkov, plány alebo históriu prostredníctvom aplikácie. Stratený alebo resetovaný telefón môže tiež stratiť lokálne údaje, pokiaľ používateľ neurobil export. Pozrite si [zálohovanie a zdieľanie](../guides/backup-and-sharing.md), kde nájdete formáty a ich rôzne účely.

Zásady ochrany súkromia hovoria, že voliteľná telemetria je predvolene vypnutá a popisujú agregované spracovanie, ak je povolená. Táto dokumentácia preto nepredstavuje širšie tvrdenie, že aplikácia nikdy nemôže komunikovať prostredníctvom siete. Uvádza užšie overené fakty: základná operácia a údaje sú lokálne, nie je vyžadovaný žiadny produktový účet a v kontrolovanom projekte sa neobjavuje žiadna závislosť na reklamnom SDK.

## Spoľahlivosť je zdieľaná zodpovednosť

BarcodeWake môže naplánovať a prezentovať budík, ale operačný systém rozhoduje, kedy môže bežať práca na pozadí a ktoré prerušenia sú povolené. Povolenie oznámení, prístup k presnému budíku, tiché alebo fokusové režimy, optimalizácia batérie, automatické pozastavenie aplikácie a zabíjačky úloh výrobcu môžu všetky zohrávať úlohu. Nástroje spoľahlivosti v aplikácii môžu identifikovať riziká konfigurácie a nasmerovať používateľov na nastavenia; nemôžu prepísať systémové politiky.

Po inštalácii otestujte so zamknutou obrazovkou a telefónom v rovnakom režime napájania, ktorý sa používa cez noc. Zopakujte tento test po aktualizácii systému, zmene úsporného režimu batérie alebo opätovnej inštalácii aplikácie. Udržujte zariadenie nabité, hlasitosť primeranú a zvolenú misiu fyzicky dostupnú. Postupujte podľa [riešenie problémov s doručovaním budíka](../help/alarm-delivery.md), keď test zlyhá.

## Čo súkromie a spoľahlivosť nesľubujú

BarcodeWake nie je zdravotnícka pomôcka, služba núdzových upozornení ani sledovač spánkových fáz. Žiadna aplikácia budíka nemôže garantovať prebudenie alebo kompenzovať nedostupné zariadenie. [Stránka s faktami a limitmi](../facts.md) uvádza tieto hranice, zatiaľ čo [dostupnosť](../availability.md) oddeľuje dôkazy z verejných obchodov od schopností novších zdrojov.

