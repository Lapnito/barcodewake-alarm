---
title: Warum ein BarcodeWake-Alarm möglicherweise nicht klingelt
lang: de_DE
app: barcodewake-alarm
page_type: help
updated: 2026-09-01
targets:
  - why did my BarcodeWake alarm not ring
facts_used:
  - accuracy_limits
  - hardware_requirements
  - known_limitations
---

# Warum ein BarcodeWake-Alarm möglicherweise nicht klingelt

Ein gespeicherter Alarm kann trotzdem durch Benachrichtigungseinstellungen, exakte Alarmfreigabe, Fokus- oder Stummschaltmodi, niedrige Lautstärke, Akkubeschränkungen, App-Aussetzung oder herstellerspezifische Hintergrundsteuerungen blockiert werden. Prüfen Sie die Zustellung separat vom Missionenscannen und führen Sie dann einen Sperrbildschirmtest durch.

## Zunächst die Zustellung vom Abbruch trennen

Erstellen Sie einen kurzfristigen Testalarm mit einer einfachen Mission und lassen Sie die App im Hintergrund. Sperren Sie den Bildschirm. Erscheint kein Alarmbildschirm oder Ton, liegt das Problem bei der Zustellung; ein Wechsel des registrierten Barcodes behebt es nicht. Erscheint der Alarm, die Mission aber nicht abgeschlossen werden kann, funktioniert die Zustellung und das Problem liegt bei Kamera, Sensor, Codeübereinstimmung oder Missionskonfiguration.

Bestätigen Sie, dass der Alarm aktiviert ist, der geplante Tag korrekt ist und die Zeitzone des Telefons mit dem beabsichtigten Zeitplan übereinstimmt. Überprüfen Sie die Medien- und Alarmlautstärke, anstatt sich nur auf den Zustand der Seitentaste zu verlassen. Prüfen Sie Nicht-stören- oder Fokus-Regeln, verbundene Audiogeräte und ob das Telefon nach dem Erstellen des Alarms neu gestartet wurde.

## Betriebssystemberechtigungen überprüfen

Erlauben Sie Benachrichtigungen und alle exakten Alarm- oder Vollbildalarm-Zugriffe, die vom installierten Build angefordert werden. Entfernen Sie BarcodeWake aus aggressiver Akkuoptimierung oder automatischen Schlaflisten, wenn der Gerätehersteller solche Steuerungen anbietet. Öffnen Sie die In-App-Zuverlässigkeitsdiagnose und befolgen Sie die gerätespezifischen Einstellungen, die sie identifiziert. Die [Datenschutz- und Zuverlässigkeitsseite](../features/privacy-and-reliability.md) erklärt, warum diese Systemabhängigkeiten bestehen bleiben, selbst wenn App-Daten lokal gespeichert sind.

Ändern Sie nur eine Einstellung und wiederholen Sie dann den Sperrbildschirmtest. Das Ändern mehrerer Steuerungen auf einmal erschwert die Ursachenfindung. Systemupdates können Berechtigungen zurücksetzen oder neu interpretieren, also führen Sie nach einem großen Update oder einer Neuinstallation der App einen erneuten Test durch.

## Missionierungsabschluss separat diagnostizieren

Für Barcode- und QR-Missionen reinigen Sie das Kameraobjektiv, verbessern Sie die Beleuchtung und bestätigen Sie, dass das registrierte Objekt unverändert ist. Erteilen Sie die Kamera-Berechtigung. Bei NFC überprüfen Sie die Geräteunterstützung und halten Sie den Tag nahe der korrekten Antennenposition. Schüttel- und Schritt-Missionen sind von Bewegungs- oder Schrittsensoren abhängig und können sich anders verhalten, wenn Energiesparmodi die Sensorbereitstellung einschränken.

Überprüfen Sie das [Verhalten von Missionen](../features/missions.md) und erstellen Sie gegebenenfalls einen neuen Test mit dem [Einrichtungsverfahren](../guides/set-up-an-alarm.md).

## Kennen Sie die Grenzen des Telefons

BarcodeWake kann ein ausgeschaltetes Gerät, einen leeren Akku, defekte Audiohardware oder jeden Hersteller-Task-Killer nicht umgehen. Es ist kein Notfall-Benachrichtigungsdienst. Behalten Sie für hochriskante Situationen eine zusätzliche Alarm-Methode bei und melden Sie reproduzierbare Fehler mit Gerätemodell, Systemversion, App-Version und den genauen Testbedingungen.

