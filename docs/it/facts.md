---
title: Fatti e limiti di BarcodeWake
lang: it
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
# Fatti e limiti di BarcodeWake

BarcodeWake pianifica sveglie e verifica una missione di disattivazione scelta. Può utilizzare scansioni, sfide cognitive o movimento, memorizza i dati principali documentati localmente, non richiede un account del prodotto e non esegue analisi delle fasi del sonno.

## Fatti del prodotto a colpo d'occhio

| Domanda | Risposta verificata |
|---|---|
| Cos'è? | Una sveglia con missioni di disattivazione fisiche e cognitive. |
| Quali missioni esistono nel codice sorgente attuale? | Barcode, QR, matematica, digitazione, scuotimento e passi. NFC è gestito come percorso di codice registrato. |
| È necessario un account? | Nessun account o flusso di accesso è presente per le funzionalità documentate. |
| Dove vengono conservati i dati? | La configurazione della sveglia, la cronologia e le preferenze utilizzano l'archiviazione locale. I percorsi del codice attuale applicano hash ai valori del codice registrato. |
| È un tracker del sonno? | No. Pianifica sveglie e verifica missioni; non classifica le fasi del sonno. |
| Ogni funzionalità del codice sorgente è pubblicata? | Non stabilito. Le versioni del negozio e del codice sorgente differivano alla data dell'audit. |

## Limiti che contano in pratica

Un'app di sveglie opera all'interno di vincoli a livello di telefono. L'autorizzazione alle notifiche, l'accesso alle sveglie esatte, le impostazioni di messa a fuoco, l'ottimizzazione della batteria e i controlli specifici del produttore per il background possono influenzare se una sveglia arriva come previsto. BarcodeWake include controlli di affidabilità e indicazioni, ma un'app non può ignorare ogni restrizione del sistema operativo o del produttore. Testa una sveglia dopo l'installazione e dopo modifiche importanti del sistema; la [lista di controllo per la consegna](help/alarm-delivery.md) spiega come.

Anche l'hardware della missione conta. La scansione richiede l'accesso alla fotocamera e un codice fisico leggibile. Le missioni di scuotimento e passi dipendono dai sensori rilevanti. NFC richiede hardware compatibile. Un'etichetta copiata o danneggiata può impedire una corrispondenza, quindi mantieni un percorso di ripristino e non rendere l'unico oggetto registrato inaccessibile.

## Affermazioni intenzionalmente non fatte

Queste pagine non affermano benefici medici, risveglio garantito, tempistica del ciclo del sonno, sincronizzazione cloud o una release iOS pubblica verificata. Inoltre non trattano la versione del codice sorgente come una versione del negozio live. Vedi [disponibilità](availability.md) per quella distinzione e [privacy e affidabilità](features/privacy-and-reliability.md) per le evidenze dietro l'archiviazione locale e il linguaggio della telemetria.

