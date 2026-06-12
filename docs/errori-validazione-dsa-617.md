---
title: Errori Denuncia Lavori in Zona Sismica - Regione Veneto
parent: Errori di validazione
nav_order: 67
description: Errori di validazione per la Denuncia dei Lavori in Zona Sismica (interventi di minore rilevanza e privi di rilevanza) - Regione Veneto (art. 93-94bis D.P.R. 380/2001, DGR 1823/2020)
keywords: [denuncia sismica, zona sismica, Veneto, minore rilevanza, privo di rilevanza, DGR 1823/2020, art. 94bis DPR 380, progettista architettonico, progettista strutturale, direttore lavori strutturale, impresa costruttrice, asseverazione, NTC 2018]
IDRegione: 6
IDTipoPratica: 617
Fonte: Manuale
---

# Errori di validazione - Denuncia dei Lavori in Zona Sismica
## Regione Veneto — Interventi di minore rilevanza e privi di rilevanza

Guida completa agli errori specifici per la **Denuncia dei Lavori in Zona Sismica con Asseverazione (DSA)** per interventi di minore rilevanza e privi di rilevanza ai sensi degli artt. 93 e 94-bis del D.P.R. 380/2001 e della DGR Veneto 1823 del 29/12/2020 — Regione Veneto.

{: .note }
> La DSA Veneto è la pratica con il numero più elevato di campi obbligatori dell'intero sistema GeoTecSUE. La struttura è completamente originale: nessun radio titolarità, nessun contributo, nessuna sicurezza lavoro. Il modulo richiede tre figure professionali con anagrafica completa a 11 campi ciascuna (Progettista architettonico, Progettista strutturale, Direttore lavori strutturale), più l'anagrafica completa dell'Impresa costruttrice delle strutture in opera. Il "Dettaglio dell'intervento" richiede la selezione di almeno una tra 35 checkbox distribuite in 4 categorie NTC. L'Impresa costruttrice delle strutture prefabbricate (ICP), il Progettista delle strutture prefabbricate (PF), il Geologo (GE) e il Collaudatore in corso d'opera (CL) sono facoltativi — nessun campo di queste sezioni viene validato. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Impresa costruttrice delle strutture in opera (IC)](#1-impresa-costruttrice-delle-strutture-in-opera-ic)
2. [Descrizione sintetica dell'intervento](#2-descrizione-sintetica-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Tipologia dell'intervento](#4-tipologia-dellintervento)
5. [Tipologia della denuncia](#5-tipologia-della-denuncia)
6. [Dettaglio dell'intervento](#6-dettaglio-dellintervento)
7. [Progettista architettonico (PR)](#7-progettista-architettonico-pr)
8. [Progettista strutturale (PS)](#8-progettista-strutturale-ps)
9. [Direttore dei lavori strutturale (DR)](#9-direttore-dei-lavori-strutturale-dr)

---

## 1. Impresa costruttrice delle strutture in opera (IC)

Tutti i campi dell'impresa costruttrice delle strutture in opera sono obbligatori. Il validatore li verifica in sequenza, fermandosi al primo campo mancante.

---

### ATTENZIONE ! Cognome del Legale Rappresentante dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Causa**: `txtCognomeImprIC` è vuoto.

**Soluzione**: Inserisci il cognome del legale rappresentante dell'impresa costruttrice delle strutture in opera.

---

### ATTENZIONE ! Nome del Legale Rappresentante dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Causa**: `txtNomeImprIC` è vuoto.

**Soluzione**: Inserisci il nome del legale rappresentante.

---

### ATTENZIONE ! Ragione Sociale dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Causa**: `txtRagioneSocialeIC` è vuoto.

**Soluzione**: Inserisci la ragione sociale dell'impresa.

---

### ATTENZIONE ! P.IVA dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Causa**: `txtPIVAIC` è vuoto.

**Soluzione**: Inserisci la Partita IVA o il Codice Fiscale dell'impresa nel campo "C.F./P.IVA".

---

### ATTENZIONE ! Sede dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Causa**: `txtSedeImprIC` è vuoto.

**Soluzione**: Inserisci il Comune della sede legale dell'impresa nel campo "con sede legale a".

---

### ATTENZIONE ! Provincia della sede dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Causa**: `txtProvImprIC` è vuoto.

**Soluzione**: Inserisci la sigla della provincia della sede legale.

---

### ATTENZIONE ! CAP della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Causa**: `txtCAPImprIC` è vuoto.

**Soluzione**: Inserisci il CAP della sede legale.

---

### ATTENZIONE ! Inidirizzo della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Causa**: `txtIndirizzoImprIC` è vuoto. Il messaggio contiene un refuso: "Inidirizzo" con doppia 'i' — è il testo esatto del codice.

**Soluzione**: Inserisci l'indirizzo (via) della sede legale dell'impresa.

---

### ATTENZIONE ! Numero civico dell'indirizzo della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Causa**: `txtNCivicoImprIC` è vuoto.

**Soluzione**: Inserisci il numero civico della sede legale.

{: .note }
> L'**Impresa costruttrice delle strutture prefabbricate** (ICP, seconda sezione imprese) è completamente **non validata** — nessun campo è obbligatorio. Può essere compilata facoltativamente se l'intervento prevede strutture prefabbricate, ma non genera errori se lasciata vuota.

---

## 2. Descrizione sintetica dell'intervento

### ATTENZIONE ! Descrizione sintetica dell'intervento obbligatoria.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga `txtDescrIntervento` "che i lavori per i quali viene inoltrata la presente consistono in:" (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione sintetica dell'intervento strutturale (max **300 caratteri**).

---

## 3. Localizzazione dell'intervento

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

## 4. Tipologia dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia dell'intervento'.

**Dove si trova**: Sezione "Tipologia dell'intervento" → 4 checkbox "Ai sensi delle vigenti Norme Tecniche sulle Costruzioni (N.T.C.) di cui al D.M. 17/01/2018"

**Causa**: Nessuna delle 4 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 4 tipologie di intervento:
- ☐ **chkNuovaCostruzione** — "Nuova costruzione"
- ☐ **chkMiglioramento** — "Miglioramento sismico"
- ☐ **chkAdeguamento** — "Adeguamento sismico"
- ☐ **chkIntervento** — "Intervento locale"

{: .note }
> È possibile spuntare più tipologie contemporaneamente se l'intervento ricade in più categorie NTC.

---

## 5. Tipologia della denuncia

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia della denuncia'.

**Dove si trova**: Sezione "Tipologia della denuncia" → 2 radio button `$TipoDenuncia`

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **d_1** — "Nuovo deposito"
- ⚪ **d_2** — "Variante sostanziale all'autorizzazione sismica n. ___ prot. n. ___ del ___" → inserisci numero autorizzazione, numero protocollo e data protocollo

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione sismica.

**Causa**: Hai selezionato d_2 ma `txtNumAut` è vuoto.

**Soluzione**: Inserisci il numero dell'autorizzazione sismica a cui si riferisce la variante sostanziale.

---

### ATTENZIONE ! Inserire il numero del protocollo dell'autorizzazione sismica.

**Causa**: Hai selezionato d_2 e inserito il numero autorizzazione, ma `txtNumProt` è vuoto.

**Soluzione**: Inserisci il numero di protocollo dell'autorizzazione sismica.

---

### ATTENZIONE ! Inserire la data del protocollo dell'autorizzazione sismica.

**Causa**: `txtDataProt` è vuoto.

**Soluzione**: Inserisci la data del protocollo nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data protocollo)

**Causa**: La data del protocollo non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/04/2024`). È l'unica data della pratica con verifica del formato.

---

## 6. Dettaglio dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Dettaglio dell'intervento'.

**Dove si trova**: Sezione "Dettaglio dell'intervento" — 35 checkbox totali distribuite in 4 categorie ai sensi dell'art. 94-bis D.P.R. 380/2001 e della DGR Veneto 1823/2020

**Causa**: Nessuna delle 35 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** checkbox tra le 35 disponibili:

**Interventi di MINORE RILEVANZA** (8 checkbox — `chkMinoreRilevanza1..8`): interventi di adeguamento o miglioramento sismico in Zona 2 (0,15g-0,20g) e Zona 3; nuove costruzioni in Zona 3; interventi su edifici di interesse strategico in Zona 3; nuove costruzioni non di tipologia complessa in Zona 1 e 2; nuove costruzioni non ricomprese in allegati A o C della DGR 1823/2020; riparazioni e interventi locali su costruzioni esistenti (Zona 1, 2 e 3); nuove costruzioni con presenza sola occasionale di persone e edifici agricoli (Zona 1, 2 e 3); opere di sostegno tra 2,5 m e 4 m di altezza (Zona 1, 2 e 3).

**Interventi PRIVI DI RILEVANZA — Nuove costruzioni** (13 checkbox — `chkPrivoRilevanzaNC1..13`): tettoie ≤30 mq e ≤3 m; manufatti leggeri ≤20 mq e ≤3 m; pergolati senza copertura ≤3 m; attraversamenti/tombinamenti <6 mq; opere di sostegno ≤2,5 m; rivestimenti corticali di scarpate; piscine interrate ≤2,50 m; strutture fotovoltaici ≤3 m; pannelli fonoassorbenti ≤3 m; coperture ingresso ≤8 mq; muri di recinzione <3 m; cartelloni e insegne ≤10 m e ≤20 mq; serre agricole con copertura leggera.

**Interventi PRIVI DI RILEVANZA — Edifici esistenti** (10 checkbox — `chkPrivoRilevanzaEE1..10`): pensiline esterne ≤1,50 m e ≤6 mq; manufatti connessi <10 mq; chiusure e riduzioni aperture esistenti; nuove aperture ≤5 mq complessivi; aperture su pareti <1 mq; sostituzione architravi senza variazione larghezza; soppalchi lignei ≤10 mq; montacarichi/ascensori <7 m; scale interne ad un piano <1,20 m; spostamento porta/finestra in parete portante con riallineamento.

**Interventi PRIVI DI RILEVANZA — Opere non accessibili** (4 checkbox — `chkPrivoRilevanzaONA1..4`): serbatoi/cisterne interrate ≤30 mc; vasche fuori terra ≤30 mc; locali tecnologici <30 mc; tombe di famiglia interrate <35 mc.

{: .note }
> È possibile spuntare più checkbox contemporaneamente se l'intervento ricade in più categorie. La scelta corretta dipende dalla classificazione sismica del Comune (zona 1, 2, 3 o 4) e dalla tipologia specifica dell'opera, definita dall'art. 94-bis del D.P.R. 380/2001 e dalla DGR Veneto 1823/2020. Per la classificazione sismica dei Comuni veneti, consultare il sito della Regione Veneto.

---

## 7. Progettista architettonico (PR)

Tutti gli 11 campi del Progettista architettonico sono obbligatori. Il validatore li verifica in sequenza dal primo all'undicesimo.

---

### ATTENZIONE ! Cognome del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il cognome nel campo `txtCognomeProf1`.

---

### ATTENZIONE ! Nome del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il nome nel campo `txtNomeProf1`.

---

### ATTENZIONE ! Codice Fiscale del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il codice fiscale nel campo `txtCodiceFiscaleProf1`.

---

### ATTENZIONE ! Città di residenza del Progettista architettonico obbligatoria.

**Soluzione**: Inserisci il Comune di residenza nel campo `txtCittaLavoroProf1` "Residente in".

---

### ATTENZIONE ! Provincia di residenza del Progettista architettonico obbligatoria.

**Soluzione**: Inserisci la sigla della provincia nel campo `txtProvLavoroProf1`.

---

### ATTENZIONE ! Indirizzo di residenza del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci la via di residenza nel campo `txtIndirizzoProf1`.

---

### ATTENZIONE ! Numero civico di residenza del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il numero civico nel campo `txtNCivicoProf1`.

---

### ATTENZIONE ! Iscrizione all'Albo del Progettista architettonico obbligatoria.

**Soluzione**: Inserisci la categoria di albo nel campo `txtAlboProf1` "Iscritto all'Albo degli" (es. "Ingegneri", "Architetti").

---

### ATTENZIONE ! Provincia di iscrizione all'Albo del Progettista architettonico obbligatoria.

**Soluzione**: Inserisci la provincia dell'ordine professionale nel campo `txtAlboDiProf1`.

---

### ATTENZIONE ! Numero di iscrizione all'Albo del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il numero di iscrizione all'albo nel campo `txtAlboNumeroProf1`.

---

### ATTENZIONE ! PEC del Progettista architettonico obbligatoria.

**Soluzione**: Inserisci l'indirizzo PEC nel campo `txtPECProf1`.

---

### ATTENZIONE ! Telefono del Progettista architettonico obbligatorio.

**Soluzione**: Inserisci il numero di telefono nel campo `txtTelNProf1`.

---

## 8. Progettista strutturale (PS)

Stessi 11 campi obbligatori del Progettista architettonico. I messaggi sono identici con "Progettista strutturale" al posto di "architettonico". I campi corrispondono a `txtCognomeProf2`, `txtNomeProf2`, `txtCodiceFiscaleProf2`, `txtCittaLavoroProf2`, `txtProvLavoroProf2`, `txtIndirizzoProf2`, `txtNCivicoProf2`, `txtAlboProf2`, `txtAlboDiProf2`, `txtAlboNumeroProf2`, `txtPECProf2`, `txtTelNProf2`.

Seguire le stesse istruzioni della sezione precedente compilando i campi corrispondenti per il progettista strutturale.

{: .note }
> Il **Progettista delle strutture prefabbricate** (PF, scheda 3) è completamente **non validato** — nessun campo è obbligatorio. Compilare facoltativamente se l'intervento prevede strutture prefabbricate.

---

## 9. Direttore dei lavori strutturale (DR)

Stessi 11 campi obbligatori. I messaggi riportano "Direttore dei lavori strutturale". I campi corrispondono a `txtCognomeProf4..txtTelNProf4` (notare che il numero è 4, non 3, perché il Progettista prefabbricati è la scheda 3).

Seguire le stesse istruzioni della sezione 7 compilando i campi corrispondenti per il direttore dei lavori strutturale.

{: .note }
> Il **Geologo** (GE, scheda 5) e il **Collaudatore in corso d'opera** (CL, scheda 6) sono completamente **non validati** — nessun campo è obbligatorio. Compilare facoltativamente se richiesti dall'intervento.

---

## Consigli pratici — DSA Veneto

### Prima di validare ✅

- [ ] Compila tutti i **9 campi dell'Impresa costruttrice in opera** (IC): cognome LR, nome LR, ragione sociale, P.IVA, sede, prov., CAP, indirizzo, n.civico
- [ ] Inserisci la **descrizione** dell'intervento (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Spunta almeno una delle **4 tipologie di intervento** NTC (nuova costruzione / miglioramento / adeguamento / locale)
- [ ] Seleziona la **tipologia di denuncia** (d_1 nuovo deposito / d_2 variante → se d_2: numero aut., n.prot., data prot. GG/MM/AAAA)
- [ ] Spunta almeno una delle **35 checkbox del dettaglio** (minore rilevanza o privo di rilevanza)
- [ ] Compila tutti i **11 campi del Progettista architettonico** (PR): cognome, nome, CF, città, prov, indirizzo, n.civico, albo, prov.albo, n.albo, PEC, tel
- [ ] Compila tutti i **11 campi del Progettista strutturale** (PS): stessi 11 campi
- [ ] Compila tutti i **11 campi del Direttore lavori strutturale** (DR): stessi 11 campi

### Sezioni presenti ma non validate ℹ️

L'Impresa costruttrice strutture prefabbricate (ICP), il Progettista strutture prefabbricate (PF), il Geologo (GE) e il Collaudatore in corso d'opera (CL) hanno tutti i campi facoltativi. Il campo `txtAltro` (sezione "Altro") è facoltativo.

### Ordine di validazione ⚠️

IC (9 campi) → Descrizione → Localizzazione → Tipologia intervento → Tipologia denuncia → Dettaglio intervento → PR (11 campi) → PS (11 campi) → DR (11 campi)

### Errori frequenti 🔍

1. **"Inidirizzo" con doppia 'i'** → refuso nel messaggio del codice sorgente; riguarda l'indirizzo della sede dell'impresa IC
2. **Dettaglio senza checkbox** → la sezione ha 35 opzioni su 4 categorie; bisogna spuntarne almeno una coerente con la zona sismica e il tipo di opera
3. **Campi professionali incompleti** → ciascuna delle 3 figure obbligatorie (PR, PS, DR) richiede 11 campi; il validatore si ferma al primo mancante
4. **d_2 senza dati autorizzazione** → se si sceglie "variante", tutti e 3 i campi (n.aut., n.prot., data prot.) sono obbligatori; la data deve essere in formato GG/MM/AAAA

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
**Fonte**: Analisi codice ValidaDatiDSAVeneto e DatiDSAVeneto.ascx
