---
title: BarcodeWake Datenschutz und Alarmzuverlässigkeit
lang: de
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
# BarcodeWake Datenschutz und Alarmzuverlässigkeit

BarcodeWake speichert dokumentierte Alarmkonfigurationen und Missionsdaten auf dem Gerät und erfordert kein App‑Konto. Aktuelle Codepfade hashen registrierte Codewerte. Optionale Telemetrie wird als standardmäßig deaktiviert beschrieben, während die Alarmzustellung weiterhin von Systemberechtigungen und Herstellersteuerungen abhängt.

## Lokale Daten entfernen keine Systemabhängigkeiten

Lokale Speicherung bedeutet, dass die gewöhnliche Alarmeinrichtung kein BarcodeWake‑Cloud‑Konto erfordert. Alarmdatensätze, Verlauf und Einstellungen werden über die lokale Datenschicht der App verwaltet. Registrierte Barcode‑, QR‑ und NFC‑Werte werden in aktuellen Speicher‑ und Importpfaden als SHA‑256‑Hashes dargestellt, wodurch das Beibehalten des rohen Werts für den Abgleich vermieden wird.

Hashing ist nicht dasselbe wie die Verschlüsselung jedes App‑Datensatzes, und lokale Speicherung ist kein Backup. Jemand mit Zugang zu einem entsperrten Gerät kann möglicherweise noch Alarmnamen, Zeitpläne oder Verlauf über die App sehen. Ein verlorenes oder zurückgesetztes Telefon kann auch lokale Daten verlieren, es sei denn, der Benutzer hat einen Export durchgeführt. Siehe [Sichern und Teilen](../guides/backup-and-sharing.md) für die Formate und ihre unterschiedlichen Zwecke.

Die Datenschutzrichtlinie besagt, dass optionale Telemetrie standardmäßig deaktiviert ist, und beschreibt die aggregierte Behandlung, falls aktiviert. Diese Dokumentation macht daher nicht die breitere Behauptung, dass die App niemals über ein Netzwerk kommunizieren kann. Sie stellt die engeren verifizierten Fakten fest: Kernbetrieb und Daten sind lokal, kein Produktkonto ist erforderlich, und in dem überprüften Projekt ist keine Werbe‑SDK‑Abhängigkeit erkennbar.

## Zuverlässigkeit ist eine gemeinsame Verantwortung

BarcodeWake kann einen Alarm planen und anzeigen, aber das Betriebssystem entscheidet, wann Hintergrundarbeit ausgeführt werden darf und welche Unterbrechungen erlaubt sind. Benachrichtigungsberechtigungen, exakte Alarmzugriffe, Stille‑ oder Fokusmodi, Akkuoptimierung, automatische App‑Aussetzung und Hersteller‑Task‑Killer können alle relevant sein. Das In‑App‑Tool zur Zuverlässigkeit kann Konfigurationsrisiken erkennen und Benutzer auf Einstellungen hinweisen; es kann keine Systemrichtlinie außer Kraft setzen.

Nach der Installation testen Sie mit gesperrtem Bildschirm und dem Telefon im gleichen Energiemodus, der über Nacht verwendet wird. Wiederholen Sie diesen Test nach einem Systemupdate, einer Änderung des Energiesparmodus oder einer Neuinstallation der App. Halten Sie das Gerät geladen, die Lautstärke angemessen und die gewählte Mission physisch verfügbar. Befolgen Sie die [Fehlerbehebung bei Alarmzustellung](../help/alarm-delivery.md), wenn ein Test fehlschlägt.

## Was Datenschutz und Zuverlässigkeit nicht versprechen

BarcodeWake ist kein medizinisches Gerät, kein Notfallwarndienst und kein Schlafphasen‑Tracker. Keine Alarm‑App kann garantieren, dass sie jemanden aufweckt oder einen nicht verfügbaren Gerät entschädigt. Die [Fakten und Grenzen](../facts.md)-Seite listet diese Grenzen auf, während [Verfügbarkeit](../availability.md) öffentliche Store‑Nachweise von neueren Quellfunktionen trennt.

