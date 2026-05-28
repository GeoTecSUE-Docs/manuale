---
title: Errori Inizio Lavori - Regione Liguria
parent: Errori di validazione
nav_order: 50
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori - Regione Liguria (art. 15 D.P.R. 380/2001, artt. 26 e 34 L.R. 16/2008, L.R. 10/2012)
keywords: [inizio lavori, comunicazione inizio lavori, Liguria, art. 15 DPR 380, L.R. 16/2008, L.R. 10/2012, opere strutturali, art. 65, art. 93, certificatore energetico, sicurezza lavoro, direttore lavori, notifica preliminare]
IDRegione: 3
IDTipoPratica: 201
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Inizio Lavori
## Regione Liguria

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori** ai sensi dell'art. 15 del D.P.R. 06/06/2001, n. 380, degli artt. 26 e 34 della L.R. 6/06/2008, n. 16 e della L.R. 5/04/2012, n. 10 — Regione Liguria.

{: .note }
> L'Inizio Lavori Liguria ha una struttura molto diversa dalla versione Nazionale (stesso IDTipoPratica 101 ma modulo completamente diverso). Le peculiarità principali sono: la sezione **"In relazione al procedimento edilizio"** viene validata per prima e richiede tipo pratica + n. + data + **numero e data protocollo** (4 campi iniziali, tutti obbligatori con le date nel formato GG/MM/AAAA). Le **Dichiarazioni** (sezione 2a) riguardano le opere strutturali ai sensi degli artt. 65/93 D.P.R. 380/2001 e hanno 6 opzioni distinte; l'opzione 5 apre due checkbox mutuamente additive. La sezione **Obblighi committente** (sezione 4) distingue se il committente coincide o meno con il responsabile dei lavori, con sotto-selezione sulla notifica preliminare. Il **Direttore Lavori (DR)** è obbligatorio nei soggetti coinvolti. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [In relazione al procedimento edilizio](#1-in-relazione-al-procedimento-edilizio)
2. [Sezione 1 — Descrizione sintetica dell'intervento e data inizio lavori](#2-sezione-1--descrizione-sintetica-dellintervento-e-data-inizio-lavori)
3. [Sezione 2 — Localizzazione dell'intervento](#3-sezione-2--localizzazione-dellintervento)
4. [Sezione 2a — Dichiarazioni (opere strutturali)](#4-sezione-2a--dichiarazioni-opere-strutturali)
5. [Sezione 3 — Rispetto degli obblighi in materia di sicurezza](#5-sezione-3--rispetto-degli-obblighi-in-materia-di-sicurezza)
6. [Sezione 4 — Obblighi del committente o del responsabile dei lavori](#6-sezione-4--obblighi-del-committente-o-del-responsabile-dei-lavori)
7. [Direttore Lavori nei soggetti coinvolti](#7-direttore-lavori-nei-soggetti-coinvolti)

---

## 1. In relazione al procedimento edilizio

Questa sezione, posizionata in cima al modulo, raccoglie i riferimenti alla pratica edilizia di base (permesso di costruire, SCIA o altro titolo) e i dati di protocollo. Viene validata **prima** di tutte le altre sezioni.

---

### ATTENZIONE ! Campo obbligatorio 'Tipo Pratica' non selezionato.

**Dove si trova**: Sezione "In relazione al procedimento edilizio" → menu a discesa "tipo pratica" (`cmbTipoPratica`)

**Causa**: Il menu del tipo di pratica è rimasto sull'opzione vuota iniziale (il campo interno `txtTipoPratica` ha valore "0").

**Soluzione**: Seleziona il tipo di pratica edilizia dal menu a discesa (es. Permesso di Costruire, SCIA alternativa al PdC, ecc.).

{: .note }
> Il menu `cmbTipoPratica` è normalmente precompilato dal sistema quando la comunicazione di inizio lavori è collegata a una pratica edilizia principale. Se il menu risulta vuoto o bloccato su "nessuno", verificare che la pratica principale sia stata correttamente protocollata e che la comunicazione di inizio lavori sia stata aperta dal dettaglio della pratica principale.

---

### ATTENZIONE ! Campo obbligatorio 'Numero Pratica' non inserito.

**Causa**: Il campo "n." del numero della pratica edilizia di riferimento è vuoto.

**Soluzione**: Inserisci il numero della pratica edilizia di riferimento nel campo "n."

---

### ATTENZIONE ! Campo obbligatorio 'Data Pratica' non inserito.

**Causa**: Il campo "presentata in data" della pratica edilizia di riferimento è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica)

**Causa**: La data della pratica edilizia non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/03/2023`).

---

### ATTENZIONE ! Campo obbligatorio 'Numero protocollo' non inserito.

**Dove si trova**: Sezione "In relazione al procedimento edilizio" → campo "Protocollo Num." (`txtProtNum`)

**Causa**: Il campo del numero di protocollo della comunicazione è vuoto.

**Soluzione**: Inserisci il numero di protocollo nel campo "Protocollo Num."

{: .note }
> L'Inizio Lavori Liguria richiede sia i dati della pratica edilizia di riferimento (tipo + n. + data) sia i dati del **protocollo** della comunicazione stessa (n. protocollo + data protocollo): sono due coppie di campi distinte, entrambe obbligatorie. Questo è diverso dalla versione Nazionale che non ha un numero di protocollo separato.

---

### ATTENZIONE ! Campo obbligatorio 'Data protocollo' non inserito.

**Causa**: Il campo "Data" del protocollo è vuoto.

**Soluzione**: Inserisci la data del protocollo nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data protocollo)

**Causa**: La data del protocollo non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 2. Sezione 1 — Descrizione sintetica dell'intervento e data inizio lavori

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Dove si trova**: Sezione "1. Descrizione sintetica dell'intervento" → campo "che in data ___" (`txtDataInizioLavori`)

**Causa**: Il campo della data di inizio lavori è vuoto.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data di inizio lavori non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "1." → campo multiriga `txtDescrLavori` sotto "darà l'inizio ai lavori di"

**Causa**: Il campo di descrizione dell'intervento è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

---

## 3. Sezione 2 — Localizzazione dell'intervento

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

## 4. Sezione 2a — Dichiarazioni (opere strutturali)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Dichiarazione'.

**Dove si trova**: Sezione "DICHIARA" → 6 radio button relativi alle opere strutturali (artt. 65/93 D.P.R. 380/2001) e al certificatore energetico

**Causa**: Nessuno dei 6 radio button della sezione dichiarazioni è selezionato.

**Soluzione**: Seleziona **uno dei sei radio button**:
- ⚪ **rdb1** — "che è stato individuato da parte dell'impresa esecutrice il certificatore energetico ai sensi della D.G.R. 4/08/09 n. 4511965 identificato nell'allegato 'Soggetti coinvolti unificato'"
- ⚪ **rdb2** — "che l'intervento non comporta la nomina a certificatore energetico ai sensi di legge"
- ⚪ **rdb3** — "che è stata consegnata la denuncia inerente le opere strutturali ai sensi degli artt. 65 e 93 del D.P.R. 06/06/2001 n. 380" → inserisci n. protocollo e data
- ⚪ **rdb4** — "di impegnarsi alla consegna della denuncia inerente le opere strutturali ai sensi degli artt. 65 e 93 del D.P.R. 06/06/2001 n. 380, prima di iniziare i corrispondenti interventi"
- ⚪ **rdb5** — "di consegnare contestualmente al presente inizio lavori la denuncia inerente le opere strutturali ai sensi degli artt. 65 e 93 del D.P.R. 06/06/2001 n. 380" → seleziona almeno una checkbox art. 65 / art. 93
- ⚪ **rdb6** — "che l'intervento edilizio non comporta l'esecuzione di opere strutturali ai sensi del D.P.R. 06/06/2001 n. 380"

{: .note }
> Le 6 opzioni riguardano due temi distinti gestiti con un unico radio group: le prime 2 riguardano il **certificatore energetico** (obbligatorio per alcune tipologie di intervento ai sensi della normativa sull'efficienza energetica), le restanti 4 riguardano la **denuncia di opere strutturali** (artt. 65/93 D.P.R. 380/2001). Nella pratica si seleziona l'opzione pertinente alla situazione specifica dell'intervento.

---

### Opzione rdb3 — Denuncia già consegnata

#### ATTENZIONE ! Campo obbligatorio 'Numero protocollo' non inserito. (denuncia strutturali)

**Causa**: Hai selezionato rdb3 ("denuncia già consegnata") ma non hai inserito il numero di protocollo della denuncia.

**Soluzione**: Inserisci il numero di protocollo della denuncia delle opere strutturali nel campo "Protocollo num." affiancato.

---

#### ATTENZIONE ! Campo obbligatorio 'Data protocollo' non inserito. (denuncia strutturali)

**Causa**: Hai inserito il numero ma non la data del protocollo della denuncia.

**Soluzione**: Inserisci la data nel campo "in data" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (protocollo denuncia strutturali)

**Causa**: La data del protocollo della denuncia non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### Opzione rdb5 — Consegna contestuale denuncia strutturali

#### ATTENZIONE ! Selezionare almeno un intervento.

**Causa**: Hai selezionato rdb5 ("consegna contestuale della denuncia opere strutturali") ma non hai spuntato nessuna delle 2 checkbox che specifica il tipo di denuncia.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkDichiarazione5_1** — "ex art. 65 del D.P.R. 06/06/2001 n. 380" (denuncia opere in cemento armato, normale e precompresso e a struttura metallica)
- ☐ **chkDichiarazione5_2** — "ex art. 93 del D.P.R. 06/06/2001 n. 380" (denuncia opere in zone sismiche)

Le due checkbox non sono mutuamente esclusive: è possibile spuntarle entrambe se l'intervento ricade in entrambe le fattispecie.

---

## 5. Sezione 3 — Rispetto degli obblighi in materia di sicurezza

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Rispetto obblighi in materia di sicurezza'.

**Dove si trova**: Sezione "3. Rispetto degli obblighi in materia di salute e sicurezza nei luoghi di lavoro" → 2 radio button

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbObblSaluteSicurezza3_1** — "che l'intervento non ricade nell'ambito di applicazione del D.Lgs. 09/04/2008 n. 81"
- ⚪ **rdbObblSaluteSicurezza3_2** — "che l'intervento ricade nell'ambito di applicazione del D.Lgs. 09/04/2008 n. 81"

{: .note }
> A differenza della versione Nazionale che ha una struttura a 3 livelli con documentazione imprese e notifica preliminare, la sezione sicurezza della versione Liguria ha **solo 2 radio button** senza sotto-selezioni — il validatore verifica solo che uno dei due sia selezionato. I dettagli della documentazione sicurezza vengono gestiti nella sezione successiva (Obblighi committente, sezione 4).

---

## 6. Sezione 4 — Obblighi del committente o del responsabile dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Obblighi del committente o del responsabile dei lavori'.

**Dove si trova**: Sezione "4. Obblighi del committente o del responsabile dei lavori" → 2 radio button principali

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbObblighi1** — "che il committente/titolare è anche responsabile dei lavori e quindi dichiara inoltre" → seleziona la modalità di notifica preliminare
- ⚪ **rdbObblighi2** — "che il committente/titolare non è anche responsabile dei lavori e quindi dichiara di allegare 'Dichiarazione ai sensi dell'art. 90 comma 9 lett. c del D.Lgs. 09/04/2008 n. 81'" → nessun campo aggiuntivo

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Allegati notifica preliminare'.

**Causa**: Hai selezionato `rdbObblighi1` (committente = responsabile dei lavori) ma non hai indicato la situazione relativa alla notifica preliminare.

**Soluzione**: Seleziona **uno dei tre radio button** del sotto-gruppo `$ObblighiAll`:
- ⚪ **rdbObblighiAll1** — "di allegare alla presente la notifica preliminare di cui all'art. 99 del D.Lgs. 09/04/2008 n. 81, impegnandosi a produrre gli eventuali aggiornamenti"
- ⚪ **rdbObblighiAll2** — "di impegnarsi a produrre la notifica preliminare di cui all'art. 99 del D.Lgs. 09/04/2008 n. 81 prima dell'effettivo inizio dei lavori"
- ⚪ **rdbObblighiAll3** — "che l'opera non rientra tra quelle soggette all'obbligo di presentazione della notifica preliminare di cui all'art. 99 del D.Lgs. 09/04/2008 n. 81"

{: .note }
> I campi relativi alla verifica documentazione imprese (checkbox `chkAvvenutaVerifica`, `chkIdoneita`, `chkContrattiLav`, `chkDatiImpreseEsecut`) sono presenti nel modulo sotto `rdbObblighi1` ma **non sono validati** dal codice VB — non generano errori se non spuntati. La loro compilazione è tuttavia raccomandata per la completezza della dichiarazione ai sensi del D.Lgs. 81/2008.

---

## 7. Direttore Lavori nei soggetti coinvolti

### ATTENZIONE ! Non è stata selezionato nessun Tecnico come Direttore Lavori.

**Causa**: Nessun tecnico con ruolo **DR** (Direttore Lavori) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **DR – Direttore Lavori**.

---

## Consigli pratici — Inizio Lavori Liguria

### Prima di validare ✅

- [ ] Seleziona il **tipo pratica** dal menu, inserisci **n. pratica** e **data** (GG/MM/AAAA)
- [ ] Inserisci il **n. protocollo** e la **data protocollo** (GG/MM/AAAA)
- [ ] Inserisci la **data di inizio lavori** (GG/MM/AAAA)
- [ ] Inserisci la **descrizione dell'intervento** (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona uno dei 6 **radio button dichiarazioni** (opere strutturali / certificatore); se rdb3: n. prot. + data (GG/MM/AAAA); se rdb5: almeno una tra art. 65 / art. 93
- [ ] Seleziona uno dei 2 **radio button sicurezza** (ricade / non ricade nel D.Lgs. 81/2008)
- [ ] Seleziona uno dei 2 **radio button obblighi committente**; se rdbObblighi1: seleziona una delle 3 opzioni notifica preliminare
- [ ] Aggiungi un tecnico con ruolo **DR** nei soggetti coinvolti

### Campi presenti ma non validati ℹ️

- **`txtIntestazione`** (intestazione nella sezione procedimento edilizio): opzionale, non validato
- **Checkbox verifica documentazione imprese** (`chkAvvenutaVerifica`, `chkIdoneita`, `chkContrattiLav`, `chkDatiImpreseEsecut`): presenti sotto rdbObblighi1, non validate
- **Privacy**: testo informativo statico senza checkbox — non genera errori
- **Coordinate**: non richieste in questa pratica

### Differenze Inizio Lavori Liguria vs Inizio Lavori Nazionale ⚠️

Pur avendo lo stesso `IDTipoPratica = 101`, le due pratiche sono completamente diverse. La versione Liguria richiede in più: numero e data del protocollo della comunicazione; 6 opzioni dichiarazioni strutturali/certificatore energetico invece delle 2 sezioni art. 65 e artt. 93/94 indipendenti del Nazionale; sezione sicurezza semplificata (2 radio senza sotto-selezioni); sezione obblighi committente con sotto-selezione notifica (3 opzioni invece delle 4 livelli del Nazionale). La versione Nazionale invece ha la sezione Amianto e l'anagrafica del responsabile dei lavori, assenti in Liguria.

### Errori frequenti 🔍

1. **Due coppie di campi nella sezione protocollo** → la sezione "In relazione al procedimento edilizio" ha tipo+n.+data (pratica edilizia) E n.+data (protocollo comunicazione): 5 campi in tutto, tutti obbligatori; è facile dimenticare la seconda coppia
2. **Opzione rdb5 senza checkbox art. 65/93** → dopo aver selezionato "consegna contestuale denuncia", bisogna specificare quale articolo (65, 93 o entrambi); dimenticare le checkbox genera "Selezionare almeno un intervento"
3. **Nessun radio sicurezza selezionato** → la sezione 3 è visivamente compatta con solo 2 radio, ma obbligatoria; può essere saltata durante la compilazione
4. **rdbObblighi1 senza selezione notifica** → dopo aver scelto "committente = responsabile", bisogna specificare la situazione della notifica preliminare (3 opzioni); dimenticarla genera "Non è stata selezionata nessuna voce per 'Allegati notifica preliminare'"
5. **DR mancante nei soggetti** → verificare in anticipo che la pratica principale abbia un Direttore Lavori nei soggetti coinvolti

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
**Fonte**: Analisi codice ValidaDatiInizioLavoriLiguria e DatiInizioLavoriLiguria.ascx
