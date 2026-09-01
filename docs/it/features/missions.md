---
title: Missioni e catene di missioni BarcodeWake
lang: it
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
# Missioni e catene di missioni BarcodeWake

Una missione BarcodeWake è la condizione utilizzata per disattivare una sveglia. La fonte attuale supporta attività di codice a barre, QR, matematica, digitazione, scuotimento e passi, con NFC registrato gestito tramite il percorso di scansione del codice. Le missioni possono essere eseguite da sole, in sequenza o per selezione casuale.

## Le missioni di scansione creano distanza fisica

Una missione con codice a barre o QR confronta una scansione della fotocamera in tempo reale con un codice registrato durante la configurazione. Il codice può essere posizionato su un oggetto fuori dalla portata del braccio: articoli da toilette in un bagno, un oggetto per la colazione in una cucina o un altro oggetto stabile in un'area ben illuminata. L'NFC segue la stessa idea generale con un tag e un dispositivo compatibili. L'app memorizza una rappresentazione hash nei percorsi correnti invece di necessitare del codice grezzo per il confronto ordinario.

Scegli un oggetto che sarà ancora disponibile quando suonerà la sveglia. Gli imballaggi vengono gettati via, le etichette sbiadiscono e i viaggi cambiano l'ambiente. Registrare un codice sull'unica scatola di medicine che potresti dover sostituire è meno robusto rispetto all'uso di un'etichetta durevole. La [guida alla configurazione della sveglia](../guides/set-up-an-alarm.md) copre il posizionamento e il test.

## Le missioni di sfida scambiano movimento per sforzo

La matematica e la digitazione richiedono input concentrati. Lo scuotimento e i passi richiedono movimento fisico e sensori supportati. Le impostazioni di difficoltà e obiettivo cambiano quanto lavoro è previsto, ma una missione più difficile non è automaticamente migliore. Un'attrito eccessivo può incoraggiare a disabilitare completamente la sveglia, mentre un compito facile può diventare automatico dopo la ripetizione.

Abbina il compito alla modalità di fallimento. Se spengi le sveglie mezza addormentata, scansionare in un'altra stanza crea una distanza utile. Se l'accesso alla fotocamera è scomodo, un breve compito di digitazione o matematica potrebbe essere più pratico. Se la mobilità, l'equilibrio o l'accessibilità sono una preoccupazione, evita le missioni basate sul movimento e scegli un compito che possa essere completato in sicurezza.

## Modalità singola, catena e casuale

La modalità singola richiede una missione configurata. La modalità catena esegue diverse missioni configurate in ordine. La modalità casuale seleziona da un set configurato, riducendo la possibilità che un'interazione memorizzata diventi automatica. Queste modalità sono presenti nella fonte verificata più recente; la [disponibilità](../availability.md) spiega perché ciò non dimostra che siano già in ogni build pubblica.

Esegui sempre un test a breve termine dopo aver cambiato modalità, permessi o oggetti registrati. Tieni l'oggetto selezionato raggiungibile e fornisci un percorso di recupero sicuro. Per problemi di consegna non correlati al completamento della missione, usa la [lista di controllo dell'affidabilità](../help/alarm-delivery.md).

