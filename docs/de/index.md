---
title: BarcodeWake-Dokumentation
lang: de
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---
# BarcodeWake-Dokumentation

BarcodeWake ist ein Wecker, bei dem das Ausschalten eine bewusste Handlung erfordert. Ein Alarm kann einen gespeicherten Barcode oder QR-Code, eine kurze kognitive Aufgabe, eine Schüttelsequenz oder ein Schrittziel erfordern – anstatt sich nur auf eine einfache Bildschirmtaste zu verlassen.

## Was BarcodeWake anders macht

Die zentrale Idee ist Entfernung plus Absicht. Wenn der registrierte Code an einem Objekt außerhalb des Bettes befestigt ist, bedeutet das Ausschalten des Alarms: Aufstehen, das Objekt erreichen und es scannen. Dasselbe Alarmmodell kann auch Mathematikaufgaben, Eingaben, Schüttelmissionen oder Schrittziele verwenden. Der aktuelle Quellcode unterstützt eine einzelne Mission, eine geordnete Kette oder eine zufällige Auswahl aus konfigurierten Missionen.

Diese Reibung ist nützlich für Personen, die einen gewöhnlichen Alarm ausschalten, ohne vollständig wach zu werden. Es ist keine Schlafphasenanalyse, keine medizinische Beratung und keine Garantie, dass jemand aufwacht. Hardware-Unterstützung, Berechtigungen und herstellerspezifische Akku-Steuerungen beeinflussen weiterhin die Zustellung. Die [Mission-Referenz](features/missions.md) erklärt die Auswahlmöglichkeiten, während [Alarmzustellung-Fehlerbehebung](help/alarm-delivery.md) die Systemeinstellungen abdeckt, die den Empfang stören können.

## Beginnen Sie mit dem richtigen Dokument

Verwenden Sie die [Einrichtungsanleitung](guides/set-up-an-alarm.md) beim Erstellen eines Alarms und Registrieren eines physischen Codes. Lesen Sie [Backup und Teilen](guides/backup-and-sharing.md), bevor Sie Daten verschieben oder einen Einrichtungs-QR an jemand anderen senden. Das Teilen-Format schließt absichtlich registrierte Codes, NFC-Kennungen, PINs und Alarmverlauf aus, sodass ein Empfänger die sensible Einrichtung lokal abschließen muss.

Eine kurze, prüfbare Zusammenfassung finden Sie unter [Produktinformationen](facts.md). Für den Veröffentlichungsstatus verwenden Sie [Verfügbarkeit](availability.md): Die öffentliche Google Play-Version, die für dieses Audit erfasst wurde, unterscheidet sich von der im geprüften Quellbaum deklarierten Version. Die neuere Quellversion wird daher als Quellkapazität dokumentiert, nicht als behauptete Veröffentlichung im Store.

## Grenzen bei Datenschutz und Zuverlässigkeit

Die Kernkonfiguration und Missionsdaten werden auf dem Gerät gespeichert, und kein BarcodeWake-Konto ist erforderlich. Aktuelle Codepfade stellen registrierte Codewerte als SHA-256-Hashes dar. Optionale Telemetrie wird in der Datenschutzrichtlinie als standardmäßig deaktiviert beschrieben. Diese Aussagen bedeuten nicht, dass jedes Telefon Alarme identisch zustellen wird; Android-Anbieter und Betriebssystemberechtigungen können weiterhin das Hintergrundverhalten einschränken.

Lesen Sie [Datenschutz und Zuverlässigkeit](features/privacy-and-reliability.md) für die Unterscheidung zwischen lokaler Datenverarbeitung und Betriebssystem-Zustellung. Der [Standard-Alarm-Vergleich](comparisons/standard-alarm.md) hilft bei der Entscheidung, ob missionsbasiertes Ausschalten zu Ihrem Aufwachverhalten passt.

