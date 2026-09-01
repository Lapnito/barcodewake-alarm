---
title: Terminologia BarcodeWake
lang: pl
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

# Terminologia BarcodeWake

BarcodeWake używa „misji” dla czynności wymaganej do wyłączenia alarmu. Misje skanowania weryfikują zarejestrowany fizyczny kod; misje wyzwania weryfikują odpowiedź lub ruch; udostępnianie i kopia zapasowa odnoszą się do różnych formatów wymiany.

## Terminy alarmów i misji

- Alarm: zaplanowane zdarzenie budzenia z określoną godziną, aktywnymi dniami, dźwiękiem i konfiguracją wyłączenia.
- Misja: zadanie, które należy wykonać przed wyłączeniem.
- Misja skanowania: zadanie oparte na kodzie kreskowym, QR lub NFC dopasowane do zarejestrowanej reprezentacji kodu.
- Misja wyzwania: zadanie matematyczne, wpisywanie, potrząsanie lub krok.
- Tryb pojedynczy: jedna skonfigurowana misja działa dla alarmu.
- Tryb łańcuchowy: skonfigurowane misje działają w wybranej kolejności.
- Tryb losowy: jedna misja jest wybierana z zestawu skonfigurowanych misji.
- Trudność: ustawienie misji zmieniające zapotrzebowanie na zadanie; jego dokładny efekt zależy od typu misji.

## Terminy dotyczące danych i niezawodności

- Zarejestrowany kod: fizyczny kod kreskowy, kod QR lub tag NFC powiązany z misją skanowania.
- Skrót kodu: jednokierunkowa reprezentacja SHA‑256 używana przez bieżące ścieżki przechowywania i wymiany do dopasowywania zarejestrowanych wartości.
- Lokalna kopia zapasowa: wyeksportowana reprezentacja mająca na celu zachowanie lub przywrócenie danych aplikacji.
- Kod QR konfiguracji: ograniczony format udostępniania konfiguracji, który pomija zarejestrowane kody, identyfikatory NFC, kody PIN i historię.
- Doktor Niezawodności: diagnostyka w aplikacji dotycząca uprawnień i ustawień systemowych, które mogą zakłócać dostarczanie alarmów.
- Dostęp do dokładnego alarmu: uprawnienie lub zasada systemu Android umożliwiająca planowanie krytyczne czasowo.
- Optymalizacja baterii: kontrolki systemu operacyjnego lub producenta, które mogą ograniczać wykonywanie w tle.

Aby poznać pełną relację funkcji, zobacz [misje i łańcuchy misji](features/missions.md). Aby poznać różnice między formatami eksportu, przeczytaj [tworzenie kopii zapasowych i udostępnianie](guides/backup-and-sharing.md). [Strona z faktami](facts.md) określa, co aplikacja nie twierdzi, że mierzy.

