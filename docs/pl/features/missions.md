---
title: Misje i łańcuchy misji BarcodeWake
lang: pl
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# Misje i łańcuchy misji BarcodeWake

Misja BarcodeWake to warunek używany do wyłączenia alarmu. Aktualne źródło obsługuje kod kreskowy, QR, matematykę, pisanie, potrząsanie i kroki, a zarejestrowany NFC jest obsługiwany przez ścieżkę skanowania kodu. Misje mogą działać pojedynczo, w sekwencji lub przez losowy wybór.

## Misje skanowania zapewniają dystans fizyczny

Misja z kodem kreskowym lub QR porównuje skan z kamery na żywo z kodem zarejestrowanym podczas konfiguracji. Kod można umieścić na obiekcie poza zasięgiem ramienia: kosmetykach w łazience, produkcie śniadaniowym w kuchni lub innym stabilnym obiekcie w dobrze oświetlonym miejscu. NFC podąża tą samą ogólną koncepcją z kompatybilnym tagiem i urządzeniem. Aplikacja przechowuje reprezentację skrótu w bieżących ścieżkach, zamiast potrzebować surowego kodu do zwykłego porównania.

Wybierz obiekt, który będzie nadal dostępny, gdy zabrzmi alarm. Opakowania są wyrzucane, etykiety blakną, a podróż zmienia środowisko. Rejestrowanie kodu na jedynej pudełeczku z lekarstwem, które możesz potrzebować wymienić, jest mniej solidne niż użycie trwałej etykiety. [Przewodnik konfiguracji alarmu](../guides/set-up-an-alarm.md) obejmuje rozmieszczenie i testowanie.

## Misje wyzwań wymieniają ruch na wysiłek

Matematyka i pisanie wymagają skupionego wprowadzania danych. Potrząsanie i kroki wymagają ruchu fizycznego i obsługiwanych czujników. Ustawienia trudności i celu zmieniają oczekiwany nakład pracy, ale trudniejsza misja nie jest automatycznie lepsza. Nadmierne tarcie może zachęcać do całkowitego wyłączenia alarmu, podczas gdy łatwe zadanie może stać się automatyczne po powtórzeniu.

Dopasuj zadanie do trybu awarii. Jeśli wyłączasz alarmy w półśnie, skanowanie w innym pokoju tworzy użyteczny dystans. Jeśli dostęp do kamery jest niewygodny, krótkie zadanie z pisaniem lub matematyką może być bardziej praktyczne. Jeśli mobilność, równowaga lub dostępność stanowią problem, unikaj misji opartych na ruchu i wybierz zadanie, które można bezpiecznie wykonać.

## Tryby pojedynczy, łańcuchowy i losowy

Tryb pojedynczy wymaga jednej skonfigurowanej misji. Tryb łańcuchowy uruchamia kilka skonfigurowanych misji w kolejności. Tryb losowy wybiera z skonfigurowanego zestawu, zmniejszając szansę, że jedna zapamiętana interakcja stanie się automatyczna. Tryby te są obecne w nowszym sprawdzonym źródle; [dostępność](../availability.md) wyjaśnia, dlaczego to nie dowodzi, że są już w każdej publicznej kompilacji.

Zawsze przeprowadzaj test wkrótce po zmianie trybu, uprawnień lub zarejestrowanych obiektów. Utrzymuj wybrany obiekt w zasięgu i zapewnij bezpieczną trasę powrotu. W przypadku problemów z dostarczeniem niezwiązanych z ukończeniem misji, użyj [listy kontrolnej niezawodności](../help/alarm-delivery.md).

