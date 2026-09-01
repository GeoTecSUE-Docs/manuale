---
title: Errori Acquisizione Atti di Assenso o Pareri per Pratica Edilizia in Corso - Regione Piemonte
parent: Errori di validazione
nav_order: 60
description: Errori di validazione per la richiesta di Acquisizione Atti di Assenso o Pareri per pratica edilizia già in corso (2PAR) - Regione Piemonte (artt. 5, 19-bis, 20 D.P.R. 380/2001, art. 19-bis L. 241/1990)
keywords: [pareri, 2PAR, acquisizione atti assenso, pratica edilizia in corso, art. 20 DPR 380, art. 19-bis L.241, art. 5 DPR 380, Piemonte, titolo edilizio, SUE, autorizzazione paesaggistica, VVF, soprintendenza]
IDRegione: 2
IDTipoPratica: 9
Fonte: Manuale
---

# Errori di validazione - Acquisizione Atti di Assenso o Pareri per Pratica Edilizia in Corso
## Regione Piemonte

Guida completa agli errori specifici per la **richiesta di Acquisizione Atti di Assenso o Pareri (2PAR)** — pratica con cui il titolare chiede allo Sportello Unico per l'Edilizia (SUE) di acquisire pareri e atti di assenso nell'ambito di una pratica edilizia **già presentata** (Permesso di Costruire, SCIA, CILA o altra), ai sensi degli artt. 20 c. 3, 5 c. 1-bis del D.P.R. 380/2001 e dell'art. 19-bis c. 3 della L. 241/1990 — Regione Piemonte.

{: .note }
> La 2PAR è la pratica "gemella" della [1PAR](errori-1par-piemonte.html) ma con una differenza fondamentale: mentre la 1PAR richiede pareri **prima** di presentare la pratica edilizia, la 2PAR li richiede per una pratica edilizia **già in corso** (già presentata). Questa differenza si riflette nel modulo: invece di indicare il tipo di pratica futura (come nella 1PAR), si indica il **titolo edilizio di riferimento** già esistente con menu, numero e data. La sezione "Tipologia di richiesta parere" identifica la base normativa (art. 20, art. 19-bis o art. 5) con cui il SUE acquisirà i pareri nell'ambito di quella pratica. La struttura delle sezioni "RICHIEDE" e la logica di validazione combinata delle checkbox sono identiche alla 1PAR. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Titolo edilizio di riferimento](#2-titolo-edilizio-di-riferimento)
3. [Tipologia di richiesta parere](#3-tipologia-di-richiesta-parere)
4. [Acquisizione atti di assenso e pareri — RICHIEDE](#4-acquisizione-atti-di-assenso-e-pareri--richiede)
5. [Tecnici nei soggetti coinvolti](#5-tecnici-nei-soggetti-coinvolti)

---

## 1. Localizzazione dell'intervento

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

**Soluzione**: Inserisci il numero civico.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

{: .note }
> La 2PAR **non ha la sezione Titolarità** (radio `$Titolarita`) a differenza della 1PAR e delle altre pratiche. Il modulo inizia direttamente con la Localizzazione. Il campo "Coordinate" (`txtCoordinate`) è presente ma non validato.

---

## 2. Titolo edilizio di riferimento

Questa sezione è specifica della 2PAR e non esiste nella 1PAR. Identifica la pratica edilizia già presentata per cui si richiedono i pareri.

---

### ATTENZIONE ! Selezionare il titolo abitativo edilizio.

**Dove si trova**: Sezione "che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente:" → menu a discesa `cmbTitoliAbitEdilizi`

**Causa**: Il menu `cmbTitoliAbitEdilizi` è rimasto sulla voce vuota iniziale (`SelectedIndex = 0`).

**Soluzione**: Seleziona dal menu il tipo di titolo edilizio della pratica già presentata (es. Permesso di Costruire, SCIA alternativa al PdC, CILA, ecc.).

---

### ATTENZIONE ! Inserire il numero.

**Causa**: Il campo `txtNTitEdilizio` "prot. / n." del titolo edilizio è vuoto.

**Soluzione**: Inserisci il numero di protocollo o il numero identificativo della pratica edilizia già presentata.

---

### ATTENZIONE ! Inserire la data.

**Causa**: Il campo `txtDataTitEdilizio` "del" della data del titolo edilizio è vuoto.

**Soluzione**: Inserisci la data del titolo edilizio nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data titolo edilizio)

**Causa**: La data del titolo edilizio non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `28/03/2025`).

---

## 3. Tipologia di richiesta parere

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia di richiesta parere'.

**Dove si trova**: Sezione "RICHIEDE — Tipologia di richiesta di parere:" → 3 radio button `$TipologiaRichParere`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button** corrispondente alla base normativa con cui il SUE acquisirà i pareri:
- ⚪ **c_1** — "ai sensi dell'art. 20 c. 3 D.P.R. n. 380/2001 e ss.mm.ii." — per pratiche soggette a Permesso di Costruire
- ⚪ **c_2** — "ai sensi dell'art. 19-bis c. 3 Legge 241/1990 e ss.mm.ii." — per pratiche soggette a SCIA (procedimento unico)
- ⚪ **c_3** — "ai sensi dell'art. 5 c. 1-bis D.P.R. n. 380/2001 e ss.mm.ii." — per pratiche di competenza dello Sportello Unico

{: .note }
> La scelta della tipologia di richiesta dipende dal tipo di pratica edilizia indicata nella sezione precedente: art. 20 c. 3 per pratiche di PdC (conferenza di servizi nell'ambito del procedimento di rilascio del permesso); art. 19-bis c. 3 per pratiche SCIA (consultazione preventiva per SCIA condizionata); art. 5 c. 1-bis per pratiche di competenza generale del SUE. In caso di dubbio, consultare l'ufficio tecnico comunale.

---

## 4. Acquisizione atti di assenso e pareri — RICHIEDE

Il validatore controlla le due sezioni "RICHIEDE" in modo **combinato**: scorre prima tutte le checkbox della sezione "Comune" (`chkAcqComune2PARd_1..10`), poi quelle della sezione "Altre Amministrazioni" (`chkAcqAltreAmm2PARe_1..28`). Deve essere spuntata **almeno una checkbox** in totale tra le due sezioni.

{: .note }
> La sezione **"COMUNICA — Acquisizione atti di assenso e pareri presso lo Sportello Unico per l'Edilizia"** (7 checkbox b_1..b_7 per atti già presentati tramite GeoTecSUE) **non è validata** — stesso comportamento della 1PAR. Può essere compilata facoltativamente per indicare al SUE atti già presentati in precedenza, ma non è obbligatoria.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Acquisizione atti di assenso e pareri'.

**Dove si trova**: Sezioni "RICHIEDE" → "Acquisizione atti di assenso e pareri presso il Comune" e/o "Acquisizione atti di assenso e pareri presso altre Amministrazioni"

**Causa**: Nessuna checkbox è spuntata in nessuna delle due sezioni RICHIEDE.

**Soluzione**: Spunta **almeno una checkbox** tra le due sezioni.

**Sezione "presso il Comune"** (10 opzioni — `chkAcqComune2PARd_1..10`):

Parere della Polizia Municipale in materia di viabilità; nulla osta commissione di vigilanza pubblici spettacoli; autorizzazione alla manomissione di suolo pubblico; autorizzazione temporanea all'occupazione di suolo pubblico; concessione all'occupazione di suolo pubblico; istanza di accertamento del possesso dei requisiti di Imprenditore Agricolo Professionale; autorizzazione per impianti o attività produttive soggette a documentazione di impatto acustico; autorizzazione per lavori all'interno della delimitazione del centro abitato; richiesta di deroga alla normativa per l'abbattimento delle barriere architettoniche; **altro** (`chkAcqComune2PARd_10`) → senza validazione descrizione (vedi nota bug).

{: .note }
> La sezione Comune della 2PAR si differenzia da quella della 1PAR per la **d_9**: qui è "richiesta di deroga alla normativa per l'abbattimento delle barriere architettoniche" invece di "pareri per interventi posti sotto la tutela dell'UNESCO" (presente nella 1PAR). Manca anche la voce UNESCO (presente invece nella sezione Comune della 1PAR come e_9).

**Sezione "presso altre Amministrazioni"** (28 opzioni — `chkAcqAltreAmm2PARe_1..28`):

Valutazione del progetto ai fini della conformità alla normativa di prevenzione incendi (VVF, D.P.R. 151/2011 categorie B e C); richiesta di deroga all'osservanza delle regole tecniche di prevenzione incendi; utilizzo di terre e rocce da scavo (VIA o AIA); autorizzazione per interventi in zone sismiche ad alta e media sismicità; autorizzazione per opere su beni culturali; autorizzazione per interventi in area sottoposta a tutela (fasce di rispetto corpi idrici); autorizzazione per costruzioni in area di rispetto del demanio marittimo; autorizzazione per costruzioni o opere in prossimità della linea doganale in mare territoriale; autorizzazione per interventi in aree naturali protette; autorizzazione per interventi nelle zone della rete "Natura 2000"; autorizzazione della soprintendenza archeologica; autorizzazione/concessione per lavori all'esterno della delimitazione del centro abitato; assenso dell'amministrazione militare (zone di salvaguardia contigue a difesa dello Stato); deroga alla fascia di rispetto cimiteriale; parere ARPA; atto di assenso su vincoli di tutela ecologica; assenso in materia di servitù viarie; assenso in materia di servitù ferroviarie o tramviarie; assenso in materia di servitù portuali; assenso in materia di servitù aeroportuali; assenso in materia di servitù di elettrodotto; assenso in materia di servitù di gasdotto; assenso in materia di vincoli di tutela ecologica; parere forestale; **parere della Regione** (e_25) → descrizione obbligatoria; **parere della Provincia/Città Metropolitana** (e_26) → descrizione obbligatoria; valutazione del progetto da parte del Comitato Tecnico Regionale (area di danno da incidente rilevante); **altro** (e_28) → descrizione obbligatoria.

---

### ATTENZIONE ! Specificare una descrizione. (e_25 — parere Regione)

**Causa**: Hai spuntato `chkAcqAltreAmm2PARe_25` "parere della Regione" ma non hai inserito la descrizione nel campo `txtDescre_25`.

**Soluzione**: Inserisci nel campo testo la specifica del parere regionale richiesto.

---

### ATTENZIONE ! Specificare una descrizione. (e_26 — parere Provincia/Città Metropolitana)

**Causa**: Hai spuntato `chkAcqAltreAmm2PARe_26` "parere della Provincia/Città Metropolitana" ma non hai inserito la descrizione nel campo `txtDescre_26`.

**Soluzione**: Inserisci nel campo testo la specifica del parere provinciale o metropolitano.

---

### ATTENZIONE ! Specificare una descrizione. (e_28 — altro Altre Amministrazioni)

**Causa**: Hai spuntato `chkAcqAltreAmm2PARe_28` "altro" nella sezione Altre Amministrazioni ma non hai inserito la descrizione nel campo `txtDescre_28`.

**Soluzione**: Inserisci nel campo testo la descrizione dell'atto da acquisire presso l'altra Pubblica Amministrazione.

{: .warning }
> **Nota bug — "altro" sezione Comune (d_10)**: come nella 1PAR, il validatore cerca `Case 11` invece di `Case 10` per la checkbox "altro" della sezione Comune. Di conseguenza `txtDescrd_10` non viene mai validata anche se la checkbox è spuntata. Ulteriore anomalia: il codice tenta di mettere il focus su `txtDescrd_11` (che non esiste) invece di `txtDescrd_10`. Compilare il campo è comunque buona pratica ma non genera errori di validazione.

---

## 5. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: La griglia dei tecnici è vuota — nessun tecnico è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico con qualsiasi ruolo.

---

## Consigli pratici — 2PAR Piemonte

### Prima di validare ✅

- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **tipo di titolo edilizio** dal menu
- [ ] Inserisci il **numero/prot.** del titolo edilizio
- [ ] Inserisci la **data** del titolo edilizio (GG/MM/AAAA)
- [ ] Seleziona la **tipologia di richiesta parere** (c_1/c_2/c_3)
- [ ] Spunta **almeno una checkbox** tra le sezioni "presso il Comune" o "presso altre Amministrazioni"; se e_25, e_26 o e_28: inserisci la descrizione nel campo testo affiancato
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti (qualsiasi ruolo)

### Differenze rispetto alla 1PAR ℹ️

La 2PAR si distingue dalla 1PAR per: assenza della sezione Titolarità (radio `$Titolarita`); presenza del blocco "Titolo edilizio di riferimento" (menu + numero + data) invece del radio "Tipo di intervento futuro"; presenza della sezione "Tipologia di richiesta parere" (3 radio normativi); sezione Comune d_9 diversa ("deroga barriere architettoniche" invece di "UNESCO"); i campi descrizione delle checkbox con testo libero usano `txtDescre_N` (con la 'e') anche nella sezione Comune — il campo per d_10 si chiama `txtDescrd_10` (con la 'd') nel modulo ma il codice cerca `txtDescre_10` (con la 'e') per il focus del bug, il che rende il bug doppiamente irrilevante.

### Sezioni presenti ma non validate ℹ️

**Sezione b** (7 checkbox `chkAcqSUE2PARb_1..7` — atti già presentati tramite GeoTecSUE): non validata, facoltativa. **`txtDescrIndicazioniSUE`**: facoltativo. **`txtCoordinate`**: non validato. **Privacy**: solo testo informativo.

### Errori frequenti 🔍

1. **Menu titolo edilizio su voce vuota** → il sistema verifica `SelectedIndex = 0`; selezionare il tipo di pratica prima di procedere
2. **Data titolo edilizio vuota o con formato errato** → obbligatoria in formato GG/MM/AAAA; a differenza della 1PAR non ci sono controlli sulla data rispetto ad oggi
3. **Tipologia richiesta parere non selezionata** → sezione specifica della 2PAR; selezionare la base normativa corretta in base al tipo di pratica
4. **Nessun parere selezionato** → stessa logica combinata della 1PAR; almeno una checkbox nelle sezioni d o e
5. **e_25/e_26/e_28 senza descrizione** → controllare i campi testo affiancati alle tre checkbox con descrizione libera

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Vedi anche [Errori 1PAR Piemonte](errori-1par-piemonte.html) — struttura analoga
3. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDati2PAR e Dati2PAR.ascx
