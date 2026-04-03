---
title: Nozioni di base
nav_order: 20
parent: Introduzione
description: Concetti fondamentali di GeoTecSUE - tipologie di istanze, ciclo di vita e gestione dei professionisti
keywords: [istanza, pratica, comunicazione, integrazione, ciclo di vita, stati, professionista principale, soggetti compilatori, retention]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Nozioni di base

Questa sezione introduce i concetti fondamentali per utilizzare **GeoTecSUE** in modo efficace.

## Cos'è GeoTecSUE

**GeoTecSUE** è la piattaforma web per la trasmissione telematica delle pratiche edilizie alla Pubblica Amministrazione.

### Un sistema di transito, non di archiviazione

**Importante**: GeoTecSUE è un sistema di **transito**, non di conservazione documentale. 

I documenti trasmessi rimangono disponibili sulla piattaforma per **6 mesi dalla data di registrazione** dell'istanza, dopodiché vengono automaticamente eliminati. È responsabilità del professionista conservare localmente copia della documentazione inviata.

{: .warning }
> **Conservazione temporanea**: Tutti gli allegati caricati saranno eliminati dopo 6 mesi dalla registrazione. Conserva sempre una copia locale dei tuoi documenti.

### Funzionalità principali

Con GeoTecSUE puoi:

- **Compilare e trasmettere** istanze edilizie
- **Rispondere** a richieste di integrazione documentale
- **Inviare comunicazioni** associate alle pratiche (es. inizio lavori, fine lavori)
- **Monitorare** in tempo reale lo stato delle tue pratiche
- **Consultare** lo storico delle istanze trasmesse
- **Gestire anagrafiche** di richiedenti, professionisti e imprese

## Tipologie di istanze

Nel portale esistono tre tipologie di istanze. Ogni istanza è identificata da un **codice univoco di 19 cifre** (la "chiave") assegnato automaticamente al momento della creazione e mai modificato durante il ciclo di vita.

### Pratica

La **pratica** è un'istanza autonoma che avvia un procedimento amministrativo indipendente.

**Esempi**: Permesso di Costruire, SCIA, CILA, Autorizzazione Paesaggistica.

**Caratteristiche**:
- Vive di "luce propria" senza dipendere da altre istanze
- Ha un proprio iter amministrativo completo
- Viene protocollata e registrata autonomamente dall'Ente
- Può contenere comunicazioni e integrazioni collegate

### Comunicazione

La **comunicazione** è un'istanza collegata a una pratica già esistente e ne definisce eventi specifici del ciclo edilizio.

**Esempi**: Inizio Lavori, Fine Lavori.

**Caratteristiche**:
- Richiede sempre una pratica "genitore" già esistente
- Non può essere creata in modo autonomo
- Non ha una registrazione indipendente
- Segue il ciclo di vita della pratica principale

{: .note }
> Una comunicazione non può esistere senza una pratica di riferimento. Una comunicazione non può essere creata fino a che la pratica principale non è stata almeno registrata dall'Ente.

### Integrazione

L'**integrazione** fornisce documentazione aggiuntiva richiesta dall'Ente o inviata spontaneamente dal professionista durante l'istruttoria.

**Tipologie**:
- **Integrazione richiesta**: l'Ente ha aperto formalmente una richiesta di integrazione documentale
- **Integrazione spontanea**: il professionista aggiunge documenti di propria iniziativa per completare la pratica

**Caratteristiche**:
- Come la comunicazione, richiede una pratica esistente
- Può essere inviata solo se la pratica è in stato "Registrata" o successivi
- La possibilità di inviare integrazioni spontanee dipende dalle impostazioni dell'Ente

{: .warning }
> **Verifica con il tuo Ente**: Alcuni Enti disabilitano le integrazioni spontanee. Controlla le impostazioni specifiche o contatta l'ufficio competente prima di procedere.

## Ciclo di vita di un'istanza

Ogni istanza attraversa diversi stati durante il suo percorso, dalla creazione alla chiusura. Di seguito gli stati principali che incontrerai più frequentemente.

### Stati di lavorazione del professionista

**In Creazione**  
L'istanza è appena stata creata ma non ancora salvata per la prima volta. Questo stato dura pochi istanti.

**In Compilazione**  
L'istanza è stata salvata ma risulta ancora incompleta. Possono mancare:
- Campi obbligatori non compilati
- Documenti obbligatori non caricati
- Pagamenti obbligatori non effettuati

Puoi salvare e riprendere la compilazione in qualsiasi momento.

**Completata**  
Tutti i dati, documenti e pagamenti obbligatori sono stati inseriti correttamente. Il sistema ha validato l'istanza con successo.

**Firmata**  
Hai generato il PDF dell'istanza, lo hai firmato digitalmente con il tuo dispositivo di firma e lo hai ricaricato sulla piattaforma. L'istanza è pronta per essere trasmessa all'Ente.

{: .note }
> La firma digitale è obbligatoria per tutte le istanze. Assicurati di avere a disposizione un dispositivo di firma valido (smart card, token USB, firma remota).

### Stati di lavorazione dell'Ente

**Inviata**  
L'istanza è stata trasmessa all'Ente ed è uscita dalla tua responsabilità diretta. Da questo momento il ciclo di vita dipende dalle azioni dell'Ente.

All'atto della trasmissione, GeoTecSUE genera automaticamente la **ricevuta di invio** scaricabile dal dettaglio dell'istanza.

**Protocollata**  
L'Ente ha assegnato numero e data di protocollo all'istanza, inserendola formalmente nel proprio sistema documentale.

GeoTecSUE genera automaticamente la **ricevuta di protocollazione**. In questa fase non puoi ancora inviare comunicazioni o integrazioni.

**Registrata** (solo per pratiche)  
L'Ufficio competente (tipicamente l'Ufficio Tecnico) ha preso in carico la pratica, assegnando:
- Numero di registrazione
- Data di registrazione
- Eventualmente un responsabile del procedimento

**Da questo momento puoi nuovamente interagire con la pratica** inviando comunicazioni e, se previsto dall'Ente, integrazioni spontanee.

GeoTecSUE genera automaticamente la **ricevuta di registrazione** (disponibile solo per le pratiche, non per comunicazioni o integrazioni).

{: .note }
> Lo stato "Registrata" è fondamentale: solo da questo momento in poi puoi inviare comunicazioni come Inizio Lavori o Fine Lavori.

### Stati di integrazione documentale

**Richiesta Integrazioni**  
L'Ente ha aperto formalmente una richiesta di integrazione durante l'istruttoria della pratica. 

Devi:
1. Accedere al dettaglio della pratica
2. Consultare la richiesta dell'Ente nell'apposita sezione
3. Caricare i documenti richiesti
4. Trasmettere l'integrazione

**Invio Integrazioni**  
Hai caricato e trasmesso all'Ente i documenti richiesti. La pratica torna in istruttoria.

### Stati finali

**Esecutiva**  
L'Ente ha completato l'istruttoria e rilasciato il provvedimento favorevole. Alla pratica sono associati:
- Numero del provvedimento
- Data del provvedimento

**Esempi**: Rilascio Permesso di Costruire, Autorizzazione Paesaggistica approvata.

**Archiviata**  
La pratica è stata archiviata. Questo può avvenire in due modi:
- Su richiesta del professionista (tramite apposita istanza)
- Per decisione diretta dell'Ente (es. pratica errata, non conforme, presentata allo sportello sbagliato)

In questo stato puoi visualizzare la pratica ma non puoi più operare (niente comunicazioni, integrazioni o modifiche).

**Diniego**  
L'Ente ha espresso parere negativo dopo l'istruttoria. Come per l'archiviazione, puoi visualizzare la pratica ma non puoi più operare su di essa.

**Revoca Delegato**  
Si verifica quando il titolare della pratica contesta l'operato del professionista originale e revoca formalmente l'incarico. Il professionista può visualizzare la pratica ma non può più operare.

{: .warning }
> Per stati meno frequenti o specifici di alcune Regioni (es. stati SPRESALWEB per il Piemonte, stato "Verificata", "Rifiutata"), consulta la sezione [Appendice: Ciclo di vita dettagliato](appendici/ciclo-vita-dettagliato.html).

## Diagramma del ciclo di vita

![Ciclo di vita di un'istanza GeoTecSUE](../assets/images/ciclo-vita-geotecsue-v2.svg)

*Il diagramma mostra il percorso completo di un'istanza dalla creazione alla chiusura. Gli stati in azzurro sono gestiti dal professionista, quelli in arancione dall'Ente.*

## Professionista principale

Chi crea un'istanza diventa automaticamente il **professionista principale** e mantiene questo ruolo per tutta la vita dell'istanza, fino a un'eventuale voltura formale.

### Visibilità verso l'Ente

Agli occhi dell'Ente, il professionista principale è:
- Il **compilatore** dell'istanza
- Il **responsabile** della trasmissione
- L'**unico interlocutore ufficiale** per la pratica

Questo rimane vero anche se altre persone collaborano alla compilazione tramite il sistema dei soggetti compilatori (vedi sezione successiva).

### Esclusione dai soggetti coinvolti

Il professionista principale può anche scegliere di non comparire tra i professionisti coinvolti nella pratica (es. progettista, direttore lavori). In questo caso:
- All'Ente risulterà solo come "compilatore" e "professionista principale"
- Non apparirà nella lista dei tecnici incaricati (progettisti, direttori lavori, ecc.)

Questa scelta è utile quando il professionista principale agisce solo come intermediario per la compilazione, ma non ha ruoli tecnici nella pratica.

## Soggetti compilatori aggiuntivi

Il professionista principale può condividere la pratica con altri professionisti per collaborare alla compilazione, sia durante la fase di compilazione iniziale che nelle fasi successive.

### Ruoli disponibili

**Amministratore**  
Ha controllo quasi completo sulla pratica:

✅ **Può**:
- Modificare dati e allegati
- Aggiungere ed eliminare documenti
- Effettuare pagamenti PagoPA
- Creare comunicazioni all'interno di pratiche già trasmesse
- Trasmettere istanze all'Ente
- Cancellare istanze in compilazione

❌ **Non può**:
- Gestire i soggetti della pratica (aggiungere/rimuovere altri compilatori)

**Utente Modifica**  
Ha controllo parziale sulla pratica:

✅ **Può**:
- Modificare i dati della pratica
- Aggiungere allegati
- Eliminare solo gli allegati caricati da lui stesso
- Effettuare pagamenti PagoPA
- Creare comunicazioni all'interno di pratiche già trasmesse

❌ **Non può**:
- Trasmettere istanze all'Ente
- Cancellare istanze in compilazione
- Eliminare allegati caricati da altri
- Gestire i soggetti della pratica

{: .note }
> La differenza principale tra i due ruoli è che solo l'Amministratore può trasmettere istanze e cancellare pratiche in compilazione. L'Utente Modifica è ideale per collaboratori che devono solo inserire dati senza responsabilità di invio.

### Come aggiungere un soggetto compilatore

**Metodo 1 - Dalla lista pratiche**:
1. Nella sezione "Lista Pratiche in fase di compilazione"
2. Clicca sul bottone "Soggetti" (icona blu o verde) accanto alla pratica
3. Inserisci il **codice fiscale** del professionista da aggiungere
4. Seleziona il ruolo (Amministratore o Utente Modifica)
5. Conferma l'operazione

**Metodo 2 - Dal dettaglio pratica**:
1. Apri il dettaglio della pratica
2. Clicca su **Gestione Soggetti** (pulsante in alto a destra)
3. Inserisci il **codice fiscale** del professionista
4. Seleziona il ruolo
5. Conferma l'operazione

Per approfondire l'interfaccia, consulta [Interfaccia e convenzioni](interfaccia-e-convenzioni.html#gestione-soggetti).

### Prerequisiti per aggiungere un soggetto

Il professionista che vuoi aggiungere deve aver effettuato **almeno un accesso** a GeoTecSUE dell'Ente di riferimento.

{: .warning }
> Se il sistema non trova il professionista cercato, significa che questa persona non ha mai effettuato il login su GeoTecSUE di quell'Ente. Non è necessario che abbia mai trasmesso pratiche, basta un singolo accesso al portale.

Chiedi al collega di:
1. Accedere a GeoTecSUE con SPID o CIE
2. Completare eventualmente il proprio profilo
3. Confermarti l'accesso avvenuto

Dopodiché potrai aggiungerlo come soggetto compilatore.

### Trasparenza per l'Ente

**Importante**: L'aggiunta di soggetti compilatori è completamente trasparente e invisibile all'Ente.

Anche se:
- Un Amministratore compila interamente la pratica
- Un Amministratore trasmette l'istanza all'Ente
- Un Amministratore crea e invia comunicazioni (es. Inizio Lavori)
- Più persone collaborano alla compilazione

All'Ente risulterà sempre e comunque il **professionista principale** come unico responsabile della compilazione e della trasmissione.

Il concetto di "soggetto compilatore" esiste esclusivamente nel rapporto interno tra professionisti e non ha alcun valore o visibilità verso la Pubblica Amministrazione.

{: .note }
> Questo sistema è ideale per studi associati, società di ingegneria o collaborazioni tra professionisti, permettendo una gestione flessibile delle pratiche senza complicare i rapporti con l'Ente.

## Riepilogo dei concetti chiave

Prima di procedere con l'uso operativo di GeoTecSUE, assicurati di aver compreso questi concetti fondamentali:

1. **Conservazione temporanea**: I documenti sono disponibili solo per 6 mesi dalla registrazione
2. **Chiave univoca**: Ogni istanza ha un codice di 19 cifre mai modificato
3. **Tre tipologie**: Pratica (autonoma), Comunicazione (collegata), Integrazione (aggiuntiva)
4. **Stati critici**: Registrata (per consentire di inviare comunicazioni e/o integrazioni), Richiesta Integrazioni (azione richiesta)
5. **Professionista principale**: Rimane il solo responsabile agli occhi dell'Ente
6. **Collaborazione**: Puoi condividere pratiche con colleghi mantenendo il controllo

---

**Prossimi passi**: 

- Consulta [Interfaccia e convenzioni](interfaccia-e-convenzioni.html) per familiarizzare con l'interfaccia
- Leggi [Creazione di una nuova istanza](nuova-istanza.html) per iniziare a lavorare
- Per stati particolari, vedi [Appendice: Ciclo di vita dettagliato](appendici/ciclo-vita-dettagliato.html)
