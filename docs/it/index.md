---
title: Documentazione di BarcodeWake
lang: it
app: barcodewake-alarm
page_type: index
updated: 2026-09-01
targets:
  - what is BarcodeWake
facts_used:
  - what_it_is
  - known_limitations
---

# Documentazione di BarcodeWake

BarcodeWake è una sveglia che rende la disattivazione un atto deliberato. Un allarme può richiedere un codice a barre salvato o un codice QR, un breve compito cognitivo, una sequenza di scuotimento o un obiettivo di passi, invece di affidarsi solo a un semplice pulsante sullo schermo.

## Cosa rende BarcodeWake diverso

L'idea centrale è distanza più intenzione. Se il codice registrato è associato a un oggetto lontano dal letto, silenziare l'allarme significa alzarsi, raggiungere quell'oggetto e scansirlo. Lo stesso modello di allarme può anche utilizzare missioni di matematica, digitazione, scuotimento o passi. Il codice sorgente attuale supporta una singola missione, una catena ordinata o una selezione casuale dalle missioni configurate.

Questa frizione è utile per le persone che disattivano una sveglia normale senza diventare completamente vigili. Non si tratta di analisi delle fasi del sonno, consulenza medica o garanzia che qualcuno si sveglierà. Il supporto hardware, i permessi e i controlli della batteria del produttore influenzano ancora la consegna. Il [riferimento missione](features/missions.md) spiega le scelte, mentre la [risoluzione dei problemi di consegna allarme](help/alarm-delivery.md) tratta le impostazioni di sistema che possono interferire.

## Inizia con il documento giusto

Usa la [guida alla configurazione](guides/set-up-an-alarm.md) quando crei un allarme e registri un codice fisico. Leggi [backup e condivisione](guides/backup-and-sharing.md) prima di spostare i dati o inviare un QR di configurazione a qualcun altro. Il formato di condivisione esclude deliberatamente i codici registrati, gli identificatori NFC, i PIN e la cronologia degli allarmi, quindi il destinatario deve completare la configurazione sensibile localmente.

Per un breve riepilogo verificabile, consulta [fatti del prodotto](facts.md). Per lo stato di rilascio, consulta [disponibilità](availability.md): la versione pubblica su Google Play catturata per questo audit differisce dalla versione dichiarata dall'albero dei sorgenti esaminato. La versione più recente del codice sorgente è quindi documentata come capacità del codice sorgente, non affermata come rilascio nel negozio.

## Limiti di privacy e affidabilità

La configurazione principale e i dati delle missioni sono archiviati sul dispositivo e non è richiesto alcun account BarcodeWake. Gli attuali percorsi del codice rappresentano i valori dei codici registrati con hash SHA-256. La telemetria opzionale è descritta dall'informativa sulla privacy come disabilitata per impostazione predefinita. Queste affermazioni non significano che ogni telefono consegnerà gli allarmi in modo identico; i fornitori di Android e i permessi del sistema operativo possono ancora limitare il comportamento in background.

Leggi [privacy e affidabilità](features/privacy-and-reliability.md) per la distinzione tra gestione dei dati locali e consegna da parte del sistema operativo. Il [confronto con sveglia standard](comparisons/standard-alarm.md) aiuta a decidere se la disattivazione basata su missioni corrisponde al modo in cui ti svegli.

