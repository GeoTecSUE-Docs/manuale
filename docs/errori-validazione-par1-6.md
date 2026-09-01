---
title: Errori Pareri Preliminari per Attività Edilizia Libera, CILA e SCIA - Regione Piemonte
parent: Errori di validazione
nav_order: 58
description: Errori di validazione per la richiesta di Pareri Preliminari (1PAR) per attività edilizia libera, CILA e SCIA - Regione Piemonte (art. 23-bis D.P.R. 380/2001)
keywords: [pareri preliminari, 1PAR, parere preventivo, atti di assenso, art. 23-bis DPR 380, Piemonte, attività edilizia libera, CILA, SCIA, SUE, sportello unico edilizia, autorizzazione paesaggistica, vincolo idrogeologico, VVF, soprintendenza]
IDRegione: 2
IDTipoPratica: 6
Fonte: Manuale
---

# Errori di validazione - Pareri Preliminari per Attività Edilizia Libera, CILA e SCIA
## Regione Piemonte

Guida completa agli errori specifici per la **richiesta di Pareri Preliminari (1PAR)** — pratica con cui il titolare chiede allo Sportello Unico per l'Edilizia (SUE) di acquisire preventivamente gli atti di assenso e pareri necessari per un futuro intervento edilizio, ai sensi dell'art. 23-bis del D.P.R. 6 giugno 2001, n. 380.

{: .note }
> La pratica 1PAR è strutturalmente diversa da tutte le altre pratiche del sistema: non è una dichiarazione di inizio lavori ma una **richiesta preliminare di pareri e autorizzazioni** che il SUE acquisisce prima che il titolare presenti la pratica edilizia vera e propria (Attività Edilizia Libera, CILA o SCIA). Il modulo si articola in tre blocchi distinti: DICHIARA (titolarità, localizzazione, tipo di intervento futuro, descrizione) → COMUNICA (atti già presentati tramite GeoTecSUE, sezione non obbligatoria) → RICHIEDE (atti da acquisire presso il Comune e presso altre Amministrazioni). Il validatore controlla le due sezioni "RICHIEDE" in modo combinato: basta spuntare **almeno una checkbox** in totale tra le due sezioni ("Comune" e "Altre Amministrazioni") per soddisfare l'obbligo. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Tipo di intervento futuro](#3-tipo-di-intervento-futuro)
4. [Descrizione dell'intervento](#4-descrizione-dellintervento)
5. [Acquisizione atti di assenso e pareri — RICHIEDE](#5-acquisizione-atti-di-assenso-e-pareri--richiede)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Dove si trova**: Sezione "Titolarità Intervento" → 2 radio button del gruppo `$Titolarita`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) è presente ma **non validato**. Non genera errori.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inserisci il nome della via nel campo testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico dell'immobile.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

{: .note }
> Il campo "Coordinate" (`txtCoordinate`) è presente ma non validato.

---

## 3. Tipo di intervento futuro

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo di intervento'.

**Dove si trova**: Sezione "Tipo di intervento che verrà eseguito successivamente all'ottenimento degli atti di assenso o pareri necessari per l'intervento edilizio" → 3 radio button del gruppo `$TipoInt`

**Causa**: Nessun radio button è selezionato. Questo campo indica il tipo di pratica edilizia che il titolare intende presentare **dopo** aver ottenuto i pareri richiesti.

**Soluzione**: Seleziona **uno dei tre radio button** corrispondente alla pratica che si presenterà in seguito:
- ⚪ **b_1** — "Attività Edilizia Libera art. 6 del D.P.R. 380/2001 e s.m.i."
- ⚪ **b_2** — "Comunicazione di Inizio Attività Asseverata ai sensi dell'art. 6-bis del D.P.R. 380/2001 e s.m.i." (CILA)
- ⚪ **b_3** — "Segnalazione Certificata di Inizio Attività ai sensi dell'art. 22 del D.P.R. 380/2001 e s.m.i." (SCIA)

{: .note }
> La scelta del tipo di intervento non attiva campi condizionali nel validatore: tutte e tre le opzioni hanno lo stesso comportamento ai fini della validazione. Indica la pratica che si prevede di presentare una volta ottenuti i pareri, in modo che il SUE possa istruire correttamente la richiesta.

---

## 4. Descrizione dell'intervento

### ATTENZIONE ! Campo obbligatorio 'Descrizione dell'intervento' non inserito.

**Dove si trova**: Sezione "Descrizione dell'intervento" → campo multiriga `txtDescrIntervento` "per l'intervento di:" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto.

**Soluzione**: Inserisci la descrizione delle opere che si intende realizzare (max **300 caratteri**).

---

## 5. Acquisizione atti di assenso e pareri — RICHIEDE

Il validatore controlla le due sezioni "RICHIEDE" in modo **combinato**: scorre prima tutte le checkbox della sezione "Comune" (`chkAcqComune1PARe_1..10`), poi tutte quelle della sezione "Altre Amministrazioni" (`chkAcqAltreAmm1PARf_1..28`). Se almeno una checkbox in totale è spuntata, il requisito è soddisfatto. Solo al termine, se nessuna checkbox risulta spuntata in nessuna delle due sezioni, viene generato il messaggio di errore.

{: .note }
> La sezione **"COMUNICA — Acquisizione atti di assenso e pareri presso lo Sportello Unico per l'Edilizia"** (7 checkbox d_1..d_7 per atti già presentati tramite GeoTecSUE) è presente nel modulo ma è **completamente commentata nel codice di validazione** e quindi non obbligatoria. Può essere compilata facoltativamente per indicare atti già presentati, ma non genera errori se lasciata vuota.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Acquisizione atti di assenso e pareri'.

**Dove si trova**: Sezioni "RICHIEDE" → "Acquisizione atti di assenso e pareri presso il Comune" e/o "Acquisizione atti di assenso e pareri presso altre Amministrazioni"

**Causa**: Nessuna checkbox è spuntata in nessuna delle due sezioni "RICHIEDE" — né nella sezione Comune né in quella Altre Amministrazioni.

**Soluzione**: Spunta **almeno una checkbox** tra le due sezioni. Indica il parere o l'atto di assenso che il SUE dovrà acquisire prima che si possa presentare la pratica edilizia.

**Sezione "presso il Comune"** (10 opzioni — `chkAcqComune1PARe_1..10`):

Parere della Polizia Municipale in materia di viabilità; nulla osta commissione di vigilanza pubblici spettacoli; autorizzazione alla manomissione di suolo pubblico; autorizzazione temporanea all'occupazione di suolo pubblico; concessione all'occupazione di suolo pubblico; istanza di accertamento del possesso dei requisiti di Imprenditore Agricolo Professionale; autorizzazione per impianti o attività produttive soggette a documentazione di impatto acustico; autorizzazione per lavori da eseguirsi all'interno della delimitazione del centro abitato; pareri per interventi posti sotto la tutela dell'UNESCO; **altro** (`chkAcqComune1PARe_10`) → senza descrizione aggiuntiva obbligatoria (vedi nota bug).

**Sezione "presso altre Amministrazioni"** (28 opzioni — `chkAcqAltreAmm1PARf_1..28`):

Valutazione del progetto ai fini della conformità alla normativa di prevenzione incendi (VVF, D.P.R. 151/2011 categorie B e C); richiesta di deroga all'osservanza delle regole tecniche di prevenzione incendi; utilizzo di terre e rocce da scavo (VIA o AIA); autorizzazione per interventi in zone sismiche ad alta e media sismicità; autorizzazione per opere su beni culturali; autorizzazione per interventi su immobili in area sottoposta a tutela (fasce di rispetto dei corpi idrici); autorizzazione per costruzioni in area di rispetto del demanio marittimo; autorizzazione per costruzioni o opere in prossimità della linea doganale in mare territoriale; autorizzazione per interventi in aree naturali protette; autorizzazione per interventi nelle zone della rete "Natura 2000"; autorizzazione della soprintendenza archeologica; autorizzazione/concessione per lavori all'esterno della delimitazione del centro abitato; assenso dell'amministrazione militare (zone di salvaguardia contigue a difesa dello Stato); deroga alla fascia di rispetto cimiteriale; parere ARPA; atto di assenso su vincoli di tutela ecologica; assenso in materia di servitù viarie; assenso in materia di servitù ferroviarie o tramviarie; assenso in materia di servitù portuali; assenso in materia di servitù aeroportuali; assenso in materia di servitù di elettrodotto; assenso in materia di servitù di gasdotto; assenso in materia di vincoli di tutela ecologica; parere forestale; **parere della Regione** (`chkAcqAltreAmm1PARf_25`) → descrizione obbligatoria; **parere della Provincia/Città Metropolitana** (`chkAcqAltreAmm1PARf_26`) → descrizione obbligatoria; valutazione del progetto da parte del Comitato Tecnico Regionale (area di danno da incidente rilevante); **altro** (`chkAcqAltreAmm1PARf_28`) → descrizione obbligatoria.

---

### ATTENZIONE ! Specificare una descrizione. (f_25 — parere Regione)

**Causa**: Hai spuntato `chkAcqAltreAmm1PARf_25` "parere della Regione" ma non hai inserito la descrizione nel campo testo affiancato `txtDescrf_25`.

**Soluzione**: Inserisci nel campo testo la specifica del parere regionale richiesto (es. `Parere Regione Piemonte - Settore Gestione delle Risorse Idriche`).

---

### ATTENZIONE ! Specificare una descrizione. (f_26 — parere Provincia/Città Metropolitana)

**Causa**: Hai spuntato `chkAcqAltreAmm1PARf_26` "parere della Provincia/Città Metropolitana" ma non hai inserito la descrizione nel campo `txtDescrf_26`.

**Soluzione**: Inserisci nel campo testo la specifica del parere provinciale o metropolitano richiesto.

---

### ATTENZIONE ! Specificare una descrizione. (f_28 — altro Altre Amministrazioni)

**Causa**: Hai spuntato `chkAcqAltreAmm1PARf_28` "altro" nella sezione Altre Amministrazioni ma non hai inserito la descrizione nel campo `txtDescrf_28`.

**Soluzione**: Inserisci nel campo testo la descrizione dell'atto di assenso o parere da acquisire presso l'altra Pubblica Amministrazione non elencata.

{: .warning }
> **Nota bug — "altro" sezione Comune (e_10)**: la checkbox `chkAcqComune1PARe_10` "altro" nella sezione Comune ha un campo di descrizione affiancato (`txtDescre_10`), ma il validatore cerca `Case 11` invece di `Case 10` a causa di un refuso nel codice. Di conseguenza, la descrizione di e_10 **non viene mai validata** anche se la checkbox è spuntata: il campo `txtDescre_10` può essere lasciato vuoto senza generare errori. Compilarlo è comunque consigliato per documentare correttamente la richiesta.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: La griglia dei tecnici (`DSTecnici`) è vuota — nessun tecnico è stato aggiunto tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico con qualsiasi ruolo.

{: .note }
> A differenza di molte altre pratiche, il validatore della 1PAR non richiede un ruolo specifico (PR, RI, ecc.) — controlla solo che esista **almeno un tecnico** con `DSTecnici.Tables(0).Rows.Count > 0`. È sufficiente aggiungere il tecnico incaricato della pratica con qualsiasi ruolo disponibile.

---

## Consigli pratici — 1PAR Piemonte

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **tipo di intervento futuro** (Attività Edilizia Libera / CILA / SCIA)
- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Spunta **almeno una checkbox** tra le sezioni "presso il Comune" o "presso altre Amministrazioni"; se f_25, f_26 o f_28: inserisci la descrizione nel campo testo affiancato
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti (qualsiasi ruolo)

### Sezioni presenti ma non validate ℹ️

La sezione **"COMUNICA — Acquisizione atti di assenso e pareri presso lo Sportello Unico per l'Edilizia"** (7 checkbox d_1..d_7 — atti già presentati tramite GeoTecSUE) è facoltativamente compilabile ma non obbligatoria: la sua validazione è commentata nel codice con il commento `'' d) Non obbligatorio`. Possono essere spuntate per indicare al SUE atti già presentati in precedenza attraverso il portale, ma non è richiesto ai fini della validazione. Anche il campo **"Indicazioni utili allo Sportello Unico per l'Edilizia"** (`txtDescrIndicazioniSUE`), il menu **`cmbTitoloSuImm`** e il campo **"Coordinate"** sono facoltativi.

### Logica combinata delle sezioni "RICHIEDE" ⚠️

Il validatore scorre le checkbox di `pnlAcqComune` (e_1..e_10) e poi quelle di `pnlAcqAltreAmm` (f_1..f_28) con un unico flag `FlagCheck`. Non è necessario compilare entrambe le sezioni: basta spuntare almeno una checkbox in totale. Il controllo delle descrizioni obbligatorie (f_25, f_26, f_28) avviene durante la scansione: se una di queste checkbox è spuntata e il campo descrizione è vuoto, il validatore si ferma subito con "Specificare una descrizione" prima di arrivare al controllo del flag finale.

### Errori frequenti 🔍

1. **Nessun parere selezionato** → la sezione d (COMUNICA, atti già presentati) non conta; serve almeno una checkbox nelle sezioni RICHIEDE (e o f)
2. **f_25/f_26/f_28 spuntate senza descrizione** → "Specificare una descrizione" appare anche se altri pareri sono già spuntati — controllare sempre i campi testo affiancati alle tre checkbox con descrizione
3. **Tipo di intervento futuro non selezionato** → radio `$TipoInt` obbligatorio; indica la pratica da presentare dopo i pareri
4. **Tecnico mancante** → qualsiasi ruolo è accettato; aggiungerne almeno uno prima di validare
5. **"altro" Comune (e_10) senza descrizione** → per il bug descritto sopra non genera errore ma è buona pratica compilarlo comunque

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
**Fonte**: Analisi codice ValidaDati1PAR e Dati1PAR.ascx
