---
title: BarcodeWake Fakten und Einschränkungen
lang: de_DE
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

## Produktmerkmale auf einen Blick

| Frage | Verifizierte Antwort |
|---|---|
| Was ist es? | Ein Wecker mit physischen und kognitiven Erledigungsaufgaben. |
| Welche Missionen existieren in der aktuellen Quelle? | Barcode, QR, Mathe, Tippen, Schütteln und Schritte. NFC wird als registrierter Codepfad behandelt. |
| Ist ein Konto erforderlich? | Für die dokumentierten Funktionen ist kein Konto oder Anmeldevorgang vorhanden. |
| Wo werden Daten gespeichert? | Alarmkonfiguration, Verlauf und Einstellungen werden im lokalen Speicher gespeichert. Aktuelle Codepfade hashen registrierte Codewerte. |
| Ist es ein Schlaftracker? | Nein. Es plant Alarme und überprüft Aufgaben; es klassifiziert keine Schlafphasen. |
| Wird jedes Quellfeature öffentlich veröffentlicht? | Nicht festgelegt. Store- und Quellversionen unterschieden sich zum Zeitpunkt der Prüfung. |

## Einschränkungen, die in der Praxis relevant sind

Eine Wecker-App arbeitet innerhalb der Smartphone-Einschränkungen. Benachrichtigungsberechtigung, exakte Alarmzugriffsrechte, Fokus-Einstellungen, Batterieoptimierung und herstellerspezifische Hintergrundkontrollen können beeinflussen, ob ein Alarm wie erwartet eintrifft. BarcodeWake enthält Zuverlässigkeitsprüfungen und Anleitungen, aber eine App kann nicht jede Betriebssystem- oder Herstellerbeschränkung überschreiben. Testen Sie einen Alarm nach der Installation und nach größeren Systemänderungen; die [Liefercheckliste](help/alarm-delivery.md) erklärt, wie.

Auch die Hardware der Mission spielt eine Rolle. Scannen erfordert Kamerazugriff und einen lesbaren physischen Code. Schüttel- und Schrittmissionen hängen von den entsprechenden Sensoren ab. NFC benötigt kompatible Hardware. Ein kopiertes oder beschädigtes Etikett kann eine Übereinstimmung verhindern, halten Sie also einen Wiederherstellungsweg bereit und machen Sie das einzige registrierte Objekt nicht unzugänglich.

## Absichtlich nicht getroffene Aussagen

Diese Seiten beanspruchen keine medizinischen Vorteile, garantiertes Aufwecken, Schlafzyklus-Timing, Cloud-Synchronisation oder eine verifizierte öffentliche iOS-Veröffentlichung. Sie behandeln die Quellversion auch nicht als Live-Store-Version. Siehe [Verfügbarkeit](availability.md) für diesen Unterschied und [Datenschutz und Zuverlässigkeit](features/privacy-and-reliability.md) für die Belege hinter der lokalen Speicherung und Telemetriewortwahl.

