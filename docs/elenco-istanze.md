---
title: Consultare l'elenco delle pratiche
nav_order: 40
parent: Le mie istanze
description: Come consultare e gestire gli elenchi delle pratiche in compilazione, inviate e importate su GeoTecSUE
keywords: [elenco istanze, lista pratiche, compilazione, inviate, importate, filtri, ricerca, ordinamento, stati]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Consultare l'elenco delle pratiche

Questa sezione spiega come consultare e gestire i tuoi elenchi di pratiche su **GeoTecSUE**. Il portale organizza le istanze in tre liste separate in base al loro stato di avanzamento.

## Tre elenchi per tre fasi

**GeoTecSUE** divide le tue pratiche in tre liste distinte per facilitarne la gestione:

### 1. Pratiche in fase di compilazione
Istanze che stai ancora preparando e non hai ancora inviato all'Ente. Puoi modificarle, cancellarle o completarle per l'invio.

**Quando consultarla**: Per riprendere la compilazione di pratiche salvate, completare campi mancanti o inviare istanze pronte.

### 2. Pratiche inviate
Istanze già trasmesse all'Ente (da "Inviata" in poi). Sono in lavorazione dall'Ente o già concluse.

**Quando consultarla**: Per monitorare lo stato delle pratiche, inviare comunicazioni, rispondere a richieste di integrazione, scaricare documentazione (inviata dall'Ente) oppure le ricevute prodotte.

### 3. Pratiche importate
Istanze presentate **prima dell'attivazione di GeoTecSUE** (via PEC, cartaceo o altri portali) e recuperate dal gestionale dell'Ente.

{: .note}
> Se nel menu "Le mie istanze" trovi la voce "Gestione Istanze non presenti su GeoTecSUE" allora significa che l'Ente ha abilitato la funzione e pertanto potrai importare delle pratiche pregresse. Se la voce di menu non è presente significa che l'Ente non ha abilitato la funzione

**Quando consultarla**: Per gestire pratiche pregresse, inviare comunicazioni su lavori in corso o rispondere a integrazioni.

{: .note }
> Ogni lista ha colonne e filtri specifici adatti alla fase della pratica. Passa da una lista all'altra usando le schede nella parte superiore della pagina.

## Pratiche in fase di compilazione

### Cosa mostra

Questa sezione visualizza tutte le istanze salvate ma **non ancora inviate** all'Ente. Include:
- Pratiche appena create
- Pratiche in corso di compilazione
- Pratiche completate ma non ancora firmate
- Pratiche firmate ma non ancora trasmesse

### Colonne dell'elenco

| Colonna | Icona | Colore | Funzione |
|---------|-------|--------|----------|
| **Modifica** | Matita | Giallo | Accedi alla pratica per proseguire la compilazione o modificare i dati |
| **Cancella** | Cestino | Rosso | Elimina definitivamente la pratica (richiede conferma) |
| **Gestione soggetti** | Persona | Blu/Verde* | Aggiungi o rimuovi [collaboratori](../docs/nozioni-di-base.html#soggetti-compilatori-aggiuntivi) |
| **PDF generato** | Documento PDF | - | Scarica il PDF dell'istanza se già generato (altrimenti vuoto) |
| **P7M firmato** | File P7M | - | Scarica il PDF firmato digitalmente se già caricato (altrimenti vuoto) |
| **Tipo** | - | - | Tipologia di pratica (es. SCIA, Permesso di Costruire) |
| **Data Registrazione** | - | - | Data in cui l'istanza è stata creata |
| **Titolare** | - | - | Cognome e nome del titolare (se già indicato) |
| **Stato Pratica** | - | - | Stato attuale ([vedi ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)) |
| **Genera PDF** | Pulsante | Blu | Genera il PDF dell'istanza (appare solo se pratica Completata) |
| **P7M** | Caricamento | Giallo | Consente il caricamento del file firmato digitalmente |
| **Invio** | Pulsante | Verde | Se la pratica è pronta per l'invio, è presente il pulsante "Invia" per trasmettere l'istanza

**\* Il pulsante "Gestione soggetti" è**:
- **Blu** se non hai ancora aggiunto collaboratori
- **Verde** se almeno un collaboratore è già presente

{: .note }
> Per approfondire le azioni disponibili (modifica, cancellazione, gestione soggetti), consulta [Interfaccia e convenzioni](../docs/interfaccia-e-convenzioni.html).

### Indicatori visivi (badge)

Le pratiche pronte per l'invio sono evidenziate con uno **sfondo verde**:

🟢 **Verde**: La pratica è **Completata** o **Firmata** (a seconda delle impostazioni dell'Ente) ed è pronta per essere trasmessa

Questo ti aiuta a identificare immediatamente quali pratiche puoi inviare.

### Ordinamento

Le pratiche sono ordinate per **Data Registrazione** (dalla più recente), ma puoi cambiare l'ordinamento cliccando sulle intestazioni delle colonne:

- **Tipo**: Ordine alfabetico per tipologia
- **Titolare**: Ordine alfabetico per cognome
- **Stato Pratica**: Raggruppamento per stato
- **Data Registrazione**: Cronologico (più recente o più vecchia)

{: .note }
> Clicca di nuovo sulla stessa colonna per invertire l'ordine (crescente/decrescente).

### Paginazione

Il sistema visualizza **25 pratiche per pagina** (impostazione predefinita).

Puoi modificare il numero di risultati per pagina selezionando:
- **10** pratiche
- **25** pratiche (predefinito)
- **50** pratiche
- **100** pratiche

Usa i pulsanti di navigazione in fondo alla lista per spostarti tra le pagine.

### Azioni disponibili

Da questa lista puoi:

✅ **Modificare** una pratica per proseguire la compilazione  
✅ **Cancellare** una pratica che non ti serve più  
✅ **Gestire i collaboratori** per condividere la compilazione  
✅ **Generare il PDF** per pratiche completate  
✅ **Scaricare PDF e P7M** già generati

{: .warning }
> **Attenzione**: La cancellazione è **definitiva e irreversibile**. Il sistema ti chiederà conferma prima di procedere.

Se il bottone di cancellazione della pratica non è attivo, probabilmente è dovuto al fatto che per quella pratica è stato generato uno (o più) IUV e pertanto finché non vengono eliminati gli IUV non è possibile procedere con la cancellazione.

## Pratiche inviate

### Cosa mostra

Questa sezione visualizza tutte le istanze **trasmesse all'Ente**, indipendentemente dal loro stato successivo. Include pratiche:

- **Inviate** (in attesa di protocollazione)
- **Protocollate** (protocollate ma non ancora registrate)
- **Registrate** (prese in carico dall'Ente)
- **In richiesta integrazioni** (l'Ente ha chiesto documenti aggiuntivi)
- **In invio integrazioni** (le integrazioni sono in attesa di essere registrate)
- **Esecutive** (provvedimento rilasciato)
- **Archiviate** o in **Diniego** (concluse negativamente)

### Colonne dell'elenco

| Colonna | Icona | Colore | Funzione |
|---------|-------|--------|----------|
| **Nascondi/Mostra** | Occhio/Divieto | Rosso/Azzurro | Nascondi o mostra la pratica nell'elenco (reversibile) |
| **Ricevuta invio** | Biglietto | Verde | Scarica la ricevuta di invio (clessidra se non ancora disponibile) |
| **Tipo** | - | - | Tipologia di pratica trasmessa |
| **Data Invio** | - | - | Data di trasmissione all'Ente |
| **Titolare** | - | - | Cognome e nome del titolare |
| **Stato Pratica** | - | - | Stato attuale (da Inviata in poi) ([vedi ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)) |
| **Descrizione Intervento** | - | - | Oggetto dell'intervento (passa il mouse per testo completo) |
| **Dettaglio** | Lente | Verde | Accedi al [dettaglio completo](dettaglio-istanza.html) della pratica |

### Indicatori visivi (badge di stato)

Gli stati delle pratiche inviate sono evidenziati con colori diversi per identificarli rapidamente:

🟡 **Giallo**: La pratica è in **Richiesta Integrazioni** (devi caricare documenti richiesti dall'Ente)  
🟢 **Verde**: La pratica è **Esecutiva** (provvedimento rilasciato, pratica conclusa positivamente)  
🔴 **Rosso**: La pratica è **Archiviata** o in **Diniego** (conclusa negativamente)

Gli altri stati (Inviata, Protocollata, Registrata) appaiono senza colorazione particolare.

{: .note }
> Il badge giallo indica che devi agire: accedi al dettaglio per vedere quali documenti caricare.

### Funzione Nascondi/Mostra

Puoi **nascondere** pratiche dall'elenco per ridurre il disordine visivo (utile per pratiche molto vecchie o concluse che non consulti spesso).

**Come funziona**:
- Clicca il pulsante **azzurro** per nascondere una pratica → sparisce dalla lista
- Le pratiche nascoste non vengono eliminate, solo temporaneamente invisibili
- Spunta "Includi le pratiche nascoste" nei filtri per vederle di nuovo
- Clicca il pulsante **rosso** per mostrare nuovamente una pratica nascosta

{: .note }
> Nascondere una pratica non la cancella e non influenza la sua visibilità per l'Ente. È solo un filtro visivo personale.

### Ordinamento

Le pratiche sono ordinate per **Data Invio** (dalla più recente), ma puoi cambiare l'ordinamento cliccando sulle intestazioni delle colonne:

- **Tipo**: Ordine alfabetico per tipologia
- **Data Invio**: Cronologico (più recente o più vecchia)
- **Titolare**: Ordine alfabetico per cognome
- **Stato Pratica**: Raggruppamento per stato
- **Descrizione Intervento**: Ordine alfabetico per oggetto

### Paginazione

Come per le pratiche in compilazione:
- **25 pratiche per pagina** (predefinito)
- Modificabile in 10, 50 o 100 pratiche
- Navigazione tra le pagine in fondo alla lista

### Filtri di ricerca

Per trovare rapidamente una pratica specifica, usa il pannello filtri che ti permette di combinare più criteri.

#### Filtri disponibili

| Filtro | Descrizione | Come usarlo |
|--------|-------------|-------------|
| **Dalla data di invio** | Data iniziale | Mostra pratiche inviate da questa data in poi |
| **Alla data di invio** | Data finale | Mostra pratiche inviate fino a questa data |
| **Tipo di pratica** | Tipologia | Seleziona una tipologia specifica (es. solo SCIA) |
| **Stato della pratica** | Stato attuale | Filtra per stato (es. solo Registrate o solo Esecutive) |
| **Tipo Condivisione** | Ruolo | Filtra per [ruolo](../docs/nozioni-di-base.html#soggetti-compilatori-aggiuntivi): Professionista Principale, Amministratore, Utente Modifica |
| **Includi pratiche nascoste** | Checkbox | Spunta per visualizzare anche le pratiche nascoste |
| **Comune** | Selezione Comune | Solo per Enti multi-comune (Unioni, Comunità...) |
| **Titolare** | Testo libero | Cerca per nome/cognome del titolare |
| **Chiave della pratica** | Codice 19 cifre | Cerca per codice univoco dell'istanza |

#### Come usare i filtri

1. Compila uno o più campi filtro
2. I filtri si **combinano** tra loro (es. SCIA + Registrate + Titolare Rossi = solo SCIA registrate del sig. Rossi)
3. Clicca **"Filtra i risultati"**
4. Il sistema aggiorna l'elenco mostrando solo le pratiche che corrispondono

{: .note }
> I menu a discesa mostrano solo le opzioni effettivamente presenti nelle tue pratiche. Se non vedi una tipologia, significa che non hai mai inviato quella tipologia di pratica.

#### Esempi pratici di filtro

**Caso 1: Trovare tutte le pratiche in attesa di integrazioni**
- Imposta "Stato della pratica" = **Richiesta Integrazioni**
- Clicca "Filtra i risultati"
- Risultato: Solo le pratiche che richiedono il tuo intervento

**Caso 2: Trovare tutte le SCIA del sig. Rossi**
- Imposta "Tipo di pratica" = **SCIA**
- Inserisci "Titolare" = **Rossi**
- Clicca "Filtra i risultati"

**Caso 3: Vedere tutte le pratiche inviate a gennaio 2025**
- Imposta "Dalla data di invio" = **01/01/2025**
- Imposta "Alla data di invio" = **31/01/2025**
- Clicca "Filtra i risultati"

**Caso 4: Trovare una pratica specifica tramite chiave**
- Inserisci "Chiave della pratica" = **1234567890123456789**
- Clicca "Filtra i risultati"
- Risultato: La singola pratica con quel codice

{: .note }
> Per rimuovere i filtri e vedere di nuovo tutte le pratiche, puoi cliccare il bottone "Cancella i filtri" ed operare nuovamente la ricerca.

### Azioni disponibili

Da questa lista puoi:

✅ **Accedere al dettaglio** per vedere tutte le informazioni  
✅ **Scaricare la ricevuta di invio** (e altre ricevute dal dettaglio)  
✅ **Nascondere pratiche** per tenere l'elenco ordinato  
✅ **Filtrare e cercare** pratiche specifiche

Per azioni più complesse (inviare comunicazioni, caricare integrazioni, effettuare pagamenti), devi accedere al [dettaglio della pratica](dettaglio-istanza.html).

## Pratiche importate

### Cosa mostra

Questa sezione visualizza le istanze **importate dal gestionale dell'Ente**, ossia pratiche presentate prima dell'attivazione di GeoTecSUE tramite altri canali (PEC, cartaceo, altri portali) ed importate via importazione.

Per maggiori dettagli sull'importazione, consulta [Importazione pratiche pregresse](non-presenti-geotecsue.html).

### Colonne dell'elenco

| Colonna | Descrizione |
|---------|-------------|
| **Tipo** | Tipologia della pratica come registrata nel gestionale (potrebbe differire dalle tipologie GeoTecSUE) |
| **Data Importazione** | Data in cui hai importato la pratica su GeoTecSUE |
| **Data Protocollo** | Data di protocollazione originale della pratica |
| **Titolare** | Cognome e nome del titolare |
| **Stato Pratica** | Stato attuale ([vedi ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)) |
| **Descrizione Intervento** | Oggetto dell'intervento (passa il mouse per testo completo) |
| **Dettaglio** | Pulsante verde per accedere al [dettaglio completo](dettaglio-istanza.html) |

### Indicatori visivi (badge di stato)

Come per le pratiche inviate, gli stati sono colorati:

🟡 **Giallo**: **Richiesta Integrazioni**  
🟢 **Verde**: **Esecutiva**  
🔴 **Rosso**: **Archiviata** o **Diniego**

### Ordinamento

Le pratiche sono ordinate per **Data Importazione** (dalla più recente), ma puoi cambiare l'ordinamento cliccando sulle intestazioni:

- **Tipo**: Ordine alfabetico per tipologia
- **Data Importazione**: Cronologico (più recente o più vecchia)
- **Data Protocollo**: Cronologico della protocollazione originale
- **Titolare**: Ordine alfabetico per cognome
- **Stato Pratica**: Raggruppamento per stato
- **Descrizione Intervento**: Ordine alfabetico per oggetto

### Paginazione

Stesso comportamento delle altre liste:
- **25 pratiche per pagina** (predefinito)
- Modificabile in 10, 50 o 100
- Navigazione tra le pagine

### Filtri di ricerca

#### Filtri disponibili

| Filtro | Descrizione |
|--------|-------------|
| **Dalla data di protocollo** | Data protocollo iniziale (protocollazione originale) |
| **Alla data di protocollo** | Data protocollo finale |
| **Dalla data di importazione** | Data importazione iniziale (quando l'hai importata su GeoTecSUE) |
| **Alla data di importazione** | Data importazione finale |
| **Tipo di pratica** | Tipologia come registrata nel gestionale (potrebbe differire dalle tipologie GeoTecSUE) |
| **Stato della pratica** | Stato attuale (da Registrata in poi) ([vedi ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)) |
| **Titolare** | Cerca per nome/cognome del titolare |

{: .note }
> Le pratiche importate partono sempre dallo stato **Registrata** o successivi, perché sono pratiche già protocollate e registrate dall'Ente.

#### Esempi pratici di filtro

**Caso 1: Pratiche importate nell'ultimo mese**
- Imposta "Dalla data di importazione" = **[un mese fa]**
- Clicca "Filtra i risultati"

**Caso 2: Pratiche protocollate nel 2023 che richiedono integrazioni**
- Imposta "Dalla data di protocollo" = **01/01/2023**
- Imposta "Alla data di protocollo" = **31/12/2023**
- Imposta "Stato della pratica" = **Richiesta Integrazioni**
- Clicca "Filtra i risultati"

### Azioni disponibili

Da questa lista puoi:

✅ **Accedere al dettaglio** della pratica  
✅ **Filtrare e cercare** pratiche specifiche  
✅ **Consultare lo stato** delle pratiche pregresse

Per inviare comunicazioni, integrazioni o effettuare pagamenti sulle pratiche importate, accedi al [dettaglio della pratica](dettaglio-istanza.html).

## Consigli pratici

### Tieni ordinato l'elenco delle pratiche inviate

- **Nascondi** le pratiche molto vecchie o concluse che non consulti più
- Usa i **filtri** per trovare rapidamente ciò che cerchi
- **Ordina per stato** per vedere immediatamente le pratiche che richiedono la tua attenzione (gialle)

### Monitora le pratiche in compilazione

- Le pratiche con **sfondo verde** sono pronte per l'invio
- Controlla periodicamente l'elenco per completare pratiche lasciate a metà
- **Cancella** le bozze non più necessarie per evitare confusione

### Sfrutta i filtri per gestire molte pratiche

Se gestisci molte istanze contemporaneamente:
- Filtra per **Titolare** per vedere tutte le pratiche di un cliente
- Filtra per **Stato** per concentrarti su pratiche che richiedono azione
- Usa la **Chiave** quando l'Ente ti comunica il codice della pratica

### Controlla i badge colorati

I colori ti aiutano a identificare rapidamente le priorità:
- 🟡 **Giallo** = Devi agire (integrazioni richieste)
- 🟢 **Verde** = Tutto ok (pratica pronta o esecutiva)
- 🔴 **Rosso** = Pratica conclusa (archiviata o diniego)

## Domande frequenti

### Come faccio a vedere solo le pratiche che richiedono la mia attenzione?

Usa i filtri:
- Nelle **Pratiche inviate**, filtra per stato **"Richiesta Integrazioni"**
- Oppure cerca visivamente i **badge gialli** scorrendo l'elenco

### Cosa succede se cancello una pratica in compilazione?

La pratica viene **eliminata definitivamente** e non è possibile recuperarla.

{: .warning }
> Prima di cancellare, assicurati di non averne più bisogno. Il sistema chiederà conferma, ma una volta confermata l'operazione è irreversibile.

### Le pratiche nascoste sono visibili all'Ente?

**Sì**, nascondere una pratica dall'elenco è solo un **filtro visivo personale** che non influenza:
- La visibilità per l'Ente
- Lo stato della pratica
- Le comunicazioni o integrazioni

Puoi sempre mostrarle di nuovo spuntando "Includi le pratiche nascoste" nei filtri.

### Qual è la differenza tra "Data Registrazione" e "Data Invio"?

- **Data Registrazione** (pratiche in compilazione): Data in cui hai **creato** l'istanza su GeoTecSUE (può essere giorni o settimane prima dell'invio)
- **Data Invio** (pratiche inviate): Data in cui hai **trasmesso** l'istanza all'Ente

### Quanto tempo rimangono visibili le pratiche negli elenchi?

- **Pratiche in compilazione**: Rimangono visibili finché non le invii o le cancelli (nessun limite di tempo)
- **Pratiche inviate**: Rimangono sempre visibili, indipendentemente dal loro stato o dalla loro età
- **Pratiche importate**: Rimangono sempre visibili dopo l'importazione

{: .note }
> Ricorda però che i documenti caricati su pratiche inviate vengono conservati solo per [6 mesi dalla registrazione](../docs/nozioni-di-base.html). Scarica e conserva localmente i documenti importanti.

### Posso selezionare più pratiche contemporaneamente?

**No**, non è possibile selezionare più pratiche insieme perché ogni azione richiede di accedere al dettaglio specifico della singola pratica.

Per lavorare su più pratiche devi:
- Accedere al dettaglio di ciascuna separatamente
- Completare l'azione necessaria (comunicazione, integrazione, ecc.)
- Tornare all'elenco e passare alla pratica successiva

## Prossimi passi

- [Visualizzare il dettaglio di una pratica](dettaglio-istanza.html)
- [Creare una nuova istanza](nuova-istanza.html)
- [Importare pratiche pregresse](non-presenti-geotecsue.html)

---
**Hai bisogno di aiuto?** Consulta la sezione [Interfaccia e convenzioni](interfaccia-e-convenzioni.html) per capire meglio i pulsanti e le icone, oppure contatta l'assistenza tecnica.
