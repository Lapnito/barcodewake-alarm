---
title: BarcodeWake-Missionen und Missionsketten
lang: de_DE
app: barcodewake-alarm
page_type: feature
updated: 2026-09-01
targets:
  - how do BarcodeWake missions work
facts_used:
  - what_it_is
  - core_measurement
  - hardware_requirements
  - known_limitations
---
# BarcodeWake-Missionen und Missionsketten

Eine BarcodeWake-Mission ist die Bedingung, die zum Deaktivieren eines Alarms verwendet wird. Die aktuelle Quelle unterstützt Barcode-, QR-, Mathe-, Tipp-, Schüttel- und Schrittaufgaben, wobei registrierte NFC über den Code-Scan-Pfad abgewickelt wird. Missionen können allein, in Sequenz oder durch Zufallsauswahl ausgeführt werden.

## Scan-Missionen schaffen physischen Abstand

Eine Barcode- oder QR-Mission vergleicht einen Live-Kamera-Scan mit einem bei der Einrichtung registrierten Code. Der Code kann auf einem Objekt außerhalb der Reichweite platziert werden: Toiletartikel im Badezimmer, ein Frühstücksartikel in einer Küche oder ein anderes stabiles Objekt in einem gut beleuchteten Bereich. NFC folgt derselben allgemeinen Idee mit einem kompatiblen Tag und Gerät. Die App speichert eine Hash-Darstellung in aktuellen Pfaden, anstatt den Rohcode für einen gewöhnlichen Vergleich zu benötigen.

Wählen Sie ein Objekt, das noch verfügbar sein wird, wenn der Alarm ertönt. Verpackungen werden weggeworfen, Etiketten verblassen und Reisen verändern die Umgebung. Einen Code auf der einzigen Medikamentenbox zu registrieren, die Sie möglicherweise ersetzen müssen, ist weniger robust als die Verwendung eines dauerhaften Etiketts. Der [Alarmeinrichtungsleitfaden](../guides/set-up-an-alarm.md) behandelt Platzierung und Tests.

## Herausforderungs-Missionen tauschen Bewegung gegen Aufwand

Mathe und Tippen erfordern konzentrierte Eingabe. Schütteln und Schritte erfordern körperliche Bewegung und unterstützte Sensoren. Schwierigkeits- und Ziel-Einstellungen ändern, wie viel Arbeit erwartet wird, aber eine schwierigere Mission ist nicht automatisch eine bessere. Übermäßige Reibung kann dazu ermutigen, den Alarm vollständig zu deaktivieren, während eine einfache Aufgabe nach Wiederholung automatisch werden kann.

Passen Sie die Aufgabe an den Fehlermodus an. Wenn Sie Alarme im Halbschlaf ausschalten, erzeugt das Scannen in einem anderen Raum nützlichen Abstand. Wenn der Kamerazugriff unbequem ist, kann eine kurze Tipp- oder Mathe-Aufgabe praktischer sein. Wenn Mobilität, Gleichgewicht oder Barrierefreiheit ein Anliegen sind, vermeiden Sie bewegungsbasierte Missionen und wählen Sie eine Aufgabe, die sicher erledigt werden kann.

## Einzel-, Ketten- und Zufallsmodi

Der Einzelmodus fordert eine konfigurierte Mission. Der Kettenmodus führt mehrere konfigurierte Missionen in Reihenfolge aus. Der Zufallsmodus wählt aus einem konfigurierten Set und reduziert die Chance, dass eine memorierte Interaktion automatisch wird. Diese Modi sind in der neueren überprüften Quelle vorhanden; [Verfügbarkeit](../availability.md) erklärt, warum das nicht beweist, dass sie bereits in jedem öffentlichen Build enthalten sind.

Führen Sie immer einen Test in naher Zukunft nach dem Ändern des Modus, der Berechtigungen oder der registrierten Objekte durch. Halten Sie das ausgewählte Objekt erreichbar und bieten Sie eine sichere Wiederherstellungsroute. Für Zustellungsprobleme, die nicht mit der Missionsfertigstellung zusammenhängen, verwenden Sie die [Zuverlässigkeits-Checkliste](../help/alarm-delivery.md).

