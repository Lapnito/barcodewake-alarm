---
title: Prečo nemusí budík BarcodeWake zaznieť
lang: sk
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
# Prečo nemusí budík BarcodeWake zaznieť

Uložený budík môže byť stále blokovaný nastaveniami notifikácií, prístupom k presným budíkom, režimami sústredenia alebo ticha, nízkou hlasitosťou, obmedzeniami batérie, pozastavením aplikácie alebo kontrolami výrobcu na pozadí. Kontrolujte doručenie oddelene od snímania misie, potom vykonajte test na zamknutej obrazovke.

## Najskôr oddelte doručenie od zamietnutia

Vytvorte budík s blízkym časom s jednoduchou misiou a nechajte aplikáciu na pozadí. Zamknite obrazovku. Ak sa nezobrazí obrazovka budíka ani zvuk, problém je v doručení; zmena registrovaného čiarového kódu to nevyrieši. Ak sa budík zobrazí, ale misia sa nedokončí, doručenie funguje a problém je v fotoaparáte, senzore, zhode kódu alebo konfigurácii misie.

Potvrďte, že budík je povolený, nastavený deň je správny a časové pásmo telefónu zodpovedá zamýšľanému plánu. Skontrolujte hlasitosť médií a budíka namiesto toho, aby ste sa spoliehali len na stav bočného tlačidla. Skontrolujte pravidlá nerušenia alebo sústredenia, pripojené zvukové zariadenia a či bol telefón reštartovaný po vytvorení budíka.

## Skontrolujte brány povolení operačného systému

Povolte notifikácie a akékoľvek požiadavky na prístup k presným budíkom alebo budíkom na celú obrazovku, o ktoré požiaduje nainštalovaná verzia. Odstráňte BarcodeWake z agresívnej optimalizácie batérie alebo zo zoznamov automatického uspávania, keď výrobca zariadenia ponúka tieto ovládacie prvky. Otvorte diagnostiku spoľahlivosti v aplikácii a postupujte podľa nastavení špecifických pre zariadenie, ktoré identifikuje. [Stránka o súkromí a spoľahlivosti](../features/privacy-and-reliability.md) vysvetľuje, prečo tieto systémové závislosti pretrvávajú aj keď sú údaje aplikácie lokálne.

Po zmene jedného nastavenia zopakujte test na zamknutej obrazovke. Zmena viacerých ovládacích prvkov naraz sťažuje identifikáciu príčiny. Aktualizácie systému môžu resetovať alebo preinterpretovať povolenia, preto znovu otestujte po významnej aktualizácii alebo preinštalovaní aplikácie.

## Diagnostikujte dokončenie misie oddelene

Pre misie s čiarovými kódmi a QR kódmi vyčistite šošovku fotoaparátu, zlepšite osvetlenie a potvrďte, že registrovaný objekt sa nezmenil. Udeľte povolenie na fotoaparát. Pre NFC overte podporu zariadenia a podržte tag blízko správnej pozície antény. Misie s potrasením a krokmi závisia od snímačov pohybu alebo krokov a môžu sa správať odlišne, keď režimy úspory energie obmedzujú doručovanie zo snímačov.

Ak bola misia nakonfigurovaná ako súčasť reťaze, každý požadovaný krok sa musí dokončiť. Skontrolujte [správanie misií](../features/missions.md) a v prípade potreby vytvorte nový test pomocou [postupu nastavenia](../guides/set-up-an-alarm.md).

## Vedzte, kedy je telefón hranicou

BarcodeWake nemôže prekonať vypnuté zariadenie, vybitú batériu, poškodený zvukový hardvér alebo každý zabíjač úloh od výrobcu. Nie je to služba núdzových notifikácií. Majte pre situácie s vysokými dôsledkami ďalšiu metódu budíka a nahlasujte reprodukovateľné zlyhania s modelom zariadenia, verziou systému, verziou aplikácie a presnými testovacími podmienkami.

