---
title: Dlaczego alarm BarcodeWake może nie dzwonić
lang: pl
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

# Dlaczego alarm BarcodeWake może nie dzwonić

Zapisany alarm może nadal być blokowany przez ustawienia powiadomień, dostęp do dokładnych alarmów, tryb skupienia lub tryb ciszy, niską głośność, ograniczenia baterii, wstrzymanie aplikacji lub mechanizmy kontroli w tle dostawcy. Sprawdź dostarczenie oddzielnie od skanowania misji, a następnie przeprowadź test z zablokowanym ekranem.

## Najpierw oddziel dostarczenie od odrzucenia

Utwórz alarm testowy na najbliższy termin z prostą misją i pozostaw aplikację w tle. Zablokuj ekran. Jeśli nie pojawi się ekran alarmu ani dźwięk, problem dotyczy dostarczenia; zmiana zarejestrowanego kodu kreskowego tego nie naprawi. Jeśli alarm się pojawia, ale misja nie może się zakończyć, dostarczenie działa, a problemem jest kamera, czujnik, dopasowanie kodu lub konfiguracja misji.

Potwierdź, że alarm jest włączony, zaplanowany dzień jest prawidłowy, a strefa czasowa telefonu odpowiada zamierzonemu harmonogramowi. Sprawdź głośność multimediów i alarmu zamiast polegać tylko na stanie przycisku bocznego. Przejrzyj reguły trybu nie przeszkadzać lub trybu skupienia, podłączone urządzenia audio oraz czy telefon został ponownie uruchomiony po utworzeniu alarmu.

## Przejrzyj uprawnienia systemu operacyjnego

Zezwól na powiadomienia oraz na dostęp do dokładnych alarmów lub pełnoekranowych alarmów wymagany przez zainstalowaną kompilację. Usuń BarcodeWake z agresywnej optymalizacji baterii lub automatycznych list uśpienia, gdy dostawca urządzenia oferuje takie funkcje. Otwórz diagnostykę niezawodności w aplikacji i postępuj zgodnie z ustawieniami specyficznymi dla urządzenia, które identyfikuje. Strona [prywatność i niezawodność](../features/privacy-and-reliability.md) wyjaśnia, dlaczego te zależności systemowe pozostają nawet wtedy, gdy dane aplikacji są lokalne.

Po zmianie jednego ustawienia powtórz test z zablokowanym ekranem. Zmiana kilku kontrol naraz utrudnia identyfikację przyczyny. Aktualizacje systemu mogą resetować lub reinterpretować uprawnienia, dlatego powtórz test po dużej aktualizacji lub ponownej instalacji aplikacji.

## Diagnozuj ukończenie misji oddzielnie

W przypadku misji z kodami kreskowymi i QR oczyść obiektyw aparatu, popraw oświetlenie i potwierdź, że zarejestrowany obiekt nie uległ zmianie. Przyznaj uprawnienia do aparatu. W przypadku NFC sprawdź obsługę urządzenia i przytrzymaj tag w pobliżu właściwej pozycji anteny. Misje wymagające potrząsania i kroków zależą od czujników ruchu lub kroków i mogą zachowywać się inaczej, gdy tryby oszczędzania energii ograniczają dostarczanie danych z czujników.

Jeśli misja została skonfigurowana jako część łańcucha, każdy wymagany krok musi zostać ukończony. Przejrzyj [zachowanie misji](../features/missions.md) i, jeśli to konieczne, utwórz nowy test korzystając z [procedury konfiguracji](../guides/set-up-an-alarm.md).

## Wiedz, kiedy telefon jest ograniczeniem

BarcodeWake nie może ominąć wyłączonego urządzenia, rozładowanej baterii, uszkodzonego sprzętu audio ani każdego menedżera zadań producenta. Nie jest to usługa powiadomień awaryjnych. Zachowaj inną metodę alarmu dla sytuacji o wysokich konsekwencjach i zgłaszaj powtarzalne błędy, podając model urządzenia, wersję systemu, wersję aplikacji oraz dokładne warunki testowe.

