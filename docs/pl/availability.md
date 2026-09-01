---
title: Dostępność i wersje BarcodeWake
lang: pl
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Dostępność i wersje BarcodeWake

BarcodeWake ma zweryfikowaną publiczną listę w Google Play dla systemu Android. Na dzień audytu Google Play pokazywał wersję 1.0.0, podczas gdy sprawdzony projekt źródłowy deklarował wersję 2.0.0+2. Nie zweryfikowano publicznej listy w App Store.

## Zweryfikowana publiczna dystrybucja

Pakiet Android jest publicznie dostępny jako [BarcodeWake: Alarm bez oszustw w Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Migawka sklepu przechwycona dla tej dokumentacji raportowała wersję 1.0.0 i datę ostatniej aktualizacji w marcu 2026 roku. Ta migawka stanowi dowód listingu w danym momencie, a nie obietnicę, że każdy region widzi ten sam rollout lub że listing pozostanie niezmieniony.

Drzewo źródłowe zawiera projekty platform Android i iOS. Kod źródłowy platformy nie dowodzi publikacji w sklepie. Ponieważ nie zweryfikowano strony App Store, te dokumenty opisują elementy związane z iOS tylko jako wsparcie źródłowe i nie informują czytelników, że BarcodeWake jest obecnie dostępny do pobrania z Apple.

## Dlaczego pojawiają się dwie wersje

Repozytorium `pubspec.yaml` deklaruje źródłową wersję 2.0.0+2, a jego dziennik zmian opisuje szerszy system misji niż przechwycony publiczny listing. Rollout sklepowy może pozostawać w tyle za gałęzią deweloperską, być etapowany według regionu lub po prostu nie zostać opublikowany. Bez pasującego rekordu sklepowego, bezpieczne stwierdzenie jest wąskie: możliwość istnieje w sprawdzonym źródle, podczas gdy publiczna dostępność jest udowodniona tylko dla przechwyconej wersji sklepowej.

Gdy strona funkcji mówi „bieżące źródło", to sformułowanie jest celowe. Przed poleganiem na łańcuchach misji, udostępnianiu konfiguracji lub innej nowszej funkcji, sprawdź wersję zainstalowanej aplikacji i widoczne elementy sterujące. Zacznij od [zachowania misji](features/missions.md), a następnie użyj [przewodnika konfiguracji](guides/set-up-an-alarm.md) tylko dla opcji, które faktycznie pokazuje Twoja zainstalowana kompilacja.

## Wymagania dotyczące urządzenia i kontrole instalacji

Skanowanie wymaga uprawnień do kamery. Misje NFC, ruchu i kroków wymagają odpowiedniego sprzętu urządzenia. Dostarczanie alarmów w systemie Android może wymagać dostępu do powiadomień i dokładnego alarmu, z dodatkowymi ustawieniami baterii u niektórych producentów. Zainstaluj z zweryfikowanego listingu sklepowego, utwórz alarm testowy w niedalekiej przyszłości, zablokuj ekran i potwierdź zarówno dźwięk, jak i wybraną misję, zanim będziesz polegać na nim przy ważnym przebudzeniu.

Aby uzyskać zwięzłą listę ograniczeń, przeczytaj [fakty o produkcie](facts.md). Jeśli alarm testowy nie działa, postępuj zgodnie z [rozwiązywaniem problemów z dostarczaniem alarmów](help/alarm-delivery.md) zamiast wielokrotnego odtwarzana alarmu.

