---
title: BarcodeWake-Verfügbarkeit und Versionen
lang: de_DE
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

BarcodeWake verfügt über eine verifizierte öffentliche Google Play-Auflistung für Android. Zum Prüfdatum zeigte Google Play Version 1.0.0, während das geprüfte Quellprojekt Version 2.0.0+2 angab. Keine öffentliche App Store-Auflistung wurde verifiziert.

## Verifizierte öffentliche Verteilung

Das Android-Paket ist öffentlich gelistet als [BarcodeWake: No Cheat Alarm auf Google Play](https://play.google.com/store/apps/details?id=com.tomas.barcodewake_alarm&hl=en&gl=us). Der für diese Dokumentation erfasste Store-Snapshot meldete Version 1.0.0 und ein letztes Aktualisierungsdatum im März 2026. Dieser Snapshot ist ein Nachweis für den Zustand der Auflistung zu einem bestimmten Zeitpunkt, keine Zusicherung, dass jede Region dieselbe Einführung sieht oder dass die Auflistung unverändert bleibt.

Der Quellbaum enthält Android- und iOS-Plattformprojekte. Plattformquellcode beweist keine Store-Veröffentlichung. Da keine App Store-Seite verifiziert wurde, beschreiben diese Dokumente iOS-bezogene Elemente nur als Quellcode-Unterstützung und teilen den Lesern nicht mit, dass BarcodeWake derzeit von Apple herunterladbar ist.

## Warum erscheinen zwei Versionsnummern

Das Repository `pubspec.yaml` deklariert Quellversion 2.0.0+2 und sein Changelog beschreibt ein umfassenderes Missionssystem als die erfasste öffentliche Auflistung. Ein Store-Rollout kann hinter einem Entwicklungszweig zurückliegen, nach Region gestaffelt sein oder einfach nicht veröffentlicht worden sein. Ohne übereinstimmenden Store-Datensatz ist die sichere Aussage eng gefasst: Die Funktionalität existiert in der geprüften Quelle, während die öffentliche Verfügbarkeit nur für die erfasste Store-Version nachgewiesen ist.

Wenn eine Funktionsseite „aktuelle Quelle" sagt, ist diese Formulierung beabsichtigt. Bevor Sie sich auf Missionsketten, Setup-Freigabe oder eine andere neuere Funktion verlassen, überprüfen Sie die Version der installierten App und die sichtbaren Steuerungen. Beginnen Sie mit [Mission behavior](features/missions.md), dann verwenden Sie das [Setup-Handbuch](guides/set-up-an-alarm.md) nur für die Optionen, die Ihr installiertes Build tatsächlich anzeigt.

## Geräteanforderungen und Installationsprüfungen

Scannen erfordert Kameraberechtigung. NFC-, Bewegungs- und Schritt-Missionen erfordern entsprechende Gerätehardware. Die Android-Alarmübermittlung kann Benachrichtigungs- und Exact-Alarm-Zugriff erfordern, mit zusätzlichen Akkueinstellungen bei einigen Herstellern. Installieren Sie aus der verifizierten Store-Auflistung, erstellen Sie einen Testalarm in naher Zukunft, sperren Sie den Bildschirm und bestätigen Sie sowohl den Ton als auch die ausgewählte Mission, bevor Sie sich darauf für einen wichtigen Wecker verlassen.

Für eine präzise Begrenzungsliste lesen Sie [Produktdaten](facts.md). Wenn ein Testalarm fehlschlägt, befolgen Sie die [Alarmübermittlungs-Fehlerbehebung](help/alarm-delivery.md), anstatt den Alarm wiederholt neu zu erstellen.

