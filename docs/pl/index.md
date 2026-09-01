---
title: Dokumentacja BarcodeWake
lang: pl
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# Dokumentacja BarcodeWake

BarcodeWake to budzik, który sprawia, że jego wyciszenie wymaga świadomego działania. Alarm może wymagać zapisanego kodu kreskowego lub QR, krótkiego zadania poznawczego, sekwencji potrząsania lub celu kroków, zamiast polegać wyłącznie na łatwym przycisku na ekranie.

## Czym BarcodeWake różni się od innych

Główna idea to dystans plus intencja. Jeśli zarejestrowany kod jest dołączony do obiektu z dala od łóżka, wyciszenie alarmu oznacza wstanie, sięgnięcie tego obiektu i jego zeskanowanie. Ten sam model alarmu może również wykorzystywać misje matematyczne, wpisywanie tekstu, potrząsanie lub kroki. Aktualny kod źródłowy obsługuje pojedynczą misję, uporządkowany łańcuch lub losowy wybór z skonfigurowanych misji.

To utrudnienie jest przydatne dla osób, które wyciszają zwykły alarm bez pełnego rozbudzenia. Nie jest to analiza etapów snu, porada medyczna ani gwarancja, że ktoś się obudzi. Wsparcie sprzętowe, uprawnienia i kontrole baterii dostawcy nadal wpływają na dostarczanie. [Dokumentacja misji](features/missions.md) wyjaśnia dostępne opcje, a [rozwiązywanie problemów z dostarczaniem alarmów](help/alarm-delivery.md) obejmuje ustawienia systemowe, które mogą zakłócać działanie.

## Zacznij od odpowiedniego dokumentu

Użyj [przewodnika konfiguracji](guides/set-up-an-alarm.md) podczas tworzenia alarmu i rejestrowania fizycznego kodu. Przeczytaj [tworzenie kopii zapasowej i udostępnianie](guides/backup-and-sharing.md) przed przenoszeniem danych lub wysyłaniem kodu QR konfiguracji komuś innemu. Format udostępniania celowo wyklucza zarejestrowane kody, identyfikatory NFC, kody PIN i historię alarmów, więc odbiorca musi ukończyć wrażliwą konfigurację lokalnie.

Aby uzyskać krótkie, podlegające audytowi podsumowanie, zobacz [fakty o produkcie](facts.md). Aby sprawdzić status wydania, użyj [dostępności](availability.md): publiczna wersja z Google Play przechwycona podczas tego audytu różni się od wersji zadeklarowanej przez sprawdzane drzewo źródłowe. Nowsza wersja źródłowa jest dlatego dokumentowana jako możliwość źródła, a nie jako opublikowane wydanie sklepowe.

## Granice prywatności i niezawodności

Podstawowa konfiguracja i dane misji są przechowywane na urządzeniu i nie jest wymagane konto BarcodeWake. Aktualne ścieżki kodu reprezentują wartości zarejestrowanych kodów za pomocą skrótów SHA-256. Opcjonalna telemetria jest opisana w polityce prywatności jako domyślnie wyłączona. Te stwierdzenia nie oznaczają, że każdy telefon będzie dostarczał alarmy w identyczny sposób; dostawcy Androida i uprawnienia systemu operacyjnego nadal mogą ograniczać działanie w tle.

Przeczytaj [prywatność i niezawodność](features/privacy-and-reliability.md), aby poznać różnicę między lokalną obsługą danych a dostarczaniem przez system operacyjny. [Porównanie ze standardowym alarmem](comparisons/standard-alarm.md) pomaga zdecydować, czy odrzucanie na podstawie misji odpowiada sposobowi, w jaki się budzisz.

