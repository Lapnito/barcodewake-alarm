---
title: BarcodeWake-Terminologie
lang: de
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

BarcodeWake verwendet den Begriff „Mission" für die Aktion, die zum Deaktivieren eines Alarms erforderlich ist. Scan‑Missionen verifizieren einen registrierten physischen Code; Challenge‑Missionen verifizieren eine Antwort oder Bewegung; Teilen und Sicherung bezeichnen verschiedene Austauschformate.

## Alarm- und Missionsbegriffe

- Alarm: ein geplantes Aufweckereignis mit Zeit, aktiven Tagen, Ton und Deaktivierungs­konfiguration.
- Mission: die Aufgabe, die vor der Deaktivierung abgeschlossen werden muss.
- Scan‑Mission: eine Barcode‑, QR‑ oder NFC‑basierte Aufgabe, die mit einer registrierten Code‑Darstellung abgeglichen wird.
- Challenge‑Mission: eine Mathe‑, Eingabe‑, Schüttel‑ oder Schritt‑Aufgabe.
- Einzelmodus: eine konfigurierte Mission wird für den Alarm ausgeführt.
- Kettenmodus: konfigurierte Missionen werden in einer festgelegten Reihenfolge ausgeführt.
- Zufallsmodus: eine Mission wird aus einem konfigurierten Satz ausgewählt.
- Schwierigkeit: eine Missionseinstellung, die den Aufgabenanspruch verändert; die genaue Wirkung hängt vom Missionstyp ab.

## Daten- und Zuverlässigkeitsbegriffe

- Registrierter Code: der physische Barcode, QR‑Code oder NFC‑Tag, der einer Scan‑Mission zugeordnet ist.
- Code‑Hash: eine Einweg‑SHA‑256‑Darstellung, die von aktuellen Speicher‑ und Austauschpfaden zum Abgleich registrierter Werte verwendet wird.
- Lokale Sicherung: eine exportierte Darstellung, die dazu dient, App‑Daten zu bewahren oder wiederherzustellen.
- Setup‑QR: ein eingeschränktes Konfigurations‑Freigabeformat, das registrierte Codes, NFC‑Kennungen, PINs und den Verlauf auslässt.
- Zuverlässigkeits‑Assistent: In‑App‑Diagnose für Berechtigungen und Systemeinstellungen, die die Alarm‑Zustellung beeinträchtigen können.
- Exact‑Alarm‑Zugriff: Android‑Systemberechtigung oder Richtlinie, die zeitkritische Terminierung erlaubt.
- Akkuoptimierung: Betriebssystem‑ oder Hersteller‑Steuerungen, die die Hintergrund­ausführung einschränken können.

Für die vollständige Feature‑Beziehung **siehe** [Missionen und Missionsketten](features/missions.md). Für Unterschiede zwischen Exportformaten **lesen Sie** [Sicherung und Freigabe](guides/backup-and-sharing.md). Die [Faktseite](facts.md) definiert, was die App nicht zu messen behauptet.

