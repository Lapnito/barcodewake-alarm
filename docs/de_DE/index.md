---
title: BarcodeWake-Dokumentation
lang: de_DE
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

BarcodeWake ist ein Wecker, der das Ausschalten zu einer bewussten Handlung macht. Ein Alarm kann einen gespeicherten Barcode oder QR-Code, eine kurze kognitive Aufgabe, eine Schüttelsequenz oder ein Schrittziel erfordern, anstatt sich nur auf eine einfache Bildschirmtaste zu verlassen.

## Was BarcodeWake anders macht

Die zentrale Idee ist Entfernung plus Absicht. Wenn der registrierte Code an einem Objekt befestigt ist, das nicht neben dem Bett liegt, bedeutet das Ausschalten des Alarms Aufstehen, zu diesem Objekt greifen und es scannen. Dasselbe Alarmmodell kann auch Matheaufgaben, Eingabe, Schütteln oder Schrittmissionen verwenden. Der aktuelle Quellcode unterstützt eine einzelne Mission, eine geordnete Kette oder eine zufällige Auswahl aus konfigurierten Missionen.

Diese Reibung ist nützlich für Menschen, die einen gewöhnlichen Wecker ausschalten, ohne vollständig wach zu werden. Es handelt sich nicht um Schlafphasenanalyse, medizinische Beratung oder eine Garantie, dass jemand aufwacht. Hardwareunterstützung, Berechtigungen und herstellerspezifische Akkusteuerungen beeinflussen weiterhin die Zustellung. Die [Missionsreferenz](features/missions.md) erläutert die Optionen, während die [Alarmzustellungs-Fehlerbehebung](help/alarm-delivery.md) Systemeinstellungen behandelt, die stören können.

## Beginnen Sie mit dem richtigen Dokument

Verwenden Sie das [Einrichtungsleitfaden](guides/set-up-an-alarm.md), wenn Sie einen Alarm erstellen und einen physischen Code registrieren. Lesen Sie [Sicherung und Freigabe](guides/backup-and-sharing.md), bevor Sie Daten verschieben oder einen Einrichtungs-QR an jemand anderen senden. Das Freigabeformat schließt bewusst registrierte Codes, NFC-Kennungen, PINs und Alarmverlauf aus, sodass ein Empfänger die sensible Einrichtung lokal durchführen muss.

Für eine kurze, prüfbare Zusammenfassung sehen Sie [Produktinformationen](facts.md). Für den Veröffentlichungsstatus verwenden Sie [Verfügbarkeit](availability.md): Die in diesem Audit erfasste öffentliche Google Play-Version unterscheidet sich von der Version, die der geprüfte Quellbaum angibt. Die neuere Quellversion wird daher als Quellkapazität dokumentiert und nicht als veröffentlichte Store-Version behauptet.

## Grenzen von Datenschutz und Zuverlässigkeit

Die Kernkonfiguration und die Missionsdaten werden auf dem Gerät gespeichert, und kein BarcodeWake-Konto ist erforderlich. Aktuelle Codepfade stellen registrierte Codewerte mit SHA-256-Hashes dar. Optionale Telemetrie wird in der Datenschutzrichtlinie als standardmäßig deaktiviert beschrieben. Diese Aussagen bedeuten nicht, dass jedes Telefon Alarme identisch zustellt; Android-Anbieter und Betriebssystemberechtigungen können das Hintergrundverhalten weiter einschränken.

Lesen Sie [Datenschutz und Zuverlässigkeit](features/privacy-and-reliability.md) für den Unterschied zwischen lokaler Datenverarbeitung und Betriebssystem-Zustellung. Der [Vergleich mit Standardweckern](comparisons/standard-alarm.md) hilft zu entscheiden, ob die missionsbasierte Deaktivierung zur Art und Weise passt, wie Sie aufwachen.

