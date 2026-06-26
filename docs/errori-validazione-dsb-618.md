---
title: Errori Denuncia Sismica Interventi Rilevanti - Veneto
parent: Errori di validazione
nav_order: 49
description: Errori di validazione specifici per la Denuncia dei lavori in zona sismica per interventi rilevanti (DSB) - Regione Veneto
keywords: [denuncia sismica, DSB, Veneto, zona sismica, interventi rilevanti, NTC 2018, D.M. 17/01/2018, art. 94-bis DPR 380/2001, DGR 1823/2020, impresa costruttrice, progettista architettonico, progettista strutturale, direttore lavori strutturale, tipologia denuncia, variante sismica, rilevanza sismica]
IDRegione: 6         # Veneto
IDTipoPratica: 618
Fonte: Manuale
---

# Errori di validazione - Denuncia Sismica Interventi Rilevanti (DSB)
## Regione Veneto

Guida completa agli errori specifici per la **Denuncia dei lavori in zona sismica per interventi rilevanti** ai sensi dell'art. 93, comma 5, del D.P.R. 380/2001 e della DGR Veneto n. 1823/2020 — Regione Veneto.

{: .note }
> La DSB Veneto è la pratica con il maggior numero di campi obbligatori della piattaforma: **49 errori distinti** sono possibili prima di completare la validazione. La struttura è organizzata in blocchi figure professionali, ciascuno con campi identici (cognome, nome, CF, città, provincia, indirizzo, n. civico, albo, provincia albo, numero albo, PEC, telefono). Sono obbligatorie tre figure: **Impresa costruttrice** (10 campi), **Progettista architettonico** (13 campi) e **Progettista strutturale** (13 campi) e **Direttore lavori strutturale** (13 campi). Le sezioni **Progettista strutture prefabbricate**, **Geologo** e **Collaudatore in corso d'opera** sono presenti nell'ASCX ma **non validate** dal codice VB. Tutte le sezioni professionisti offrono il pulsante **"Carica Soggetto"** per importare i dati dal registro soggetti. La privacy non è presente. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Impresa costruttrice delle strutture in opera](#1-impresa-costruttrice-delle-strutture-in-opera)
2. [Descrizione sintetica dell'intervento](#2-descrizione-sintetica-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Tipologia dell'intervento (NTC 2018)](#4-tipologia-dellintervento-ntc-2018)
5. [Tipologia della denuncia](#5-tipologia-della-denuncia)
6. [Dettaglio dell'intervento — rilevanza sismica](#6-dettaglio-dellintervento--rilevanza-sismica)
7. [Progettista architettonico](#7-progettista-architettonico)
8. [Progettista strutturale](#8-progettista-strutturale)
9. [Direttore dei lavori strutturale](#9-direttore-dei-lavori-strutturale)

---

## 1. Impresa costruttrice delle strutture in opera

Questa sezione richiede i dati completi del Legale Rappresentante e della sede legale dell'impresa. Il pulsante **"Carica Soggetto"** consente di importare i dati automaticamente dal registro soggetti.

---

### ATTENZIONE ! Cognome del Legale Rappresentante dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Soluzione**: Inserisci il cognome del Legale Rappresentante nel campo **"Cognome"** della sezione **"Impresa costruttrice delle strutture in opera"**, oppure usa **"Carica Soggetto"** per importarlo.

---

### ATTENZIONE ! Nome del Legale Rappresentante dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Soluzione**: Inserisci il nome del Legale Rappresentante nel campo **"Nome"**.

---

### ATTENZIONE ! Ragione Sociale dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Soluzione**: Inserisci la ragione sociale dell'impresa nel campo **"Ragione Sociale Ditta"** (max 16 caratteri).

---

### ATTENZIONE ! P.IVA dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Dove si trova**: Campo **"C.F./P.IVA"**

**Soluzione**: Inserisci il Codice Fiscale o la Partita IVA dell'impresa nel campo **"C.F./P.IVA"** (max 16 caratteri).

---

### ATTENZIONE ! Sede dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Dove si trova**: Campo **"con sede legale a"**

**Soluzione**: Inserisci la città della sede legale dell'impresa.

---

### ATTENZIONE ! Provincia della sede dell'Impresa costruttrice delle strutture in opera obbligatoria.

**Dove si trova**: Campo **"Prov."**

**Soluzione**: Inserisci la sigla della provincia della sede legale (es. `VE`, `PD`, `TV`).

---

### ATTENZIONE ! CAP della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Dove si trova**: Campo **"CAP"** della sezione Impresa

**Soluzione**: Inserisci il CAP della sede legale (5 cifre, es. `30100`).

{: .note }
> Il CAP della sede dell'impresa è distinto dal CAP dell'immobile oggetto dell'intervento. Inserire il CAP della **sede legale dell'impresa** in questo campo, non quello dell'intervento.

---

### ATTENZIONE ! Inidirizzo della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Dove si trova**: Campo **"via"** della sezione Impresa

**Soluzione**: Inserisci l'indirizzo (via/viale/piazza) della sede legale dell'impresa nel campo **"via"**.

{: .warning }
> **Refuso nel messaggio**: il testo recita "**Inidirizzo**" invece di "Indirizzo" — è un errore di battitura nel codice sorgente (`txtIndirizzoImprIC`). Il campo da compilare è inequivocabilmente quello della via nella sezione Impresa costruttrice.

---

### ATTENZIONE ! Numero civico dell'indirizzo della sede dell'Impresa costruttrice delle strutture in opera obbligatorio.

**Dove si trova**: Campo **"n."** accanto a "via"

**Soluzione**: Inserisci il numero civico della sede legale nel campo **"n."**.

---

## 2. Descrizione sintetica dell'intervento

### ATTENZIONE ! Descrizione sintetica dell'intervento obbligatoria.

**Dove si trova**: Sezione **"Descrizione sintetica dell'intervento"** → campo di testo **"che i lavori per i quali viene inoltrata la presente consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere strutturali oggetto della denuncia.

**Soluzione**: Inserisci una descrizione sintetica dei lavori nel campo di testo (max **300 caratteri**). Esempi:
- `Costruzione di edificio residenziale bifamiliare in muratura portante, 2 piani fuori terra.`
- `Miglioramento sismico di edificio produttivo esistente mediante inserimento di controventi metallici.`
- `Nuova palazzina commerciale in c.a., 4 piani, con piano interrato, zona sismica 2.`

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP dell'immobile è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** dell'immobile oggetto dell'intervento (es. `30100`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico dell'immobile nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Tipologia dell'intervento (NTC 2018)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia dell'intervento'.

**Dove si trova**: Sezione **"Tipologia dell'intervento"** → checkbox NTC 2018

**Causa**: Non hai indicato in quale categoria di intervento ai sensi delle NTC (D.M. 17/01/2018) ricadono i lavori.

**Soluzione**: Spunta **almeno uno** dei quattro checkbox:
- ☑ **"Nuova costruzione"**
- ☑ **"Miglioramento sismico"**
- ☑ **"Adeguamento sismico"**
- ☑ **"Intervento locale"**

È possibile spuntare più checkbox se i lavori ricadono in più categorie. La classificazione si riferisce alle definizioni delle Norme Tecniche sulle Costruzioni di cui al D.M. 17/01/2018.

---

## 5. Tipologia della denuncia

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia della denuncia'.

**Dove si trova**: Sezione **"Tipologia della denuncia"** → radio button

**Causa**: Non hai dichiarato se si tratta di un nuovo deposito o di una variante a un'autorizzazione sismica precedente.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"Nuovo deposito"** → nessun campo aggiuntivo
- ⚪ **"Variante sostanziale all'autorizzazione sismica n."** → si attivano tre campi obbligatori (vedi sotto)

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione sismica.

**Causa**: Hai selezionato "Variante sostanziale" ma non hai inserito il numero dell'autorizzazione sismica originaria.

**Soluzione**: Inserisci il numero dell'autorizzazione sismica nel campo **"autorizzazione sismica n."** che si attiva accanto al radio button.

---

### ATTENZIONE ! Inserire il numero del protocollo dell'autorizzazione sismica.

**Causa**: Hai selezionato "Variante sostanziale" ma non hai inserito il numero di protocollo.

**Soluzione**: Inserisci il numero di protocollo nel campo **"prot. n."**.

---

### ATTENZIONE ! Inserire la data del protocollo dell'autorizzazione sismica. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Il campo data del protocollo è vuoto oppure in formato non valido.

**Soluzione**: Inserisci la data nel campo **"del"** nel formato **GG/MM/AAAA** (es. `15/03/2023`). Puoi usare l'icona calendario.

---

## 6. Dettaglio dell'intervento — rilevanza sismica

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Dettaglio dell'intervento'.

**Dove si trova**: Sezione **"Dettaglio dell'intervento"** → checkbox rilevanza sismica (art. 94-bis D.P.R. 380/2001 e DGR 1823/2020)

**Causa**: Non hai indicato per quale motivo l'intervento è classificato come **RILEVANTE** ai fini sismici.

**Soluzione**: Spunta **almeno uno** dei tre checkbox:
- ☑ **Rilevanza 1** — interventi di adeguamento o miglioramento sismico di costruzioni esistenti in **Zona 1** e in **Zona 2** (limitatamente a 0,20 g ≤ ag ≤ 0,25 g)
- ☑ **Rilevanza 2** — nuove costruzioni che si discostino dalle usuali tipologie o di particolare complessità strutturale, situate in **Zona 1 e 2**
- ☑ **Rilevanza 3** — interventi relativi a edifici di interesse strategico e opere infrastrutturali rilevanti ai fini della protezione civile o per le conseguenze del loro eventuale collasso, in **Zona 1 e 2** (DGRV n. 3645/2003)

{: .note }
> La classificazione come intervento "rilevante" è obbligatoria per questo tipo di denuncia (DSB). Se l'intervento non ricade in nessuna delle tre categorie, verificare con il SUE se la pratica corretta è invece quella per interventi "non rilevanti" o "privi di rilevanza". La classificazione sismica del Comune (Zona 1, 2, 3, 4) è consultabile sul sito della Regione Veneto o del Dipartimento della Protezione Civile.

---

## 7. Progettista architettonico

Ogni figura professionale obbligatoria richiede **13 campi**. Il pulsante **"Carica Soggetto"** consente di importare automaticamente tutti i dati dal registro soggetti.

{: .note }
> Per tutte le sezioni professionisti (7, 8, 9) usa **"Carica Soggetto"**: seleziona tipo soggetto, poi il soggetto dall'elenco, poi clicca il pulsante. Evita errori di digitazione su CF, PEC e numero albo.

---

### ATTENZIONE ! Cognome del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"Cognome"** della sezione **"Progettista architettonico"**.

### ATTENZIONE ! Nome del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"Nome"**.

### ATTENZIONE ! Codice Fiscale del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"Codice Fiscale"**.

### ATTENZIONE ! Città di residenza del Progettista architettonico obbligatoria.
**Soluzione**: Campo **"Residente in"**.

### ATTENZIONE ! Provincia di residenza del Progettista architettonico obbligatoria.
**Soluzione**: Campo **"Provincia di"** (sigla, es. `VE`).

### ATTENZIONE ! Indirizzo di residenza del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"Via"**.

### ATTENZIONE ! Numero civico di residenza del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"n."** accanto a "Via".

### ATTENZIONE ! Iscrizione all'Albo del Progettista architettonico obbligatoria.
**Soluzione**: Campo **"Iscritto all'Albo degli"** (es. `ARCHITETTI`, `INGEGNERI`, `GEOMETRI`).

### ATTENZIONE ! Provincia di iscrizione all'Albo del Progettista architettonico obbligatoria.
**Soluzione**: Campo **"della provincia di"** (sigla provincia dell'albo, es. `VE`).

### ATTENZIONE ! Numero di iscrizione all'Albo del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"al n."** (numero di iscrizione all'albo professionale).

### ATTENZIONE ! PEC del Progettista architettonico obbligatoria.
**Soluzione**: Campo **"PEC"** (indirizzo email certificata del professionista).

### ATTENZIONE ! Telefono del Progettista architettonico obbligatorio.
**Soluzione**: Campo **"tel. n."** (numero di telefono del professionista).

---

## 8. Progettista strutturale

Stessa struttura del Progettista architettonico: 13 campi tutti obbligatori.

---

### ATTENZIONE ! Cognome del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"Cognome"** della sezione **"Progettista strutturale"**.

### ATTENZIONE ! Nome del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"Nome"**.

### ATTENZIONE ! Codice Fiscale del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"Codice Fiscale"**.

### ATTENZIONE ! Città di residenza del Progettista strutturale obbligatoria.
**Soluzione**: Campo **"Residente in"**.

### ATTENZIONE ! Provincia di residenza del Progettista strutturale obbligatoria.
**Soluzione**: Campo **"Provincia di"**.

### ATTENZIONE ! Indirizzo di residenza del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"Via"**.

### ATTENZIONE ! Numero civico di residenza del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"n."** accanto a "Via".

### ATTENZIONE ! Iscrizione all'Albo del Progettista strutturale obbligatoria.
**Soluzione**: Campo **"Iscritto all'Albo degli"**.

### ATTENZIONE ! Provincia di iscrizione all'Albo del Progettista strutturale obbligatoria.
**Soluzione**: Campo **"della provincia di"**.

### ATTENZIONE ! Numero di iscrizione all'Albo del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"al n."**.

### ATTENZIONE ! PEC del Progettista strutturale obbligatoria.
**Soluzione**: Campo **"PEC"**.

### ATTENZIONE ! Telefono del Progettista strutturale obbligatorio.
**Soluzione**: Campo **"tel. n."**.

---

## 9. Direttore dei lavori strutturale

Stessa struttura del Progettista architettonico: 13 campi tutti obbligatori.

---

### ATTENZIONE ! Cognome del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"Cognome"** della sezione **"Direttore dei lavori strutturale dell'intero intervento"**.

### ATTENZIONE ! Nome del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"Nome"**.

### ATTENZIONE ! Codice Fiscale del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"Codice Fiscale"**.

### ATTENZIONE ! Città di residenza del Direttore dei lavori strutturale obbligatoria.
**Soluzione**: Campo **"Residente in"**.

### ATTENZIONE ! Provincia di residenza del Direttore dei lavori strutturale obbligatoria.
**Soluzione**: Campo **"Provincia di"**.

### ATTENZIONE ! Indirizzo di residenza del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"Via"**.

### ATTENZIONE ! Numero civico di residenza del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"n."** accanto a "Via".

### ATTENZIONE ! Iscrizione all'Albo del Direttore dei lavori strutturale obbligatoria.
**Soluzione**: Campo **"Iscritto all'Albo degli"**.

### ATTENZIONE ! Provincia di iscrizione all'Albo del Direttore dei lavori strutturale obbligatoria.
**Soluzione**: Campo **"della provincia di"**.

### ATTENZIONE ! Numero di iscrizione all'Albo del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"al n."**.

### ATTENZIONE ! PEC del Direttore dei lavori strutturale obbligatoria.
**Soluzione**: Campo **"PEC"**.

### ATTENZIONE ! Telefono del Direttore dei lavori strutturale obbligatorio.
**Soluzione**: Campo **"tel. n."**.

---

## Consigli pratici DSB Veneto

### Prima di validare ✅

**Impresa costruttrice** (10 campi):
- [ ] Cognome Legale Rappresentante
- [ ] Nome Legale Rappresentante
- [ ] Ragione Sociale (max 16 car.)
- [ ] C.F./P.IVA (max 16 car.)
- [ ] Città sede legale
- [ ] Provincia sede legale (sigla)
- [ ] CAP sede legale
- [ ] Via sede legale
- [ ] Numero civico sede legale

**Intervento**:
- [ ] Descrizione sintetica (max 300 car.)
- [ ] Indirizzo immobile (menu o "Toponimo mancante")
- [ ] CAP immobile (5 cifre)
- [ ] Numero civico immobile
- [ ] Almeno un mappale con ✅
- [ ] Destinazione d'uso
- [ ] Almeno una **tipologia NTC 2018** (Nuova costr. / Miglioramento / Adeguamento / Intervento locale)
- [ ] **Tipologia denuncia** (Nuovo deposito o Variante)
- [ ] Se Variante: numero autorizzazione + numero protocollo + data protocollo (GG/MM/AAAA)
- [ ] Almeno una **rilevanza sismica** (Rilevanza 1, 2 o 3)

**Progettista architettonico** (13 campi — usa "Carica Soggetto"):
- [ ] Cognome, Nome, CF, Città, Provincia, Via, N. civico, Albo, Prov. albo, N. albo, PEC, Telefono

**Progettista strutturale** (13 campi — usa "Carica Soggetto"):
- [ ] Cognome, Nome, CF, Città, Provincia, Via, N. civico, Albo, Prov. albo, N. albo, PEC, Telefono

**Direttore lavori strutturale** (13 campi — usa "Carica Soggetto"):
- [ ] Cognome, Nome, CF, Città, Provincia, Via, N. civico, Albo, Prov. albo, N. albo, PEC, Telefono

- [ ] **Salva** frequentemente — con 49+ campi obbligatori un salvataggio intermedio è essenziale

### Sezioni presenti ma non validate ⚠️

| Sezione ASCX | Validata nel VB? |
|---|---|
| Impresa costruttrice strutture in opera | ☑ Sì (10 campi) |
| Impresa costruttrice strutture prefabbricate | ✗ No (facoltativi) |
| Progettista architettonico | ☑ Sì (13 campi) |
| Progettista strutturale | ☑ Sì (13 campi) |
| Progettista strutture prefabbricate | ✗ No (facoltativi) |
| Direttore lavori strutturale | ☑ Sì (13 campi) |
| Geologo | ✗ No (facoltativo) |
| Collaudatore in corso d'opera | ✗ No (facoltativo) |
| Altro (campo note) | ✗ No (facoltativo) |

### Errori frequenti DSB Veneto 🔍

1. **CAP impresa vs CAP immobile** → due campi CAP distinti: uno per la sede dell'impresa (sezione 1), uno per l'immobile oggetto dei lavori (sezione 3); non confonderli
2. **Refuso "Inidirizzo"** → messaggio per il campo via dell'impresa ha un errore di battitura; il campo è inequivocabile
3. **Tipologia NTC non selezionata** → quattro checkbox, almeno uno obbligatorio; facile da dimenticare perché visivamente tra la descrizione e la denuncia
4. **Nessuna rilevanza sismica** → i tre checkbox della rilevanza sono in fondo al modulo, dopo la tipologia denuncia; spesso il primo in assoluto ad essere dimenticato
5. **Carica Soggetto** → con tre blocchi da 13 campi ciascuno, usare sempre "Carica Soggetto" per evitare i 39 errori possibili sui professionisti

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

**Ultima revisione**: Giugno 2026
**Fonte**: Analisi codice `ValidaDatiDSBVeneto` e `DatiDSBVeneto.ascx`
