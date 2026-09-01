---
title: Errori Regolarizzazione Opere in Parziale Difformità - Regione Liguria
parent: Errori di validazione
nav_order: 55
description: Errori di validazione specifici per la Regolarizzazione Opere in Parziale Difformità (ROPD) - Regione Liguria (art. 48 L.R. 16/2008)
keywords: [regolarizzazione opere parziale difformità, ROPD, Liguria, art. 48 L.R. 16/2008, licenza edilizia, abitabilità, agibilità, versamento, titolarità, progettista]
IDRegione: 3
IDTipoPratica: 91
Fonte: Manuale
---

# Errori di validazione - Regolarizzazione Opere in Parziale Difformità
## Regione Liguria

Guida completa agli errori specifici per la **Regolarizzazione Opere in Parziale Difformità (ROPD)** ai sensi dell'art. 48 della L.R. 6 giugno 2008, n. 16 e successive modifiche e integrazioni — Regione Liguria.

{: .note }
> La ROPD Liguria è una pratica di regolarizzazione amministrativa per opere realizzate in parziale difformità dalla Licenza Edilizia, applicabile alle opere eseguite prima o in corso di realizzazione al 1° settembre 1967. La struttura della sezione "Tipo di intervento" è la più complessa: i tre commi dell'art. 48 L.R. 16/2008 hanno logiche condizionali diverse, con date e sotto-selezioni specifiche per ciascuno. La **Titolarità** ha una particolarità: se il valore del menu è "altron" (altro), deve essere compilato il campo di specificazione, **e** se si dichiara titolarità non esclusiva, deve essere presente almeno un titolare aggiuntivo nei soggetti coinvolti. Il **Progettista (PR)** è il ruolo richiesto per i tecnici. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Tipo di intervento — Licenza Edilizia di riferimento](#1-tipo-di-intervento--licenza-edilizia-di-riferimento)
2. [Tipo di intervento — Epoca realizzazione](#2-tipo-di-intervento--epoca-realizzazione)
3. [Tipo di intervento — Sensi dell'articolo (art. 48 L.R. 16/2008)](#3-tipo-di-intervento--sensi-dellarticolo-art-48-lr-162008)
4. [Descrizione dell'intervento](#4-descrizione-dellintervento)
5. [Titolarità dell'intervento](#5-titolarità-dellintervento)
6. [Localizzazione dell'intervento](#6-localizzazione-dellintervento)
7. [Progettista nei soggetti coinvolti](#7-progettista-nei-soggetti-coinvolti)

---

## 1. Tipo di intervento — Licenza Edilizia di riferimento

### ATTENZIONE ! Inserire il numero.

**Dove si trova**: Sezione "Tipo di intervento" → campo `txtNumLIC` "n°" in cima alla sezione, nel testo "intende procedere alla regolarizzazione [...] delle opere realizzate in parziale difformità dalla Licenza Edilizia n° ___ rilasciata in data ___"

**Causa**: Il campo del numero della Licenza Edilizia è vuoto.

**Soluzione**: Inserisci il numero della Licenza Edilizia di riferimento.

---

### ATTENZIONE ! Inserire la data.

**Causa**: Il campo `txtDataLIC` della data della Licenza Edilizia è vuoto.

**Soluzione**: Inserisci la data di rilascio della Licenza Edilizia nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data Licenza Edilizia)

**Causa**: La data della Licenza Edilizia non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/03/1965`).

---

## 2. Tipo di intervento — Epoca realizzazione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo di intervento'.

**Dove si trova**: Sezione "Tipo di intervento" → 2 radio button sotto "e realizzate:"

**Causa**: Nessuno dei 2 radio button del gruppo `$TipoIntervento` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbTipoInterventoa_1** — "prima del 1° settembre 1967"
- ⚪ **rdbTipoInterventoa_2** — "in corso di realizzazione alla data del 1° settembre 1967"

{: .note }
> I due radio button indicano l'epoca di realizzazione delle opere in difformità rispetto alla data rilevante prevista dall'art. 48 L.R. 16/2008. La scelta non attiva campi condizionali nel validatore — entrambe le opzioni hanno lo stesso comportamento ai fini della validazione.

---

## 3. Tipo di intervento — Sensi dell'articolo (art. 48 L.R. 16/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Sensi dell'articolo'.

**Dove si trova**: Sezione "Tipo di intervento" → 3 radio button sotto "si procede ai sensi dei seguenti articoli:"

**Causa**: Nessuno dei 3 radio button del gruppo `$SensiArt` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button** e compila i campi condizionali richiesti:
- ⚪ **rdbSensiArt_1** — "ai sensi del comma 1 art. 48 L.R. 16/2008" → seleziona il tipo pratica (abitabilità o agibilità) e inserisci data e numero
- ⚪ **rdbSensiArt_2** — "ai sensi del comma 2 art. 48 L.R. 16/2008" → inserisci la data di versamento del pagamento di €516,00
- ⚪ **rdbSensiArt_3** — "ai sensi del comma 3 art. 48 L.R. 16/2008" → seleziona la fascia di versamento e inserisci la data (se applicabile)

---

### Opzione rdbSensiArt_1 — Comma 1 (abitabilità/agibilità)

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo di pratica'.

**Causa**: Hai selezionato il comma 1 ma non hai indicato se si tratta di abitabilità o agibilità.

**Soluzione**: Seleziona **uno dei due radio button** del gruppo `$TipoPratica`:
- ⚪ **rdbTipoPratica_1_1** — "abitabilità rilasciata" → inserisci data e numero dell'abitabilità
- ⚪ **rdbTipoPratica_1_2** — "agibilità rilasciata" → inserisci data e numero dell'agibilità

---

#### ATTENZIONE ! Inserire la data di abitabilità.

**Causa**: Hai selezionato "abitabilità rilasciata" ma il campo data `txtDataAbi` è vuoto.

**Soluzione**: Inserisci la data di rilascio dell'abitabilità nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (abitabilità)

**Causa**: La data dell'abitabilità non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero pratica di abitabilità.

**Causa**: Hai compilato la data ma manca il numero dell'abitabilità nel campo `txtNumAbi`.

**Soluzione**: Inserisci il numero del certificato di abitabilità nel campo "n."

---

#### ATTENZIONE ! Inserire la data di agibilità.

**Causa**: Hai selezionato "agibilità rilasciata" ma il campo data `txtDataAgi` è vuoto.

**Soluzione**: Inserisci la data di rilascio dell'agibilità nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (agibilità)

**Causa**: La data dell'agibilità non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero pratica di agibilità.

**Causa**: Hai compilato la data ma manca il numero dell'agibilità nel campo `txtNumAgi`.

**Soluzione**: Inserisci il numero del certificato di agibilità nel campo "n."

---

### Opzione rdbSensiArt_2 — Comma 2 (versamento €516,00)

#### ATTENZIONE ! Inserire la data di realizzazione.

**Dove si trova**: Campo `txtDataRealizzazione` nel testo "il versamento della somma di €516,00 [...] è stato effettuato in data ___"

**Causa**: Hai selezionato il comma 2 ma il campo della data di versamento è vuoto.

**Soluzione**: Inserisci la data in cui è stato effettuato il versamento di €516,00 nel formato **GG/MM/AAAA**.

{: .note }
> Il comma 2 si applica alle variazioni non già accatastate all'epoca della loro realizzazione o non risultanti dal certificato di abitabilità/agibilità. Il versamento di €516,00 deve essere già stato effettuato e la ricevuta allegata alla comunicazione.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (versamento comma 2)

**Causa**: La data di versamento del comma 2 non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### Opzione rdbSensiArt_3 — Comma 3 (versamento variabile per aumento superficie)

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Versamento'.

**Causa**: Hai selezionato il comma 3 ma non hai indicato la fascia di versamento.

**Soluzione**: Seleziona **uno dei tre radio button** del gruppo `$Versamento`:
- ⚪ **rdbVersamento_1** — "di €5.164,00 (per variazioni in aumento della superficie [...] fino alla soglia di 10 mq) è stato effettuato in data ___" → inserisci la data di versamento
- ⚪ **rdbVersamento_2** — "di €10.328,00 (per variazioni in aumento della superficie [...] compresa fra 10,01 mq e la soglia di 20 mq) è stato effettuato in data ___" → inserisci la data di versamento
- ⚪ **rdbVersamento_3** — "verrà determinata dal Comune (essendo la variazione in aumento della superficie [...] superiore alla soglia di 20 mq)" → nessun campo aggiuntivo

{: .note }
> L'importo nel modulo per `rdbVersamento_1` è indicato come "€ 5.1640,00" — si tratta di un refuso nel testo del modulo; l'importo corretto è €5.164,00. La terza opzione (>20 mq, rdbVersamento_3) non richiede alcun campo aggiuntivo perché l'importo verrà determinato dal Comune successivamente.

---

#### ATTENZIONE ! Inserire la data di versamento. (versamento_1 — fino 10 mq)

**Causa**: Hai selezionato `rdbVersamento_1` ma il campo data `txtDataVersamento_1` è vuoto.

**Soluzione**: Inserisci la data in cui è stato effettuato il versamento di €5.164,00 nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (versamento_1)

**Causa**: La data del versamento_1 non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data di versamento. (versamento_2 — 10,01–20 mq)

**Causa**: Hai selezionato `rdbVersamento_2` ma il campo data `txtDataVersamento_2` è vuoto.

**Soluzione**: Inserisci la data in cui è stato effettuato il versamento di €10.328,00 nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (versamento_2)

**Causa**: La data del versamento_2 non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 4. Descrizione dell'intervento

### ATTENZIONE ! Inserire la Descrizione dell'intervento.

**Dove si trova**: Sezione "Tipo di intervento" → campo multiriga `txtDescrizioneIntervento` sotto "che consistono in" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto. Viene validato **dopo** tutta la logica dei sensi articolo.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

---

## 5. Titolarità dell'intervento

### ATTENZIONE ! Inserire la Titolarità dell'intervento.

**Dove si trova**: Sezione "Titolarità dell'intervento" → campo `txtSpecifTitolarita1` "(Specificare se altro)"

**Causa**: Il menu `cmbTitoloSuImm` ha il valore "altron" (opzione "altro") selezionato ma il campo di specificazione `txtSpecifTitolarita1` è vuoto.

**Soluzione**: Inserisci la specificazione del titolo di proprietà sull'immobile nel campo "(Specificare se altro)".

{: .note }
> Il controllo viene eseguito solo se `cmbTitoloSuImm.SelectedValue = "altron"`. Per tutte le altre selezioni del menu (proprietario, usufruttuario, ecc.) il campo non viene validato. Il menu `cmbTitoloSuImm` è presente nel modulo ma il suo valore non viene verificato direttamente come "non vuoto" — solo il caso "altron" scatta la validazione del campo specificazione.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Nessuno dei 2 radio button del gruppo `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbTitolaritab_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **rdbTitolaritab_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori" → devono essere presenti titolari aggiuntivi nei soggetti coinvolti

---

### ATTENZIONE ! Non è stato inserito nessun Titolare aggiuntivo.

**Causa**: Hai selezionato `rdbTitolaritab_2` ("non esclusiva") ma la griglia `GdvSoggTitolari` dei titolari aggiuntivi è vuota — non hai aggiunto nessun co-titolare tra i soggetti coinvolti.

**Soluzione**: Vai alla sezione **"Soggetti coinvolti"** → **"Titolari"** e aggiungi almeno un titolare aggiuntivo (co-proprietario, usufruttuario, titolare di altro diritto reale o obbligatorio di cui si dispone la dichiarazione di assenso).

{: .note }
> La ROPD Liguria è una delle poche pratiche del sistema che verifica la presenza di titolari aggiuntivi nei soggetti coinvolti. Questo controllo è specifico per il caso di titolarità non esclusiva: il sistema verifica che `GdvSoggTitolari.Rows.Count > 0` prima di procedere.

---

## 6. Localizzazione dell'intervento

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

---

## 7. Progettista nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Causa**: Nessun tecnico con ruolo **PR** (Progettista) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **PR – Progettista**.

---

## Consigli pratici — ROPD Liguria

### Prima di validare ✅

- [ ] Inserisci il **numero** e la **data** della Licenza Edilizia (GG/MM/AAAA)
- [ ] Seleziona l'**epoca** di realizzazione (ante/post 1° settembre 1967)
- [ ] Seleziona il **comma art. 48** applicabile e compila i campi condizionali:
  - Comma 1: seleziona abitabilità o agibilità, inserisci **data** (GG/MM/AAAA) e **numero**
  - Comma 2: inserisci la **data di versamento** di €516,00 (GG/MM/AAAA)
  - Comma 3: seleziona la **fascia di versamento**; se rdbVersamento_1 o _2: inserisci la **data di versamento** (GG/MM/AAAA); se rdbVersamento_3: nessun campo
- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Se `cmbTitoloSuImm = "altron"`: inserisci la specificazione nel campo "(Specificare se altro)"
- [ ] Seleziona il **radio titolarità** (esclusiva o non esclusiva); se non esclusiva: aggiungi almeno un **titolare aggiuntivo** nei soggetti
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Aggiungi un tecnico con ruolo **PR** nei soggetti coinvolti

### Campi presenti ma non validati ℹ️

- **`chkViolazioneArt21`** — "ed eseguite su bene culturale in violazione dell'art. 21 del D.Lgs. 42/2004": checkbox informativa facoltativa, non validata
- **Privacy**: testo informativo statico, nessuna checkbox, nessun errore

### Schema logico — sezione "Sensi articolo" ⚠️

Il validatore segue questa catena condizionale:

**rdbSensiArt_1** → radio `$TipoPratica` obbligatorio → se TipoPratica_1_1: data abitabilità (formato) + n. abitabilità; se TipoPratica_1_2: data agibilità (formato) + n. agibilità

**rdbSensiArt_2** → data versamento `txtDataRealizzazione` (formato)

**rdbSensiArt_3** → radio `$Versamento` obbligatorio → se Versamento_1: data `txtDataVersamento_1` (formato); se Versamento_2: data `txtDataVersamento_2` (formato); se Versamento_3: nessun campo

### Errori frequenti 🔍

1. **Sensi articolo senza sotto-selezione** → il comma 1 richiede obbligatoriamente la scelta abitabilità/agibilità; dimenticare il sotto-radio genera "Non è stata selezionata nessuna voce per 'Tipo di pratica'"
2. **Comma 3 senza selezione versamento** → dopo aver scelto rdbSensiArt_3, bisogna specificare la fascia; rdbVersamento_3 (>20 mq) è l'unica che non richiede una data
3. **Titolarità non esclusiva senza titolari aggiuntivi** → la griglia dei titolari deve contenere almeno un soggetto; aggiungere il co-titolare prima di validare
4. **Menu `cmbTitoloSuImm` su "altron" senza specificazione** → se si sceglie "altro" nel menu, il campo "(Specificare se altro)" diventa obbligatorio
5. **Tecnico PR mancante** → a differenza di molte altre pratiche liguri, qui è richiesto specificamente il ruolo PR (Progettista), non un tecnico qualsiasi

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
**Fonte**: Analisi codice ValidaDatiROPD_Liguria e DatiROPDLiguria.ascx
