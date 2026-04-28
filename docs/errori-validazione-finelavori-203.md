---
title: Errori Fine Lavori - Regione Liguria
parent: Errori di validazione
nav_order: 29
description: Errori di validazione specifici per la Comunicazione di Fine Lavori - Regione Liguria (art. 25 L.R. 16/2008)
keywords: [fine lavori, comunicazione fine lavori, Liguria, varianti in corso d'opera, art. 25 L.R. 16/2008, tipo ultimazione, titolo edilizio, progettista asseverante]
IDRegione: 3
IDTipoPratica: 203
Fonte: Manuale
---

# Errori di validazione - Fine Lavori
## Regione Liguria

Guida completa agli errori specifici per la **Comunicazione di Fine Lavori** ai sensi dell'art. 25 della L.R. 10 novembre 2008, n. 16 e successive modifiche, relativa alla **Regione Liguria**.

{: .note }
> Il Fine Lavori Liguria include, oltre alla localizzazione standard e alla comunicazione della data di ultimazione, una sezione **"Dichiarazioni del progettista"** obbligatoria per le varianti in corso d'opera (art. 25, commi 1 e 2, L.R. 16/2008). Particolarità esclusive rispetto alle altre regioni: il **titolo edilizio** è identificato con 3 campi distinti (tipo pratica, prot./n., data) anziché i 5 della Lombardia; la sezione **varianti in corso d'opera** è un radio button obbligatorio con 2 opzioni; il codice non verifica il formato delle date e non controlla la sezione anagrafica del progettista (compilabile ma facoltativa ai fini della validazione). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Data di ultimazione e modalità](#2-data-di-ultimazione-e-modalità)
3. [Titolo edilizio di riferimento](#3-titolo-edilizio-di-riferimento)
4. [Dichiarazioni del progettista — Varianti in corso d'opera](#4-dichiarazioni-del-progettista--varianti-in-corso-dopera)

---

## 1. Localizzazione dell'intervento

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma indirizzo non inserito.

**Soluzione**: Compila il campo di testo accanto a "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona dal menu a discesa, oppure spunta ☑ "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: CAP mancante.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `16121`).

{: .warning }
> **CRITICO**: CAP errato blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Numero civico mancante.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila Sezione/Foglio/Mappale/Subalterno e salva con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 2. Data di ultimazione e modalità

---

### ATTENZIONE ! Inserire la data di ultimazione lavori.

**Dove si trova**: Sezione **"COMUNICA"** → campo data nella frase **"che in data ___ i lavori sono stati ultimati"**

**Causa**: Non hai inserito la data in cui i lavori sono stati completati.

**Soluzione**:
1. Trova il campo data nella sezione "COMUNICA" (dopo la localizzazione)
2. Inserisci la data di ultimazione nel formato **GG/MM/AAAA** (es. `15/04/2026`)
3. Puoi usare l'**icona calendario** accanto al campo oppure digitare direttamente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il codice non verifica il formato della data di ultimazione lavori. Inserisci comunque GG/MM/AAAA per evitare incongruenze nel sistema.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Ultimazione lavori'.

**Dove si trova**: Due radio button sotto la data → "completamente" e "in forma parziale come da planimetria allegata"

**Causa**: Non hai dichiarato se i lavori sono stati ultimati interamente o solo parzialmente.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"completamente"**
- ⚪ **"in forma parziale come da planimetria allegata"** → allega la planimetria che documenta la parte completata

---

## 3. Titolo edilizio di riferimento

Il titolo edilizio che ha legittimato l'intervento è identificato con tre campi distinti, tutti obbligatori. Il sistema li verifica in sequenza.

{: .note }
> Il codice non verifica il formato di `txtDataProt`. Inserisci la data comunque nel formato GG/MM/AAAA per coerenza con il sistema.

---

### ATTENZIONE ! Indicare il tipo di pratica.

**Dove si trova**: Campo di testo **"che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente:"** → prima riga (campo tipo pratica)

**Causa**: Non hai indicato la tipologia del titolo edilizio che ha autorizzato i lavori.

**Soluzione**: Inserisci il tipo di pratica nel campo testo (es. `CILA`, `SCIA`, `Permesso di Costruire`, `SCIA alternativa al PdC`).

---

### ATTENZIONE ! Campo obbligatorio 'Prot. / N.' non inserito.

**Dove si trova**: Campo **"prot. / n."** sotto il tipo di pratica

**Causa**: Non hai inserito il numero di protocollo o il numero del titolo edilizio.

**Soluzione**: Inserisci il numero di protocollo o il numero assegnato al titolo nel campo **"prot. / n."** (es. `PROT-2024-12345`, `CILA-2024-42`).

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserita.

**Dove si trova**: Campo **"del"** (data) accanto al numero di pratica

**Causa**: Non hai inserito la data del titolo edilizio.

**Soluzione**: Inserisci la data nel campo **"del"** nel formato **GG/MM/AAAA** (es. `10/03/2024`).

---

## 4. Dichiarazioni del progettista — Varianti in corso d'opera

Questa sezione è compilata dal progettista e riguarda le eventuali varianti realizzate durante i lavori rispetto al titolo edilizio originario. È richiesta sempre, anche se non vi sono varianti.

{: .note }
> I campi anagrafici del progettista (Cognome e Nome, Ordine/Collegio, sede, numero iscrizione) visibili nella sezione "DICHIARAZIONI DEL PROGETTISTA" **non sono verificati dal codice di validazione**: possono essere compilati facoltativamente. La sezione è indicata come necessaria solo "nel caso di varianti in corso d'opera" ai sensi dell'art. 25, commi 1 e 2, L.R. 16/2008. Analogamente, i campi **"data"** e **"luogo"** in fondo al modulo non vengono controllati.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Varianti in corso d'opera'.

**Dove si trova**: Sezione **"DICHIARAZIONI DEL PROGETTISTA"** → sezione **"Tipologia di intervento e descrizione sintetica delle opere"** → due radio button dopo la frase "che le varianti in corso d'opera realizzate"

**Causa**: Non hai dichiarato la natura delle varianti in corso d'opera rispetto al titolo edilizio originario.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"non configurano variazione essenziale e sono conformi alle prescrizioni urbanistico edilizie"** (art. 25, c. 2, L.R. 16/2008 e s.m.) → da usare quando le varianti sono di lieve entità e non costituiscono variazione essenziale ai sensi dell'art. 32 D.P.R. 380/2001
- ⚪ **"consistono in opere realizzabili mediante CILA ai sensi articolo 6-bis D.P.R. 380/2001"** (art. 25, c. 3, L.R. 16/2008 e s.m.) → da usare quando le varianti sono assimilabili a interventi soggetti a CILA

{: .note }
> Se non ci sono varianti rispetto al titolo edilizio originario, seleziona la prima opzione ("non configurano variazione essenziale"). Il radio button è obbligatorio in ogni caso: non è possibile lasciare la sezione senza una selezione anche quando le varianti sono inesistenti.

---

### ATTENZIONE ! Indicare descrizione lavori.

**Dove si trova**: Campo di testo **"e che consistono in:"** nella sezione Dichiarazioni del progettista

**Causa**: Non hai inserito la descrizione delle varianti (o dei lavori) nella sezione del progettista.

**Soluzione**: Inserisci la descrizione delle varianti in corso d'opera (max **300 caratteri**). Esempi:
- `Nessuna variante rispetto al progetto approvato. I lavori sono stati eseguiti in completa conformità al titolo edilizio.`
- `Leggera modifica della distribuzione interna al piano primo, senza variazione di superfici o volumi.`
- `Spostamento di una porta interna e modifica del percorso dell'impianto idraulico in bagno.`

---

## Consigli pratici Fine Lavori Liguria

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data di ultimazione lavori** nel formato GG/MM/AAAA
- [ ] Seleziona la **modalità di ultimazione** (completamente / in forma parziale)
- [ ] Inserisci il **tipo di pratica** (es. CILA, SCIA, PdC)
- [ ] Inserisci il **prot. / n.** del titolo edilizio
- [ ] Inserisci la **data** del titolo edilizio nel formato GG/MM/AAAA
- [ ] Seleziona la voce **"Varianti in corso d'opera"** (primo o secondo radio button — sempre obbligatorio)
- [ ] Inserisci la **descrizione lavori/varianti** nella sezione progettista (max 300 caratteri)
- [ ] **Salva** frequentemente

### Confronto con Fine Lavori delle altre regioni ⚠️

Il Fine Lavori Liguria si distingue per la presenza della **sezione varianti in corso d'opera** con radio button obbligatorio (art. 25 L.R. 16/2008), assente nelle versioni Piemonte e Lombardia. Il **titolo edilizio** è identificato con 3 campi (tipo pratica + n. + data) come nel vecchio schema Piemonte, a differenza della Lombardia che usa 5 campi separati (TipoProcedimento, EnteRicevente, PratEdilizia, NProt, DataProt). Non ci sono le **coordinate UTM** della Lombardia né le **dichiarazioni energetiche** obbligatorie. Non c'è la **Privacy checkbox** della Lombardia. La sezione anagrafica del progettista (cognome, nome, ordine) è **presente ma non controllata** dal validatore.

### Errori frequenti Fine Lavori Liguria 🔍

1. **Radio button "Varianti in corso d'opera" non selezionato** → sezione nella seconda parte del modulo, sotto la sezione "DICHIARAZIONI DEL PROGETTISTA"; spesso saltata perché meno visibile
2. **Tipo di pratica mancante** → primo campo del blocco titolo edilizio, a volte confuso con la sezione localizzazione
3. **Descrizione lavori vuota** → il campo `txtDescrLavori` nella sezione progettista è separato da qualsiasi altro campo descrizione; si trova quasi in fondo al modulo
4. **Data ultimazione inserita ma modalità (completamente/parzialmente) non selezionata** → i due radio button sono subito sotto la data ma non molto evidenti

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
**Fonte**: Analisi codice ValidaDatiFineLavoriLiguria e DatiFineLavoriLiguria.ascx
