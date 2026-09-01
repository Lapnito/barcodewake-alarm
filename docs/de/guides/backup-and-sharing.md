---
title: BarcodeWake-Alarme sicher sichern und teilen
lang: de
app: barcodewake-alarm
page_type: guide
updated: 2026-09-01
targets:
  - how to back up or share BarcodeWake alarms
facts_used:
  - export_formats
  - data_storage
  - known_limitations
---
# BarcodeWake-Alarme sicher sichern und teilen

Verwenden Sie einen JSON-Export, wenn Sie Ihre eigenen App-Daten bewahren oder verschieben möchten, ein druckbares PDF-Backup-Barcode für die Wiederherstellung, und die Einrichtungs-QR-Freigabe, wenn eine andere Person nur die Alarmstruktur benötigt. Das Teilen erfolgt absichtlich ohne registrierte Secrets und Chronik.

## Das Format für die Aufgabe auswählen

Die aktuelle Quelle bietet verschiedene Austauschwege, da Sicherung und Teilen nicht dieselbe Operation sind. Ein JSON-Backup ist für strukturierte Datenübertragung und Wiederherstellung gedacht. Ein PDF-Backup wandelt Wiederherstellungsmaterial in ein druckbares Barcode-Dokument um. Ein Einrichtungs-QR ist bewusst enger gefasst: Es kann eine begrenzte Alarmkonfiguration weitergeben, ohne registrierte Barcode-Werte, NFC-Kennungen, PINs oder Chronik zu enthalten.

Behandeln Sie einen Einrichtungs-QR nicht als vollständiges Geräte-Backup. Der Empfänger muss seine eigenen physischen Codes registrieren und Berechtigungen lokal überprüfen. Das aktuelle Einrichtungs-Teilen begrenzt auch, wie viele Alarme es trägt. Überprüfen Sie also das importierte Ergebnis, anstatt anzunehmen, dass jeder Zeitplan übertragen wurde. Die [Produktfakten](../facts.md) dokumentieren diese Grenzen.

## Ein persönliches Backup erstellen und schützen

Verwenden Sie die in der installierten Build verfügbare Export-Aktion, wählen Sie JSON oder das druckbare Backup gemäß dem Wiederherstellungsplan und speichern Sie das Ergebnis an einem Ort, den Sie kontrollieren. Ein Backup kann Alarmnamen, Zeitpläne und andere Konfiguration offenlegen, selbst wenn registrierte Rohcode-Werte geschützt oder weggelassen werden. Behandeln Sie es wie persönliche Routinedaten: vermeiden Sie öffentliche Links, gemeinsam genutzte Drucker und nicht vertrauenswürdige Messaging-Kanäle.

Bestätigen Sie nach dem Exportieren, dass die Datei gefunden werden kann und dass ihr Zeitstempel dem beabsichtigten Backup entspricht. Löschen Sie die ursprünglichen App-Daten nicht einfach, nur weil ein Export-Befehl Erfolg gemeld hat. Die Wiederherstellungstestung ist die einzige zuverlässige Überprüfung, führen Sie sie jedoch auf einem sicheren Gerät oder nach dem Erstellen einer zweiten Kopie durch, damit der Test selbst kein Verlustereignis wird.

## Einrichtung teilen ohne Secrets zu teilen

Generieren Sie einen Einrichtungs-QR nur für Alarme, die der Empfänger erhalten soll. Der Empfänger scannt ihn, überprüft den importierten Zeitplan und liefert seinen eigenen Code, NFC-Tag oder Wiederherstellungsdetails. Dieses Design verhindert, dass eine geteilte Konfiguration stillschweigend den physischen Schlüssel überträgt, der den Alarm einer anderen Person dismissed.

Nach dem Import sollte jede Person den vollständigen [Alarmeinrichtungstest](set-up-an-alarm.md) durchführen. Berechtigungen, Sensoren und Betriebssystemeinschränkungen werden nicht im QR übertragen. Wenn ein importierter Alarm beim Sperren nicht erscheint, folgen Sie der [Alarmzustellungs-Fehlerbehebung](../help/alarm-delivery.md).

Quelle und Speicherversionen unterschieden sich während dieses Audits, daher zeigt eine installierte öffentliche Build möglicherweise nicht jede hier beschriebene Austauschoption. [Verfügbarkeit](../availability.md) erklärt, wie man Quell-only-Funktionen interpretiert.

