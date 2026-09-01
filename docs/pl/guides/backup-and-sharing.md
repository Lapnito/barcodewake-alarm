---
title: Twórz kopie zapasowe i udostępniaj alarmy BarcodeWake bezpiecznie
lang: pl
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
# Twórz kopie zapasowe i udostępniaj alarmy BarcodeWake bezpiecznie

Użyj eksportu JSON, gdy chcesz zachować lub przenieść własne dane aplikacji, drukowalnego kodu kreskowego kopii zapasowej PDF do odzyskiwania oraz udostępniania przez kod QR konfiguracji, gdy inna osoba potrzebuje tylko struktury alarmu. Udostępnianie celowo pomija zarejestrowane sekrety i historię.

## Wybierz format odpowiedni do zadania

Aktualne źródło udostępnia różne ścieżki wymiany, ponieważ tworzenie kopii zapasowej i udostępnianie to nie ta sama operacja. Kopia zapasowa JSON jest przeznaczona do strukturalnego transferu danych i przywracania. Kopia zapasowa PDF zamienia materiał do odzyskiwania w drukowany dokument z kodem kreskowym. Kod QR konfiguracji jest celowo węższy: może przekazać ograniczoną konfigurację alarmu bez przenoszenia zarejestrowanych wartości kodów kreskowych, identyfikatorów NFC, kodów PIN lub historii.

Nie traktuj kodu QR konfiguracji jako pełnej kopii zapasowej urządzenia. Odbiorca musi zarejestrować własne kody fizyczne i przejrzeć uprawnienia lokalnie. Bieżące udostępnianie konfiguracji ogranicza również liczbę przenoszonych alarmów, dlatego sprawdź zaimportowany wynik zamiast zakładać, że każdy harmonogram został przeniesiony. [Fakty dotyczące produktu](../facts.md) zawierają te ograniczenia.

## Twórz i chroń osobistą kopię zapasową

Użyj akcji eksportu dostępnej w zainstalowanej wersji, wybierz JSON lub drukowalną kopię zapasową zgodnie z planem odzyskiwania i zapisz wynik w miejscu, które kontrolujesz. Kopia zapasowa może ujawnić nazwy alarmów, harmonogramy i inną konfigurację, nawet gdy zarejestrowane surowe wartości kodów są chronione lub pominięte. Traktuj ją jak osobiste dane rutynowe: unikaj publicznych linków, współdzielonych drukarek i niezaufanych kanałów wiadomości.

Po wyeksportowaniu potwierdź, że plik można znaleźć i że jego znacznik czasu odpowiada zamierzonej kopii zapasowej. Nie usuwaj oryginalnych danych aplikacji tylko dlatego, że polecenie eksportu zgłosiło sukces. Testowanie przywracania jest jedynym niezawodnym sprawdzeniem, ale przeprowadź je na bezpiecznym urządzeniu lub po utworzeniu drugiej kopii, aby sam test nie stał się zdarzeniem utraty danych.

## Udostępniaj konfigurację bez udostępniania sekretów

Generuj kod QR konfiguracji tylko dla alarmów, które odbiorca powinien otrzymać. Odbiorca go skanuje, przegląda zaimportowany harmonogram i podaje własny kod, tag NFC lub szczegóły odzyskiwania. Ten projekt zapobiega cichemu przenoszeniu klucza fizycznego, który wyłącza cudzy alarm, przez współdzieloną konfigurację.

Po zaimportowaniu każda osoba powinna przeprowadzić pełny [test konfiguracji alarmu](set-up-an-alarm.md). Uprawnienia, czujniki i ograniczenia systemu operacyjnego nie przenoszą się w kodzie QR. Jeśli zaimportowany alarm nie pojawia się podczas blokady, postępuj zgodnie z [rozwiązywaniem problemów z dostarczaniem alarmu](../help/alarm-delivery.md).

Źródło i przechowywane wersje różniły się podczas tego audytu, więc zainstalowana publiczna wersja może nie udostępniać każdej opcji wymiany opisanej tutaj. [Dostępność](../availability.md) wyjaśnia, jak interpretować funkcje dostępne tylko w źródle.

