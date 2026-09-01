---
title: Warum ein BarcodeWake-Alarm möglicherweise nicht klingelt
lang: de
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

Ein gespeicherter Alarm kann weiterhin durch Benachrichtigungseinstellungen, exakte Alarmzugriffe, Fokus- oder Stummschaltungsmodi, niedrige Lautstärke, Batterieeinschränkungen, App-Anhaltung oder Hersteller-Hintergrundsteuerungen blockiert werden. Prüfen Sie die Zustellung getrennt vom Mission‑Scannen und führen Sie dann einen Sperrbildschirmtest durch.

## Zunächst die Zustellung von der Entlassung trennen

Erstellen Sie einen baldigen Testalarm mit einer einfachen Mission und lassen Sie die App im Hintergrund. Sperren Sie den Bildschirm. Wenn keine Alarmanzeige oder kein Ton erscheint, liegt das Problem an der Zustellung; das Ändern des registrierten Barcodes wird es nicht beheben. Wenn der Alarm erscheint, die Mission jedoch nicht abgeschlossen werden kann, funktioniert die Zustellung und das Problem liegt bei der Kamera, dem Sensor, dem Codeabgleich oder der Missionskonfiguration.

Bestätigen Sie, dass der Alarm aktiviert ist, der geplante Tag korrekt ist und die Zeitzone des Telefons mit dem beabsichtigten Zeitplan übereinstimmt. Überprüfen Sie die Medien‑ und Alarmlautstärke, anstatt sich nur auf den Zustand der Seitentaste zu verlassen. Überprüfen Sie Nicht‑Stören‑ oder Fokusregeln, verbundene Audiogeräte und ob das Telefon nach dem Erstellen des Alarms neu gestartet wurde.

## Überprüfen der Berechtigungstore des Betriebssystems

Erlauben Sie Benachrichtigungen und jeden exakten Alarm‑ oder Vollbildalarm‑Zugriff, der von der installierten Build angefordert wird. Entfernen Sie BarcodeWake aus aggressiver Batterieoptimierung oder automatischen Ruhezustandslisten, wenn der Gerätehersteller diese Steuerungen anbietet. Öffnen Sie die In‑App‑Zuverlässigkeitsdiagnose und befolgen Sie die gerätespezifischen Einstellungen, die sie identifiziert. Die [Datenschutz‑ und Zuverlässigkeitsseite](../features/privacy-and-reliability.md) erklärt, warum diese Systemabhängigkeiten bestehen bleiben, selbst wenn App‑Daten lokal sind.

Nach dem Ändern einer Einstellung wiederholen Sie den Sperrbildschirmtest. Das Ändern mehrerer Steuerungen auf einmal erschwert die Ursachenidentifikation. Systemupdates können Berechtigungen zurücksetzen oder neu interpretieren, daher sollten Sie nach einem großen Update oder einer Neuinstallation der App erneut testen.

## Mission‑Ausführung separat diagnostizieren

Bei Barcode‑ und QR‑Missionen reinigen Sie das Kameraobjektiv, verbessern Sie die Beleuchtung und bestätigen Sie, dass das registrierte Objekt unverändert ist. Erteilen Sie die Kamera‑Berechtigung. Bei NFC überprüfen Sie die Geräteunterstützung und halten Sie den Tag in der Nähe der richtigen Antennenposition. Schüttel‑ und Schrittmessionen hängen von Bewegungs‑ oder Schrittsensoren ab und können sich anders verhalten, wenn Energiesparmodi die Sensorbereitstellung einschränken.

Wenn eine Mission als Teil einer Kette konfiguriert wurde, muss jeder erforderliche Schritt abgeschlossen werden. Lesen Sie das [Mission‑Verhalten](../features/missions.md) und erstellen Sie bei Bedarf einen neuen Test mit dem [Einrichtungsverfahren](../guides/set-up-an-alarm.md).

## Wissen, wann das Telefon die Grenze ist

BarcodeWake kann ein ausgeschaltetes Gerät, einen leeren Akku, defekte Audiohardware oder jeden Hersteller‑Task‑Killer nicht überschreiben. Es ist kein Notfall‑Benachrichtigungsdienst. Behalten Sie eine alternative Alarmmethode für Situationen mit hohem Risiko und melden Sie reproduzierbare Fehler mit Gerätemodell, Systemversion, App‑Version und den genauen Testbedingungen.

