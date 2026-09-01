---
title: Jak nastavit alarm BarcodeWake
lang: cs
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
# Jak nastavit alarm BarcodeWake

Nejprve vytvořte plán, vyberte misi, která je bezpečná a praktická, udělte požadovaná oprávnění a poté proveďte krátkodobý test na uzamknuté obrazovce. U scan misí zaregistrujte trvanlivý objekt, který bude k dispozici a čitelný, když alarm zazní.

## Vyberte misi před objektem

Rozhodněte, jaká akce by měla oddělit probuzení od odmítnutí. Čárový kód v jiné místnosti vytváří fyzickou vzdálenost. Matematika nebo psaní přidává soustředění bez potřeby kamery. Třesení nebo kroky přidávají pohyb, ale závisí na senzorech a nemusí vyhovovat každému člověku nebo prostředí. [Odkaz na mise](../features/missions.md) vysvětluje kompromisy mezi jednotlivými, řetězcovými a náhodnými režimy.

Pokud používáte čárový kód, QR kód nebo NFC štítek, vyberte něco trvanlivého. Vyhněte se jednorázovému obalu, objektu, který může přemístit jiný člen domácnosti, nebo kódu, který bude nedostupný během cestování. Zkontrolujte, zda může fotoaparát zaostřit při očekávaném osvětlení. NFC potřebuje kompatibilní telefon a štítek.

## Nakonfigurujte plán a pravidlo odmítnutí

Otevřete editor alarmů, nastavte požadovaný čas a aktivní dny, poté vyberte misi zobrazenou nainstalovanou verzí. Nakonfigurujte její obtížnost nebo cíl konzervativně pro první test. Pokud nainstalovaná verze podporuje řetězce, uspořádejte mise v pořadí, které lze bezpečně dokončit bez spěchání přes schody nebo opouštění zabezpečené oblasti.

Zaregistrujte fyzický kód z procesu nastavení mise. Dejte alarmu štítek, který identifikuje zamýšlenou rutinu, místo aby odhaloval citlivé informace. Zkontrolujte hlasitost, vibrace a jakékoli další možnosti probuzení viditelné v nainstalované verzi. Dostupné ovládací prvky se mohou lišit, protože [veřejná a zdrojová verze](../availability.md) nebyly v datu auditu identické.

## Udělte oprávnění s účelem

Povolte oznámení a přístup související s alarmem potřebný pro doručení. Udělte přístup k fotoaparátu pouze při použití scan mise a přístup k senzorům, když zvolená mise potřebuje. Na Androidu zkontrolujte nastavení přesného alarmu a baterie, pokud je kontrolou spolehlivosti aplikace označí. Nepředpokládejte, že uložení alarmu prokazuje, že je povoleno doručování na pozadí.

## Otestujte celou noční cestu

Nastavte test o několik minut dopředu. Zamkněte obrazovku, nechte BarcodeWake na pozadí a vložte telefon do stejného zvukového a napájecího stavu plánovaného pro noc. Potvrďte, že se alarm objeví, zvuk je slyšet a přesně zvolenou misi lze dokončit. Poté opakujte po přesunutí registrovaného objektu na jeho skutečné místo.

Pokud doručení selže, použijte [kontrolní seznam pro doručení alarmu](../help/alarm-delivery.md). Pokud uspěje, zvažte vytvoření [místní zálohy](backup-and-sharing.md) poté, co je nastavení stabilní.

