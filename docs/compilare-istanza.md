---
title: Compilare un'istanza
nav_order: 20
parent: Le mie istanze
description: Guida completa alla compilazione di pratiche edilizie su GeoTecSUE - inserimento dati, soggetti, localizzazione, allegati, pagamenti e invio
keywords: [compilare pratica, inserimento dati, titolare, soggetti, localizzazione, mappali, allegati, pagamenti PagoPA, validazione, firma digitale, invio]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Compilare un'istanza

Questa sezione spiega come compilare un'istanza edilizia su **GeoTecSUE**, dall'inserimento dei dati fino all'invio all'Ente.

## Quando usi questa guida

Accedi alla schermata di compilazione quando:
- [Crei una nuova istanza](nuova-istanza.html) (pulsante "Nuova")
- [Duplichi una pratica esistente](nuova-istanza.html#metodo-2-duplicare-una-pratica-esistente)
- Avvii una nuova comunicazione dal [dettaglio di una pratica](dettaglio-istanza.html#comunicazioni-verso-lente)
- Riprendi una pratica salvata in compilazione

## Panoramica della compilazione

### Interfaccia principale

La schermata di compilazione mostra:

**Barra superiore**:
- **Tipologia pratica**: es. "Permesso di Costruire", "SCIA", "CILA"
- **Stato**: In Creazione → In Compilazione → Completata → Firmata
- **Numero pratica**: Chiave univoca a 19 cifre

**Menu azioni**: Pulsanti per salvare, validare, generare PDF, tornare indietro

**Form di compilazione**: Sezioni con campi da compilare (sfondo giallo = obbligatori)

### Libertà di compilazione

Non sei obbligato a seguire un ordine specifico. Puoi:
- Compilare prima la localizzazione e poi i soggetti
- Caricare gli allegati prima di inserire i dati
- Salvare e riprendere in qualsiasi momento

{: .note }
> I **campi con sfondo giallo** sono obbligatori. Devi compilarli tutti per completare l'istanza.

### Salvare e riprendere

Puoi salvare in qualsiasi momento e riprendere la compilazione quando vuoi. Non ci sono limiti di tempo.
Se rimani inattivo, dopo 10 minuti il sistema procede con un *salvataggio automatico* della tua pratica.

---

## Menu azioni dell'istanza

Nella parte superiore della pagina trovi i pulsanti per gestire l'istanza.

### Salva (pulsante blu con dischetto)

**Cosa fa**: Salva l'istanza **senza validazione**.

**Quando usarlo**:
- Vuoi salvare il lavoro fatto fino a ora
- Devi interrompere la compilazione e riprenderla dopo
- Hai compilato solo parte dei campi

**Comportamento**:
- ✅ Salva tutto ciò che hai inserito
- ✅ Messaggio verde di conferma: "Salvataggio della pratica avvenuto con successo" (con data e ora)
- ✅ Se era "In Creazione", passa a "In Compilazione"
- ❌ **Non** effettua alcun tipo di validazione (campi, allegati, pagamenti...)

### Valida e Salva (pulsante verde con dischetto e spunta)

**Cosa fa**: **Verifica** tutti i dati e poi salva.

**Quando usarlo**:
- Hai compilato tutti i campi obbligatori
- Vuoi verificare se l'istanza è pronta per l'invio
- Vuoi passare a "Completata"

**Comportamento del sistema**:

**Se trova errori**:
1. ❌ Messaggio rosso di errore
2. Il sistema si posiziona sul **primo errore** rilevato
3. Indica esattamente cosa manca o cosa è sbagliato
4. **Non salva** l'istanza

**Errori tipici**:
- Campo obbligatorio non compilato
- Allegato obbligatorio mancante
- Pagamento obbligatorio non effettuato
- Soggetto obbligatorio non inserito
- Dato incoerente (es. data futura dove non consentita)

{: .warning }
> Il sistema mostra il **primo errore** che trova. Potrebbero essercene altri. Dopo averlo corretto, clicca di nuovo "Valida e Salva".

**Se tutto è corretto**:
1. ✅ Messaggio verde di conferma
2. L'istanza passa da "In Compilazione" a **"Completata"**
3. Puoi procedere con la generazione del PDF

### Genera la Bozza (pulsante rosso con stampante)

**Disponibilità**: Solo se l'istanza è **almeno** in stato "In Compilazione" (non in "Creazione")

**Cosa fa**: Genera e scarica il **PDF dell'istanza** anche se incompleta.

**Quando usarlo**:
- Vuoi vedere come apparirà la pratica finale
- Vuoi verificare su un pdf i dati che hai finora inserito

**Caratteristiche**:
- Genera PDF anche se mancano campi obbligatori
- Deve essere usato per il solo scopo consultativo

{: .note }
> La bozza è utile per verificare visivamente i dati prima della validazione finale. Non è il PDF ufficiale da firmare e inviare.

### Ritorna (pulsante azzurro con freccia)

**Cosa fa**: Torna alla pagina precedente.

**Dove torna**:
- All'[elenco istanze](elenco-istanze.html) (se sei arrivato da lì)
- Al [dettaglio della pratica](dettaglio-istanza.html) (se stai compilando una comunicazione)

{: .warning }
> Prima di cliccare "Ritorna", assicurati di aver salvato. I dati non salvati andranno persi.

---

## Sezioni di compilazione

L'istanza è organizzata in sezioni tematiche. Di seguito le sezioni comuni a tutte le tipologie di pratica.

{: .note }
> Alcune sezioni potrebbero non apparire o avere campi diversi in base al tipo di pratica selezionato.

## Dati Titolare

**Obbligatorietà**: ✅ Sempre obbligatoria

**Cosa inserire**: I dati anagrafici del **titolare principale** dell'istanza (chi presenta la pratica).

### Campi richiesti

| Campo | Obbligatorio | Note |
|-------|--------------|------|
| **Cognome** | Sì | |
| **Nome** | Sì | |
| **Sesso** | Sì | |
| **Codice Fiscale** | Sì | Viene validato automaticamente |
| **Nato a** | Sì | |
| **Prov.** | Sì | |
| **Stato (indicare se diverso da Italia)** | No | |
| **Nato il** | Sì | |
| **Residente in** | Sì | Città di residenza |
| **Prov.** | Sì | |
| **Stato (indicare se diverso da Italia)** | No | |
| **Indirizzo** | Sì | |
| **n.** | Sì | |
| **CAP** | Sì | |
| **PEC** | No | Se disponibile |
| **posta elettronica** | No | Se disponibile (per comunicazioni)|
| **Telefono fisso** | No | Se disponibile |
| **Cellulare** | No | Se disponibile  |

### Autocompilazione

Il sistema può autocompilare questa sezione in alcuni casi:

**Compilazione di una comunicazione**:
- I dati vengono prelevati automaticamente dalla **pratica principale**
- Puoi comunque modificarli

**Duplicazione di un'istanza**:
- Se l'istanza originale aveva il titolare, i dati vengono copiati
- Puoi modificarli se necessario

**Uso dell'anagrafica richiedenti**:
1. Se hai caricato un'anagrafica di richiedenti
2. Seleziona il soggetto dal menu "Seleziona il richiedente"
3. Clicca **"Carica Titolare"**
4. I dati vengono compilati automaticamente

{: .note }
> L'anagrafica richiedenti è una funzionalità che ti permette di salvare i dati dei titolari ricorrenti per riutilizzarli velocemente. Gestiscila dalla tua area **Anagrafica**.

### Istanza nuova

Se crei un'istanza completamente nuova, **devi inserire tutti i dati manualmente**.

---

## Dati della Ditta/Società/Ente/Altro

**Obbligatorietà**: ⚠️ Diventa obbligatoria se selezioni una qualifica

**Quando compilarla**: Se il titolare agisce in qualità di rappresentante di una persona giuridica.

### Campi richiesti

| Campo | Quando obbligatorio |
|-------|---------------------|
| **In qualità di** | Diventa trigger: Amministratore, Legale Rappresentante, Socio, ecc. |
| **Altro (eventuale)** | Diventa obbligatorio se selezionato "Altro (specificare)" |
| **della ditta / società / ente / altro** | Se "In qualità di" è compilato |
| **Codice Fiscale** | Se "In qualità di" è compilato |
| **P. IVA** | Se "In qualità di" è compilato |
| **Iscritta alla C.C.I.A.A.** | Se "In qualità di" è compilato |
| **Prov.** | Se "In qualità di" è compilato |
| **n.** | Se "In qualità di" è compilato |
| **con sede in** | Se "In qualità di" è compilato |
| **Prov.** | Se "In qualità di" è compilato |
| **Indirizzo** | Se "In qualità di" è compilato |
| **n.** | Se "In qualità di" è compilato |
| **CAP** | Se "In qualità di" è compilato |
| **PEC** | Se "In qualità di" è compilato |
| **posta elettronica** | Se "In qualità di" è compilato |
| **Telefono fisso** | Se "In qualità di" è compilato |
| **cellulare** | |

### Comportamento

**Se NON selezioni nulla in "In qualità di"**:
- Questa sezione è **facoltativa**
- Puoi lasciarla vuota
- Il titolare agisce come persona fisica

**Se selezioni una voce in "In qualità di"**:
- Tutti i campi della sezione diventano **obbligatori**
- Il titolare agisce come rappresentante della società/ente

### Autocompilazione

Come per "Dati Titolare", questa sezione si autocompila se:
- Stai compilando una comunicazione (eredita dalla pratica)
- Hai duplicato un'istanza che aveva questi dati
- Usi l'anagrafica richiedenti e il soggetto aveva una società associata

---

## Dati del Procuratore / Delegato

**Obbligatorietà**: ✅ Sempre obbligatoria

**Cosa inserire**: I dati del professionista che presenta la pratica per conto del titolare.

### Compilazione automatica

Di **default**, il sistema inserisce automaticamente **i tuoi dati** prelevati dal tuo [profilo utente](../docs/accesso-e-profilo.html#modificare-i-dati-del-profilo).

### Campi richiesti

| Campo | Obbligatorio | Note |
|-------|--------------|------|
| **Cognome** | Sì | |
| **Nome** | Sì | |
| **Sesso** | Sì | |
| **Codice Fiscale** | Sì | Viene validato automaticamente |
| **Nato a** | Sì | |
| **Prov.** | Sì | |
| **Stato (indicare se diverso da Italia)** | No | |
| **Nato il** | Sì | |
| **Residente in** | Sì | Città di residenza |
| **Prov.** | Sì | |
| **Stato (indicare se diverso da Italia)** | No | |
| **Indirizzo** | Sì | |
| **n.** | Sì | |
| **CAP** | Sì | |
| **PEC** | No | Se disponibile |
| **posta elettronica** | No | Se disponibile (per comunicazioni)|
| **Telefono fisso** | No | Se disponibile |
| **Cellulare** | No | Se disponibile  |

### Modificare i dati

Puoi modificare i dati in due modi:

**Manualmente**: Cambia i singoli campi se necessario

**Dall'anagrafica professionisti**:
1. Se hai caricato un'anagrafica di professionisti
2. Seleziona dal menu "Selezione Proc. / Del."
3. I dati del professionista selezionato vengono caricati

{: .note }
> Normalmente lasci i tuoi dati. Modifichi solo se la pratica è presentata da un altro professionista dello studio.

---

## Localizzazione dell'Intervento

**Obbligatorietà**: ✅ Sempre obbligatoria

**Cosa inserire**: Dove si trova l'intervento oggetto della pratica.

### Indirizzo

#### Campi obbligatori

Il **comune** ed il **CAP** sono sempre obbligatori ma normalmente sono già compilati (caso Ente individuale) o selezionati precedentemente (Ente Unione).

| Campo | Descrizione |
|-------|-------------|
| **Indirizzo (Via, Viale, Piazza, ecc.)** | Seleziona dal menu a discesa (stradario comunale) |
| **Numero civico** | Inserisci il numero |

#### Toponimo mancante

Se l'indirizzo **non è presente** nel menu a discesa:

**Se l'Ente lo consente**:
1. Spunta la voce **"Toponimo mancante"**
2. Inserisci manualmente via e numero civico

**Se l'Ente NON lo consente**:
- La spunta non è disponibile
- **Contatta l'Ente** per richiedere l'inserimento del toponimo mancante
- L'Ente ti comunicherà il toponimo corretto da selezionare

{: .warning }
> Non puoi procedere senza un indirizzo valido. Se non trovi la via, contatta subito l'Ente per evitare ritardi.

### Dati Catastali

Devi inserire **almeno un dato catastale**: Fabbricati **o** Terreni (o entrambi).

#### Fabbricati

| Campo | Obbligatorio |
|-------|--------------|
| **Sezione** | No |
| **Foglio** | Sì |
| **Mappale** | Sì |
| **Subalterno** | No |

Puoi aggiungere più fabbricati cliccando **"Aggiungi fabbricato"**.

#### Terreni

| Campo | Obbligatorio |
|-------|--------------|
| **Sezione** | No |
| **Foglio** | Sì |
| **Mappale** | Sì |

Puoi aggiungere più terreni cliccando **"Aggiungi terreno"**.

{: .note }
> Devi inserire **almeno un mappale** (fabbricato o terreno). Se l'intervento coinvolge più particelle, aggiungile tutte.

### Cartografia (se disponibile)

Se l'Ente ha attivato il **sistema cartografico**, puoi usarlo per facilitare l'inserimento dei dati catastali.

#### Tipologie di cartografia

- **Base catastale**: Visualizza solo i confini catastali
- **PRGC** (Piano Regolatore): Visualizza anche zonizzazione urbanistica

#### Funzionalità disponibili

**1. Ricerca pratiche in cartografia**
- Icona "squadretta e matita" nella barra laterale
- Cerca pratiche esistenti direttamente sulla mappa
- Utile per verificare interventi nelle vicinanze

**2. Importazione mappali dalla cartografia alla pratica**
- Seleziona i mappali cliccando sulla mappa
- Clicca il pulsante **"Importa in pratica"**
- I dati catastali vengono inseriti automaticamente nel form
- Per comuni in **Regione Lombardia**: importa anche le coordinate

**3. Evidenziazione mappali in cartografia**
- Inserisci i mappali nel form
- I mappali si evidenziano automaticamente sulla mappa
- Utile per verificare visivamente la correttezza

{: .note }
> La cartografia è un grande aiuto per evitare errori nei dati catastali. Usala quando disponibile!

### Coordinate (solo Regione Lombardia)

**Obbligatorio per Comuni lombardi**: Sì

Se operi in **Regione Lombardia**, devi inserire le **coordinate geografiche** dell'intervento.

**Inserimento**:
- Manuale: Inserisci latitudine e longitudine
- Automatico: Usando la cartografia (importa mappali)

**Formato**: Sistema di riferimento specificato dall'Ente (caso di Regione Lombardia: *UTM - WGS 84 32N*)

### Destinazione d'uso

**Obbligatorietà**: Sì (almeno una)

Seleziona la destinazione d'uso dell'immobile/area:

- Altro
- Residenziale
- Commerciale
- Produttiva e direzionale
- Rurale
- Turistico-ricettiva

{: .note }
> Puoi selezionare **più destinazioni** se l'intervento è a uso misto (es. Residenziale + Commerciale).

---

## Soggetti Coinvolti

**Obbligatorietà**: ⚠️ Dipende dalla tipologia di pratica e intervento

**Cosa inserire**: Altri titolari, professionisti incaricati, imprese esecutrici.

### Struttura della sezione

La sezione è divisa in sottosezioni:

1. **Altri titolari** (co-intestatari)
2. **Tecnici incaricati** (progettisti, direttori lavori, ecc.)
3. **Imprese esecutrici**

### 1. Altri Titolari (Co-intestatari)

**Quando compilare**: Se la pratica ha più titolari.

**Come aggiungere**:
1. Clicca **"Aggiungi titolare"**
2. Inserisci i dati anagrafici (come per il titolare principale)
3. Salva

Puoi aggiungere quanti co-intestatari necessari.

### 2. Tecnici Incaricati

**Quando obbligatorio**: Dipende dal tipo di pratica.

**Ruoli principali richiesti**:
- **Progettista** 
- **Direttore dei Lavori**
- **Rilevatore**
- **Geologo** (se richiesta relazione geologica)
- **Coordinatore per la sicurezza in fase di esecuzione**
- **Coordinatore per la sicurezza in fase di progettazione**
...

**Quali ruoli sono obbligatori**:
- Varia in base a: **tipo di pratica** + **tipo di intervento**
- In fase di validazione il sistema indica i ruoli mancanti
- Es: CILA richiede almeno un progettista abilitato; se Sanatoria viene richiesto un Rilevatore

**Come aggiungere**:
1. Scegli il **ruolo** dal menu a discesa
2. Inserisci i dati del tecnico (simili alle sezioni viste in precedenza)
3. Clicca **"Aggiungi"**

**Autocompilazione dall'anagrafica**:
- Se hai caricato un'anagrafica professionisti
- Seleziona dal menu "Seleziona professionista"
- Dati compilati automaticamente

{: .note }
> Puoi inserire te stesso anche come progettista/direttore lavori se sei il tecnico incaricato (oltre che come procuratore).

### 3. Imprese Esecutrici

**Quando obbligatorio**: Dipende dal tipo di pratica e dalle dichiarazioni.

**Casi particolari**: Per pratiche come **CILA**, se l'intervento è di modesta entità, potresti avere l'opzione:

☑️ *"In quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"*

**Se spunti questa opzione**:
- **Non** devi inserire imprese
- La sezione diventa facoltativa

**Se NON spunti** o se la pratica richiede imprese:
- Devi inserire **almeno un'impresa**

**Come aggiungere**:
1. Clicca **"Aggiungi impresa"**
2. Inserisci i dati (simili alle sezioni viste in precedenza)
3. Salva

**Autocompilazione dall'anagrafica**:
- Se hai caricato un'anagrafica imprese
- Seleziona dal menu
- Dati compilati automaticamente

---

## PagoPA

**Obbligatorietà**: ⚠️ I pagamenti **obbligatori** devono essere completati; i **facoltativi** possono essere ignorati

**Cosa inserire**: Codici IUV per i pagamenti richiesti dalla pratica.

### Tipologie di pagamenti

La sezione mostra due tipi di pagamenti:

#### Pagamenti Obbligatori

**Esempi**:
- Diritti di Segreteria
- Sanzioni (per pratiche in sanatoria, quando in pratica viene selezionata la voce)

**Effetto**: **Senza completare i pagamenti obbligatori, l'istanza non può essere validata**.

#### Pagamenti Facoltativi

**Esempi**:
- Oneri di Urbanizzazione
- Contributo di Costruzione

**Effetto**: Puoi ignorarli e validare comunque l'istanza.

### Due modalità di pagamento

Per ogni pagamento puoi scegliere:

#### Opzione A: Inserire uno IUV già in tuo possesso

**Quando usarla**: Se hai già un codice IUV (ad esempio creato sul portale dell'Ente)

**Come fare**:
1. Clicca **"Inserisci IUV esistente"**
2. Incolla il codice IUV (17 cifre)
3. Salva

{: .warning }
> Verifica che lo IUV sia corretto e relativo a **questa pratica**. Inserire IUV sbagliati causa problemi di contabilizzazione.

{: .warning }
> Non confondere il codice IUV con il codice avviso: il codice IUV ha 17 cifre, il codice avviso è più lungo (normalmente 18 cifre) ed aggiunge un 3 davanti al codice IUV

#### Opzione B: Creare lo IUV su GeoTecSUE (consigliato)

**Vantaggi**:
- ✅ Certezza della **tipologia corretta** del pagamento
- ✅ **Importo esatto** (se inserito dall'Ente)
- ✅ Collegamento automatico alla pratica
- ✅ Tracciabilità completa

**Come fare**:
1. Clicca **"Crea IUV"**
2. Se l'importo è pre-compilato, verifica e conferma
3. Se l'importo è "da valorizzare", inseriscilo manualmente
4. Il sistema genera lo IUV
5. Scarica il PDF con i dati di pagamento
6. Procedi al pagamento tramite PagoPA

**Pagare lo IUV**:
- Home banking (sezione PagoPA)
- App bancarie (cerca "Paga con PagoPA")
- Tabaccherie abilitate
- Sportelli ATM
- Uffici postali

{: .note }
> È **fortemente consigliato** creare lo IUV direttamente su GeoTecSUE. Evita errori e semplifica la tracciabilità.

### Verifica del pagamento

Dopo aver pagato:
1. Torna su GeoTecSUE
2. Nella sezione PagoPA, clicca **"Aggiorna stato"**
3. Il sistema interroga PagoPA e mostra lo stato aggiornato

Se lo stato è **"Pagamento eseguito"**, puoi procedere con la validazione dell'istanza.

{: .warning }
> L'aggiornamento dello stato può richiedere alcuni minuti. Se non vedi subito il cambiamento, attendi e riprova.

Per i dettagli su tutti gli stati PagoPA, consulta [Appendice: Stati PagoPA](appendici/pagopa-stati.html).

---

## Quadro Riepilogativo della Documentazione

**Obbligatorietà**: ✅ Tutti i documenti obbligatori devono essere caricati

**Cosa caricare**: Allegati richiesti dalla tipologia di pratica.

### Tre categorie di documenti

La sezione è divisa in:

1. **Documenti obbligatori** (es. Relazione tecnica, Elaborati grafici)
2. **Documenti liberi** (puoi aggiungere ciò che vuoi)
3. **Documenti facoltativi** (richiesti dall'Ente ma non bloccanti)

### 1. Documenti Obbligatori

**Elenco**: Varia in base al tipo di pratica.

**Esempi generici**:
- Documentazione fotografica dello stato di fatto
- Elaborati di progetto
- Copia di documento di identità del titolare principale

**Caratteristiche**:
- Ogni documento ha un **nome specifico** (es. "Relazione tecnica asseverata")
- Alcuni richiedono **firma digitale obbligatoria**
- Hanno un **limite di dimensione** (es. max 20 MB)

**Effetto**: **Senza caricare tutti i documenti obbligatori, l'istanza non può essere validata**.

### 2. Documenti Liberi

**Cosa sono**: Allegati che puoi aggiungere liberamente senza che siano richiesti esplicitamente.

**Quando usarli**:
- Vuoi aggiungere documentazione integrativa
- Hai allegati esplicativi non previsti dall'elenco obbligatorio

**Come aggiungere**:
1. Clicca **"Aggiungi documento libero"**
2. Inserisci una **descrizione** del file
3. Carica il file
4. Salva

### 3. Documenti Facoltativi

**Cosa sono**: Documenti richiesti dall'Ente ma **non bloccanti** per la validazione.

**Esempi**:
- Copia del documento di identità dei co-titolari
- Dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori

**Caratteristiche**:
- Visibili nell'elenco
- Se non carichi, puoi comunque validare

### Caricare un documento

**Procedura**:

1. **Individua il documento** nell'elenco (obbligatori/facoltativi) o inserisci direttamente la *descrizione del file* e il file stesso (liberi)

2. **Verifica i requisiti**:
   - Firma digitale necessaria?
   - Dimensione massima (es. "Max 20 MB")
   - Tipo di file richiesto (es. File PDF)

3. **Prepara il file**:
   - **Se firma NON richiesta**: Carica file privo di firma
   - **Se firma richiesta**: Firma il file *CAdES* con dispositivo di firma (smart card, token USB, firma remota) → Ottieni file **.p7m** → Carica il .p7m
     
{: .note }
> Se la firma non è richiesta si può comunque caricare un file firmato digitalmente

4. **Carica**:
   - Clicca **"Sfoglia"** o **"Scegli file"**
   - Seleziona il file dal computer
   - Clicca **"Carica"** o **"Salva"**

5. **Verifica**:
   - Il file appare nell'elenco con icona ✅
   - Puoi scaricarlo per verificarlo (pulsante verde)
   - Puoi eliminarlo e ricaricare se sbagliato (pulsante rosso)

{: .warning }
> **Firma digitale**: Se richiesta, devi caricare il file firmato (**.p7m**). I file non firmati verranno rifiutati dal sistema.

### Caricare più file per lo stesso documento

Puoi caricare **più file** (es. Elaborati grafici: TAV01, TAV02, TAV03).

**Procedura**:
1. Carica il primo file
2. Clicca di nuovo **"Aggiungi file"** sullo stesso documento
3. Carica il secondo file
4. Ripeti per tutti i file necessari

Tutti i file caricati per lo stesso documento verranno considerati come un unico allegato complessivo.

### Formati accettati

**Formati tipicamente accettati**:
- PDF (preferito)
- PDF firmato digitalmente (.p7m)
- Immagini (JPG, PNG) - solo per documentazione fotografica
- DWG, DXF - per elaborati grafici tecnici (dipende dall'Ente)

{: .note }
> Verifica sempre i formati accettati specificati accanto a ogni documento. In caso di dubbio, usa **PDF**.

---

## Prossimi passi

Dopo aver compilato l'istanza:

- [Consultare l'elenco delle istanze](elenco-istanze.html)
- [Visualizzare il dettaglio della pratica](dettaglio-istanza.html)
- [Comprendere il ciclo di vita](../docs/nozioni-di-base.html#ciclo-di-vita-di-unistanza)

---

**Hai bisogno di aiuto durante la compilazione?** 
- Consulta [Interfaccia e convenzioni](../docs/interfaccia-e-convenzioni.html) per capire i pulsanti
- Verifica [Nozioni di base](../docs/nozioni-di-base.html) per concetti fondamentali
- Contatta l'assistenza tecnica in caso di dubbi specifici sulla pratica
