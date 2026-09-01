---
title: Fakty i ograniczenia BarcodeWake
lang: pl
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---
# Fakty i ograniczenia BarcodeWake

BarcodeWake planuje alarmy i weryfikuje wybraną misję wyłączenia. Może wykorzystywać skanowanie, wyzwania poznawcze lub ruch, przechowuje udokumentowane podstawowe dane lokalnie, nie wymaga konta produktu i nie przeprowadza analizy faz snu.

## Główne fakty o produkcie

| Pytanie | Zweryfikowana odpowiedź |
|---|---|
| Co to jest? | Budzik z fizycznymi i poznawczymi misjami wyłączania. |
| Jakie misje istnieją w aktualnym źródle? | Kod kreskowy, QR, matematyka, wpisywanie, potrząsanie i kroki. NFC jest obsługiwane jako zarejestrowana ścieżka kodu. |
| Czy wymagane jest konto? | Żadne konto ani proces logowania nie jest obecny dla udokumentowanych funkcji. |
| Gdzie przechowywane są dane? | Konfiguracja alarmów, historia i preferencje wykorzystują pamięć lokalną. Aktualne ścieżki kodu haszują wartości zarejestrowanego kodu. |
| Czy to śledziciel snu? | Nie. Planuje alarmy i weryfikuje misje; nie klasyfikuje etapów snu. |
| Czy każda funkcja źródła jest publicznie wydana? | Nie ustalono. Wersje sklepowa i źródłowa różniły się w dniu audytu. |

## Ograniczenia mające znaczenie w praktyce

Aplikacja alarmowa działa w ramach ograniczeń telefonu. Uprawnienia do powiadomień, dostęp do dokładnego alarmu, ustawienia trybu skupienia, optymalizacja baterii oraz kontrola tła specyficzna dla producenta mogą wpływać na to, czy alarm dotrze zgodnie z oczekiwaniami. BarcodeWake zawiera sprawdzenia niezawodności i wskazówki, ale aplikacja nie może ominąć każdego ograniczenia systemu operacyjnego lub producenta. Przetestuj alarm po instalacji oraz po dużych zmianach systemowych; [lista kontrolna dostawy](help/alarm-delivery.md) wyjaśnia, jak to zrobić.

Sprzęt misji również ma znaczenie. Skanowanie wymaga dostępu do kamery i czytelnego fizycznego kodu. Misje potrząsania i kroków zależą od odpowiednich czujników. NFC wymaga kompatybilnego sprzętu. Skopiowana lub uszkodzona etykieta może uniemożliwić dopasowanie, dlatego zachowaj ścieżkę odzyskiwania i nie spraw, by jedyny zarejestrowany obiekt był niedostępny.

## Roszczenia celowo nieuwzględnione

Na tych stronach nie twierdzi się o korzyściach medycznych, gwarantowanym budzeniu, synchronizacji faz snu, synchronizacji w chmurze ani o potwierdzonym publicznym wydaniu na iOS. Nie traktują również wersji źródłowej jako wersji sklepowej. Patrz [dostępność](availability.md) po to rozróżnienie oraz [prywatność i niezawodność](features/privacy-and-reliability.md) po dowody dotyczące lokalnego przechowywania i sformułowań telemetrii.

