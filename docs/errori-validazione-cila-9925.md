---
title: Errori CILA - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 40
description: Errori di validazione specifici per la CILA Nazionale - Comunicazione di Inizio Lavori Asseverata (art. 6-bis D.P.R. 380/2001, D.Lgs. 222/2016)
keywords: [CILA, comunicazione inizio lavori asseverata, art. 6-bis DPR 380/2001, DLgs 222/2016, nazionale, tolleranze costruttive, art. 34-bis, art. 34-ter, zona sismica, Progettista, sanzione 333 euro, sanzione 1000 euro]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 125 }  # Valle d'Aosta - CILA
  - { Reg: 6, Prat: 625 } # Veneto - CILA
  - { Reg: 8, Prat: 825 } # Emilia-Romagna - CILA
  - { Reg: 12, Prat: 1225 } # Lazio - CILA
  - { Reg: 13, Prat: 1325 } # Abruzzo - CILA
  - { Reg: 15, Prat: 1525 } # Campania - CILA
  - { Reg: 16, Prat: 1625 } # Basilicata - CILA
  - { Reg: 17, Prat: 1725 } # Puglia - CILA
  - { Reg: 18, Prat: 1825 } # Calabria - CILA
  - { Reg: 19, Prat: 1925 } # Sicilia - CILA
Fonte: Manuale
---

# Errori di validazione - CILA Nazionale
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori Asseverata (CILA)** ai sensi dell'art. 6-bis del D.P.R. 6 giugno 2001, n. 380 e della Tabella A, Sezione II, del D.Lgs. 25 novembre 2016, n. 222, applicabile su tutto il territorio nazionale.

{: .note }
> La CILA Nazionale è una delle pratiche più complete della piattaforma. Ha due macro-sezioni distinte: le **dichiarazioni del titolare** (titolarità, opere parti comuni, presentazione, qualificazione, localizzazione, contributo, tecnici, impresa, sicurezza) e le **dichiarazioni del progettista** (tipologia intervento, descrizione, dichiarazione tolleranze, altre comunicazioni, atti di assenso). La sezione **Regolarità urbanistica** è presente nel modulo ASCX ma è completamente **commentata nel validatore** e non genera errori. La sezione **Dichiarazione di tolleranze** del progettista è invece pienamente validata con una gerarchia di controlli a 5+ livelli per le zone sismiche ad alta sismicità. È richiesto obbligatoriamente un **Progettista (PR)** nei soggetti coinvolti.

---

## Indice sezioni

**Dichiarazioni del Titolare:**
1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Presentazione della comunicazione di inizio dei lavori](#3-presentazione-della-comunicazione-di-inizio-dei-lavori)
4. [Qualificazione dell'intervento](#4-qualificazione-dellintervento)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Calcolo del contributo di costruzione](#6-calcolo-del-contributo-di-costruzione)
7. [Tecnici incaricati e impresa esecutrice](#7-tecnici-incaricati-e-impresa-esecutrice)
8. [Sicurezza sul lavoro — D.Lgs. 81/2008](#8-sicurezza-sul-lavoro--dlgs-812008)

**Dichiarazioni del Progettista:**

9. [Tipologia di intervento e descrizione sintetica](#9-tipologia-di-intervento-e-descrizione-sintetica)
10. [Dichiarazione di tolleranze](#10-dichiarazione-di-tolleranze)
11. [Altre comunicazioni, segnalazioni, asseverazioni](#11-altre-comunicazioni-segnalazioni-asseverazioni)
12. [Atti di assenso da acquisire](#12-atti-di-assenso-da-acquisire)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Non hai selezionato il radio button della titolarità.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"**

---

## 2. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Non hai dichiarato se i lavori interessano parti comuni.

**Soluzione**: Seleziona **una delle quattro opzioni**:
- ⚪ **"non riguardano parti comuni"**
- ⚪ **"riguardano le parti comuni di un fabbricato condominiale"** (l'amministratore deve disporre della delibera assembleare)
- ⚪ **"riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio..."** (con approvazione di tutti i comproprietari)
- ⚪ **"riguardano parti dell'edificio di proprietà comune ma non necessitano di assenso..."** (art. 1102 c.c.)

---

## 3. Presentazione della comunicazione di inizio dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della comunicazione di inizio dei lavori'.

**Dove si trova**: Sezione "Presentazione della comunicazione di inizio dei lavori asseverata" → tre checkbox nel testo "l'inizio dei lavori per interventi soggetti a CILA"

**Causa**: Nessuna delle tre checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra le tre opzioni:
- ☐ **"per la cui realizzazione non sono necessari altri atti di assenso, altre segnalazioni o comunicazioni"**
- ☐ **"per la cui realizzazione presenta in allegato alla CILA le comunicazioni o segnalazioni certificate di inizio attività indicate nel quadro riepilogativo allegato"**
- ☐ **"per la cui realizzazione presenta contestualmente alla CILA la domanda per l'acquisizione d'ufficio degli atti d'assenso necessari..."**

{: .note }
> Nella versione attuale del modulo, le opzioni "LAVORI IN CORSO DI ESECUZIONE" e "LAVORI GIÀ ESEGUITI" (con campo data e sanzione) sono presenti nell'ASCX ma **commentate** e non visibili. Queste casistiche vengono gestite dalla sezione "Qualificazione dell'intervento" (sezione 4 di questa guida) tramite i radio button e_2 ed e_3.

---

## 4. Qualificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'intervento'.

**Causa**: Non hai indicato lo stato dei lavori.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **e.1** — Intervento normale (lavori da iniziare o da iniziare dopo acquisizione atti di assenso) → seleziona un sotto-radio inizio lavori
- ⚪ **e.2** — Intervento in corso di esecuzione (art. 6-bis c. 5 D.P.R. 380/2001) → inserisci data di inizio + allega ricevuta € 333,00
- ⚪ **e.3** — Intervento realizzato (art. 6-bis c. 5 D.P.R. 380/2001) → inserisci data realizzazione + allega ricevuta € 1.000,00

---

### Opzione e.1 — Intervento normale

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione di inizio lavori'.

**Causa**: Hai selezionato e.1 ma non hai indicato come e quando inizieranno i lavori.

**Soluzione**: Seleziona **uno dei due sotto-radio**:
- ⚪ **"i lavori avranno inizio in data"** → inserisci la data nel campo accanto (obbligatoria)
- ⚪ **"i lavori avranno inizio dopo la comunicazione, da parte dello sportello unico, dell'avvenuta acquisizione degli atti di assenso presupposti"**

---

#### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: Hai selezionato "i lavori avranno inizio in data" ma non hai compilato il campo data.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data inserita non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `01/06/2025`).

---

### Opzione e.2 — Lavori in corso di esecuzione

#### ATTENZIONE ! Campo obbligatorio 'Data lavori iniziati' non inserito.

**Causa**: Hai selezionato e.2 (lavori in corso) ma non hai inserito la data di inizio.

**Soluzione**: Inserisci nel campo a fianco del radio button la data in cui sono iniziati i lavori, nel formato **GG/MM/AAAA**.

{: .warning }
> Selezionando e.2 il sistema richiede l'allegato della ricevuta di versamento della **sanzione di € 333,00** (art. 6-bis c. 5 D.P.R. 380/2001). Assicurati di averla effettuata e allegata prima di inviare.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data lavori iniziati)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### Opzione e.3 — Lavori già realizzati

#### ATTENZIONE ! Campo obbligatorio 'Data lavori realizzati' non inserito.

**Causa**: Hai selezionato e.3 (lavori realizzati) ma non hai inserito la data di ultimazione.

**Soluzione**: Inserisci nel campo a fianco del radio button la data in cui i lavori sono stati completati, nel formato **GG/MM/AAAA**.

{: .warning }
> Selezionando e.3 il sistema richiede l'allegato della ricevuta di versamento della **sanzione di € 1.000,00** (art. 6-bis c. 5 D.P.R. 380/2001). Assicurati di averla effettuata e allegata.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data lavori realizzati)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 5. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inseriscilo nel campo testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure usa "Toponimo mancante".

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista.

---

## 6. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Non hai indicato se il contributo è dovuto.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"è a titolo gratuito"**
- ⚪ **"è a titolo oneroso"** (manutenzione straordinaria con aumento carico urbanistico/superficie) → spunta almeno una checkbox pagamento

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Pagamento'.

**Causa**: Hai selezionato "a titolo oneroso" ma non hai spuntato nessuna delle 2 checkbox del pagamento.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"allega la ricevuta di versamento"**
- ☐ **"effettuerà, prima dell'inizio dei lavori, il pagamento del contributo commisurato all'incidenza delle sole opere di urbanizzazione"**

{: .note }
> Il contributo nella CILA Nazionale è dovuto solo per interventi di manutenzione straordinaria che comportano **aumento del carico urbanistico** e **aumento della superficie calpestabile**. Nella maggioranza dei casi la CILA è gratuita.

---

## 7. Tecnici incaricati e impresa esecutrice

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"di aver incaricato in qualità di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'Soggetti coinvolti'"**
- ⚪ **"che gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"che i lavori sono/saranno eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'"** → l'impresa diventa obbligatoria nei soggetti
- ⚪ **"che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"**

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato la prima opzione impresa ma non hai aggiunto nessuna impresa nei soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi l'impresa esecutrice.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Causa**: Nessun tecnico con ruolo **PR (Progettista)** è presente nei soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **PR – Progettista**.

{: .note }
> Il Progettista (PR) è sempre obbligatorio nella CILA Nazionale, indipendentemente dalla semplicità dell'intervento, perché il modulo include la **dichiarazione del progettista** come parte integrante della comunicazione (asseverazione).

---

## 8. Sicurezza sul lavoro — D.Lgs. 81/2008

La CILA Nazionale ha la struttura sicurezza a **3 livelli** (senza il 4° livello Ge.CA/Allega presente in Lombardia).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **"non ricade nell'ambito di applicazione..."**
- ⚪ **"ricade nell'ambito di applicazione..."** → seleziona documentazione imprese + eventuale notifica
- ⚪ **"ricade nell'ambito... ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Soluzione**: Seleziona radio < 200 UG o ≥ 200 UG.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Soluzione**: Seleziona se la notifica è richiesta o meno.

{: .note }
> La CILA Nazionale non ha il 4° livello di notifica (nessun radio `$Allega`): quando si dichiara che la notifica è obbligatoria, compare solo la checkbox "allega la notifica" senza ulteriori sotto-opzioni da validare.

---

## 9. Tipologia di intervento e descrizione sintetica

Queste sezioni appartengono alle **Dichiarazioni del Progettista**.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia di intervento'.

**Dove si trova**: Sezione "DICHIARAZIONI DEL PROGETTISTA" → "Tipologia di intervento e descrizione sintetica delle opere" → lista di 8 radio button

**Causa**: Non hai selezionato la tipologia di intervento CILA applicabile secondo la Tabella A D.Lgs. 222/2016.

**Soluzione**: Seleziona **uno degli otto radio button**:
- ⚪ **1** — Manutenzione straordinaria (art. 3 c. 1 lett. b D.P.R. 380/2001) inclusa apertura porte/spostamento pareti non strutturali *(Attività n. 3, Tab. A, Sez. II)*
- ⚪ **2** — Restauro e risanamento conservativo (art. 3 c. 1 lett. c) non strutturale *(Attività n. 5)*
- ⚪ **3** — Eliminazione barriere architettoniche con ascensori esterni o manufatti che alterano la sagoma *(Attività n. 22)*
- ⚪ **4** — Opere temporanee per attività di ricerca nel sottosuolo (geognostica) in aree interne al centro edificato *(Attività n. 31)*
- ⚪ **5** — Movimenti di terra non pertinenti all'attività agricola *(Attività n. 32)*
- ⚪ **6** — Serre mobili stagionali con strutture in muratura *(Attività n. 33)*
- ⚪ **7** — Pertinenze minori (volume < 20% edificio principale) *(Attività n. 34)*
- ⚪ **8** — Altri interventi non riconducibili agli artt. 6, 10, 22 D.P.R. 380/2001 *(Attività n. 30)* → inserisci specificazione nel campo testo

---

### ATTENZIONE ! Specificare il tipo di intervento.

**Causa**: Hai selezionato la tipologia 8 ("altri interventi") ma non hai compilato il campo testo di specificazione.

**Soluzione**: Inserisci nel campo `txtSpecif1_8` la descrizione del tipo di intervento specifico (es. `Installazione di pannelli fotovoltaici integrati`, `Modifica prospetto senza alterazione sagoma`).

---

### ATTENZIONE ! Inserire la Descrizione sintetica delle opere.

**Dove si trova**: Nella sezione del progettista → punto "e che consistono in:" → campo multiriga `txtDescrIntervento`

**Causa**: Il campo descrizione sintetica delle opere nella sezione progettista è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

{: .note }
> Questo campo `txtDescrIntervento` è distinto dalla sezione "Qualificazione dell'intervento" del titolare. È la descrizione tecnica redatta dal progettista come parte dell'asseverazione.

---

## 10. Dichiarazione di tolleranze

La sezione tolleranze si attiva spuntando la checkbox `chkTolleranzev4_0` ("che l'immobile/U.I. oggetto dell'intervento presenta la/e seguente/i tolleranza/e"). Se non spuntata, nessun controllo viene eseguito.

---

### ATTENZIONE ! Selezionare almeno un tipo di tolleranza.

**Causa**: Hai spuntato la checkbox tolleranze ma non hai indicato nessuno dei 5 tipi.

**Soluzione**: Spunta **almeno una** tra le 5 tolleranze:
- ☐ **v4.1** — Tolleranza art. 34-bis c. 1 e 1-ter secondo periodo: scostamento ≤ 2% delle misure del titolo
- ☐ **v4.2** — Tolleranza art. 34-bis cc. 1-bis e 1-ter primo periodo: intervento entro il 24/05/2024, percentuali variabili per superficie → seleziona la percentuale applicabile
- ☐ **v4.3** — Tolleranza art. 34-bis c. 2: irregolarità geometriche e modifiche finiture di minima entità
- ☐ **v4.4** — Tolleranza art. 34-bis c. 2-bis: intervento entro il 24/05/2024, minore dimensionamento, errori progettuali corretti in cantiere
- ☐ **v4.5** — Tolleranza art. 34-ter c. 4: parziali difformità accertate in sopralluogo senza ordine di demolizione, con agibilità rilasciata

---

### ATTENZIONE ! Non è stata selezionata nessuna voce relativa alla percentuale di tolleranza.

**Causa**: Hai spuntato v4.2 (tolleranza per interventi ante 24/05/2024) ma non hai selezionato la percentuale applicabile in base alla superficie dell'unità immobiliare.

**Soluzione**: Seleziona **uno dei cinque radio button** della percentuale:
- ⚪ **2%** — per U.I. > 500 mq di superficie utile
- ⚪ **3%** — per U.I. da ≤ 500 mq e ≥ 300 mq
- ⚪ **4%** — per U.I. da < 500 mq e ≥ 100 mq
- ⚪ **5%** — per U.I. da < 100 mq e ≥ 60 mq
- ⚪ **6%** — per U.I. < 60 mq

---

### ATTENZIONE ! Non è stata selezionata nessuna voce relativa alla rilevanza sismica.

**Causa**: Hai spuntato almeno una tolleranza ma non hai indicato la zona sismica dell'immobile (obbligatorio per tutte le tolleranze).

**Soluzione**: Seleziona **uno dei due radio button** della zona sismica:
- ⚪ **"dà atto che l'immobile è ubicato in zona sismica a bassa sismicità (zone 3 e 4)"**
- ⚪ **"trattandosi di immobile ubicato in zona sismica a media o alta sismicità (zone 1 e 2)..."** → seleziona la rilevanza strutturale

---

### ATTENZIONE ! Non è stata selezionata nessuna voce relativa alla rilevanza strutturale.

**Causa**: Hai indicato zona sismica ad alta/media sismicità ma non hai specificato se la tolleranza ha rilevanza strutturale.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"non ha rilevanza strutturale"**
- ⚪ **"ha rilevanza strutturale..."** → seleziona la tipologia di intervento strutturale

---

### ATTENZIONE ! Non è stata selezionata nessuna voce relativa tipologia di intervento di rilevanza strutturale.

**Causa**: Hai dichiarato che la tolleranza ha rilevanza strutturale ma non hai indicato il livello di rilevanza pubblica.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **"intervento rilevante nei riguardi della pubblica incolumità"** (art. 94-bis c. 1 lett. a) → spunta almeno una delle 2 checkbox di autorizzazione sismica
- ⚪ **"intervento di minore rilevanza nei riguardi della pubblica incolumità"** (art. 94-bis c. 1 lett. b) → spunta la checkbox decorso del termine
- ⚪ **"intervento privo di rilevanza nei riguardi della pubblica incolumità"** (art. 94-bis c. 1 lett. c) → spunta la checkbox decorso del termine

---

### ATTENZIONE ! Selezionare almeno un tipo di autorizzazione. (rilevanza pubblica incolumità)

**Causa**: Hai selezionato "intervento rilevante" ma non hai spuntato nessuna delle 2 checkbox dell'autorizzazione sismica.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"allega l'autorizzazione sismica rilasciata in data ___ prot. n. ___"** → inserisci data + numero protocollo
- ☐ **"attesta che sulla istanza di autorizzazione presentata in data ___ prot. n. ___ si è formato il silenzio assenso"** → inserisci data + numero protocollo

---

#### ATTENZIONE ! Inserire la data di rilascio dell'autorizzazione sismica.

**Causa**: Hai spuntato "allega l'autorizzazione" ma non hai inserito la data.

**Soluzione**: Inserisci la data di rilascio nel campo accanto nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero del rilascio dell'autorizzazione sismica.

**Causa**: Hai spuntato "allega l'autorizzazione" ma non hai inserito il numero di protocollo.

**Soluzione**: Inserisci il numero nel campo "prot. n." accanto alla checkbox.

---

#### ATTENZIONE ! Inserire la data di presentazione dell'autorizzazione sismica.

**Causa**: Hai spuntato "attesta silenzio assenso" ma non hai inserito la data di presentazione dell'istanza.

**Soluzione**: Inserisci la data di presentazione dell'istanza di autorizzazione nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero di protocollo di presentazione dell'autorizzazione sismica.

**Causa**: Hai spuntato "attesta silenzio assenso" ma non hai inserito il numero di protocollo dell'istanza.

**Soluzione**: Inserisci il numero nel campo "prot. n." della seconda checkbox.

---

### ATTENZIONE ! Selezionare il decorso del termine. (minore rilevanza o privo di rilevanza)

**Causa**: Hai selezionato "intervento di minore rilevanza" o "intervento privo di rilevanza" ma non hai spuntato la checkbox del decorso del termine.

**Soluzione**: Spunta ☑ **"dichiara il decorso del termine del procedimento per i controlli regionali, in assenza di richieste di integrazione documentale o istruttorie inevase e di esito negativo dei controlli stessi"**.

---

## 11. Altre comunicazioni, segnalazioni, asseverazioni

La sezione mostra 5 righe opzionali (`chkPres3_1`–`chkPres3_5`). Se una checkbox è spuntata, entrambi i campi della riga diventano obbligatori.

---

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito. (sezione 3)

**Causa**: Hai spuntato una checkbox nella sezione "Altre comunicazioni" ma non hai compilato il campo "Comunicazioni, segnalazioni, etc." della stessa riga.

**Soluzione**: Inserisci la descrizione della comunicazione/segnalazione nel campo testo della riga corrispondente (es. `Comunicazione inizio lavori strutturali`, `SCIA antincendio`).

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito. (sezione 3)

**Causa**: Hai spuntato una checkbox nella sezione "Altre comunicazioni" e hai compilato la tipologia ma non l'autorità competente.

**Soluzione**: Inserisci il nome dell'autorità competente nel campo "Autorità competente" della stessa riga (es. `Ufficio Tecnico Comunale`, `Vigili del Fuoco`, `ASL`).

---

## 12. Atti di assenso da acquisire

La sezione mostra 5 righe opzionali (`chkPres4_1`–`chkPres4_5`). Stessa logica della sezione 11: se spuntata, tipologia + autorità obbligatorie.

---

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito. (sezione 4)

**Causa**: Hai spuntato una checkbox nella sezione "Atti di assenso" ma non hai compilato la tipologia di atto.

**Soluzione**: Inserisci la tipologia nel campo testo (es. `Autorizzazione paesaggistica`, `Nulla osta Soprintendenza`, `Parere AUSL`).

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito. (sezione 4)

**Causa**: Hai compilato la tipologia ma non l'autorità competente al rilascio.

**Soluzione**: Inserisci il nome dell'autorità competente (es. `Soprintendenza ABAP`, `Regione Piemonte`, `AUSL`).

---

## Consigli pratici CILA Nazionale

### Prima di validare ✅

**Sezione Titolare:**
- [ ] Seleziona la **titolarità** (radio button)
- [ ] Seleziona le **opere parti comuni** (una delle 4 opzioni)
- [ ] Spunta almeno una delle 3 **checkbox presentazione CILA**
- [ ] Seleziona la **qualificazione** (e.1, e.2 o e.3) e compila la data se richiesta
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **contributo** (gratuito o oneroso con almeno una checkbox)
- [ ] Seleziona **tecnici** e **impresa**; aggiungi **PR** nei soggetti e impresa se necessario
- [ ] Seleziona la voce **sicurezza** e compila le sotto-dichiarazioni

**Sezione Progettista:**
- [ ] Seleziona la **tipologia di intervento** (1–8); se 8 inserisci specificazione
- [ ] Inserisci la **descrizione sintetica delle opere** (max 300 caratteri)
- [ ] Se presenti tolleranze: spunta `chkTolleranzev4_0` → almeno una tolleranza → percentuale se v4.2 → zona sismica → rilevanza strutturale se zona 1/2 → autorizzazioni o decorso
- [ ] Per ogni riga spuntata in **"Altre comunicazioni"**: inserisci tipologia + autorità
- [ ] Per ogni riga spuntata in **"Atti di assenso"**: inserisci tipologia + autorità

### Sezioni presenti ma non validate ℹ️

- **Regolarità urbanistica**: sezione molto articolata (3 macro-opzioni con decine di sotto-checkbox) presente nell'ASCX ma **completamente commentata** nel validatore — non genera errori. Compilarla è comunque buona prassi documentale.
- **Dichiarazione tolleranze nella sezione titolare**: anch'essa commentata — non validata.
- **Contributo gratuito**: non richiede testo normativa (a differenza di CILA Liguria).
- **Calcolo del contributo nella sezione "oneroso"**: i sotto-radio "chiede allo Sportello" / "allega prospetto" non sono validati — solo le checkbox di pagamento.

### Differenze principali CILA Nazionale vs CILA regionali ⚠️

La CILA Nazionale si distingue per la presenza della **sezione progettista** con 8 tipologie di intervento D.Lgs. 222/2016. La dichiarazione di tolleranze è nel modulo del progettista, non come sezione separata come in alcune pratiche regionali. Le opzioni "lavori in corso" e "lavori già eseguiti" con le rispettive sanzioni (€ 333 e € 1.000) sono gestite direttamente nella sezione qualificazione con radio button e date. La sicurezza ha solo 3 livelli (no Ge.CA della Lombardia). Non ci sono coordinate UTM.

### Errori frequenti CILA Nazionale 🔍

1. **Checkbox presentazione CILA non spuntata** → sezione c) con tre opzioni, si trova in mezzo al modulo prima della qualificazione; viene saltata perché visivamente poco evidente
2. **Nessuna tipologia progettista selezionata** → le 8 opzioni della sezione progettista si trovano molto in fondo al modulo; scorrere fino alla sezione "DICHIARAZIONI DEL PROGETTISTA"
3. **Descrizione sintetica progettista vuota** → ci sono DUE campi descrizione: uno nella sezione qualificazione (se presente) e uno nella sezione progettista (`txtDescrIntervento`); quest'ultimo è quello obbligatorio
4. **Tolleranza v4.2 senza percentuale** → spuntare la checkbox v4.2 attiva immediatamente l'obbligo di selezionare la percentuale; le 5 opzioni (2%–6%) si trovano visivamente staccate sotto la checkbox
5. **Zona sismica alta senza completare la gerarchia** → la sezione tolleranze zona 1/2 ha fino a 5 livelli di radio button e checkbox; è facile fermarsi a metà lasciando un livello non compilato

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
3. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiCILANazionale e DatiCILANaz.ascx
