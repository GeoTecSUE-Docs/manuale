---
title: Errori Autorizzazione Paesaggistica Semplificata - Regione Liguria
parent: Errori di validazione
nav_order: 38
description: Errori di validazione specifici per l'Autorizzazione Paesaggistica Semplificata (APS) - Regione Liguria (art. 3 D.M. 31/2017, art. 146 D.Lgs. 42/2004)
keywords: [autorizzazione paesaggistica semplificata, APS, Liguria, DM 31/2017, art. 146 D.Lgs. 42/2004, art. 136, art. 142, art. 134, Allegato B, vincolo paesaggistico, variante]
IDRegione: 4
IDTipoPratica: 541
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Semplificata (APS)
## Regione Liguria

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Semplificata** ai sensi dell'art. 3 del D.M. 13 febbraio 2017, n. 31 e dell'art. 146 del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio), relativa alla **Regione Liguria**.

{: .note }
> L'APS Liguria ha una struttura diversa da tutte le altre pratiche della piattaforma. La **titolarità** ha solo il menu a discesa — il radio button è presente nell'ASCX ma **non è validato dal codice** (nessun controllo su `$Titolarita` nel VB). Le sezioni critiche sono i **vincoli paesaggistici** (almeno uno dei tre obbligatorio, con campi aggiuntivi per i primi due) e la sezione **Opere** con articolo e legge regionale sempre obbligatori. La sezione **Variante** è condizionale a una checkbox opzionale. Non ci sono sezioni di sicurezza, contributo, regolarità urbanistica o tecnici da validare. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Descrizione sintetica dell'intervento](#2-descrizione-sintetica-dellintervento)
3. [Dichiarazioni — Normativa di riferimento vincolo paesaggistico](#3-dichiarazioni--normativa-di-riferimento-vincolo-paesaggistico)
4. [Opere](#4-opere)
5. [In caso di intervento di variante](#5-in-caso-di-intervento-di-variante)

---

## 1. Localizzazione dell'intervento

{: .note }
> A differenza di quasi tutte le altre pratiche, nell'APS Liguria il validatore **non controlla** la sezione titolarità (né il radio button né il valore `altron` del menu). Il menu a discesa `cmbTitoloSuImm` è presente nel modulo ma non genera errori di validazione. La prima sezione effettivamente validata è la localizzazione.

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato "Toponimo mancante" ma non hai compilato il campo testo.

**Soluzione**: Inserisci il toponimo nel campo di testo accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: "Toponimo mancante" non è spuntato e nessun indirizzo è selezionato dal menu a discesa.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure spunta "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP (es. `16100`).

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila i dati e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso" (usa Ctrl+click per più voci).

---

## 2. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga "che i lavori per i quali viene inoltrata la richiesta consistono in:"

**Causa**: Il campo `txtDescrizioneIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**). La descrizione deve descrivere l'intervento di lieve entità per cui si richiede l'autorizzazione paesaggistica semplificata.

{: .note }
> Nella stessa sezione è presente il campo **"Voce Allegato B"** (`txtVoceAllegatoB`): si tratta del numero di voce dell'Allegato B al D.M. 31/2017 a cui è riconducibile l'intervento (es. `A.2`, `B.14`). Questo campo **non è validato** dal codice — non genera errori se lasciato vuoto — ma è importante compilarlo correttamente per la correttezza del procedimento. Analogamente, i campi del redattore (nome, sede, ordine) presenti nella stessa sezione non sono soggetti a validazione automatica.

---

## 3. Dichiarazioni — Normativa di riferimento vincolo paesaggistico

Questa è la sezione più critica dell'APS Liguria. L'intervento deve ricadere in almeno uno dei tre tipi di vincolo paesaggistico previsti dal D.Lgs. 42/2004. Ogni checkbox attiva campi aggiuntivi specifici.

---

### ATTENZIONE ! Nessuna voce relativa a normativa di riferimento è stata indicata.

**Causa**: Non hai spuntato nessuna delle 3 checkbox che identificano la base normativa del vincolo paesaggistico.

**Soluzione**: Spunta **almeno una** delle tre opzioni:
- ☐ **V1** — "dell'art. 136, c. 1, lett. ___) del D.Lgs. n. 42/2004" → inserisci lettera + estremi del provvedimento
- ☐ **V2** — "dell'art. 142, c. 1, lett. ___) del D.Lgs. n. 42/2004" → inserisci la lettera
- ☐ **V3** — "dell'art. 134, c. 1, lett. c) del D.Lgs. n. 42/2004" → nessun campo aggiuntivo

{: .note }
> Le tre basi normative si riferiscono alle diverse categorie di beni paesaggistici tutelati dal Codice. L'art. 136 riguarda i beni paesaggistici dichiarati di notevole interesse pubblico con provvedimento espresso (decreto ministeriale o delibera di giunta regionale). L'art. 142 riguarda le aree tutelate per legge (fiumi, laghi, montagne, parchi, foreste, ecc.). L'art. 134 c. 1 lett. c) riguarda gli ulteriori immobili e aree indicati da piani paesaggistici.

---

### Vincolo V1 — Art. 136 D.Lgs. 42/2004

#### ATTENZIONE ! Inserire la lettera relativa all'articolo 136.

**Causa**: Hai spuntato V1 ma non hai inserito la lettera del comma 1 dell'art. 136 (a, b, c o d).

**Soluzione**: Inserisci la lettera nel campo piccolo (70px) accanto al testo "dell'art. 136, c. 1, lett." (es. `a`, `b`, `c`, `d`).

---

#### ATTENZIONE ! Inserire estremi del provvedimento - d.m./d.g.r.

**Causa**: Hai inserito la lettera ma non hai compilato il campo degli estremi del provvedimento istitutivo del vincolo.

**Soluzione**: Inserisci nel campo `txtEstremiProvvedimento` gli estremi del decreto ministeriale o della delibera di giunta regionale che ha istituito il vincolo (es. `D.M. 02/01/1972`, `D.G.R. n. 1234 del 15/06/2005`).

---

### Vincolo V2 — Art. 142 D.Lgs. 42/2004

#### ATTENZIONE ! Inserire la lettera relativa all'articolo 142.

**Causa**: Hai spuntato V2 ma non hai inserito la lettera del comma 1 dell'art. 142.

**Soluzione**: Inserisci la lettera nel campo piccolo (70px) accanto al testo "dell'art. 142, c. 1, lett." (es. `a`=territori costieri, `b`=territori lacuali, `c`=fiumi e torrenti, `f`=parchi e riserve, `g`=boschi e foreste, ecc.).

{: .note }
> Il vincolo V3 (art. 134 c. 1 lett. c) non richiede campi aggiuntivi: è sufficiente spuntare la checkbox e il sistema la accetta senza ulteriori verifiche.

---

## 4. Opere

Questa sezione dichiara la competenza dell'amministrazione destinataria in base alla legge regionale applicabile. Entrambi i campi sono sempre obbligatori.

---

### ATTENZIONE ! Inserire l'articolo della Legge regionale relativa alle Opere.

**Dove si trova**: Sezione "Opere" → campo piccolo (70px) nel testo "che le opere previste sono attribuite alla competenza di codesta Amministrazione ai sensi dell'art. ___"

**Causa**: Il campo `txtOpereArt` è vuoto.

**Soluzione**: Inserisci il numero dell'articolo della legge regionale che attribuisce la competenza (es. `10`, `25`, `3`).

---

### ATTENZIONE ! Inserire la Legge regionale di riferimento.

**Dove si trova**: Sezione "Opere" → campo testo (400px) nel testo "della legge regionale ___"

**Causa**: Il campo `txtLeggeReg` è vuoto.

**Soluzione**: Inserisci il riferimento alla legge regionale applicabile (es. `n. 28 del 4 settembre 1997`, `n. 16 del 6 giugno 2008`).

---

## 5. In caso di intervento di variante

La sezione è opzionale e si attiva solo spuntando la checkbox `chkInterventoVariante`. Se non la spunti, nessun campo viene validato. Se la spunti, i 3 campi seguenti diventano tutti obbligatori.

---

### ATTENZIONE ! Inserire l'Ente che ha rilasciato l'autorizzazione.

**Dove si trova**: Sezione "In caso di intervento di variante" → campo testo (300px) accanto a "Il sottoscritto dichiara altresì che per precedenti interventi su tale immobile è stata rilasciata dall'Ente ___"

**Causa**: Hai spuntato la checkbox variante ma non hai indicato l'ente che ha rilasciato la precedente autorizzazione paesaggistica.

**Soluzione**: Inserisci il nome dell'ente nel campo di testo (es. `Regione Liguria`, `Comune di Genova`, `Soprintendenza ABAP Liguria`).

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione rilasciata.

**Causa**: Hai compilato l'ente ma non hai inserito il numero dell'autorizzazione paesaggistica precedente.

**Soluzione**: Inserisci il numero dell'autorizzazione nel campo accanto a "l'autorizzazione paesaggistica n." (es. `123/2019`, `AP/45/2021`).

---

### ATTENZIONE ! Inserire la data di rilascio dell'autorizzazione.

**Causa**: Hai compilato ente e numero ma non hai inserito la data di rilascio.

**Soluzione**: Inserisci la data nel campo accanto a "in data" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (variante)

**Causa**: La data inserita per l'autorizzazione precedente non rispetta il formato richiesto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/06/2019`).

---

## Consigli pratici APS Liguria

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** dal menu (o spunta "Toponimo mancante" e inseriscilo)
- [ ] Inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Spunta **almeno una checkbox vincolo** (V1, V2 o V3)
- [ ] Se V1: inserisci la **lettera art. 136** e gli **estremi del provvedimento**
- [ ] Se V2: inserisci la **lettera art. 142**
- [ ] Inserisci l'**articolo** della legge regionale (sezione Opere)
- [ ] Inserisci il **riferimento alla legge regionale** (sezione Opere)
- [ ] Se variante: spunta la checkbox e compila **ente**, **n. autorizzazione** e **data** (GG/MM/AAAA)

### Campi presenti ma non validati ℹ️

I seguenti campi sono presenti nel modulo ma **non generano errori** se lasciati vuoti — è comunque buona pratica compilarli per la completezza della documentazione:

- **Menu titolarità** (`cmbTitoloSuImm`) e radio button titolarità → presenti ma non controllati dal validatore
- **Voce Allegato B** (`txtVoceAllegatoB`) → numero voce D.M. 31/2017, non validato
- **Redattore** (nome, sede, via, civico, tel/fax, email) → dati professionista, non validati
- **Iscrizione all'ordine** (n. iscrizione, tipo ruolo, provincia) → non validati

### Differenze principali APS Liguria vs APS Piemonte e APS Lombardia ⚠️

L'APS Liguria si distingue per alcune caratteristiche uniche. I vincoli sono 3 checkbox (non 4 come in Lombardia) e la struttura è diversa: V1 richiede sia lettera che estremi provvedimento, V2 solo lettera, V3 nulla. La sezione Opere con articolo e legge regionale è specifica della Liguria e non presente nelle versioni Piemonte e Lombardia. Non ci sono controlli su titolarità, tecnici o contributo. La variante è una checkbox opzionale (non una sezione separata come in altre pratiche).

### Errori frequenti APS Liguria 🔍

1. **Estremi provvedimento V1 dimenticati** → spuntare V1 (art. 136) richiede **due** campi: lettera E estremi del provvedimento (d.m. o d.g.r.); spesso si inserisce solo la lettera
2. **Sezione Opere ignorata** → i campi articolo e legge regionale sembrano facoltativi per la struttura visiva della sezione, ma sono sempre obbligatori
3. **Variante parzialmente compilata** → se si spunta la checkbox variante, tutti e tre i campi (ente, n. autorizzazione, data) diventano obbligatori; non basta compilarne uno o due

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
**Fonte**: Analisi codice ValidaDatiAPSLiguria e DatiAPSLiguria.ascx
