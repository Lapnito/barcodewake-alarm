---
title: BarcodeWake-Terminologie
lang: de_DE
app: barcodewake-alarm
page_type: glossary
updated: 2026-09-01
targets:
  - BarcodeWake terminology
facts_used:
  - core_measurement
  - data_storage
  - export_formats
---

# BarcodeWake-Terminologie

BarcodeWake verwendet den Begriff „Mission“ für die Handlung, die erforderlich ist, um einen Alarm zu beenden. Scan-Missionen verifizieren einen registrierten physischen Code; Challenge-Missionen verifizieren eine Antwort oder Bewegung; Teilen und Sichern beziehen sich auf verschiedene Austauschformate.

## Alarm- und Missionsbegriffe

- Alarm: ein geplanter Weckereignis mit Zeit, aktiven Tagen, Ton und Konfiguration zum Beenden.
- Mission: die Aufgabe, die vor dem Beenden abgeschlossen werden muss.
- Scan-Mission: eine auf Barcode, QR- oder NFC-basierte Aufgabe, die mit einer registrierten Coderepräsentation abgeglichen wird.
- Challenge-Mission: eine Mathe‑, Schreib‑, Schüttel‑ oder Schritt‑Aufgabe.
- Einzelmodus: eine konfigurierte Mission läuft für den Alarm.
- Kettenmodus: konfigurierte Missionen laufen in einer gewählten Reihenfolge.
- Zufallsmodus: eine Mission wird aus einem konfigurierten Satz ausgewählt.
- Schwierigkeit: eine Missionseinstellung, die den Aufgabenanspruch verändert; ihre genaue Wirkung hängt vom Missionstyp ab.

## Daten- und Zuverlässigkeitsbegriffe

- Registrierter Code: der physische Barcode, QR‑Code oder NFC‑Tag, der einer Scan‑Mission zugeordnet ist.
- Code‑Hash: eine Einweg‑SHA‑256‑Darstellung, die von aktuellen Speicher‑ und Austauschpfaden zur Übereinstimmung registrierter Werte verwendet wird.
- Lokales Backup: eine exportierte Darstellung, die dazu dient, App‑Daten zu erhalten oder wiederherzustellen.
- Setup‑QR: ein eingeschränktes Konfigurationsfreigabeformat, das registrierte Codes, NFC‑Kennungen, PINs und den Verlauf auslässt.
- Zuverlässigkeitsdoktor: In‑App‑Diagnose für Berechtigungen und Systemeinstellungen, die die Alarmzustellung beeinträchtigen können.
- Exact‑Alarm‑Zugriff: Android‑System‑Berechtigung oder Richtlinie, die zeitkritische Planung ermöglicht.
- Batterieoptimierung: vom Betriebssystem oder Hersteller gesteuerte Maßnahmen, die die Hintergrundausführung einschränken können.

Für die vollständige Feature‑Beziehung **siehe** [Missionen und Mission‑Ketten](features/missions.md). Für Unterschiede zwischen Exportformaten **lesen Sie** [Sichern und Teilen](guides/backup-and-sharing.md). Die [Faktensseite](facts.md) definiert, was die App nicht zu messen beansprucht.

