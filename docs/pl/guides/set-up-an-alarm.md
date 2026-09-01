---
title: Jak skonfigurować alarm BarcodeWake
lang: pl
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
# Jak skonfigurować alarm BarcodeWake

Najpierw utwórz harmonogram, wybierz misję, która jest bezpieczna i praktyczna, przyznaj wymagane uprawnienia, a następnie przeprowadź test zablokowanego ekranu w najbliższym czasie. W przypadku misji skanowania zarejestruj trwały obiekt, który będzie dostępny i czytelny, gdy zadzwoni alarm.

## Wybierz misję przed obiektem

Zdecyduj, jakie działanie powinno rozdzielić budzenie od odrzucenia. Kod kreskowy w innym pokoju tworzy fizyczny dystans. Matematyka lub wpisywanie tekstu dodaje koncentracji bez konieczności korzystania z kamery. Wstrząs lub kroki dodają ruchu, ale zależą od czujników i mogą nie być odpowiednie dla każdej osoby lub środowiska. [Dokumentacja misji](../features/missions.md) wyjaśnia kompromisy między trybami pojedynczym, łańcuchowym i losowym.

Jeśli używasz kodu kreskowego, kodu QR lub tagu NFC, wybierz coś trwałego. Unikaj jednorazowych opakowań, obiektu, który może przemieścić inny domownik, lub kodu, który będzie niedostępny podczas podróży. Sprawdź, czy kamera może ustawić ostrość w spodziewanym oświetleniu. NFC wymaga kompatybilnego telefonu i tagu.

## Skonfiguruj harmonogram i regułę odrzucenia

Otwórz edytor alarmów, ustaw żądaną godzinę i aktywne dni, a następnie wybierz misję wyświetlaną przez zainstalowaną wersję. Skonfiguruj jej trudność lub cel konserwatywnie podczas pierwszego testu. Jeśli zainstalowana wersja obsługuje łańcuchy, ułóż misje w kolejności, którą można bezpiecznie ukończyć bez pośpiechu na schodach lub opuszczania bezpiecznego obszaru.

Zarejestruj fizyczny kod z przepływu konfiguracji misji. Nadaj alarmowi etykietę identyfikującą zamierzony harmonogram, a nie ujawniającą wrażliwe informacje. Sprawdź głośność, wibracje i opcje dalszych działań po przebudzeniu widoczne w zainstalowanej wersji. Dostępne elementy sterujące mogą się różnić, ponieważ [wersje publiczna i źródłowa](../availability.md) nie były identyczne w dacie audytu.

## Udziel uprawnień zgodnie z przeznaczeniem

Zezwól na powiadomienia i dostęp związany z alarmem wymagany do realizacji. Przyznaj dostęp do kamery tylko w przypadku korzystania z misji skanowania oraz dostęp do czujników, gdy wybrana misja tego wymaga. W systemie Android sprawdź ustawienia dokładnego alarmu i baterii, jeśli sprawdzanie niezawodności aplikacji je zasygnalizuje. Nie zakładaj, że zapisanie alarmu oznacza, że dostarczanie w tle jest dozwolone.

## Przetestuj całą ścieżkę nocną

Ustaw test na kilka minut do przodu. Zablokuj ekran, pozostaw BarcodeWake w tle i umieść telefon w tym samym stanie dźwięku i zasilania, który planujesz na noc. Potwierdź, że alarm się pojawia, dźwięk jest słyszalny i dokładnie wybrana misja może zostać ukończona. Następnie powtórz po przeniesieniu zarejestrowanego obiektu do jego rzeczywistej lokalizacji.

Jeśli dostarczenie się nie powiedzie, użyj [listy kontrolnej dostarczania alarmów](../help/alarm-delivery.md). Jeśli się powiedzie, rozważ wykonanie [lokalnej kopii zapasowej](backup-and-sharing.md) po ustabilizowaniu konfiguracji.

