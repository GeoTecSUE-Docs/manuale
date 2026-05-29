---
title: Errori Accertamento di Compatibilità Paesaggistica - Regione Lombardia
parent: Errori di validazione
nav_order: 46
description: Errori di validazione specifici per l'Accertamento di Compatibilità Paesaggistica - Regione Lombardia (artt. 167 e 181 D.Lgs. 42/2004, L.R. 12/2005)
keywords: [accertamento compatibilità paesaggistica, ACP, Lombardia, art. 167 D.Lgs. 42/2004, art. 181, vincolo paesaggistico, art. 136, art. 142, coordinate UTM, stato attuale immobile, vincolo idrogeologico]
IDRegione: 4
IDTipoPratica: 453
Fonte: Manuale
---

# Errori di validazione - Accertamento di Compatibilità Paesaggistica
## Regione Lombardia

Guida completa agli errori specifici per l'**Accertamento di Compatibilità Paesaggistica** ai sensi degli artt. 167 e 181 del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio) e della L.R. Lombardia 11 marzo 2005, n. 12.

{: .note }
> L'ACP Lombardia è una pratica relativamente snella ma con alcune caratteristiche specifiche. La sezione **Tipologia dell'intervento** ha due checkbox principali indipendenti (almeno una obbligatoria), ciascuna con sotto-checkbox opzionali che, se spuntate, richiedono un campo testo. La sezione **Stato attuale immobile** ha 4 radio group Si/No completamente indipendenti: il validatore richiede che almeno uno dei 4 sia compilato, poi verifica i campi testo condizionali per le risposte "Sì". La sezione **Tecnici incaricati** è presente nel modulo ma **non validata** dal codice. Le coordinate UTM WGS84 32N sono obbligatorie con controllo di intervallo. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Tipologia dell'intervento](#3-tipologia-dellintervento)
4. [Descrizione dell'intervento](#4-descrizione-dellintervento)
5. [Stato attuale immobile](#5-stato-attuale-immobile)
6. [Rispetto della normativa sulla privacy](#6-rispetto-della-normativa-sulla-privacy)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Dove si trova**: Sezione "Titolarità dell'intervento" → 2 radio button sotto "dell'immobile interessato dall'intervento e di"

**Causa**: Non hai indicato se hai titolarità esclusiva sull'immobile.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu a discesa `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) e il campo "Specificare se altro" (`txtSpecifTitolarita1`) sono presenti nel modulo ma **non vengono validati** dal codice VB — non generano errori. Solo il radio button della titolarità esclusiva/non esclusiva è obbligatorio.

---

## 2. Localizzazione dell'intervento

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

**Soluzione**: Inserisci il numero civico.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

---

### Coordinate UTM WGS84 32N

#### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Causa**: Il campo "Coord. asse X" è vuoto.

**Soluzione**: Inserisci la coordinata X. Il valore deve essere compreso tra **430.000 e 700.000** (UTM WGS84 32N, in metri).

---

#### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: Il valore inserito è fuori dall'intervallo ammesso oppure non è un numero valido.

**Soluzione**: Inserisci un numero compreso tra **430.000** e **700.000**. Le coordinate UTM WGS84 32N per la Lombardia hanno tipicamente X nell'ordine di 480.000–580.000 m (es. `514523`). Inserire gradi decimali (es. `9.1`) o testo genera questo errore. Usa il pulsante "Calcola Coordinate" dalla cartografia se disponibile.

---

#### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo "Coord. asse Y" è vuoto.

**Soluzione**: Inserisci la coordinata Y. Il valore deve essere compreso tra **4.800.000 e 5.700.000**.

---

#### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Il valore inserito per Y è fuori intervallo o non numerico.

**Soluzione**: Inserisci un numero compreso tra **4.800.000** e **5.700.000** (es. `5034512`).

---

## 3. Tipologia dell'intervento

La sezione "Tipologia dell'intervento" contiene **due checkbox principali indipendenti** (`chkRicade_1` e `chkRicade_2`). Il validatore richiede che **almeno una** delle due sia spuntata. Ciascuna checkbox, se spuntata, può aprire sotto-opzioni con comportamenti diversi.

---

### ATTENZIONE !  Indicare tipologia dell'intervento.

**Dove si trova**: Sezione "Tipologia dell'intervento" → testo "che l'intervento:" → 2 checkbox principali. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice sorgente.

**Causa**: Nessuna delle due checkbox principali è spuntata.

**Soluzione**: Spunta **almeno una** tra le due checkbox principali:
- ☐ **chkRicade_1** — "è ricadente in ambito sottoposto a tutela ai sensi del d.lgs. 42/2004 (specificare la natura del vincolo)"
- ☐ **chkRicade_2** — "ricade tra gli interventi elencati all'art. 167, comma 4, del D.Lgs. 42/2004"

Le due checkbox non sono mutuamente esclusive: è possibile spuntarle entrambe.

---

### Sotto-opzioni di chkRicade_1 — Vincolo paesaggistico

Se spunti `chkRicade_1`, si abilitano 5 sotto-checkbox per specificare la natura del vincolo. Queste sotto-checkbox sono **tutte opzionali** — non è obbligatorio spuntarne alcuna. Tuttavia, **se una sotto-checkbox viene spuntata**, il campo testo affiancato diventa obbligatorio.

---

#### ATTENZIONE ! Specificare per art. 136.

**Causa**: Hai spuntato `chkRicade_1_1` ("art. 136 apposto con") ma il campo testo affiancato è vuoto.

**Soluzione**: Inserisci nel campo testo la specificazione del provvedimento che ha apposto il vincolo ai sensi dell'art. 136 del D.Lgs. 42/2004 (es. `D.M. 12/05/1967`, `D.Lgs. Pres. Rep. n. 45/2003`).

---

#### ATTENZIONE ! Specificare per art. 142.

**Causa**: Hai spuntato `chkRicade_1_2` ("art. 142") ma il campo testo affiancato è vuoto.

**Soluzione**: Inserisci la lettera o la specificazione del comma dell'art. 142 del D.Lgs. 42/2004 applicabile (es. `comma 1, lettera c) - fiumi e torrenti`, `comma 1, lettera g) - boschi`).

---

#### ATTENZIONE ! Specificare in dettaglio.

**Causa**: Hai spuntato una delle sotto-checkbox `chkRicade_1_3`, `chkRicade_1_4` o `chkRicade_1_5` (etichettate "Specificare" nel modulo) ma il campo testo affiancato corrispondente è vuoto.

**Soluzione**: Inserisci la specificazione dettagliata del vincolo nel campo testo accanto alla checkbox spuntata. Il messaggio è identico per tutte e tre le checkbox 1_3, 1_4 e 1_5.

---

### Sotto-opzioni di chkRicade_2 — Art. 167 c.4

Se spunti `chkRicade_2`, si visualizzano 3 sotto-checkbox relative alle tipologie di intervento dell'art. 167, comma 4:
- ☐ "lavori... che non abbiano determinato creazione di superfici utili o volumi..."
- ☐ "impiego di materiali in difformità dall'autorizzazione paesaggistica"
- ☐ "lavori comunque configurabili quali interventi di manutenzione ordinaria o straordinaria ai sensi dell'art. 27 della L.R. 12/2005"

{: .note }
> Le 3 sotto-checkbox di `chkRicade_2` **non generano errori** se non spuntate — non hanno campi testo associati e il validatore non le verifica. È possibile spuntare `chkRicade_2` senza selezionare nessuna delle 3 sotto-opzioni. Ai fini documentali è comunque opportuno specificare la tipologia applicabile.

---

## 4. Descrizione dell'intervento

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Descrizione dell'intervento" → campo multiriga sotto "consiste, sinteticamente, nelle seguenti opere:". Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice sorgente.

**Causa**: Il campo `txtDescrIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione sintetica delle opere nel campo multiriga (max **300 caratteri**).

---

## 5. Stato attuale immobile

La sezione "Stato attuale immobile" contiene **4 radio group Si/No completamente indipendenti**, ognuno relativo a una caratteristica dell'immobile. Il validatore verifica che **almeno uno dei 4 gruppi** abbia una risposta (Si o No). Poi controlla i campi testo condizionali per le risposte "Sì".

I 4 radio group corrispondono alle domande:
1. `$StatoAttualeImm1` — "ricade in zona assoggettata a vincolo idrogeologico" (Si/No)
2. `$StatoAttualeImm2` — "è interno al perimetro di aree regionali protette" (Si/No)
3. `$StatoAttualeImm3` — "è sottoposto a tutela ai sensi degli artt. 10 e 11 del d.lgs. 42/2004" (Si/No)
4. `$StatoAttualeImm4` — "è stato oggetto di precedenti autorizzazioni paesaggistiche" (Si/No)

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Stato attuale immobile'.

**Causa**: Nessuno dei 4 radio group ha una risposta — tutti e 4 i gruppi sono lasciati senza selezione.

**Soluzione**: Rispondi **almeno a uno** dei 4 radio group (Si o No). La buona prassi è rispondere a tutti e 4.

{: .note }
> Il validatore usa una condizione `And` su tutti e 4 i gruppi: genera l'errore solo se nessuno dei 4 è risposto. Tecnicamente è sufficiente rispondere a uno solo per superare questo controllo. Tuttavia, trattandosi di dichiarazioni su caratteristiche dell'immobile, è corretto rispondere a tutti e 4.

---

### ATTENZIONE ! Specificare aree regionali protette.

**Causa**: Hai risposto "Sì" alla seconda domanda ("è interno al perimetro di aree regionali protette") ma non hai compilato il campo testo affiancato.

**Soluzione**: Inserisci nel campo testo (`txtSpecificareAree`) il nome dell'area regionale protetta (es. `Parco Regionale delle Groane`, `Parco Naturale della Valle del Ticino`, `Riserva Naturale di Bosco Fontana`).

---

### ATTENZIONE ! Specificare beni sottoposti a tutela.

**Causa**: Hai risposto "Sì" alla terza domanda ("è sottoposto a tutela ai sensi degli artt. 10 e 11 del d.lgs. 42/2004") ma non hai compilato il campo testo affiancato.

**Soluzione**: Inserisci nel campo testo (`txtSpecificareBeni`) la descrizione del bene sottoposto a tutela culturale (es. `Villa storica d'interesse nazionale - D.M. 15/03/1985`, `immobile di interesse storico-artistico`).

---

### ATTENZIONE ! Specificare precedenti autorizzazioni paesaggistiche.

**Causa**: Hai risposto "Sì" alla quarta domanda ("è stato oggetto di precedenti autorizzazioni paesaggistiche") ma non hai compilato il **primo** campo testo affiancato (`txtSpecificarePrecAP`).

**Soluzione**: Inserisci nel primo campo la descrizione o i riferimenti alle precedenti autorizzazioni paesaggistiche (es. `AP n. 12/2018`, `autorizzazione paesaggistica del 15/06/2015`).

---

### ATTENZIONE ! Specificare ente e dati autorizzazione.

**Causa**: Hai compilato il primo campo delle precedenti autorizzazioni paesaggistiche ma non hai compilato il **secondo** campo (`txtSpecificareEnteDatiAut`).

**Soluzione**: Inserisci nel secondo campo l'ente che ha rilasciato la precedente autorizzazione e i dati identificativi (es. `Comune di Varese, prot. n. 4521 del 15/06/2015`, `Soprintendenza ABAP per la città metropolitana di Milano, n. 8734/2018`).

{: .note }
> Per la quarta domanda (precedenti autorizzazioni paesaggistiche) il sistema verifica **due campi separati** in sequenza: prima `txtSpecificarePrecAP` (descrizione AP), poi `txtSpecificareEnteDatiAut` (ente e dati). Entrambi diventano obbligatori se si risponde "Sì". La quarta domanda riguarda le precedenti AP sull'immobile, non quella attuale in richiesta.

---

## 6. Rispetto della normativa sulla privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione "Rispetto della normativa sulla privacy" → checkbox `chkPrivacy`

**Causa**: Non hai spuntato la dichiarazione "di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune".

**Soluzione**: Spunta la checkbox `chkPrivacy`.

---

## Consigli pratici — ACP Lombardia

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (esclusiva o non esclusiva)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci **coordinata X** (430.000–700.000) e **Y** (4.800.000–5.700.000) UTM WGS84 32N
- [ ] Spunta almeno una checkbox tra **chkRicade_1** e **chkRicade_2**; se chkRicade_1: per ogni sotto-checkbox spuntata, compila il campo testo affiancato
- [ ] Inserisci la **descrizione dell'intervento** (max 300 caratteri)
- [ ] Rispondi a tutti e 4 i radio Si/No nella sezione **Stato attuale immobile**; per ogni "Sì" compila i campi testo richiesti
- [ ] Spunta **chkPrivacy**

### Differenza ACP Piemonte vs ACP Lombardia

Rispetto all'[ACP Piemonte](errori-acp-piemonte.html), la versione Lombardia ha alcune differenze strutturali: le coordinate sono UTM WGS84 32N (X e Y in metri, non coordinate geografiche); la sezione tipologia ha 2 checkbox principali invece di 3 basi normative; lo stato attuale immobile è strutturato come 4 radio Si/No invece di checkbox; la sezione tecnici non è validata (in Piemonte è assente o diversamente gestita).

### Campi presenti ma non validati ℹ️

- **Menu titolarità** (`cmbTitoloSuImm`) e **"Specificare se altro"** (`txtSpecifTitolarita1`) — non validati
- **Sotto-checkbox di chkRicade_2** (chkRicade_2_1, 2_2, 2_3) — non validate, nessun campo testo
- **Sezione "Tecnici incaricati"** — presente nel modulo con testo descrittivo ma **completamente commentata nel codice VB**: nessun controllo tecnici viene eseguito
- **Radio Si/No del vincolo idrogeologico** (`$StatoAttualeImm1`) — non genera campi condizionali: rispondere Sì o No non richiede nessun testo aggiuntivo

### Struttura dello stato attuale immobile ⚠️

I 4 radio group Si/No sono completamente indipendenti — non è richiesta una risposta coerente o correlata tra di essi. Le risposte "Sì" ai gruppi 2, 3 e 4 aprono rispettivamente 1, 1 e 2 campi testo obbligatori. Il gruppo 1 (vincolo idrogeologico) non apre nessun campo, qualunque sia la risposta.

### Errori frequenti 🔍

1. **Nessuna checkbox tipologia spuntata** → sia chkRicade_1 che chkRicade_2 lasciate vuote generano il messaggio "Indicare tipologia dell'intervento"; spuntarne almeno una è sufficiente
2. **Sotto-checkbox di chkRicade_1 spuntata senza campo testo** → ogni sotto-checkbox (1_1..1_5) richiede obbligatoriamente il testo affiancato; dimenticare di compilarlo blocca la validazione
3. **Coordinate fuori intervallo** → valori in gradi decimali generano l'errore di intervallo; le coordinate UTM 32N per la Lombardia hanno X ~500.000 e Y ~5.000.000
4. **Stato attuale immobile ignorato** → la sezione Si/No è spesso trascurata perché visivamente non sembra obbligatoria; almeno un gruppo deve avere risposta
5. **Secondo campo AP mancante** → per la quarta domanda (precedenti AP) ci sono 2 campi distinti; compilarne solo uno blocca al secondo errore

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
**Fonte**: Analisi codice ValidaDatiACPLombardia e DatiACPLombardia.ascx
