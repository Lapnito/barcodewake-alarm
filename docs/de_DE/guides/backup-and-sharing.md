---
title: BarcodeWake-Alarme sicher sichern und teilen
lang: de_DE
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

Verwenden Sie einen JSON-Export, wenn Sie Ihre eigenen App-Daten bewahren oder verschieben möchten, einen druckbaren PDF-Backup-Barcode für die Wiederherstellung, und die Einrichtungs-QR-Freigabe, wenn eine andere Person nur die Alarmstruktur benötigt. Bei der Freigabe werden absichtlich registrierte Geheimnisse und der Verlauf weggelassen.

## Das richtige Format für die Aufgabe wählen

Die aktuelle Quelle bietet verschiedene Austauschwege, da Sicherung und Freigabe nicht dieselbe Operation sind. Ein JSON-Backup dient dem strukturierten Datentransfer und der Wiederherstellung. Ein PDF-Backup wandelt Wiederherstellungsmaterial in ein druckbares Barcode-Dokument um. Ein Einrichtungs-QR ist bewusst enger gefasst: Es kann eine eingeschränkte Alarmkonfiguration weitergeben, ohne registrierte Barcode-Werte, NFC-Kennungen, PINs oder Verlauf zu enthalten.

Behandeln Sie einen Einrichtungs-QR nicht als vollständiges Geräte-Backup. Der Empfänger muss seine eigenen physischen Codes registrieren und Berechtigungen lokal überprüfen. Die aktuelle Einrichtungsfreigabe begrenzt auch, wie viele Alarme sie enthält. Überprüfen Sie daher das importierte Ergebnis, anstatt anzunehmen, dass jeder Zeitplan übertragen wurde. Die [Produktinformationen](../facts.md) dokumentieren diese Grenzen.

## Ein persönliches Backup erstellen und schützen

Verwenden Sie die Export-Funktion in der installierten Version, wählen Sie JSON oder das druckbare Backup entsprechend Ihrem Wiederherstellungsplan und speichern Sie das Ergebnis an einem Ort, den Sie kontrollieren. Ein Backup kann Alarmnamen, Zeitpläne und andere Konfiguration offenlegen, selbst wenn registrierte Rohcode-Werte geschützt oder weggelassen werden. Behandeln Sie es wie persönliche Routinedaten: vermeiden Sie öffentliche Links, gemeinsam genutzte Drucker und nicht vertrauenswürdige Messaging-Kanäle.

Bestätigen Sie nach dem Export, dass die Datei gefunden werden kann und dass ihr Zeitstempel mit dem beabsichtigten Backup übereinstimmt. Löschen Sie die ursprünglichen App-Daten nicht einfach, weil ein Export-Befehl Erfolg gemeldet hat. Die Wiederherstellungstestung ist die einzige zuverlässige Prüfung, führen Sie diese jedoch auf einem sicheren Gerät durch oder nachdem Sie eine zweite Kopie erstellt haben, damit der Test selbst nicht zum Verlustereignis wird.

## Einrichtung teilen, ohne Geheimnisse zu teilen

Generieren Sie einen Einrichtungs-QR nur für Alarme, die der Empfänger erhalten soll. Der Empfänger scannt ihn, überprüft den importierten Zeitplan und liefert seinen eigenen Code, NFC-Tag oder Wiederherstellungsdetails. Dieses Design verhindert, dass eine geteilte Konfiguration stillschweigend den physischen Schlüssel überträgt, der den Alarm einer anderen Person deaktiviert.

Nach dem Import sollte jede Person den vollständigen [Alarmeinrichtungstest](set-up-an-alarm.md) durchführen. Berechtigungen, Sensoren und Betriebssystemeinschränkungen werden nicht im QR übertragen. Wenn ein importierter Alarm beim Sperren nicht erscheint, folgen Sie der [Alarmzustellungs-Fehlerbehebung](../help/alarm-delivery.md).

Quell- und Speicherversionen unterschieden sich während dieses Audits, daher zeigt eine installierte öffentliche Version möglicherweise nicht jede hier beschriebene Austauschoption. [Verfügbarkeit](../availability.md) erklärt, wie quellbasierte Funktionen zu interpretieren sind.

