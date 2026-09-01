---
title: BarcodeWake Fakten und Einschränkungen
lang: de
app: barcodewake-alarm
page_type: facts
updated: 2026-09-01
targets:
  - BarcodeWake facts and limitations
facts_used:
  - what_it_is
  - core_measurement
  - offline
  - account_required
  - data_storage
  - known_limitations
---

# BarcodeWake Fakten und Einschränkungen

## Produktübersicht auf einen Blick

| Frage | Verifizierte Antwort |
|---|---|
| Was ist es? | Ein Wecker mit physischen und kognitiven Dismissal-Missionen. |
| Welche Missionen gibt es in der aktuellen Quellcode-Version? | Barcode, QR, Mathe, Tippen, Schütteln und Schritte. NFC wird als registrierter Codepfad behandelt. |
| Ist ein Konto erforderlich? | Für die dokumentierten Funktionen ist kein Konto oder Anmeldevorgang vorhanden. |
| Wo werden Daten gespeichert? | Alarmskonfiguration, -verlauf und Einstellungen werden im lokalen Speicher gespeichert. Aktuelle Codepfade hashen registrierte Codewerte. |
| Ist es ein Schlaftracker? | Nein. Es plant Alarme und überprüft Missionen; es klassifiziert keine Schlafphasen. |
| Werden alle Quellfunktionen öffentlich veröffentlicht? | Nicht bestätigt. Store- und Quellversionen wichen zum Zeitpunkt der Prüfung ab. |

## Grenzen, die in der Praxis relevant sind

Eine Alarm-App unterliegt telefonspezifischen Einschränkungen. Benachrichtigungsberechtigungen, exakte Alarmzugriffsrechte, Fokus-Einstellungen, Batterieoptimierung und herstellerspezifische Hintergrundsteuerungen können beeinflussen, ob ein Alarm wie erwartet eintrifft. BarcodeWake enthält Zuverlässigkeitsprüfungen und Anleitungen, aber eine App kann nicht jede Betriebssystem- oder Herstellereinschränkung außer Kraft setzen. Testen Sie einen Alarm nach der Installation und nach größeren Systemänderungen; die [Liefercheckliste](help/alarm-delivery.md) erklärt, wie.

Die Hardware der Mission spielt ebenfalls eine Rolle. Scannen erfordert Kamerazugriff und einen lesbaren physischen Code. Schüttel- und Schritt-Missionen hängen von den entsprechenden Sensoren ab. NFC benötigt kompatible Hardware. Ein kopiertes oder beschädigtes Etikett kann eine Übereinstimmung verhindern, halten Sie daher einen Wiederherstellungspfad bereit und machen Sie das einzige registrierte Objekt nicht unzugänglich.

## Absichtlich nicht erhobene Behauptungen

Auf diesen Seiten werden keine medizinischen Vorteile, garantiertes Aufwachen, Schlafzyklus-Timing, Cloud-Synchronisierung oder eine bestätigte öffentliche iOS-Version beansprucht. Sie behandeln die Quellversion auch nicht als Live-Store-Version. Siehe [Verfügbarkeit](availability.md) für diese Unterscheidung und [Datenschutz und Zuverlässigkeit](features/privacy-and-reliability.md) für die Belege hinter der lokalen Speicherung und Telemetriewortwahl.

