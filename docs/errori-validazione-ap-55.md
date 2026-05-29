---
title: Errori Autorizzazione Paesaggistica Ordinaria - Regione Liguria
parent: Errori di validazione
nav_order: 49
description: Errori di validazione specifici per l'Autorizzazione Paesaggistica Ordinaria - Regione Liguria (art. 146 D.Lgs. 42/2004, L.R. 32/2008)
keywords: [autorizzazione paesaggistica, AP, Liguria, art. 146 D.Lgs. 42/2004, L.R. 32/2008, art. 136, art. 142, art. 157, vincolo paesaggistico, stato immobile, precedenti autorizzazioni]
IDRegione: 3
IDTipoPratica: 55
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Ordinaria
## Regione Liguria

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Ordinaria** ai sensi dell'art. 146 del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio), della L.R. Liguria 1 dicembre 2008, n. 32 — Regione Liguria.

{: .note }
> L'AP Liguria ha alcune caratteristiche specifiche rispetto alle versioni delle altre regioni. La sezione **"Estremi di precedenti autorizzazioni paesaggistiche rilasciate"** ha 4 opzioni di stato dell'immobile con logiche condizionali diverse; la checkbox "interventi in corso" (`chkStatoe_1_3`) è **indipendente** dal radio group dello stato e viene verificata sempre dopo. La sezione **"Tipo di vincolo"** richiede obbligatoriamente almeno una delle 14 checkbox; solo V1 (art. 136), V13 (art. 157 c.1) e V14 (altro) richiedono un campo testo specificazione. Non sono richieste coordinate geografiche. La sezione **Tecnici** richiede almeno un tecnico di qualsiasi ruolo. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Descrizione sintetica dell'intervento](#3-descrizione-sintetica-dellintervento)
4. [Estremi di precedenti autorizzazioni paesaggistiche](#4-estremi-di-precedenti-autorizzazioni-paesaggistiche)
5. [Tipo di vincolo in cui ricade l'intervento](#5-tipo-di-vincolo-in-cui-ricade-lintervento)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Dove si trova**: Sezione "Titolarità dell'intervento" → 2 radio button sotto "dell'immobile interessato dall'intervento e di"

**Causa**: Non hai indicato se hai titolarità esclusiva sull'immobile.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) e il campo "Specificare se altro" sono presenti ma **non validati** dal codice. La sezione **Qualificazione dell'intervento** (sezione b, art. 146 D.Lgs. 42/2004 e L.R. 32/2008) è mostrata come testo informativo statico — il radio group di qualificazione è **completamente commentato** nel VB e non genera errori.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inseriscilo nel campo testo.

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
> A differenza delle versioni lombarde, l'AP Liguria **non richiede le coordinate geografiche** — il campo coordinate non è presente nel modulo.

---

## 3. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga sotto "che i lavori per i quali viene inoltrata la richiesta consistono in:"

**Causa**: Il campo `txtDescrizioneIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

---

## 4. Estremi di precedenti autorizzazioni paesaggistiche

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Estremi di precedenti autorizzazioni paesaggistiche rilasciate'.

**Dove si trova**: Sezione "Estremi di precedenti autorizzazioni paesaggistiche rilasciate" → 4 radio button sotto "che lo stato attuale dell'immobile risulta:"

**Causa**: Non hai indicato lo stato attuale dell'immobile rispetto alle precedenti autorizzazioni paesaggistiche.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **e_1** — "pienamente conforme alla documentazione dello stato di fatto legittimato dalle seguenti autorizzazioni paesaggistiche:" → seleziona il tipo di AP e compila n. e data
- ⚪ **e_2** — "non sono state reperite precedenti autorizzazioni paesaggistiche essendo l'immobile di remota costruzione e non interessato successivamente da interventi edilizi per i quali era necessario munirsi di autorizzazione paesaggistica" → nessun campo aggiuntivo
- ⚪ **e_3** — "in difformità rispetto all'autorizzazione paesaggistica" → compila n. pratica, data pratica e data realizzazione opere
- ⚪ **e_4** — "in assenza di autorizzazione paesaggistica, tali opere sono state realizzate in data ___" → compila la data di realizzazione

---

### Opzione e_1 — Stato conforme con AP precedenti

#### ATTENZIONE ! Non è stata selezionata nessun tipo di autorizzazione paesaggistica.

**Causa**: Hai selezionato e_1 ("pienamente conforme") ma non hai spuntato nessuna delle 2 checkbox del tipo di autorizzazione.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoe_1_1** — "autorizzazione paesaggistica" → inserisci numero e data
- ☐ **chkStatoe_1_2** — "accertamento di compatibilità paesaggistica" → inserisci numero e data

Le due checkbox non sono mutuamente esclusive: è possibile indicare entrambe.

---

#### ATTENZIONE ! Inserire il numero di pratica. (e_1_1 — AP)

**Causa**: Hai spuntato `chkStatoe_1_1` (autorizzazione paesaggistica) ma non hai compilato il campo numero.

**Soluzione**: Inserisci il numero dell'autorizzazione paesaggistica nel campo "numero" affiancato.

---

#### ATTENZIONE ! Inserire la data della pratica. (e_1_1 — AP)

**Causa**: Hai compilato il numero ma non la data dell'AP.

**Soluzione**: Inserisci la data nel campo "del" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero di pratica. (e_1_2 — ACP)

**Causa**: Hai spuntato `chkStatoe_1_2` (accertamento compatibilità paesaggistica) ma non hai compilato il numero.

**Soluzione**: Inserisci il numero dell'accertamento nel campo "numero".

---

#### ATTENZIONE ! Inserire la data della pratica. (e_1_2 — ACP)

**Causa**: Manca la data dell'accertamento di compatibilità paesaggistica.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### Opzione e_3 — Stato in difformità

#### ATTENZIONE ! Inserire il numero di pratica. (e_3 — in difformità)

**Causa**: Hai selezionato e_3 ("in difformità rispetto all'autorizzazione paesaggistica") ma non hai inserito il numero della pratica AP di riferimento nel campo "Pratica n."

**Soluzione**: Inserisci il numero della pratica di autorizzazione paesaggistica rispetto alla quale sono state realizzate le opere in difformità.

---

#### ATTENZIONE ! Inserire la data della pratica. (e_3 — in difformità)

**Causa**: Manca la data della pratica AP di riferimento nel campo "del".

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data di realizzazione dell'intervento.

**Causa**: Hai selezionato e_3 ma non hai compilato il campo "tali opere sono state realizzate in data" (`txtDataReal3_1`).

**Soluzione**: Inserisci la data in cui sono state realizzate le opere in difformità, nel formato **GG/MM/AAAA**.

{: .note }
> L'opzione e_3 è l'unica che richiede **3 campi distinti**: numero della pratica AP, data della pratica AP, e data di realizzazione delle opere in difformità. Il numero e la data si riferiscono all'autorizzazione paesaggistica originaria rispetto alla quale si è verificata la difformità; la data di realizzazione indica quando le opere non autorizzate o difformi sono state eseguite.

---

### Opzione e_4 — Stato in assenza di AP

#### ATTENZIONE ! Inserire la data della pratica. (e_4 — in assenza)

**Causa**: Hai selezionato e_4 ("in assenza di autorizzazione paesaggistica, tali opere sono state realizzate in data ___") ma il campo data è vuoto.

**Soluzione**: Inserisci nel campo affiancato al radio button la data in cui le opere sono state realizzate in assenza di autorizzazione paesaggistica, nel formato **GG/MM/AAAA**.

---

### Checkbox "interventi in corso" — indipendente dal radio group

La checkbox `chkStatoe_1_3` ("per lo stesso immobile sono in corso interventi/sono state presentate pratiche per interventi di ___") è posizionata sotto il radio group ma viene verificata **indipendentemente** dall'opzione di stato scelta. Il validatore la controlla sempre dopo il radio group, qualunque sia la risposta allo stato dell'immobile.

#### ATTENZIONE ! Inserire il tipo di pratica.

**Dove si trova**: Checkbox `chkStatoe_1_3` → campo testo "interventi di ___"

**Causa**: Hai spuntato la checkbox "per lo stesso immobile sono in corso interventi" ma non hai specificato il tipo di intervento nel primo campo testo.

**Soluzione**: Inserisci nel primo campo il tipo di pratica o intervento in corso (es. `Permesso di Costruire`, `SCIA`, `Ristrutturazione edilizia`).

---

#### ATTENZIONE ! Inserire il numero di pratica. (interventi in corso)

**Causa**: Hai compilato il tipo ma non il numero della pratica in corso.

**Soluzione**: Inserisci il numero nel campo "numero".

---

#### ATTENZIONE ! Inserire la data della pratica. (interventi in corso)

**Causa**: Manca la data della pratica in corso nel campo "del".

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

{: .note }
> Nel codice sorgente è presente un refuso: in caso di data mancante per `chkStatoe_1_3`, il focus viene posto erroneamente su `txtDataPrat1_2` (data dell'accertamento ACP) invece di `txtDataPrat1_3` (data interventi in corso). Questo non influisce sulla validazione né sul messaggio di errore, ma può causare uno spostamento visivo inatteso del cursore in quel campo invece del campo corretto.

---

## 5. Tipo di vincolo in cui ricade l'intervento

### ATTENZIONE ! Selezionare almeno un tipo di vincolo.

**Dove si trova**: Sezione "Tipo di vincolo in cui ricade l'intervento" → 14 checkbox

**Causa**: Nessuna delle 14 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 14 checkbox che descrive il tipo di vincolo paesaggistico che interessa l'immobile:

- ☐ **V1** — art. 136 – immobili ed aree di notevole interesse pubblico → richiede specificazione testo
- ☐ **V2** — art. 142 c. 1 lett. a) – territori costieri (fascia 300 m dalla battigia)
- ☐ **V3** — art. 142 c. 1 lett. b) – territori contermini ai laghi (fascia 300 m)
- ☐ **V4** — art. 142 c. 1 lett. c) – fiumi, torrenti e corsi d'acqua (fascia 150 m)
- ☐ **V5** — art. 142 c. 1 lett. d) – montagne (> 1.600 m alpina / > 1.200 m appenninica)
- ☐ **V6** — art. 142 c. 1 lett. e) – ghiacciai e circhi glaciali
- ☐ **V7** — art. 142 c. 1 lett. f) – parchi e riserve nazionali o regionali
- ☐ **V8** — art. 142 c. 1 lett. g) – territori coperti da foreste e boschi
- ☐ **V9** — art. 142 c. 1 lett. h) – aree università agrarie e zone con usi civici
- ☐ **V10** — art. 142 c. 1 lett. i) – zone umide (elenco d.P.R. 448/1976)
- ☐ **V11** — art. 142 c. 1 lett. l) – vulcani
- ☐ **V12** — art. 142 c. 1 lett. m) – zone di interesse archeologico
- ☐ **V13** — art. 157 c. 1 – notifiche e provvedimenti normativa previgente → richiede specificazione testo
- ☐ **V14** — altro → richiede specificazione testo

{: .note }
> Le checkbox V2–V12 (art. 142 lettere a-m e zone umide) non richiedono nessun campo testo aggiuntivo — è sufficiente spuntarle. Solo V1 (art. 136), V13 (art. 157) e V14 (altro) richiedono una specificazione nel campo accanto.

---

### ATTENZIONE ! Inserire il dettaglio del vincolo.

**Causa**: Hai spuntato `chkVincolo1` (art. 136), `chkVincolo13` (art. 157 c.1) o `chkVincolo14` (altro) ma il campo testo affiancato è vuoto.

Il messaggio è identico per tutti e tre i casi.

**Soluzione**:
- Se hai spuntato **V1** (art. 136): inserisci la specificazione del provvedimento che ha dichiarato il bene/area di notevole interesse pubblico (es. `D.M. 05/09/1966 – Promontorio di Portofino`).
- Se hai spuntato **V13** (art. 157 c.1): inserisci gli estremi della notifica, dell'elenco o del provvedimento emesso ai sensi della normativa paesaggistica previgente.
- Se hai spuntato **V14** (altro): inserisci la descrizione del tipo di vincolo non ricompreso nelle categorie precedenti.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Nessun tecnico è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico. Il modulo indica "progettista/i o rilevatore/i" — non è richiesto un ruolo specifico, è sufficiente qualsiasi tecnico abilitato.

---

## Consigli pratici — AP Liguria

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (esclusiva o non esclusiva)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Seleziona lo **stato dell'immobile** (e_1..e_4) e compila i campi condizionali:
  - e_1: spunta almeno una tra AP/ACP e compila n. + data
  - e_2: nessun campo
  - e_3: n. pratica + data pratica + **data realizzazione** (3 campi)
  - e_4: data realizzazione (1 campo)
- [ ] Se ci sono **interventi in corso** (`chkStatoe_1_3`): tipo pratica + n. + data
- [ ] Spunta almeno una delle **14 checkbox vincolo**; per V1, V13, V14: compila il campo testo specificazione
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti

### Struttura sezione stato immobile — schema rapido ⚠️

Il radio group `$Stato` (e_1..e_4) e la checkbox `chkStatoe_1_3` sono due blocchi indipendenti. Il validatore prima risolve il radio group (con i suoi campi condizionali), poi controlla sempre `chkStatoe_1_3` indipendentemente dall'opzione scelta. Questo significa che `chkStatoe_1_3` può essere spuntata in combinazione con qualsiasi opzione di stato.

### Differenze AP Liguria vs AP Piemonte / Lombardia

Rispetto alle versioni delle altre regioni: non sono richieste coordinate geografiche; lo stato dell'immobile ha 4 opzioni distinte (inclusi e_3 "in difformità" ed e_4 "in assenza") che sono specifiche per la procedura ligure; i vincoli sono 14 checkbox (contro le 4 dell'APS o le varianti di Piemonte e Lombardia) con la copertura completa dell'art. 142 lettere a-m del Codice.

### Errori frequenti 🔍

1. **Opzione e_1 selezionata senza checkbox AP/ACP** → dopo aver scelto "pienamente conforme", bisogna anche spuntare il tipo di AP precedente e compilare n. e data; dimenticare le checkbox genera un errore specifico
2. **Opzione e_3: 3 campi distinti** → "in difformità" è l'unica opzione con 3 campi; spesso si compila n. e data della pratica AP ma si dimentica la data di realizzazione delle opere
3. **chkStatoe_1_3 spuntata per sbaglio** → se la checkbox "interventi in corso" viene spuntata accidentalmente senza compilare i 3 campi, il validatore si blocca su quell'errore dopo aver superato tutto il radio group
4. **Nessun vincolo selezionato** → la sezione vincolo viene raggiunta solo dopo aver superato tutte le sezioni precedenti; verificarla in anticipo evita di dover rivalidare dopo una lunga compilazione
5. **V1/V13/V14 senza specificazione** → spuntare una di queste checkbox senza compilare il campo testo genera "Inserire il dettaglio del vincolo" con lo stesso messaggio per tutti e tre

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
**Fonte**: Analisi codice ValidaDatiAPLiguria e DatiAPLiguria.ascx
