---
title: BarcodeWake Datenschutz und Alarmzuverlässigkeit
lang: de_DE
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

BarcodeWake speichert dokumentierte Alarmkonfigurationen und Missionsdaten auf dem Gerät und erfordert kein App-Konto. Aktuelle Codepfade hashen registrierte Codewerte. Optionale Telemetrie ist standardmäßig als deaktiviert beschrieben, während die Alarmübermittlung weiterhin von Systemberechtigungen und Herstellersteuerungen abhängt.

## Lokale Daten entfernen keine Systemabhängigkeiten

Lokale Speicherung bedeutet, dass die gewöhnliche Alarmeinrichtung kein BarcodeWake-Cloud-Konto erfordert. Alarmdatensätze, Verlauf und Einstellungen werden über die lokale Datenschicht der App verarbeitet. Registrierte Barcode-, QR- und NFC-Werte werden in aktuellen Speicher- und Importpfaden als SHA-256-Hashes dargestellt, wodurch die Beibehaltung des gewöhnlichen Rohwerts für den Abgleich vermieden wird.

Hashing ist nicht dasselbe wie die Verschlüsselung jedes App-Datensatzes, und lokale Speicherung ist kein Backup. Jemand mit Zugang zu einem entsperrten Gerät kann möglicherweise trotzdem Alarmnamen, Zeitpläne oder Verlauf durch die App sehen. Ein verlorenes oder zurückgesetztes Telefon kann auch lokale Daten verlieren, es sei denn, der Benutzer hat einen Export erstellt. Siehe [Backup und Teilen](../guides/backup-and-sharing.md) für die Formate und ihre unterschiedlichen Zwecke.

Die Datenschutzrichtlinie besagt, dass optionale Telemetrie standardmäßig deaktiviert ist, und beschreibt das aggregierte Handling, falls aktiviert. Diese Dokumentation macht daher nicht die breitere Behauptung, dass die App niemals über ein Netzwerk kommunizieren kann. Sie stellt die engeren verifizierten Fakten fest: Kernbetrieb und Daten sind lokal, kein Produktkonto ist erforderlich, und keine Werbe-SDK-Abhängigkeit erscheint im überprüften Projekt.

## Zuverlässigkeit ist eine gemeinsame Verantwortung

BarcodeWake kann Alarme planen und präsentieren, aber das Betriebssystem entscheidet, wann Hintergrundarbeit ausgeführt werden darf und welche Unterbrechungen erlaubt sind. Benachrichtigungsberechtigung, exakte Alarmfreigabe, lautlose oder Fokus-Modi, Batterieoptimierung, automatische App-Aussetzung und Hersteller-Task-Killer können alle relevant sein. Das In-App-Zuverlässigkeitswerkzeug kann Konfigurationsrisiken identifizieren und Benutzer zu Einstellungen leiten; es kann keine Systemrichtlinie überschreiben.

Nach der Installation testen Sie mit gesperrtem Bildschirm und dem Telefon im gleichen Strommodus, der über Nacht verwendet wird. Wiederholen Sie diesen Test nach einem Systemupdate, Batterie-Spar-Änderung oder App-Neuinstallation. Halten Sie das Gerät geladen, die Lautstärke angemessen und die gewählte Mission physisch verfügbar. Befolgen Sie die [Alarmübermittlungs-Fehlerbehebung](../help/alarm-delivery.md), wenn ein Test fehlschlägt.

## Was Datenschutz und Zuverlässigkeit nicht garantieren

BarcodeWake ist kein medizinisches Gerät, Notfallwarndienst oder Schlafphasen-Tracker. Keine Alarm-App kann Aufwecken garantieren oder für ein nicht verfügbares Gerät entschädigen. Die Seite [Fakten und Grenzen](../facts.md) listet diese Grenzen auf, während [Verfügbarkeit](../availability.md) öffentliche Store-Beweise von neueren Quellfähigkeiten trennt.

