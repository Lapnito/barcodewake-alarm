---
title: BarcodeWake-Verfügbarkeit und Versionen
lang: de
app: barcodewake-alarm
page_type: availability
updated: 2026-09-01
targets:
  - where is BarcodeWake available
facts_used:
  - known_limitations
  - hardware_requirements
---
# BarcodeWake-Verfügbarkeit und Versionen

BarcodeWake verfügt über eine verifizierte öffentliche Google Play-Auflistung für Android. Zum Prüfdatum zeigte Google Play Version 1.0.0, während das geprüfte Quellprojekt Version 2.0.0+2 angab. Es wurde keine öffentliche App Store-Auflistung verifiziert.

## Verifizierte öffentliche Verteilung

Das Android-Paket ist öffentlich gelistet als [BarcodeWake: No Cheat Alarm auf Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Der für diese Dokumentation erfasste Store-Schnappschuss meldete Version 1.0.0 und ein letztes Aktualisierungsdatum im März 2026. Dieser Schnappschuss ist ein Nachweis der Auflistung zu einem bestimmten Zeitpunkt, keine Zusicherung, dass jede Region dieselbe schrittweise Einführung sieht oder dass die Auflistung unverändert bleibt.

Der Quellbaum enthält Android- und iOS-Plattformprojekte. Plattformquellcode beweist keine Store-Veröffentlichung. Da keine App Store-Seite verifiziert wurde, beschreiben diese Dokumente iOS-bezogene Elemente nur als Quellunterstützung und teilen den Lesern nicht mit, dass BarcodeWake derzeit aus dem Apple Store heruntergeladen werden kann.

## Warum zwei Versionsnummern erscheinen

Die Repository-Datei `pubspec.yaml` deklariert Quellversion 2.0.0+2 und ihr Änderungsprotokoll beschreibt ein umfassenderes Missionssystem als die erfasste öffentliche Auflistung. Eine Store-Einführung kann hinter einem Entwicklungszweig zurückbleiben, nach Region gestaffelt sein oder einfach nicht veröffentlicht worden sein. Ohne übereinstimmenden Store-Datensatz ist die sichere Aussage eng gefasst: Die Funktion existiert im geprüften Quellcode, während die öffentliche Verfügbarkeit nur für die erfasste Store-Version nachgewiesen ist.

Wenn eine Funktionsseite „aktueller Quellcode" sagt, ist diese Formulierung beabsichtigt. Bevor Sie sich auf Missionsketten, Setup-Freigabe oder eine andere neuere Funktion verlassen, überprüfen Sie die Version der installierten App und die sichtbaren Steuerelemente. Beginnen Sie mit [Missionsverhalten](features/missions.md), dann verwenden Sie das [Setup-Handbuch](guides/set-up-an-alarm.md) nur für Optionen, die Ihr installiertes Build tatsächlich anzeigt.

## Geräteanforderungen und Installationsprüfungen

Das Scannen erfordert Kameraberechtigung. NFC-, Bewegungs- und Schrittmissionen erfordern entsprechende Gerätehardware. Die Android-Alarmübermittlung kann Benachrichtigungs- und Exaktalarm-Zugriff erfordern, mit zusätzlichen Batterieeinstellungen bei einigen Herstellern. Installieren Sie aus der verifizierten Store-Auflistung, erstellen Sie einen zeitnahen Testalarm, sperren Sie den Bildschirm und bestätigen Sie sowohl den Ton als auch die ausgewählte Mission, bevor Sie sich für einen wichtigen Wecker darauf verlassen.

Für eine präzise Grenzenliste lesen Sie [Produktinformationen](facts.md). Wenn ein Testalarm fehlschlägt, folgen Sie der [Alarmübermittlung-Fehlerbehebung](help/alarm-delivery.md), anstatt den Alarm wiederholt neu zu erstellen.

