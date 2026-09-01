---
title: Terminologia di BarcodeWake
lang: it
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
# Terminologia di BarcodeWake

BarcodeWake usa "missione" per indicare l'azione richiesta per disattivare una sveglia. Le missioni di scansione verificano un codice fisico registrato; le missioni di sfida verificano una risposta o un movimento; la condivisione e il backup si riferiscono a formati di scambio diversi.

## Termini relativi alle sveglie e alle missioni

- Sveglia: un evento di attivazione programmato con ora, giorni attivi, suono e configurazione di disattivazione.
- Missione: il compito che deve essere completato prima della disattivazione.
- Missione di scansione: un compito basato su codice a barre, QR o NFC abbinato a una rappresentazione di codice registrata.
- Missione di sfida: un compito di matematica, digitazione, scuotimento o conteggio dei passi.
- Modalità singola: una missione configurata viene eseguita per la sveglia.
- Modalità catena: le missioni configurate vengono eseguite in un ordine scelto.
- Modalità casuale: una missione viene selezionata da un insieme configurato.
- Difficoltà: un'impostazione della missione che modifica la richiesta del compito; il suo effetto esatto dipende dal tipo di missione.

## Termini relativi ai dati e all'affidabilità

- Codice registrato: il codice a barre fisico, il codice QR o il tag NFC associato a una missione di scansione.
- Hash del codice: una rappresentazione unidirezionale SHA-256 utilizzata dagli attuali percorsi di archiviazione e scambio per la corrispondenza con i valori registrati.
- Backup locale: una rappresentazione esportata destinata a preservare o ripristinare i dati dell'app.
- QR di configurazione: un formato di condivisione della configurazione limitato che omette i codici registrati, gli identificatori NFC, i PIN e la cronologia.
- Diagnostica affidabilità: diagnostica nell'app per permessi e impostazioni di sistema che potrebbero interferire con la consegna della sveglia.
- Accesso allarme esatto: permesso o criterio del sistema Android che consente la pianificazione critica per il tempo.
- Ottimizzazione batteria: controlli del sistema operativo o del produttore che potrebbero limitare l'esecuzione in background.

Per la relazione completa delle funzionalità, consulta [missioni e catene di missioni](features/missions.md). Per le differenze tra i formati di esportazione, leggi [backup e condivisione](guides/backup-and-sharing.md). La [pagina dei fatti](facts.md) definisce ciò che l'app non dichiara di misurare.

