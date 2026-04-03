---
title: Ciclo di vita dettagliato
parent: Appendici
nav_order: 1
description: Descrizione completa di tutti gli stati possibili durante il ciclo di vita di un'istanza su GeoTecSUE, inclusi stati regionali e deprecati
keywords: [stati pratica, ciclo di vita, inviata, protocollata, registrata, esecutiva, archiviata, diniego, integrazioni, verificata, rifiutata]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Ciclo di vita dettagliato

Questa appendice descrive **tutti gli stati possibili** durante il ciclo di vita di un'istanza su **GeoTecSUE**, inclusi stati specifici regionali, stati deprecati e casistiche particolari.

{: .note }
> Per una panoramica semplificata degli stati principali, consulta [Nozioni di base - Ciclo di vita](../nozioni-di-base.html#ciclo-di-vita-di-unistanza).

## Organizzazione degli stati

Gli stati sono organizzati in categorie:

1. **Stati di lavorazione del professionista**: Fasi sotto il tuo controllo
2. **Stati di lavorazione dell'Ente**: Fasi gestite dall'amministrazione
3. **Stati di integrazione**: Richieste e invii di documentazione aggiuntiva
4. **Stati finali**: Conclusione del procedimento
5. **Stati regionali specifici**: Piemonte (Notifica Preliminare)
6. **Stati non utilizzati**: Deprecati o in disuso

---

## Stati di lavorazione del professionista

Questi stati si verificano quando la pratica è sotto il tuo controllo, prima della trasmissione all'Ente.

### In Creazione

**Durata**: Pochi minuti

**Cosa significa**: L'istanza è stata appena creata ma **non ancora salvata** per la prima volta.

**Cosa puoi fare**:
- Compilare i campi iniziali
- Salvare per passare a "In Compilazione"
- Chiudere senza salvare (l'istanza viene persa)

**Stato successivo**:
- **In Compilazione** (se salvi)
- Nessuno (se chiudi senza salvare)

{: .note }
> Questo stato è transitorio e dura solo il tempo necessario per il primo salvataggio.

### In Compilazione

**Cosa significa**: L'istanza è stata salvata ma **non è ancora completa**. Mancano:
- Campi obbligatori non compilati
- Allegati obbligatori non caricati
- Pagamenti PagoPA obbligatori non effettuati

**Cosa puoi fare**:
- Proseguire la compilazione
- Salvare e riprendere in seguito (nessun limite di tempo)
- Condividere con [soggetti compilatori](../nozioni-di-base.html#soggetti-compilatori-aggiuntivi)
- Cancellare l'istanza se non serve più

**Stato successivo**:
- **Completata** (quando tutti i campi/allegati/pagamenti obbligatori sono inseriti)

{: .note }
> Puoi tenere un'istanza "In Compilazione" per tutto il tempo necessario. Non ci sono scadenze.

### Completata

**Cosa significa**: Il sistema ha **validato con successo** l'istanza. Tutti i requisiti sono soddisfatti:
- ✅ Tutti i campi obbligatori compilati
- ✅ Tutti gli allegati obbligatori caricati
- ✅ Pagamenti obbligatori effettuati

**Cosa puoi fare**:
- Generare il PDF dell'istanza
- Passare a "Firmata" (se la firma è obbligatoria)
- Inviare direttamente (se la firma non è obbligatoria)

**Stato successivo**:
- **Firmata** (se l'Ente richiede la firma digitale)
- **Inviata** (se la firma non è obbligatoria e invii direttamente)

{: .note }
> La necessità della firma digitale dipende dalle impostazioni dell'Ente. Se richiesta, devi firmare il PDF generato prima di inviare.

### Firmata

**Cosa significa**: Il PDF dell'istanza è stato:
1. Generato dal sistema
2. Scaricato sul tuo computer
3. Firmato digitalmente con firma **CAdES** (.p7m)
4. Ricaricato su GeoTecSUE

**Cosa puoi fare**:
- Inviare l'istanza all'Ente

**Stato successivo**:
- **Inviata** (dopo la trasmissione)

{: .warning }
> La firma deve essere in formato **CAdES** (.p7m). Formati diversi (PAdES) non sono accettati da tutti gli Enti.

---

## Stati di lavorazione dell'Ente

Questi stati si verificano dopo la trasmissione, quando la pratica è in gestione all'Ente.

### Inviata

**Cosa significa**: L'istanza è stata **trasmessa all'Ente** ed è in attesa di protocollazione.

**Cosa genera il sistema**:
- **Ricevuta di invio**: Disponibile per il download pochi istanti dopo la trasmissione

**Cosa puoi fare**:
- Consultare il dettaglio della pratica
- Scaricare la ricevuta di invio
- Attendere la protocollazione

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni
- ❌ Inviare integrazioni
- ❌ Modificare i dati

**Durata tipica**: Nel caso in cui sia attiva la *protocollazione automatica*, questo stato durerà pochi minuti. Se non è attiva, potrebbe durare anche qualche giorno

**Stato successivo**:
- **Protocollata** (dopo l'assegnazione del protocollo)
- **Rifiutata** (raro, solo se l'Ente non ha protocollazione automatica - deprecato)

{: .note }
> In molti Enti la protocollazione è automatica, rendendo la transizione da "Inviata" a "Protocollata" molto rapida (pochi minuti).

### Protocollata

**Cosa significa**: L'Ufficio Protocollo dell'Ente ha:
- Ricevuto la pratica
- Assegnato un **numero di protocollo**
- Assegnato una **data di protocollo**
- Inserito la pratica nel sistema documentale

**Cosa genera il sistema**:
- **Ricevuta di protocollazione**: Disponibile per il download pochi istanti dopo

**Cosa puoi fare**:
- Consultare numero e data di protocollo
- Scaricare la ricevuta di protocollazione
- Attendere la registrazione

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni (fino allo stato "Registrata")
- ❌ Inviare integrazioni
- ❌ Modificare i dati

**Durata tipica**: Da poche ore a diversi giorni (dipende dai tempi dell'Ufficio Tecnico)

**Stato successivo**:
- **Registrata** (dopo la presa in carico dall'Ufficio Tecnico)

### Registrata

**Cosa significa**: L'Ufficio competente (solitamente Ufficio Tecnico) ha **preso in carico** la pratica assegnando:
- **Numero di registrazione** (numero di pratica interno)
- **Data di registrazione**
- Contestualmente potrebbe essere stato anche indicato il **Responsabile del Procedimento** (se previsto)
- Contestualmente potrebbe essere stato anche indicato il **Responsabile del Servizio** (se previsto)

**Cosa genera il sistema**:
- **Ricevuta di registrazione**: Disponibile per il download pochi istanti dopo

**Cosa puoi fare**:
- ✅ **Inviare comunicazioni** (es. Inizio Lavori, Fine Lavori)
- ✅ **Inviare integrazioni spontanee** (se l'Ente lo consente)
- ✅ Consultare l'assegnazione ai responsabili
- ✅ Monitorare lo stato dell'istruttoria

**Stato successivo**:
- **Richiesta Integrazioni** (se l'Ente richiede documenti)
- **Esecutiva** (se l'Ente rilascia il provvedimento)
- **Archiviata** (se richiedi l'archiviazione o l'Ente la decide)
- **Diniego** (se l'Ente respinge la pratica)

{: .note }
> **Importante**: Solo da questo stato in poi puoi interagire attivamente con la pratica inviando comunicazioni e integrazioni.

---

## Stati di integrazione documentale o richiesta di archiviazione

Questi stati si verificano quando l'Ente richiede documentazione aggiuntiva o quando richiedi l'archiviazione.

### Richiesta Integrazioni

**Cosa significa**: L'Ente ha **aperto formalmente** una richiesta di integrazione documentale durante l'istruttoria.

**Effetti**:
- I **termini del procedimento** vengono interrotti
- Il sistema si predispone a ricevere i documenti richiesti
- A seconda della configurazione dell'Ente, altre attività potrebbero essere bloccate

**Cosa puoi fare**:
- ✅ Visualizzare i documenti richiesti dall'Ente
- ✅ Caricare i file richiesti
- ✅ Caricare anche documenti aggiuntivi (se l'Ente lo consente)
- ✅ Trasmettere l'integrazione (quando hai caricato tutto)

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni (dipende dalla configurazione dell'Ente - alcuni lo consentono)
- ❌ Modificare i dati della pratica originale

**Configurazioni possibili**:
- **Solo documenti richiesti**: Puoi caricare solo ciò che l'Ente ha esplicitamente richiesto
- **Documenti aggiuntivi consentiti**: Puoi aggiungere anche altra documentazione

**Stato successivo**:
- **Invio Integrazioni** (dopo aver trasmesso i documenti)

{: .warning }
> Le richieste di integrazione hanno spesso **termini da rispettare**. Verifica la richiesta dell'Ente e rispondi nei tempi previsti.

### Invio Integrazioni

**Cosa significa**: Hai caricato e **trasmesso correttamente** l'integrazione documentale richiesta.

**Durata tipica**: Breve (simile allo stato "Inviata")

**Cosa puoi fare**:
- Attendere che l'Ente prenda in carico i documenti

**Cosa NON puoi fare**:
- ❌ Modificare o aggiungere documenti all'integrazione inviata
- ❌ Inviare comunicazioni (fino al ritorno allo stato precedente)

**Stato successivo**:
- Ritorna allo stato precedente alla richiesta (solitamente **Registrata**, in alcuni casi **Esecutiva**)

{: .note }
> Il ritorno allo stato precedente avviene quando l'Ente ha verificato e accettato i documenti integrativi.

### Richiesta Archiviazione

**Cosa significa**: Hai compilato e trasmesso un'**istanza di Richiesta Archiviazione** collegata alla pratica.

**Quando si usa**:
- I lavori non verranno eseguiti
- La pratica non è più necessaria
- Vuoi chiudere formalmente il procedimento

**Cosa puoi fare**:
- Attendere la decisione dell'Ente

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni
- ❌ Modificare la pratica

**Stato successivo**:
- **Archiviata** (se l'Ente accetta la richiesta)
- Rimane in **Richiesta di Archiviazione** se l'Ente non accetta (deve effettuare ulteriori controlli)

{: .note }
> La richiesta di archiviazione deve essere **accettata** dall'Ente. Non archivia automaticamente la pratica.

---

## Stati finali

Questi stati rappresentano la conclusione del procedimento amministrativo. Se raggiunti quelli **negativi** (ad esempio **Archiviata** o **Diniego**), le possibilità di azione sono limitate o nulle.

### Esecutiva

**Cosa significa**: L'Ente ha completato l'istruttoria e **rilasciato il provvedimento** favorevole.

**Dati associati**:
- **Numero del provvedimento**
- **Data del provvedimento**

**Esempi**:
- Rilascio Permesso di Costruire
- Approvazione Autorizzazione Paesaggistica

**Cosa puoi fare**:
- ✅ Inviare comunicazioni (es. Inizio Lavori, Fine Lavori)
- ✅ Inviare integrazioni spontanee (se consentite)
- ✅ Scaricare il provvedimento e gli allegati timbrati
- ✅ Operare sulla pratica come nello stato "Registrata"

**Caratteristiche**:
- **Non è uno stato bloccante**: Puoi continuare a interagire
- La pratica è tecnicamente conclusa ma gestibile

{: .note }
> "Esecutiva" significa che il provvedimento è stato rilasciato ed è efficace. Puoi comunque inviare comunicazioni (es. Inizio Lavori).

### Archiviata

**Cosa significa**: La pratica è stata **archiviata** e chiusa definitivamente.

**Come si arriva**:
1. **Su tua richiesta**: Hai inviato una Richiesta di Archiviazione accettata dall'Ente
2. **Per decisione dell'Ente**: L'Ente ha archiviato la pratica per vari motivi

**Motivi tipici di archiviazione dell'Ente**:
- Pratica presentata per errore
- Documentazione non conforme e non integrabile
- Pratica presentata allo sportello sbagliato (SUAP invece di SUE)
- Mancato rispetto dei termini di integrazione
- Rinuncia del titolare

**Cosa puoi fare**:
- ✅ Visualizzare la pratica
- ✅ Scaricare documenti e ricevute
- ✅ Consultare la motivazione dell'archiviazione

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni
- ❌ Inviare integrazioni
- ❌ Modificare alcun dato
- ❌ Riaprire la pratica

**Visibilità**: La pratica rimane visibile nel tuo [elenco istanze](../elenco-istanze.html) ma non è più operativa.

{: .warning }
> L'archiviazione è **definitiva**. Se hai bisogno di ripresentare la pratica, dovrai creare una nuova istanza.

### Diniego

**Cosa significa**: L'Ente ha **respinto** la pratica dopo l'istruttoria, esprimendo parere negativo.

**Come si arriva**: Solo per **decisione dell'Ente** (dopo aver valutato la pratica)

**Differenza con "Archiviata"**:
- **Diniego**: Esito negativo dell'istruttoria tecnica con rigetto formale
- **Archiviata**: Chiusura amministrativa per motivi procedurali

**Cosa puoi fare**:
- ✅ Visualizzare la pratica
- ✅ Scaricare il provvedimento di diniego
- ✅ Consultare le motivazioni

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni
- ❌ Inviare integrazioni
- ❌ Modificare alcun dato
- ❌ Riaprire la pratica

**Visibilità**: La pratica rimane visibile nel tuo elenco istanze ma non è più operativa.

{: .note }
> In caso di diniego, se vuoi ripresentare la pratica dovrai creare una nuova istanza, eventualmente risolvendo i motivi del rigetto.

### Revoca Delegato

**Cosa significa**: Il **titolare della pratica** ha richiesto all'Ente (fuori dal portale) di **revocare il professionista** incaricato.

**Come si arriva**:
- Il titolare contesta l'operato del professionista ma non c'è accordo su una possibile **voltura** del tecnico a favore di un nuovo tecnico

**Procedura**:
1. Il titolare contatta l'Ente
2. Richiede formalmente la revoca del delegato
3. L'Ente modifica l'assegnazione nel gestionale
4. Lo stato passa a "Revoca Delegato"

**Cosa puoi fare**:
- ✅ Visualizzare la pratica

**Cosa NON puoi fare**:
- ❌ Inviare comunicazioni
- ❌ Inviare integrazioni
- ❌ Modificare alcun dato
- ❌ Operare in alcun modo

**Caratteristiche**:
- Stato **transitorio**: In attesa dell'assegnazione a un nuovo professionista
- Effetti simili ad "Archiviata" o "Diniego" per il professionista revocato

{: .warning }
> Se la tua pratica è in "Revoca Delegato", contatta il titolare e l'Ente per chiarire la situazione. Non potrai più operare su questa pratica.

---

## Stati regionali specifici: Piemonte

Questi stati si applicano **solo ai Comuni della Regione Piemonte** che hanno attivato la trasmissione della **Notifica Preliminare** tramite GeoTecSUE.

{: .note }
> Se non operi in Piemonte o non gestisci Notifiche Preliminari, puoi saltare questa sezione.

### Inviata SPRESALWEB (via MUDE)

**Ambito**: Solo **Notifica Preliminare** in Regione Piemonte

**Cosa significa**: La Notifica Preliminare è stata trasmessa al sistema **MUDE** (Modello Unico Digitale per l'Edilizia) che la inoltrerà a **SPRESALWEB** (sistema SPRESAL regionale).

**Cosa genera il sistema**:
- **Ricevuta di invio**: Disponibile per il download dall'elenco istanze o dal dettaglio

**Cosa puoi fare**:
- Attendere la protocollazione da parte di SPRESALWEB

**Stato successivo**:
- **Protocollata SPRESALWEB**

### Protocollata SPRESALWEB

**Ambito**: Solo **Notifica Preliminare** in Regione Piemonte

**Cosa significa**: Il sistema **SPRESAL** ha protocollato la Notifica Preliminare in modalità **asincrona** (non in tempo reale).

**Cosa genera il sistema**:
- **Ricevuta di protocollazione**: Disponibile per il download

**Durata protocollazione**: Normalmente **poche ore** (non immediato come altre pratiche)

**Caratteristiche**:
- La protocollazione **non** è eseguita dall'Ente comunale
- È gestita centralmente dal sistema SPRESAL regionale
- Questo è lo **stato finale** per le Notifiche Preliminari

**Stato successivo**:
- **Nessuno** (è uno stato finale)

{: .note }
> Per le Notifiche Preliminari Piemonte non sono previsti ulteriori stati oltre "Protocollata SPRESALWEB". Il procedimento si conclude qui.

---

## Stati non utilizzati o deprecati

Questi stati esistono ancora tecnicamente ma sono **sconsigliati**, **in disuso** o **non più applicabili** nella maggior parte dei casi.

### Rifiutata

**Stato**: **DEPRECATO** - Sconsigliato l'utilizzo

**Cosa significava**: Prima della protocollazione, l'Ente poteva "intercettare" la pratica e **rifiutarla con motivazione** senza inserirla nei sistemi gestionali (Protocollo e Ufficio Tecnico).

**Quando si raggiungeva**:
- Stato: **Inviata** → L'Ente valutava → Passava a **Rifiutata**
- La pratica veniva respinta **prima** della protocollazione

**Perché è deprecato**:

1. **Protocollazione automatica**: La maggior parte degli Enti ha protocollazione automatica che non consente più il rifiuto preventivo

2. **Perdita di tracciabilità**: Con il rifiuto non si tiene alcuna traccia della pratica nei sistemi dell'Ente (problematico per ricerche future, statistiche, trasparenza)

3. **Migliore pratica**: È consigliato protocollare, registrare e poi **archiviare** (con motivazione), mantenendo così tracciabilità completa

**Alternativa consigliata**:
- Protocollo → Registrazione → **Archiviazione** (con motivazione del rifiuto)

**Effetto per il professionista**:
- Simile ad "Archiviata": Pratica non operativa, visibile ma bloccata
- Differenza: Non ha protocollo né registrazione

{: .warning }
> Se vedi una pratica in stato "Rifiutata", significa che l'Ente usa ancora procedure manuali vecchie. Contatta l'ufficio per chiarimenti.

### Verificata

**Stato**: **NON TRASMESSO SU GEOTECSUE** - Uso interno Ente

**Cosa significa**: Su alcuni gestionali dell'Ente è possibile marcare una pratica come **"verificata"** dopo controllo.

**Pratiche interessate**:
- **SCIA** (Segnalazione Certificata Inizio Attività)
- **CILA** (Comunicazione Inizio Lavori Asseverata)
- Altre pratiche **non soggette a rilascio di titolo**

**Contesto normativo**:
- Queste pratiche sono **auto-certificate** dal professionista
- L'Ente può effettuare **controlli** (puntuali o a campione)
- Alcuni regolamenti prevedono controllo su percentuale minima di pratiche

**Perché NON viene trasmesso su GeoTecSUE**:

1. **Concetto interno**: La verifica è una procedura amministrativa interna all'Ente

2. **Irrilevanza per il professionista**: Il professionista non ha bisogno di conoscere se/quando l'Ente ha verificato (vale il **silenzio assenso**)

3. **Nessun effetto procedurale**: La verifica non cambia lo stato formale della pratica

**Cosa vede il professionista**:
- La pratica rimane in stato **Registrata** o **Esecutiva**
- L'eventuale verifica è trasparente e non comunicata

{: .note }
> Se il tuo gestionale mostra "Verificata" internamente, va bene. Semplicemente non viene propagato al professionista su GeoTecSUE perché non rilevante per lui.

---

## Riepilogo degli stati per categoria

### Stati operativi del professionista
- ✅ In Creazione
- ✅ In Compilazione
- ✅ Completata
- ✅ Firmata

### Stati di lavorazione Ente
- ✅ Inviata
- ✅ Protocollata
- ✅ Registrata

### Stati di integrazione
- ✅ Richiesta Integrazioni
- ✅ Invio Integrazioni
- ✅ Richiesta Archiviazione

### Stati finali
- ✅ Esecutiva (operativa, con provvedimento)
- ✅ Archiviata (chiusa)
- ✅ Diniego (respinta)
- ✅ Revoca Delegato (sospesa, in attesa nuovo professionista)

### Stati regionali (solo Piemonte - Notifica Preliminare)
- ✅ Inviata SPRESALWEB (via MUDE)
- ✅ Protocollata SPRESALWEB

### Stati deprecati/non utilizzati
- ❌ Rifiutata (deprecato)
- ❌ Verificata (non trasmesso)

---

## Prossimi passi

- [Ciclo di vita semplificato](../nozioni-di-base.html#ciclo-di-vita-di-unistanza) (nozioni di base)
- [Visualizzare il dettaglio di una pratica](../dettaglio-istanza.html)
- [Stati PagoPA](pagopa-stati.html) (appendice)

---

**Hai bisogno di chiarimenti?** Contatta l'assistenza tecnica.
