---
title: Visualizzare il dettaglio di una pratica
nav_order: 50
parent: Le mie istanze
description: Guida completa alla pagina di dettaglio delle pratiche inviate e importate - sezioni, azioni disponibili e gestione comunicazioni e integrazioni
keywords: [dettaglio pratica, visualizza pratica, comunicazioni, integrazioni, pagamenti PagoPA, ricevute, archiviazione, allegati, tracciabilità]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Visualizzare il dettaglio di una pratica

Questa sezione spiega come consultare il dettaglio completo di una pratica inviata o importata, con tutte le informazioni, i documenti e le azioni disponibili.

## Accedere al dettaglio

Per visualizzare il dettaglio di una pratica:

1. Vai all'[elenco istanze](elenco-istanze.html)
2. Nella sezione **Pratiche inviate** o **Pratiche importate**
3. Clicca sul pulsante **verde** (lente di ingrandimento) a fianco della pratica

Il sistema apre la pagina di dettaglio con tutte le informazioni e le azioni disponibili.

{: .note }
> Questa guida si applica a tutte le pratiche **tranne** la Notifica Preliminare (specifica del Piemonte), che ha un dettaglio leggermente personalizzato.

## Panoramica della pagina

La pagina di dettaglio è organizzata in sezioni che appaiono in base a:
- **Stato della pratica** (alcune sezioni appaiono solo in determinati stati)
- **Tipo di pratica** (pratiche standard vs importate)
- **Configurazione dell'Ente** (funzionalità abilitate o meno)
- **Ruolo del professionista** (principale, amministratore, utente modifica)

Le sezioni principali sono:
- Intestazione con tipo, numero e stato
- Azioni disponibili (pulsanti)
- Gestione integrazioni e comunicazioni
- Pagamenti PagoPA
- Dati della pratica e documenti
- Ricevute e tracciabilità

## Intestazione pratica

### Tipologia e numero pratica

Nella parte superiore della pagina vengono mostrati:

**A sinistra**:
- **Tipo di pratica**: es. "SCIA", "Permesso di Costruire", "Autorizzazione Paesaggistica"
- **Chiave univoca**: Il codice identificativo a 19 cifre della pratica

**A destra**:
- **Stato attuale**: stato della pratica (vedi [ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza))

### Riferimento a variante

Se durante la compilazione hai indicato che la pratica è una **variante** di una pratica precedente, in questa sezione appare un link diretto alla pratica originale.

Cliccando il link si apre il dettaglio della pratica variata.

{: .note }
> Questo collegamento è disponibile solo per pratiche standard. Le pratiche importate non mostrano riferimenti a varianti.

## Avviso: Ente non più attivo

Nel caso in cui l'Ente presso cui hai presentato la pratica abbia cessato di esistere (es. Unione sciolta, Comune confluito in altra Unione), il sistema mostra un **messaggio di avviso** che indica:

- L'Ente non è più attivo
- Eventuale indicazione del nuovo Ente in cui è confluito

{: .warning }
> Se l'Ente è variato, le funzionalità di interazione non sono disponibili (es. nuove comunicazioni, integrazioni spontanee).

## Azioni disponibili

Nella parte superiore della pagina sono presenti fino a **4 pulsanti** per compiere azioni sulla pratica. La visibilità di ciascun pulsante dipende dallo stato della pratica e dal tuo ruolo.

### Ritorna

**Sempre disponibile**

Cliccando questo pulsante torni alla pagina da cui provieni (solitamente l'[elenco istanze](elenco-istanze.html)).

### Richiedi Archiviazione

**Disponibile per**:
- Professionista principale
- Soggetti compilatori con ruolo **Amministratore**

**Disponibile se la pratica è in stato**:
- Registrata
- Esecutiva
- Verificata (anche se lo stato non è utilizzato)
- Richiesta Integrazioni

**Cosa fa**: Avvia una nuova istanza di tipo "Richiesta Archiviazione" collegata alla pratica corrente. La compilazione è analoga a quella di qualsiasi altra pratica.

**Quando usarlo**:
- La proprietà non intende proseguire con l'istanza
- Non è possibile fornire le integrazioni richieste

{: .note }
> La richiesta di archiviazione viene valutata dall'Ente, che può accettarla o respingerla. Non archivia automaticamente la pratica.

### Scarica l'archivio della pratica

**Disponibile per**: Pratiche **standard** (non importate)

**Sempre attivo** (per pratiche standard)

**Cosa fa**: Scarica un file **ZIP** contenente tutta la documentazione della pratica:

✅ **Documenti principali**:
- PDF dell'istanza (non firmato)
- PDF firmato digitalmente (se previsto)

✅ **Allegati**:
- Allegati principali della pratica (se non scaduti)
- Allegati delle comunicazioni associate (se non scaduti)
- Integrazioni protocollate (se non scadute)

✅ **Ricevute**:
- Ricevute generate dal sistema (invio, protocollo, registrazione)
- Ricevute di comunicazioni e integrazioni (invio, protocollo)

✅ **Documenti dell'Ente**:
- Tutti i documenti prodotti dall'Ente (senza scadenza)

✅ **Altri file**:
- File XML della tracciabilità
- Eventuale file di testo con errori rilevati

{: .warning }
> **Importante**: Gli allegati sono disponibili solo se non ancora scaduti (6 mesi dalla registrazione). I documenti dell'Ente non scadono mai.

{: .note }
> Questa funzionalità **non è disponibile** per le pratiche importate, che non hanno un archivio completo disponibile su GeoTecSUE.

### Gestione Soggetti

**Disponibile per**:
- Professionista principale
- Soggetti compilatori con ruolo **Amministratore**

**Cosa fa**: Apre la schermata per gestire i [soggetti compilatori](../docs/nozioni-di-base.html#soggetti-compilatori-aggiuntivi) della pratica:
- Aggiungere nuovi collaboratori
- Rimuovere collaboratori esistenti
- Modificare i ruoli (Amministratore/Utente Modifica)

## Avviso: Stati che bloccano le interazioni

Quando la pratica si trova in determinati stati, il sistema mostra un **messaggio di avviso** che indica l'impossibilità di interagire con la pratica fino al cambio di stato.

**Stati che bloccano le interazioni**:
- **Inviata**: In attesa di protocollazione da parte dell'Ente
- **Protocollata**: In attesa di registrazione
- **Invio Integrazioni**: Integrazioni trasmesse, in attesa di presa in carico

{: .note }
> Non puoi inviare comunicazioni o integrazioni spontanee finché la pratica non passa allo stato **Registrata**.

## Motivazione di archiviazione

Se la pratica è stata **archiviata** dall'Ente (o su tua richiesta accettata), questa sezione mostra:

- **Motivo dell'archiviazione**: Testo descrittivo prodotto dall'Ente che spiega le ragioni dell'archiviazione

Esempi di motivi:
- "Pratica presentata per errore"
- "Documentazione non conforme e non integrabile"
- "Richiesta archiviazione accettata su richiesta del professionista"
- "Pratica presentata allo sportello errato (SUAP invece di SUE)"

## Richiesta integrazioni attiva

Se l'Ente ha aperto una **richiesta di integrazione documentale**, questa sezione mostra tutti i dettagli e permette di caricare i documenti richiesti.

### Informazioni generali

La sezione mostra:

| Campo | Descrizione |
|-------|-------------|
| **Data Richiesta** | Data in cui l'Ente ha aperto la richiesta |
| **Descrizione** | Testo descrittivo dell'Ente che spiega cosa integrare |
| **Firma necessaria** | ✅ Spunta verde = documenti devono essere firmati digitalmente<br>❌ Croce rossa = firma non obbligatoria |
| **Dimensione massima file** | Limite in MB per singolo file |

### Documenti richiesti

Sotto le informazioni generali appare l'elenco dei documenti specifici richiesti dall'Ente.

Per ogni documento:
- **Nome documento**: es. "Relazione tecnica integrativa", "Elaborato grafico modificato"
- **Stato caricamento**: Indica se il file è già stato caricato o meno
- **Sezione di upload**: Pulsante per selezionare e caricare il file

### Caricare un documento

1. Clicca su **Sfoglia** o **Scegli file** accanto al documento richiesto
2. Seleziona il file dal tuo computer
3. Se richiesta firma digitale, carica il file **.p7m**
4. Il sistema valida dimensione e formato
5. Il file viene caricato e appare nell'elenco

### File già caricati

Se hai già caricato file, per ciascuno puoi:
- **Scaricare** il file (pulsante verde) per verificarlo
- **Eliminare** il file (pulsante rosso) se devi sostituirlo

### Documenti aggiuntivi

Se l'Ente lo consente, puoi caricare **documenti aggiuntivi** oltre a quelli esplicitamente richiesti.

Apparirà un'apposita sezione "Altri documenti" dove potrai aggiungere file liberi con una descrizione.

### Inviare l'integrazione

Una volta caricati tutti i documenti obbligatori:

1. Verifica che tutti i file richiesti siano presenti
2. Clicca sul pulsante **Invia integrazione**
3. Il sistema valida i file e li trasmette all'Ente
4. Ricevi la ricevuta di invio dell'integrazione

{: .warning }
> Dopo l'invio non potrai più modificare i file caricati. Verifica accuratamente prima di trasmettere.

## Pagamenti aperti (PagoPA)

Questa sezione mostra i pagamenti in sospeso legati alla pratica, sia quelli generati dall'Ente che quelli facoltativi disponibili.

### Pagamenti da creare (senza IUV)

Se esistono **pagamenti facoltativi** per cui non hai ancora generato il codice IUV, appaiono in una tabella:

| Colonna | Descrizione |
|---------|-------------|
| **Descrizione Pagamento** | Tipo di pagamento (es. "Diritti di Segreteria", "Oblazione Sanzione") |
| **Importo (€)** | Cifra da versare (può essere già valorizzata o da definire) |
| **Creazione IUV** | Pulsante per generare il codice di pagamento |

**Procedura**:
1. Compila eventuali campi richiesti (es. importo se da valorizzare)
2. Clicca **Creazione IUV**
3. Il sistema genera il codice IUV PagoPA
4. Il pagamento si sposta nella tabella "Pagamenti già creati"

### Pagamenti già creati (con IUV)

I pagamenti per cui è già stato generato lo IUV (dall'Ente o da te) appaiono in questa tabella:

| Colonna | Descrizione |
|---------|-------------|
| **Descrizione Pagamento** | Tipo di pagamento |
| **Rata** | Numero rata (1 se unica soluzione, 1/2/3... se dilazionato) |
| **Scadenza** | Data entro cui pagare |
| **Importo (€)** | Cifra da versare |
| **Stato** | Stato del pagamento (vedi [Stati PagoPA](appendici/pagopa-stati.html)) |
| **Dettaglio** | Pulsante azzurro per vedere i dati dello IUV |
| **Aggiorna** | Pulsante arancione per verificare l'avvenuto pagamento |

### Visualizzare i dettagli dello IUV

Cliccando il pulsante **Dettaglio** (azzurro) vedi:
- Codice IUV generato
- Scadenza
- Importo
- Eventuale avviso di scadenza (se lo IUV è scaduto)

Se lo IUV è scaduto, dovrai generarne uno nuovo.

### Aggiornare lo stato del pagamento

Dopo aver pagato tramite PagoPA:

1. Clicca il pulsante **Aggiorna** (arancione)
2. Il sistema interroga PagoPA
3. Se il pagamento è stato ricevuto, lo stato cambia in "Pagato"

{: .note }
> L'aggiornamento può richiedere alcuni minuti dopo l'effettivo pagamento. Se lo stato non cambia immediatamente, riprova dopo qualche minuto.

{: .note }
> Per la spiegazione dettagliata di tutti gli stati possibili, consulta [Appendice: Stati PagoPA](appendici/pagopa-stati.html).

## Comunicazioni verso l'Ente

Questa sezione ti permette di inviare **comunicazioni strutturate** collegate alla pratica (es. Inizio Lavori, Fine Lavori...).

La sezione si divide in due parti:
1. **Nuova Comunicazione**: Crea e invia una nuova comunicazione
2. **Comunicazioni in compilazione**: Elenco di comunicazioni salvate ma non ancora inviate

### Quando puoi inviare comunicazioni

Puoi creare nuove comunicazioni **solo se**:

✅ La pratica è in stato **Registrata** o successivi (tranne quelli bloccanti)

❌ **Non puoi** se la pratica è in stato:
- Archiviata
- Diniego
- Inviata
- Protocollata
- Rifiutata
- Richiesta Archiviazione
- Revoca Delegato

❌ **Non puoi** se l'Ente è variato (confluito in altra amministrazione)

**Caso particolare**: Se la pratica è in **Richiesta Integrazioni** o **Invio Integrazioni**, la possibilità di inviare comunicazioni dipende dalla configurazione dell'Ente (alcuni Enti lo consentono, altri no).

### Nuova Comunicazione

#### Selezionare il tipo di comunicazione

Dal menu a discesa **"Seleziona il tipo di Comunicazione"**, scegli la comunicazione che devi inviare.

Le comunicazioni disponibili dipendono da:
- Regione in cui opera l'Ente
- Tipo di pratica
- Configurazione specifica dell'Ente

**Esempi di comunicazioni tipiche**:
- Inizio Lavori
- Fine Lavori
- Segnalazione Certificata di Agibilità

{: .note }
> Se la comunicazione che cerchi non è presente nel menu, contatta l'Ente segnalando quale comunicazione ti serve. L'Ente può abilitarla se effettivamente applicabile alla tua pratica.

#### Avviare la compilazione

1. Seleziona la comunicazione dal menu
2. Clicca sul pulsante **Nuova**
3. Il sistema crea una nuova comunicazione collegata alla pratica
4. Vieni reindirizzato alla schermata di compilazione

La compilazione di una comunicazione è analoga a quella di una pratica normale.

### Comunicazioni in compilazione

Se hai avviato comunicazioni ma non ancora trasmesse, appaiono in questa lista con le stesse funzionalità dell'[elenco pratiche in compilazione](elenco-istanze.html#pratiche-in-fase-di-compilazione):

- **Modifica** (pulsante giallo): Prosegui la compilazione
- **Cancella** (pulsante rosso): Elimina la comunicazione
- **Gestione soggetti** (pulsante blu/verde): Condividi con collaboratori
- **PDF** e **P7M**: Scarica documenti generati
- **Genera PDF**: Genera il PDF se completata

### Comunicazioni sospese

Se avvii una comunicazione e successivamente la pratica cambia stato in uno dei **stati bloccanti** (es. l'Ente richiede integrazioni), la comunicazione viene **sospesa** e non sarà più visibile in questa lista.

La comunicazione riapparirà automaticamente quando la pratica tornerà in uno stato compatibile (es. Registrata dopo aver inviato le integrazioni).

{: .note }
> Le comunicazioni sospese non vengono eliminate, solo temporaneamente nascoste. Recupereranno visibilità al cambio di stato della pratica.

## Invio documentazione all'Ente (integrazioni spontanee)

Le **integrazioni spontanee** ti permettono di inviare documenti aggiuntivi all'Ente di tua iniziativa, senza che ci sia una richiesta formale.

### Disponibilità della funzione

Le integrazioni spontanee sono disponibili **solo se**:

✅ L'Ente ha **abilitato** questa funzionalità  
✅ L'Ente **non è variato**  
✅ La pratica **non è** in stato bloccante (vedi lista in "Comunicazioni")

{: .note }
> Non tutti gli Enti consentono le integrazioni spontanee. Se non vedi questa sezione, significa che l'Ente ha disabilitato la funzionalità.

### Caricare documenti

1. Clicca su **Nuovo Invio**
2. Il sistema mostra le caratteristiche richieste:
   - Firma digitale necessaria (sì/no)
   - Dimensione massima file

Per ogni file da caricare:

1. **Descrizione file** (obbligatorio): Inserisci una descrizione chiara (es. "Relazione geologica aggiuntiva", "Documentazione fotografica stato dei luoghi")
2. **Scegli file**: Seleziona il file dal computer
3. Clicca **Carica**

Il file viene aggiunto alla lista e puoi:
- **Eliminarlo** (pulsante rosso) se hai sbagliato
- **Scaricarlo** (pulsante verde) per verificarlo

### Inviare l'integrazione

Dopo aver caricato tutti i file desiderati:

1. Verifica l'elenco dei file caricati
2. Clicca sul pulsante **Invia documenti**
3. L'integrazione spontanea viene trasmessa all'Ente
4. Ricevi la ricevuta di invio

{: .warning }
> Dopo l'invio non potrai più modificare o aggiungere file a questa integrazione. Per inviare altra documentazione dovrai creare un nuovo invio.

## Dati Generali della Pratica

Questa sezione riepiloga tutte le informazioni principali della pratica.

### Informazioni di sistema

| Campo | Descrizione |
|-------|-------------|
| **Numero pratica** | Chiave univoca a 19 cifre |
| **Anno** | Anno di creazione della pratica su GeoTecSUE |
| **Stato** | Stato attuale (vedi [ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)) |
| **Tipo** | Tipologia di pratica |
| **Descrizione Intervento** | Oggetto dell'intervento come inserito in compilazione |

### Date significative

| Campo | Descrizione |
|-------|-------------|
| **Data Registrazione** | Data e ora di creazione su GeoTecSUE (utile per verificare se la pratica è stata creata prima/dopo aggiornamenti normativi) |
| **Data Ultima Modifica** | Data e ora dell'ultima modifica prima della trasmissione |
| **Data Invio** | Data e ora di trasmissione all'Ente |

### Documenti scaricabili

- **Documento istanza (non firmato)**: Scarica il PDF generato dal sistema
- **Documento istanza (firmato digitalmente)**: Scarica il PDF firmato (se previsto)

### Sezioni aggiuntive

Sotto i dati generali appaiono tre sezioni dedicate:

1. [Dati Titolare Originale](#dati-titolare-originale)
2. [Localizzazione dell'intervento](#localizzazione-dellintervento)
3. [Documentazione allegata alla pratica](#documentazione-allegata-alla-pratica)

## Dati Titolare Originale

### Anagrafica principale

Questa sezione mostra i dati del **titolare originale** della pratica:

- Cognome e Nome
- Codice Fiscale
- Data di nascita
- Luogo di nascita
- Residenza (indirizzo completo)

### Ditta/Società/Ente associata

Se al titolare è associata una persona giuridica, appare una sottosezione con:

- **Denominazione** (Ragione sociale)
- **Partita IVA**
- **Sede** (indirizzo completo)
- **Email**
- **PEC**

### Co-intestatari

Se la pratica ha **co-intestatari** (altri titolari oltre al principale), appaiono in una tabella:

| Cognome | Nome | Codice Fiscale | Data di nascita |
|---------|------|----------------|-----------------|
| Rossi | Mario | RSSMRA... | 01/01/1980 |
| Bianchi | Anna | BNCNNA... | 15/05/1975 |

### Voltura del titolare

Se è stata effettuata una **voltura** (cambio di titolare), appare la sezione **"Dati Titolari (dopo voltura)"** con una tabella:

| Cognome | Nome | Codice Fiscale | Data Richiesta | Data Conferma | Ref. PagoPA |
|---------|------|----------------|----------------|---------------|-------------|
| Verdi | Luigi | VRDLGU... | 10/03/2025 | 15/03/2025 | [Pulsante] |

**Ref. PagoPA**: Pulsante per definire o rimuovere il soggetto come **referente dei pagamenti PagoPA** (attivo/disattivo).

{: .note }
> La voltura trasferisce la titolarità della pratica a un altro soggetto. Richiede l'autorizzazione dell'Ente e deve essere richiesta formalmente.

## Localizzazione dell'intervento

Questa sezione riepiloga dove si trova l'intervento oggetto della pratica:

### Indirizzo

- **Via/Piazza** e numero civico
- **Comune** (mostrato se l'Ente è multi-comune)

### Riferimenti catastali

Se indicati in fase di compilazione, vengono mostrati i dati catastali:

**Fabbricati**:
- Foglio
- Particella (Mappale)
- Subalterno

**Terreni**:
- Foglio
- Particella (Mappale)

{: .note }
> Questa sezione **non è disponibile** per le pratiche importate, che hanno visibilità limitata sui dati di localizzazione.

## Documentazione allegata alla pratica

Questa sezione mostra tutti gli **allegati** caricati contestualmente alla pratica al momento dell'invio.

Per ogni allegato:

| Campo | Descrizione |
|-------|-------------|
| **Data Inserimento** | Quando è stato caricato |
| **Descrizione** | Nome/descrizione dell'allegato |
| **Disponibile fino al** | Data di scadenza ([retention 6 mesi](../docs/nozioni-di-base.html#un-sistema-di-transito-non-di-archiviazione)) |
| **Visualizza** | Pulsante verde per scaricare (se non scaduto) |

{: .warning }
> Gli allegati scadono dopo **6 mesi dalla registrazione**. Scarica e conserva localmente tutti i documenti importanti prima della scadenza.

{: .note }
> Questa sezione **non è disponibile** per le pratiche importate. Gli allegati originali restano archiviati dall'Ente secondo il canale di presentazione iniziale (PEC, cartaceo, altro portale).

## Dati dell'Ente

Questa sezione mostra le informazioni inserite dall'Ente durante la lavorazione della pratica.

### Informazioni base

| Campo | Descrizione |
|-------|-------------|
| **Numero Protocollo** | Numero assegnato alla protocollazione |
| **Data Protocollo** | Data di protocollazione |
| **Numero Pratica** | Numero di registrazione (se già in stato Registrata) |
| **Data Registrazione** | Data di presa in carico dall'Ufficio Tecnico |
| **Responsabile del Procedimento** | Nome del responsabile del procedimento (se indicato dall'Ente) |
| **Responsabile del Servizio** | Nome del responsabile di servizio (se indicato) |
| **Data Assegnazione** | Data di assegnazione ai responsabili |

### Sezioni aggiuntive

Sotto le informazioni base possono apparire fino a 5 sezioni dedicate (se l'Ente ha compiuto determinate azioni):

1. [Dati verifica pratica](#dati-verifica-pratica)
2. [Dati provvedimento](#dati-provvedimento)
3. [Comunicazioni](#comunicazioni-dellente)
4. [Storico richieste integrazioni](#storico-richieste-integrazioni)
5. [Agibilità](#agibilità)

## Dati verifica pratica

{: .note }
> Questa sezione **non è utilizzata** in quanto lo stato **Verificata** non viene trasmesso su GeoTecSUE. Vedi [Appendice: Ciclo di vita dettagliato](appendici/ciclo-vita-dettagliato.html#verificata) per maggiori informazioni.

## Dati provvedimento

Se l'Ente ha rilasciato un **provvedimento** (es. Permesso di Costruire, Autorizzazione Paesaggistica), questa sezione mostra:

- **Numero Provvedimento**: Numero dell'atto rilasciato
- **Data Provvedimento**: Data di emissione del provvedimento

### Documenti del provvedimento

Se l'Ente ha allegato documenti al provvedimento, appaiono in una tabella:

| Data Emissione | Descrizione | Data Lettura | Visualizza |
|----------------|-------------|--------------|------------|
| 15/01/2025 | Permesso di Costruire n. 123 | 16/01/2025 | [Pulsante verde] |
| 15/01/2025 | Elaborati grafici timbrati | - | [Pulsante verde] |

- **Data Lettura**: Quando hai scaricato il documento (vuota se non ancora scaricato)
- **Visualizza**: Pulsante verde per scaricare il documento

{: .note }
> I documenti prodotti dall'Ente **non hanno scadenza** e restano sempre disponibili su GeoTecSUE, a differenza degli allegati del professionista che scadono dopo 6 mesi.

## Comunicazioni dell'Ente

Se l'Ente ha trasmesso documentazione (es. richieste di integrazione, pareri, avvio del procedimento), questa sezione tiene traccia di tutti i documenti inviati.

### Tabella comunicazioni

| Tipo Documento | Data Emissione | Descrizione | Data Lettura | Visualizza |
|----------------|----------------|-------------|--------------|------------|
| Documento | 10/01/2025 | Avvio del procedimento | 11/01/2025 | [Verde] |
| Parere | 20/01/2025 | Parere AUSL favorevole | - | [Verde] |
| Rilascio provvedimento | 30/01/2025 | Permesso di Costruire | 31/01/2025 | [Verde] |

**Tipo Documento**:
- **Documento**: Comunicazione generica
- **Parere**: Parere di enti terzi
- **Rilascio provvedimento**: Provvedimento finale

**Data Lettura**: Indica quando hai scaricato il documento (vuota se non ancora visualizzato)

{: .note }
> I documenti dell'Ente **non scadono mai** e rimangono sempre scaricabili, sia qui che nella sezione "Dati provvedimento".

## Storico richieste integrazioni

Se l'Ente ha richiesto integrazioni documentali nel corso dell'istruttoria e tu hai risposto, questa sezione mostra lo **storico completo** di tutte le richieste concluse.

### Dati della richiesta

Per ogni richiesta di integrazione completata:

| Campo | Descrizione |
|-------|-------------|
| **Numero Pratica** | Chiave a 19 cifre della richiesta di integrazione |
| **Data Richiesta** | Quando l'Ente ha aperto la richiesta |
| **Data Invio** | Quando hai trasmesso la risposta |
| **Data Protocollo** | Data di protocollazione della risposta |
| **Numero Protocollo** | Numero di protocollo assegnato |
| **Data Accettazione** | Data in cui l'Ente ha registrato l'integrazione nella pratica |

### Documenti dell'integrazione

Sotto ogni richiesta appare l'elenco degli allegati che hai inviato in risposta:

| Data Accettazione | Allegato | Disponibile fino al | Visualizza |
|-------------------|----------|---------------------|------------|
| 25/01/2025 | Relazione tecnica integrativa.pdf | 25/07/2025 | [Verde] |
| 25/01/2025 | Elaborato grafico modificato.pdf | 25/07/2025 | [Verde] |

{: .warning }
> Gli allegati delle integrazioni seguono la stessa regola di **retention** degli allegati principali: scadono dopo 6 mesi dalla data di accettazione.

## Agibilità

{: .note }
> Questa sezione è **obsoleta** e non viene più utilizzata. Con l'introduzione della **Segnalazione Certificata di Agibilità** (SCA), le vecchie "Richiesta di Agibilità" e "Comunicazione di Agibilità" non sono più presenti. Se vedi questa sezione, si riferisce a pratiche molto vecchie.

## Comunicazioni Inviate collegate alla Pratica

Se hai trasmesso **comunicazioni strutturate** legate alla pratica (es. Inizio Lavori, Fine Lavori, Varianti), questa sezione mostra lo storico completo.

### Tabella comunicazioni

| Tipo | Numero Pratica | Data Invio | Stato | Data Protocollo | Numero Protocollo |
|------|----------------|------------|-------|-----------------|-------------------|
| Inizio Lavori | 1234567890123456789 | 05/02/2025 | Protocollata | 06/02/2025 | 1234/2025 |
| Fine Lavori | 9876543210987654321 | 20/03/2025 | Inviata | - | - |

**Campi**:
- **Tipo di comunicazione**: Tipologia (Inizio Lavori, Fine Lavori, ecc.)
- **Numero Pratica**: Chiave univoca della comunicazione
- **Data Invio**: Quando hai trasmesso la comunicazione
- **Stato**: Stato attuale della comunicazione
- **Data/Numero Protocollo**: Se già protocollata

### Allegati delle comunicazioni

Sotto ogni comunicazione appare l'elenco degli allegati trasmessi:

| Data Inserimento | Allegato | Disponibile fino al | Visualizza |
|------------------|----------|---------------------|------------|
| 05/02/2025 | Comunicazione Inizio Lavori.pdf | 05/08/2025 | [Verde] |
| 05/02/2025 | Piano Sicurezza e Coordinamento.pdf | 05/08/2025 | [Verde] |

{: .warning }
> Gli allegati delle comunicazioni scadono dopo **6 mesi dalla data di inserimento**. Conserva copie locali di tutti i documenti importanti.

## Ricevute

Questa sezione mostra tutte le **ricevute** generate automaticamente da GeoTecSUE per la pratica principale e per eventuali comunicazioni e integrazioni.

### Ricevute della pratica principale

A seconda dello stato raggiunto dalla pratica, sono disponibili:

| Ricevuta | Quando viene generata | Azioni |
|----------|----------------------|--------|
| **Ricevuta di invio** | Pochi istanti dopo la trasmissione | Scarica / Rigenera |
| **Ricevuta di protocollazione** | Dopo la protocollazione da parte dell'Ente | Scarica / Rigenera |
| **Ricevuta di registrazione** | Dopo la registrazione all'Ufficio Tecnico | Scarica / Rigenera |

### Rigenerare le ricevute

Ogni ricevuta ha un pulsante **giallo di aggiornamento** che permette di rigenerarla.

**Quando è utile rigenerare**:
- L'Ente ha corretto il numero di pratica dopo la registrazione
- L'Ente ha modificato il tipo di pratica
- Vuoi avere una ricevuta aggiornata con i dati più recenti

Il sistema rilegge i dati dal gestionale dell'Ente e genera un nuovo PDF aggiornato.

{: .note }
> Le ricevute, come i documenti dell'Ente, **non scadono mai** e sono sempre scaricabili.

### Ricevute di comunicazioni e integrazioni

Se hai inviato comunicazioni o integrazioni, appare una sezione aggiuntiva con le ricevute di:

- **Invio** della comunicazione/integrazione
- **Protocollazione** della comunicazione/integrazione

{: .note }
> Le comunicazioni e integrazioni **non** hanno ricevuta di registrazione perché ereditano il numero di pratica della pratica principale.

## Pagamenti completati (PagoPA)

Se hai effettuato pagamenti tramite **PagoPA** per la pratica o per comunicazioni collegate, questa sezione mostra lo storico completo.

### Tabella pagamenti

| Descrizione | Data Richiesta IUV | Data Pagamento | Importo (€) | Stato |
|-------------|-------------------|----------------|-------------|-------|
| Diritti di Segreteria | 05/01/2025 | 06/01/2025 | 50,00 | Pagato |
| Oneri Urbanizzazione | 05/01/2025 | 10/01/2025 | 1.500,00 | Pagato |

**Campi**:
- **Descrizione pagamento**: Tipo di pagamento effettuato
- **Data Richiesta IUV**: Quando è stato generato il codice IUV
- **Data Pagamento IUV**: Quando hai effettivamente pagato
- **Importo**: Cifra versata
- **Stato**: Stato finale (vedi [Stati PagoPA](appendici/pagopa-stati.html))

## Tracciabilità

Questa sezione mostra la **cronologia completa** di tutti gli eventi significativi della pratica, dal momento della creazione fino allo stato attuale.

### Cosa viene tracciato

La tracciabilità include **tutte le azioni** compiute sia dal professionista che dall'Ente, in ordine cronologico (dal più vecchio al più recente):

**Azioni del professionista**:
- Invio pratica all'Ente
- Invio documentazione integrativa
- Generazione IUV per pagamenti
- Trasmissione comunicazioni

**Azioni dell'Ente**:
- Pratica protocollata con Numero X
- Pratica registrata con Numero Y
- Pubblicazione documento Z
- Richiesta integrazioni aperta
- Provvedimento rilasciato

**Esempio di tracciabilità**:
```
10/01/2025 10:30 - Invio pratica all'Ente
10/01/2025 14:15 - Pratica Protocollata con Numero 1234/2025
15/01/2025 09:00 - Pratica Registrata con Numero 567/2025
20/01/2025 11:30 - Richiesta integrazioni aperta
25/01/2025 16:00 - Invio documentazione all'Ente: Relazione tecnica integrativa
26/01/2025 10:00 - Pubblicazione documento: Parere favorevole AUSL
30/01/2025 15:30 - Generazione IUV 123456789 per Diritti di Segreteria dell'importo di 50 Euro
05/02/2025 14:00 - Rilascio provvedimento: Permesso di Costruire n. 123

04/03/2025 09:33:13	Invio pratica all'Ente
04/03/2025 09:39:15  Pratica Protocollata con Numero 1234/2025
05/03/2025 10:01:19  Pratica Registrata con Numero 567/2025
09/03/2025 15:30:18  Generazione IUV 123456789 per Diritti di Segreteria dell'importo di 50 Euro
12/03/2025 19:05:57	Invio comunicazione all'Ente: Invio documentazione libera
13/03/2025 10:12:29	[Comunicazione - Invio documentazione libera]: Comunicazione Protocollata con Numero 2763
13/03/2025 10:16:24	[Comunicazione - Invio documentazione libera]: Comunicazione Registrata in Pratica Numero 2022/12/1
26/03/2025 10:00:44  Pubblicazione documento: Parere favorevole AUSL
28/03/2025 15:48:04	ROSSI MARIO ha aggiunto VERDI IRENE alla gestione della pratica con ruolo: Amministratore

```

{: .note }
> La tracciabilità è utile per avere una visione d'insieme dell'iter della pratica e verificare quando sono avvenuti eventi specifici.

## Interoperabilità Regione Lombardia

{: .note }
> Questa sezione riguarda **esclusivamente** gli Enti della Regione Lombardia che operano in **interoperabilità** con il sistema regionale.

Se l'Ente lombardo ha attivato l'interoperabilità, questa sezione mostra tutte le operazioni di dialogo tra GeoTecSUE e il sistema di Regione Lombardia.

### Tabella trasmissioni

| Fase Aggiornamento | Cod. Pratica R.L. | ID R.L. | ID Int. R.L. | Proc. R.L. | Data Trasmissione |
|-------------------|-------------------|---------|--------------|------------|-------------------|
| Primo Aggiornamento | RSSMRA80A01F205X-20250110-103045 | 12345 | - | SCIA | 10/01/2025 10:30 |
| Integrazioni | RSSMRA80A01F205X-20250110-103045 | 12345 | 67890 | SCIA | 25/01/2025 16:00 |

**Campi**:
- **Fase di Aggiornamento**: Primo Aggiornamento, Integrazioni, Aggiornamento Finale
- **Cod. Pratica R.L.**: Codice generato da GeoTecSUE (formato: CodiceFiscale-Data-Ora)
- **ID R.L.**: Identificativo assegnato da Regione Lombardia
- **ID Int. R.L.**: Identificativo integrazione (se la trasmissione riguarda un'integrazione)
- **Proc. R.L.**: Tipo di procedimento secondo nomenclatura regionale
- **Data Trasmissione**: Quando è avvenuto lo scambio dati

{: .note }
> Se non vedi questa sezione e operi in Lombardia, significa che l'Ente non ha attivato l'interoperabilità con Regione Lombardia.

---

# Differenze per pratiche importate

Le pratiche importate (presentate prima dell'attivazione di GeoTecSUE) hanno un dettaglio molto simile a quello delle pratiche standard, con alcune differenze descritte di seguito.

## Sezione aggiuntiva: Dati Importazione della Pratica

Le pratiche importate mostrano una sezione dedicata ai **dati di importazione** non presente nelle pratiche standard.

### Informazioni dall'importazione

| Campo | Descrizione |
|-------|-------------|
| **Data Importazione** | Data e ora in cui hai importato la pratica su GeoTecSUE |
| **Numero Pratica** | Numero pratica come registrato nel gestionale dell'Ente |
| **Numero Protocollo** | Numero di protocollo originale |
| **Data Protocollo** | Data di protocollazione originale |
| **Tipo Pratica** | Tipologia come registrata nel gestionale |
| **Qualificazione Intervento** | Qualificazione come registrata nel gestionale |
| **Oggetto Intervento** | Descrizione dell'intervento originale |
| **Titolare** | Nome e cognome del titolare |
| **Codice Fiscale** | Codice fiscale del titolare |

### Dati del portale di origine (se disponibili)

Se il gestionale trasmette informazioni sul portale attraverso cui la pratica fu presentata, appare anche:

| Campo | Descrizione |
|-------|-------------|
| **Portale** | Nome del portale di riferimento (es. nome del vecchio portale) |
| **Tipo Istanza** | Tipologia secondo nomenclatura del portale originale |
| **Numero Istanza** | Numero identificativo sul portale originale |

{: .note }
> Questi dati sono utili per rintracciare la pratica nei sistemi precedenti o nelle comunicazioni con l'Ente che fanno riferimento al vecchio portale.

## Funzionalità non disponibili

Le pratiche importate hanno alcune **limitazioni** rispetto alle pratiche standard:

### Completamente assenti

❌ **Riferimenti a varianti**: Non è possibile vedere se la pratica importata è variante di un'altra

❌ **Scarica archivio completo**: Non è disponibile il download del file ZIP con tutta la documentazione

❌ **Comunicazioni verso l'Ente**: Non puoi inviare nuove comunicazioni (es. Inizio/Fine Lavori)

❌ **Integrazioni spontanee**: Non puoi inviare documentazione aggiuntiva di tua iniziativa

❌ **Pagamenti PagoPA**: Non puoi generare codici IUV o effettuare pagamenti

❌ **Interoperabilità Regione Lombardia**: Non è gestita per pratiche pregresse

### Parzialmente disponibili

⚠️ **Dati Generali della Pratica**: Versione semplificata che mostra solo le informazioni base

**Mancano**:
- Sezione "Localizzazione dell'intervento"
- Sezione "Documentazione allegata alla pratica"

**Disponibili**:
- Informazioni di sistema (numero, anno, stato, tipo)
- Date significative (importazione, protocollo originale)
- Dati del titolare originale

### Funzionalità disponibili

Nonostante le limitazioni, sulle pratiche importate puoi comunque:

✅ **Visualizzare** tutti i dati generali disponibili  
✅ **Consultare ricevute** generate dal sistema  
✅ **Gestire soggetti compilatori** per condividere la visibilità  
✅ **Richiedere archiviazione** se la pratica non serve più  
✅ **Consultare la tracciabilità** delle operazioni  
✅ **Rispondere a richieste di integrazione** se l'Ente le apre

{: .note }
> Le limitazioni dipendono dal fatto che la pratica è stata presentata fuori da GeoTecSUE. Il sistema ha visibilità parziale sui dati originali, che restano archiviati dall'Ente secondo il canale di presentazione iniziale (PEC, cartaceo, altro portale).

## Perché importare una pratica pregressa

Anche con le limitazioni, importare una pratica può essere utile per:

✅ **Centralizzare** tutte le tue pratiche in un unico portale  
✅ **Rispondere a integrazioni** richieste dall'Ente dopo l'importazione  
✅ **Consultare lo stato** aggiornato della pratica  
✅ **Scaricare ricevute** e documenti dell'Ente  
✅ **Avere visibilità** sulle pratiche in corso anche se presentate prima di GeoTecSUE

Per maggiori informazioni sull'importazione, consulta [Importazione pratiche pregresse](non-presenti-geotecsue.html).

---

## Domande frequenti

### Posso modificare i dati di una pratica già inviata?

**No**, i dati di una pratica trasmessa **non sono modificabili**. 

Se devi correggere errori o aggiornare informazioni:
- Invia una **Comunicazione** (es. Voltura Professionisti / Imprese)
- Rispondi a una **richiesta di integrazione** se l'Ente ne apre una
- Invia **integrazioni spontanee** se l'Ente le consente

### Come faccio a sapere se devo pagare qualcosa?

Controlla la sezione **"Pagamenti aperti"**. Se è presente, mostra tutti i pagamenti in sospeso.

Se non vedi questa sezione, non ci sono pagamenti aperti per la pratica.

### Cosa devo fare quando vedo "Richiesta Integrazioni" nello stato?

1. Vai alla sezione **"Richiesta integrazioni attiva"**
2. Leggi attentamente cosa richiede l'Ente
3. Carica tutti i documenti obbligatori
4. Clicca **Invia integrazione**

Non aspettare troppo: le integrazioni hanno spesso termini da rispettare.
Molto spesso la richiesta di integrazioni è "accompagnata" da un documento: consulta il documento per avere il dettaglio della richiesta.

### Le ricevute hanno una scadenza?

**No**, le ricevute **non scadono mai** e restano sempre disponibili per il download.

Lo stesso vale per i **documenti prodotti dall'Ente** (pareri, provvedimenti, comunicazioni).

### Quanto tempo ho prima che scadano gli allegati?

Gli allegati caricati dal professionista (tuoi documenti) scadono **6 mesi dalla data di registrazione** della pratica.

Dopo la scadenza non potrai più scaricarli da GeoTecSUE. Conserva sempre copie locali.

### Posso delegare un collega a gestire la pratica?

**Sì**, usa il pulsante **Gestione Soggetti** per aggiungere collaboratori.

Puoi assegnare due ruoli:
- **Amministratore**: Controllo completo (tranne gestione soggetti)
- **Utente Modifica**: Può modificare dati e aggiungere allegati ma non inviare

Vedi [Soggetti compilatori](../docs/nozioni-di-base.html#soggetti-compilatori-aggiuntivi) per maggiori dettagli.

### Come faccio a scaricare tutta la documentazione in una volta?

Clicca sul pulsante **Scarica l'archivio della pratica** (se disponibile).

Riceverai un file ZIP con tutti i documenti, allegati e ricevute.

{: .warning }
> Questa funzione **non è disponibile** per le pratiche importate.

### Cosa significa "Ente variato"?

Significa che l'Ente presso cui hai presentato la pratica ha cessato di esistere (es. Comune confluito in Unione, Unione sciolta).

Se l'Ente è variato:
- Non puoi inviare nuove comunicazioni
- Non puoi inviare integrazioni spontanee
- Puoi solo consultare i dati e rispondere a eventuali richieste formali

## Prossimi passi

- [Consultare l'elenco delle istanze](elenco-istanze.html)
- [Creare una nuova istanza](nuova-istanza.html)
- [Importare pratiche pregresse](non-presenti-geotecsue.html)

---

**Hai bisogno di aiuto?** Contatta l'assistenza tecnica.
