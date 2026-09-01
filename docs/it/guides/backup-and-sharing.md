---
title: Eseguire il backup e condividere gli allarmi BarcodeWake in modo sicuro
lang: it
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
# Eseguire il backup e condividere gli allarmi BarcodeWake in modo sicuro

Utilizzare un'esportazione JSON quando si desidera conservare o spostare i propri dati dell'app, un codice a barre PDF stampabile per il backup per il ripristino e la condivisione tramite QR di configurazione quando un'altra persona necessita solo della struttura dell'allarme. La condivisione omette intenzionalmente i segreti registrati e la cronologia.

## Scegliere il formato adatto al caso

L'origine attuale fornisce diversi percorsi di scambio perché backup e condivisione non sono la stessa operazione. Un backup JSON è pensato per il trasferimento strutturato dei dati e il ripristino. Un backup PDF trasforma il materiale di ripristino in un documento con codice a barre stampabile. Un QR di configurazione è deliberatamente più limitato: può trasferire una configurazione di allarme limitata senza includere i valori dei codici a barre registrati, gli identificatori NFC, i PIN o la cronologia.

Non trattare un QR di configurazione come un backup completo del dispositivo. Il destinatario deve registrare i propri codici fisici e rivedere le autorizzazioni localmente. L'attuale condivisione della configurazione limita anche il numero di allarmi che può trasportare, quindi verificare il risultato importato invece di presumere che ogni programmazione sia stata trasferita. I [fatti del prodotto](../facts.md) registrano questi limiti.

## Creare e proteggere un backup personale

Utilizzare l'azione di esportazione disponibile nella build installata, scegliere JSON o il backup stampabile in base al piano di ripristino e salvare il risultato in un luogo sotto il proprio controllo. Un backup potrebbe rivelare nomi di allarmi, programmazioni e altre configurazioni anche quando i valori grezzi dei codici registrati sono protetti o omessi. Gestirlo come dati personali di routine: evitare link pubblici, stampanti condivise e canali di messaggistica non affidabili.

Dopo l'esportazione, confermare che il file possa essere trovato e che il suo timestamp corrisponda al backup previsto. Non eliminare i dati originali dell'app solo perché un comando di esportazione ha riportato successo. Il test di ripristino è l'unico controllo affidabile, ma eseguirlo su un dispositivo sicuro o dopo aver creato una seconda copia affinché il test stesso non diventi un evento di perdita.

## Condividere la configurazione senza condividere segreti

Generare un QR di configurazione solo per gli allarmi che il destinatario deve ricevere. Il destinatario lo scansiona, esamina la programmazione importata e fornisce il proprio codice, tag NFC o dettagli di ripristino. Questa progettazione impedisce che una configurazione condivisa trasferisca silenziosamente la chiave fisica che disattiva l'allarme di qualcun altro.

Dopo l'importazione, ciascuna persona dovrebbe eseguire il [test di configurazione dell'allarme](set-up-an-alarm.md) completo. Autorizzazioni, sensori e restrizioni del sistema operativo non vengono trasferiti nel QR. Se un allarme importato non viene visualizzato mentre è bloccato, consultare la [risoluzione dei problemi di recapito dell'allarme](../help/alarm-delivery.md).

Le versioni del codice sorgente e dello store differivano durante questo controllo, quindi una build pubblica installata potrebbe non esporre ogni opzione di scambio descritta qui. [Disponibilità](../availability.md) spiega come interpretare le funzionalità disponibili solo nel codice sorgente.

