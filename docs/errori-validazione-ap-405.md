---
title: Errori Autorizzazione Paesaggistica Ordinaria - Regione Lombardia
parent: Errori di validazione
nav_order: 43
description: Errori di validazione specifici per l'Autorizzazione Paesaggistica Ordinaria - Regione Lombardia (art. 146 D.Lgs. 42/2004, L.R. 12/2005)
keywords: [autorizzazione paesaggistica, AP, Lombardia, art. 146 D.Lgs. 42/2004, art. 136, art. 142, art. 80 LR 12/2005, L.R. 12/2005, coordinate UTM, WGS84, 32N, vincolo paesaggistico, variante, altron]
IDRegione: 4
IDTipoPratica: 405
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Ordinaria
## Regione Lombardia

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Ordinaria** ai sensi dell'art. 146, comma 2, del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio) e della L.R. Lombardia 11 marzo 2005, n. 12, relativa alla **Regione Lombardia**.

{: .note }
> L'AP Lombardia ha alcune caratteristiche distintive rispetto alle altre regioni. La **titolarità** ha un campo testo "Specificare se altro" che diventa obbligatorio solo se si seleziona il valore `altron` dal menu. Le **coordinate UTM WGS84 32N** sono obbligatorie e validate su intervalli precisi (X: 430.000–700.000; Y: 4.800.000–5.700.000) — un valore non numerico o fuori range produce lo stesso messaggio di errore. Le **dichiarazioni di vincolo** (4 checkbox) non hanno un controllo "almeno una obbligatoria": ogni checkbox, se spuntata, richiede la lettera corrispondente, ma è possibile non spuntarne nessuna. Nei soggetti coinvolti è sufficiente almeno **un tecnico di qualsiasi ruolo** (non è richiesto un ruolo specifico come PR o DR). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Descrizione sintetica dell'intervento](#3-descrizione-sintetica-dellintervento)
4. [Dichiarazioni — Vincolo paesaggistico](#4-dichiarazioni--vincolo-paesaggistico)
5. [In caso di intervento di variante](#5-in-caso-di-intervento-di-variante)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Specificare la titolarità dell'intervento.

**Dove si trova**: Sezione "Titolarità dell'intervento" → campo testo "Specificare se altro" (`txtSpecifTitolarita1`)

**Causa**: Il menu `cmbTitoloSuImm` è impostato sul valore `altron` (voce "Altro") ma il campo di specificazione è vuoto.

**Soluzione**: Inserisci nel campo testo la specificazione della tua titolarità (es. `Usufruttuario`, `Affittuario con diritto di esecuzione lavori`, `Condominio`).

{: .note }
> Per tutte le altre voci del menu (proprietario, promissario acquirente, ecc.) non viene generato nessun errore sulla titolarità — il menu è presente ma non validato dal codice VB per i valori diversi da `altron`. Se selezioni "Altro" devi obbligatoriamente specificare nel campo testo.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato "Toponimo mancante" ma non hai compilato il campo testo.

**Soluzione**: Inserisci il toponimo nel campo testo accanto alla checkbox.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure spunta "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

---

### Coordinate UTM WGS84 32N

Le coordinate sono obbligatorie e sottoposte a **validazione dell'intervallo numerico**. Sia un valore vuoto, sia un valore non numerico, sia un valore fuori range producono lo stesso messaggio di errore.

---

#### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Causa**: Il campo "Coord. asse X" è vuoto.

**Soluzione**: Inserisci la coordinata X nel campo. Il valore deve essere un numero compreso tra **430.000 e 700.000**.

---

#### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: Il valore inserito nel campo X non è valido per uno dei seguenti motivi: è fuori dall'intervallo ammesso (< 430.000 o > 700.000), oppure non è un numero (es. contiene lettere o simboli non numerici).

**Soluzione**: Inserisci un valore numerico compreso tra **430.000** e **700.000**. Le coordinate UTM WGS84 32N per la Lombardia hanno tipicamente X nell'ordine di 480.000–580.000 (es. `514523`, `498765`). Usa il pulsante "Calcola Coordinate" dalla cartografia se disponibile, oppure ricava le coordinate dallo strumento di localizzazione (GIS comunale, Geoportale Regione Lombardia).

{: .note }
> Le coordinate X e Y richieste sono in formato **UTM WGS84 fuso 32N** (coordinate piane in metri). Non si tratta di gradi decimali come in altre pratiche. La X (Est) per la Lombardia è tipicamente nell'ordine di 480.000–580.000 m. La Y (Nord) è nell'ordine di 5.000.000–5.150.000 m. Il sistema si riferisce al numero civico dell'indirizzo dell'intervento o, in assenza, a un punto centrale interno all'immobile.

---

#### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo "Coord. asse Y" è vuoto.

**Soluzione**: Inserisci la coordinata Y nel campo. Il valore deve essere un numero compreso tra **4.800.000 e 5.700.000**.

---

#### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Il valore Y non è valido: è fuori dall'intervallo (< 4.800.000 o > 5.700.000), oppure non è un numero.

**Soluzione**: Inserisci un valore numerico compreso tra **4.800.000** e **5.700.000** (es. `5034512`, `5087234`).

---

## 3. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga "che i lavori per i quali viene inoltrata la richiesta consistono in:"

**Causa**: Il campo `txtDescrIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

{: .note }
> Nella stessa sezione sono presenti i campi del redattore (nome, sede, via, civico, tel/fax, email, n. iscrizione ordine, tipo ordine, provincia ordine): questi campi **non sono validati** dal codice e non generano errori se lasciati vuoti. Compilarli è comunque buona prassi per la completezza della documentazione.

---

## 4. Dichiarazioni — Vincolo paesaggistico

La sezione dichiarazioni contiene **4 checkbox indipendenti**. A differenza di altre pratiche paesaggistiche, il validatore dell'AP Lombardia **non verifica che almeno una sia spuntata**: è tecnicamente possibile inviare il modulo senza spuntare nessuna checkbox (anche se non avrebbe senso ai fini della pratica). Ogni checkbox, se spuntata, richiede però il campo lettera o testo corrispondente.

---

### ATTENZIONE ! Inserire lettera relativa art. 36.

**Dove si trova**: Prima checkbox della sezione dichiarazioni → "all'art. 136, lettera ___) del suddetto decreto legislativo"

**Causa**: Hai spuntato la prima checkbox (art. 136) ma non hai inserito la lettera del comma applicabile.

**Soluzione**: Inserisci la lettera nel campo piccolo (70px) accanto al testo "all'art. 136, lettera" (es. `a`, `b`, `c`, `d`).

{: .note }
> L'art. 136 del D.Lgs. 42/2004 riguarda i beni dichiarati di notevole interesse pubblico con provvedimento espresso. Il messaggio riporta "art. 36" ma si riferisce all'art. 136 del Codice — si tratta di un'abbreviazione nel codice sorgente.

---

### ATTENZIONE ! Inserire lettera relativa art. 142 comma 1.

**Dove si trova**: Seconda checkbox → "all'art. 142, comma 1, lettera ___) del suddetto decreto legislativo"

**Causa**: Hai spuntato la seconda checkbox (art. 142 c.1) ma non hai inserito la lettera del tipo di vincolo per legge applicabile.

**Soluzione**: Inserisci la lettera nel campo piccolo accanto al testo "all'art. 142, comma 1, lettera" (es. `a`=territori costieri, `b`=laghi, `c`=fiumi e torrenti, `f`=parchi, `g`=boschi, `m`=ghiacciai, ecc.).

---

### ATTENZIONE ! Inserire lettera relativa art. 80 comma 3.

**Dove si trova**: Terza checkbox → "e che le opere previste sono attribuite alla competenza di codesta Amministrazione ai sensi dell'art. 80, comma 3, lettera ___) della legge regionale 11 marzo 2005, n. 12"

**Causa**: Hai spuntato la terza checkbox (art. 80 c.3 L.R. 12/2005) ma non hai inserito la lettera.

**Soluzione**: Inserisci la lettera nel campo piccolo accanto al testo "lettera" (es. `a`, `b`, `c`). L'art. 80 c.3 della L.R. 12/2005 riguarda la competenza dell'amministrazione comunale per determinate tipologie di intervento in ambiti vincolati.

---

### ATTENZIONE ! Inserire vincoli per intervento proposto.

**Dove si trova**: Quarta checkbox → "Segnala che l'ambito interessato dall'intervento proposto è inoltre assoggettato ai seguenti vincoli ___"

**Causa**: Hai spuntato la quarta checkbox (altri vincoli) ma non hai inserito la descrizione dei vincoli aggiuntivi.

**Soluzione**: Inserisci nel campo testo (`txtVincolo4`) la descrizione degli ulteriori vincoli che gravano sull'ambito interessato dall'intervento (es. `Parco regionale delle Groane`, `Zona SIC IT2020007`).

---

## 5. In caso di intervento di variante

La sezione è opzionale e si attiva solo spuntando la checkbox `chkInterventoVariante`. Se non spuntata, nessun campo viene validato. Se spuntata, tutti e tre i campi diventano obbligatori.

---

### ATTENZIONE ! Inserire l'Ente che ha rilasciato l'autorizzazione.

**Dove si trova**: Sezione variante → campo testo (300px) dopo "è stata rilasciata dall'Ente"

**Causa**: Hai spuntato la checkbox variante ma non hai indicato l'ente che ha rilasciato la precedente autorizzazione paesaggistica.

**Soluzione**: Inserisci il nome dell'ente nel campo testo (es. `Comune di Milano`, `Regione Lombardia`, `Soprintendenza ABAP per la città metropolitana di Milano`).

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione rilasciata.

**Causa**: Hai compilato l'ente ma non il numero dell'autorizzazione paesaggistica precedente.

**Soluzione**: Inserisci il numero dell'autorizzazione nel campo accanto a "l'autorizzazione paesaggistica n." (es. `123/2020`, `AP/45/2019`).

---

### ATTENZIONE ! Inserire la data di rilascio dell'autorizzazione.

**Causa**: Hai compilato ente e numero ma non la data di rilascio.

**Soluzione**: Inserisci la data nel campo "in data" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (variante)

**Causa**: La data inserita per l'autorizzazione precedente non rispetta il formato richiesto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/06/2020`).

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Non è presente nessun tecnico nei soggetti coinvolti della pratica.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico. Per l'AP Lombardia non è richiesto un ruolo specifico: è sufficiente qualsiasi tecnico abilitato.

{: .note }
> A differenza di altre pratiche (CILA Nazionale richiede PR, Inizio Lavori richiede DR), l'AP Lombardia richiede solo che esista **almeno un tecnico** nei soggetti coinvolti, indipendentemente dal ruolo. Tipicamente il tecnico inserito è il professionista redattore della relazione paesaggistica.

---

## Consigli pratici AP Lombardia

### Prima di validare ✅

- [ ] Se titolarità = "Altro": inserisci la **specificazione** nel campo testo
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **coordinata X** (UTM WGS84 32N, tra 430.000 e 700.000)
- [ ] Inserisci la **coordinata Y** (UTM WGS84 32N, tra 4.800.000 e 5.700.000)
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Per ogni checkbox vincolo spuntata: inserisci la **lettera** corrispondente (V1, V2, V3) o il **testo** (V4)
- [ ] Se variante: spunta la checkbox e compila **ente**, **n. autorizzazione** e **data** (GG/MM/AAAA)
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti

### Differenze principali AP Lombardia vs AP Piemonte ⚠️

Sono tre le differenze principali. Le coordinate sono UTM WGS84 32N (X e Y in metri) invece di latitudine/longitudine ETRF89 come in Piemonte: i valori sono nell'ordine delle centinaia di migliaia, non gradi decimali. Il validatore delle coordinate ha anche un controllo di intervallo che genera errore se i valori sono fuori range o non numerici. I vincoli (checkbox 1-3) richiedono solo la lettera, senza gli estremi del provvedimento richiesti invece dalla versione Piemonte per il vincolo V1 (art. 136). Il campo "altri vincoli" (V4 Lombardia) non ha equivalente diretto nell'AP Piemonte. La terza checkbox è specifica della Lombardia: art. 80 c.3 L.R. 12/2005.

### Errori frequenti AP Lombardia 🔍

1. **Coordinate fuori intervallo** → le coordinate UTM 32N hanno valori molto diversi dalle coordinate geografiche; inserire gradi decimali (es. `45.4` o `9.1`) genera il messaggio di errore "deve essere compresa tra 430000 e 700000" perché 45 e 9 sono fuori dall'intervallo delle centinaia di migliaia
2. **Coordinata non numerica** → il campo accetta solo numeri (decimali con punto o virgola); inserire testo, spazi o simboli genera lo stesso messaggio dell'intervallo
3. **Vincolo V4 spuntato senza testo** → la quarta checkbox è un campo testo libero, non una lettera; se si spunta la checkbox bisogna sempre descrivere i vincoli nel campo accanto
4. **Nessun tecnico nei soggetti coinvolti** → l'errore appare per ultimo nel processo di validazione; verificare prima di avviare la validazione che la sezione soggetti abbia almeno un tecnico

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
**Fonte**: Analisi codice ValidaDatiAPLombardia e DatiAPLombardia.ascx
