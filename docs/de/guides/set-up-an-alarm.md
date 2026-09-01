---
title: So richten Sie einen BarcodeWake-Alarm ein
lang: de
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to set up a BarcodeWake alarm
facts_used:
  - what_it_is
  - hardware_requirements
  - accuracy_limits
---

# So richten Sie einen BarcodeWake-Alarm ein

Erstellen Sie zuerst den Zeitplan, wählen Sie eine Mission, die sicher und praktisch ist, erteilen Sie die erforderlichen Berechtigungen und führen Sie dann einen zeitnahen Sperrbildschirm-Test durch. Für Scan-Missionen registrieren Sie ein dauerhaftes Objekt, das verfügbar und lesbar sein wird, wenn der Alarm ertönt.

## Wählen Sie die Mission vor dem Objekt

Entscheiden Sie, welche Aktion das Aufwecken vom Abbrechen trennen soll. Ein Barcode in einem anderen Raum erzeugt physischen Abstand. Mathe oder Tippen fügt Konzentration hinzu, ohne eine Kamera zu benötigen. Schütteln oder Schritte fügen Bewegung hinzu, hängt jedoch von Sensoren ab und eignet sich möglicherweise nicht für jede Person oder Umgebung. Die [Mission-Referenz](../features/missions.md) erläutert die Kompromisse zwischen Einzel-, Ketten- und Zufallsmodus.

Wenn Sie einen Barcode, QR-Code oder NFC-Tag verwenden, wählen Sie etwas Dauerhaftes. Vermeiden Sie Einwegverpackungen, ein Objekt, das ein anderer Haushaltsangehöriger möglicherweise bewegt, oder einen Code, der während Reisen unzugänglich sein wird. Überprüfen Sie, ob die Kamera im erwarteten Licht fokussieren kann. NFC benötigt ein kompatibles Telefon und Tag.

## Zeitplan und Abweisungsregel konfigurieren

Öffnen Sie den Alarm-Editor, stellen Sie die gewünschte Zeit und aktive Tage ein und wählen Sie dann die Mission aus, die von der installierten Build angezeigt wird. Konfigurieren Sie deren Schwierigkeit oder Ziel zunächst konservativ für den ersten Test. Wenn die installierte Version Ketten unterstützt, ordnen Sie Missionen in einer Reihenfolge an, die sicher ohne Hetze über Treppen oder Verlassen eines gesicherten Bereichs abgeschlossen werden kann.

Registrieren Sie den physischen Code aus dem Missions-Setup-Flow. Geben Sie dem Alarm ein Label, das die beabsichtigte Routine identifiziert, anstatt sensible Informationen preiszugeben. Überprüfen Sie Lautstärke, Vibration und etwaige Aufwach-Nachfolge-Optionen, die in der installierten Build sichtbar sind. Die verfügbaren Steuerungen können sich unterscheiden, da die [öffentliche und Quellversionen](../availability.md) zum Prüfzeitpunkt nicht identisch waren.

## Berechtigungen zweckgerichtet erteilen

Erlauben Sie Benachrichtigungen und alarmbezogene Zugriffe, die für die Zustellung erforderlich sind. Erteilen Sie Kamerazugriff nur bei Verwendung einer Scan-Mission und Sensorzugriff, wenn die gewählte Mission dies benötigt. Überprüfen Sie auf Android die Exact-Alarm- und Batterieeinstellungen, wenn die Zuverlässigkeitsprüfung der App diese beanstandet. Gehen Sie nicht davon aus, dass das Speichern eines Alarms bedeutet, dass die Hintergrundauslieferung erlaubt ist.

## Den vollständigen Nachtpfad testen

Stellen Sie einen Test einige Minuten im Voraus ein. Sperren Sie den Bildschirm, lassen Sie BarcodeWake im Hintergrund und legen Sie das Telefon in denselben Klang- und Stromzustand, der für die Nacht geplant ist. Bestätigen Sie, dass der Alarm erscheint, der Ton hörbar ist und die ausgewählte Mission exakt abgeschlossen werden kann. Wiederholen Sie dann, nachdem Sie das registrierte Objekt an seinen tatsächlichen Standort gebracht haben.

Wenn die Zustellung fehlschlägt, verwenden Sie die [Alarm-Benachrichtigungs-Checkliste](../help/alarm-delivery.md). Wenn sie erfolgreich ist, erwägen Sie, nach Stabilisierung der Einrichtung eine [lokale Sicherung](backup-and-sharing.md) zu erstellen.

