---
title: Ako nastaviť alarm BarcodeWake
lang: sk
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
# Ako nastaviť alarm BarcodeWake

Najprv vytvorte plán, vyberte misiu, ktorá je bezpečná a praktická, udelte potrebné povolenia a potom vykonajte krátkodobý test so zamknutou obrazovkou. Pri skenovacích misiách zaregistrujte trvanlivý objekt, ktorý bude k dispozícii a čitateľný, keď alarm zazvoní.

## Vyberte misiu pred objektom

Rozhodnite sa, aká akcia by mala oddeliť vstávanie od odmietnutia. Čiarový kód v inej miestnosti vytvára fyzickú vzdialenosť. Matematika alebo písanie pridáva sústredenie bez potreby fotoaparátu. Potrasenie alebo kroky pridávajú pohyb, ale závisia od senzorov a nemusia vyhovovať každému človeku alebo prostrediu. [Referencia misií](../features/missions.md) vysvetľuje kompromisy medzi jednotlivými, reťazovými a náhodnými režimami.

Ak používate čiarový kód, QR kód alebo NFC štítok, vyberte niečo trvanlivé. Vyhnite sa jednorazovému baleniu, objektu, ktorý môže presunúť iný člen domácnosti, alebo kódu, ktorý bude nedostupný počas cestovania. Skontrolujte, či môže fotoaparát zaostriť pri očakávanom osvetlení. NFC potrebuje kompatibilný telefón a štítok.

## Konfigurujte plán a pravidlo odmietnutia

Otvorte editor alarmov, nastavte požadovaný čas a aktívne dni a potom vyberte misiu zobrazenú nainštalovanou verziou. Pri prvom teste nakonfigurujte jej obtiažnosť alebo cieľ konzervatívne. Ak nainštalovaná verzia podporuje reťaze, usporiadajte misie v poradí, ktoré je možné bezpečne dokončiť bez naháňania sa po schodoch alebo opúšťania bezpečnej oblasti.

Zaregistrujte fyzický kód z nastavenia misie. Dajte alarmu štítok, ktorý identifikuje zamýšľanú rutinu, namiesto odhaľovania citlivých informácií. Skontrolujte hlasitosť, vibrácie a všetky možnosti sledovania prebudenia viditeľné v nainštalovanej verzii. Dostupné ovládacie prvky sa môžu líšiť, pretože [verejná a zdrojová verzia](../availability.md) neboli v deň auditu identické.

## Udeľte povolenia s účelom

Povolte notifikácie a prístup súvisiaci s alarmom potrebný na doručenie. Udeľte prístup k fotoaparátu len pri použití skenovacej misie a prístup k senzorom, keď to zvolená misia potrebuje. V systéme Android skontrolujte nastavenia presného alarmu a batérie, ak ich aplikácia označí. Nepredpokladajte, že uloženie alarmu dokazuje, že doručovanie na pozadí je povolené.

## Otestujte celú nočnú cestu

Nastavte test o niekoľko minút dopredu. Zamknite obrazovku, nechajte BarcodeWake v pozadí a vložte telefón do rovnakého zvukového a napájacieho stavu plánovaného na noc. Potvrďte, že sa alarm zobrazí, zvuk je počuť a presne zvolenú misiu je možné dokončiť. Potom zopakujte po presune zaregistrovaného objektu na jeho skutočné miesto.

Ak doručenie zlyhá, použite [kontrolný zoznam doručenia alarmov](../help/alarm-delivery.md). Ak je úspešné, zvážte vytvorenie [miestnej zálohy](backup-and-sharing.md) po stabilizácii nastavenia.

