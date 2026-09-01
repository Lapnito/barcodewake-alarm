---
title: Dostupnost a verze BarcodeWake
lang: cs
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# Dostupnost a verze BarcodeWake

BarcodeWake má ověřenou veřejnou nabídku na Google Play pro Android. K datu auditu Google Play uváděl verzi 1.0.0, zatímco kontrolovaný zdrojový projekt deklaroval verzi 2.0.0+2. Nebyla ověřena žádná veřejná nabídka v App Store.

## Ověřená veřejná distribuce

Android balíček je veřejně uveden jako [BarcodeWake: No Cheat Alarm na Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Snímkový stav obchodu zachycený pro tuto dokumentaci uváděl verzi 1.0.0 a datum poslední aktualizace v březnu 2026. Tento snímek je důkazem nabídky v daném časovém bodě, nikoli zárukou, že každý region vidí stejnou distribuci nebo že nabídka zůstane nezměněna.

Ve stromu zdrojového kódu jsou projekty platforem Android a iOS. Zdrojový kód platformy neprokazuje publikaci v obchodě. Protože nebyla ověřena žádná stránka App Store, tyto dokumenty popisují položky související s iOS pouze jako podporu zdrojového kódu a neinformují čtenáře, že je BarcodeWake aktuálně ke stažení od Apple.

## Proč se zobrazují dvě čísla verzí

Soubor `pubspec.yaml` v repozitáři deklaruje zdrojovou verzi 2.0.0+2 a jeho seznam změn popisuje širší systém misí než zachycená veřejná nabídka. Distribuce v obchodě může zaostávat za vývojovou větví, být postupně zaváděna podle regionů, nebo prostě nebyla publikována. Bez odpovídajícího záznamu v obchodě je bezpečné tvrzení úzké: schopnost existuje v kontrolovaném zdrojovém kódu, zatímco veřejná dostupnost je prokázána pouze pro zachycenou verzi obchodu.

Když stránka funkcí uvádí „aktuální zdrojový kód", je toto slovní spojení záměrné. Před spoléháním na řetězce misí, sdílení nastavení nebo jinou novější schopnost si ověřte verzi nainstalované aplikace a viditelné ovládací prvky. Začněte s [chováním misí](features/missions.md), poté použijte [průvodce nastavením](guides/set-up-an-alarm.md) pouze pro možnosti, které vaše skutečně nainstalovaná verze zobrazuje.

## Požadavky na zařízení a kontroly instalace

Skenování vyžaduje oprávnění k fotoaparátu. Mise NFC, pohybu a kroků vyžadují odpovídající hardwarové vybavení zařízení. Doručování alarmů v Androidu může vyžadovat oprávnění k oznámením a přesným alarmům, s dalšími nastaveními baterie u některých výrobců. Instalujte z ověřené nabídky obchodu, vytvořte alarm na blízký termín, zamkněte obrazovku a potvrďte zvuk i vybranou misi dříve, než se na něj budete spoléhat při důležitém buzení.

Pro stručný seznam omezení si přečtěte [fakta o produktu](facts.md). Pokud testovací alarm selže, postupujte podle [řešení problémů s doručováním alarmů](help/alarm-delivery.md) místo opakovaného vytváření alarmu.

