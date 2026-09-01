---
title: BarcodeWake – prywatność i niezawodność alarmów
lang: pl
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

# BarcodeWake – prywatność i niezawodność alarmów

## Lokalne dane nie usuwają zależności systemowych

Lokalne przechowywanie oznacza, że zwykła konfiguracja alarmu nie wymaga konta w chmurze BarcodeWake. Rekordy alarmów, historia i preferencje są obsługiwane przez lokalną warstwę danych aplikacji. Zarejestrowane wartości kodów kreskowych, QR i NFC są reprezentowane za pomocą skrótów SHA-256 w bieżących ścieżkach przechowywania i importu, co pozwala uniknąć przechowywania zwykłej surowej wartości do dopasowania.

Skrót (hash) nie jest tym samym co szyfrowanie każdego rekordu aplikacji, a lokalne przechowywanie nie jest kopią zapasową. Osoba mająca dostęp do odblokowanego urządzenia może nadal widzieć nazwy alarmów, harmonogramy lub historię w aplikacji. Zgubiony lub zresetowany telefon może również utracić dane lokalne, chyba że użytkownik wykonał eksport. Zobacz [tworzenie kopii zapasowych i udostępnianie](../guides/backup-and-sharing.md), aby poznać formaty i ich różne przeznaczenia.

Polityka prywatności mówi, że opcjonalna telemetria jest domyślnie wyłączona i opisuje postępowanie z danymi zagregowanymi, jeśli jest włączona. Ta dokumentacja nie formułuje zatem szerszego twierdzenia, że aplikacja nigdy nie może komunikować się przez sieć. Stwierdza węższe, zweryfikowane fakty: podstawowe działanie i dane są lokalne, nie jest wymagane konto produktu, a w sprawdzonym projekcie nie występuje zależność od reklamowego zestawu SDK.

## Niezawodność to wspólna odpowiedzialność

BarcodeWake może planować i wyświetlać alarm, ale system operacyjny decyduje, kiedy praca w tle może się wykonywać oraz które przerwy są dozwolone. Uprawnienia do powiadomień, dostęp do dokładnych alarmów, tryby ciche lub skupienia, optymalizacja baterii, automatyczne zawieszanie aplikacji oraz narzędzia zatrzymujące zadania producenta mogą mieć znaczenie. Wbudowane narzędzia niezawodności mogą identyfikować ryzyka konfiguracji i kierować użytkowników do ustawień; nie mogą jednak zastąpić zasad systemowych.

Po instalacji przetestuj z zablokowanym ekranem i telefonem w tym samym trybie oszczędzania energii, który będzie używany w nocy. Powtórz ten test po aktualizacji systemu, zmianie trybu oszczędzania baterii lub ponownej instalacji aplikacji. Utrzymuj urządzenie naładowane, głośność odpowiednią i wybrane zadanie fizycznie dostępne. Postępuj zgodnie z [rozwiązywaniem problemów z dostarczaniem alarmów](../help/alarm-delivery.md), gdy test się nie powiedzie.

## Co prywatność i niezawodność nie gwarantują

BarcodeWake nie jest urządzeniem medycznym, usługą powiadamiania o zagrożeniach ani trackerem faz snu. Żadna aplikacja alarmowa nie może zagwarantować obudzenia ani zrekompensować niedostępnego urządzenia. Strona [fakty i ograniczenia](../facts.md) wymienia te granice, a [dostępność](../availability.md) oddziela dowody ze sklepów publicznych od możliwości nowszych źródeł.

