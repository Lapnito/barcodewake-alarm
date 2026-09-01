---
title: BarcodeWake-Missionen und Missionketten
lang: de
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
# BarcodeWake-Missionen und Missionketten

Eine BarcodeWake-Mission ist die Bedingung, die zum Deaktivieren eines Alarms verwendet wird. Die aktuelle Quelle unterstützt Barcode-, QR-, Mathe-, Tipp-, Schüttel- und Schrittaufgaben, wobei registrierte NFC über den Code-Scan-Pfad verarbeitet wird. Missionen können einzeln, in einer Sequenz oder nach Zufallsauswahl ausgeführt werden.

## Scan-Missionen schaffen physischen Abstand

Eine Barcode- oder QR-Mission vergleicht einen Live-Kamera-Scan mit einem während der Einrichtung registrierten Code. Der Code kann auf einem Objekt außerhalb der Reichweite platziert werden: Toilettenartikel im Badezimmer, ein Frühstücksartikel in der Küche oder ein anderes stabiles Objekt in einem gut beleuchteten Bereich. NFC folgt derselben allgemeinen Idee mit einem kompatiblen Tag und Gerät. Die App speichert eine Hash-Darstellung in aktuellen Pfaden, anstatt den rohen Code für einen gewöhnlichen Vergleich zu benötigen.

Wählen Sie ein Objekt, das noch verfügbar sein wird, wenn der Alarm ertönt. Verpackungen werden weggeworfen, Beschriftungen verblassen und Reisen verändern die Umgebung. Einen Code auf der einzigen Medikamentenschachtel zu registrieren, die Sie möglicherweise ersetzen müssen, ist weniger robust als die Verwendung eines dauerhaften Etiketts. Die [Alarmeinrichtungsanleitung](../guides/set-up-an-alarm.md) behandelt Platzierung und Testen.

## Herausforderungs-Missionen tauschen Bewegung gegen Aufwand

Mathe und Tippen erfordern konzentrierte Eingabe. Schütteln und Schritte erfordern körperliche Bewegung und unterstützte Sensoren. Schwierigkeits- und Zielwerte ändern, wie viel Arbeit erwartet wird, aber eine schwierigere Mission ist nicht automatisch eine bessere. Übermäßige Reibung kann dazu ermutigen, den Alarm vollständig zu deaktivieren, während eine einfache Aufgabe nach Wiederholung automatisch werden kann.

Passen Sie die Aufgabe an den Fehlermodus an. Wenn Sie Alarme im Halbschlaf ausschalten, erzeugt das Scannen in einem anderen Raum nützlichen Abstand. Wenn Kamerazugriff umständlich ist, kann eine kurze Tipp- oder Matheaufgabe praktischer sein. Wenn Mobilität, Gleichgewicht oder Barrierefreiheit ein Problem darstellen, vermeiden Sie bewegungsbasierte Missionen und wählen Sie eine Aufgabe, die sicher erledigt werden kann.

## Einzel-, Ketten- und Zufallsmodi

Im Einzelmodus wird nach einer konfigurierten Mission gefragt. Der Kettenmodus führt mehrere konfigurierte Missionen der Reihe nach aus. Der Zufallsmodus wählt aus einem konfigurierten Satz aus, wodurch die Wahrscheinlichkeit verringert wird, dass eine auswendig gelernte Interaktion automatisch wird. Diese Modi sind in der neueren geprüften Quelle vorhanden; [Verfügbarkeit](../availability.md) erklärt, warum das nicht beweist, dass sie bereits in jedem öffentlichen Build enthalten sind.

Führen Sie immer einen Test im nahen Zeitrahmen durch, nachdem Sie den Modus, die Berechtigungen oder registrierte Objekte geändert haben. Halten Sie das ausgewählte Objekt erreichbar und bieten Sie einen sicheren Rückgewinnungsweg. Für Lieferprobleme, die nicht mit dem Abschluss der Mission zusammenhängen, verwenden Sie die [Zuverlässigkeits-Checkliste](../help/alarm-delivery.md).

