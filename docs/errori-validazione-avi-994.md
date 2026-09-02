---
title: Errori Autorizzazione Vincolo Idrogeologico - Tutte le regioni
parent: Errori di validazione
nav_order: 36
description: Errori di validazione specifici per la domanda di Autorizzazione ai fini del Vincolo Idrogeologico (AVNAZ) - Tutte le regioni
keywords: [vincolo idrogeologico, AVI nazionale, R.D. 3267/1923, movimenti di terra, superficie complessiva, vincolo ambientale, area protetta, aree a rischio, PAI, Piano di Assetto Idrogeologico]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 994
IDTarget:
  - { Reg: 1, Prat: 104 }   # Valle d'Aosta - Autorizzazione Vincolo Idrogeologico
  - { Reg: 4, Prat: 444 }   # Lombardia - Autorizzazione Vincolo Idrogeologico
  - { Reg: 6, Prat: 604 }   # Veneto - Autorizzazione Vincolo Idrogeologico
  - { Reg: 8, Prat: 804 }   # Emilia-Romagna - Autorizzazione Vincolo Idrogeologico
  - { Reg: 12, Prat: 1204 }  # Lazio - Autorizzazione Vincolo Idrogeologico
  - { Reg: 13, Prat: 1304 }  # Abruzzo - Autorizzazione Vincolo Idrogeologico
  - { Reg: 15, Prat: 1504 }  # Campania - Autorizzazione Vincolo Idrogeologico
  - { Reg: 16, Prat: 1604 }  # Basilicata - Autorizzazione Vincolo Idrogeologico
  - { Reg: 17, Prat: 1704 }  # Puglia - Autorizzazione Vincolo Idrogeologico
  - { Reg: 18, Prat: 1804 }  # Calabria - Autorizzazione Vincolo Idrogeologico
  - { Reg: 19, Prat: 1904 }  # Sicilia - Autorizzazione Vincolo Idrogeologico
Fonte: Analisi codice
---

# Errori di validazione - Autorizzazione Vincolo Idrogeologico (AVI Nazionale)
## Tutte le regioni

Guida completa agli errori specifici per la domanda di **Autorizzazione ai fini del Vincolo Idrogeologico** ai sensi del R.D. 3267/1923 e della Legge Regionale applicabile — pratica nazionale valida per tutte le regioni.

{: .note }
> L'AVI Nazionale si distingue dall'[AVI Liguria](errori-validazione-avi-41.html) e dalla [SCIAVI Liguria](errori-validazione-sciaavi-21.html) per la presenza della sezione **"Caratteristiche dell'intervento"** che richiede: la **superficie complessiva** in mq, la dichiarazione sui **movimenti di terra/roccia** (radio button), i **vincoli del sito** (almeno uno tra Ambientale, Area Protetta, Altro — ciascuno con descrizione obbligatoria se spuntato) e la dichiarazione sulle **aree a rischio PAI** (radio button). Non sono richiesti tecnici specifici. Sono presenti due **bug critici** nel codice: i controlli Focus per gli errori di Titolarità e Tipo Intervento puntano a `DatiAP1` anziché a `DatiAVINaz1`, causando potenziali eccezioni runtime o focus mancante. La privacy è solo informativa. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Tipo di intervento e descrizione](#2-tipo-di-intervento-e-descrizione)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Caratteristiche dell'intervento — superficie](#4-caratteristiche-dellintervento--superficie)
5. [Caratteristiche dell'intervento — movimenti di terra o roccia](#5-caratteristiche-dellintervento--movimenti-di-terra-o-roccia)
6. [Caratteristiche dell'intervento — vincoli del sito](#6-caratteristiche-dellintervento--vincoli-del-sito)
7. [Caratteristiche dell'intervento — aree a rischio PAI](#7-caratteristiche-dellintervento--aree-a-rischio-pai)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Non hai compilato il menu a discesa iniziale né selezionato il radio button sulla titolarità.

**Soluzione**: Compila il menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"** e seleziona una delle due opzioni:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva... ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"**

{: .warning }
> **Bug critico nel codice**: in caso di errore sulla Titolarità, il sistema tenta di impostare il focus su `DatiAP1.FindControl("rdbTitolaritaa_1")` invece di `DatiAVINaz1.FindControl("rdbTitolaritaa_1")`. L'oggetto `DatiAP1` non esiste in questo contesto: il Focus fallisce silenziosamente oppure genera un'eccezione runtime che può impedire la visualizzazione del messaggio di errore. Se il modulo non mostra il messaggio di errore e si comporta in modo anomalo dopo aver tentato di validare senza selezionare la titolarità, questo è il motivo. Segnalare al team di sviluppo per correzione urgente.

---

## 2. Tipo di intervento e descrizione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo Intervento'.

**Dove si trova**: Sezione **"Tipo di intervento"** → radio button

**Causa**: Non hai selezionato se l'intervento viene eseguito o conservato.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"esegue"** — intervento da realizzare
- ⚪ **"conserva"** — intervento già realizzato che si intende conservare

{: .warning }
> **Bug critico nel codice (identico alla Titolarità)**: anche per questo errore il Focus è puntato a `DatiAP1.FindControl("rdbTitolaritaa_1")` — stesso oggetto inesistente, stessa conseguenza. Il messaggio potrebbe non essere visualizzato correttamente in presenza di eccezioni runtime. Segnalare al team di sviluppo per correzione urgente insieme al bug della Titolarità.

---

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione **"Tipo di intervento"** → campo di testo sotto i radio button

**Causa**: Non hai inserito la descrizione degli interventi da autorizzare.

**Soluzione**: Inserisci una descrizione chiara nel campo di testo **"gli interventi di seguito descritti:"** (max **300 caratteri**). Esempi:
- `Sbancamento di mc 350 per realizzazione piano interrato di fabbricato residenziale.`
- `Rinterro e livellamento di area agricola per sistemazione idraulica, superficie 5000 mq.`
- `Consolidamento versante con palificate in legno e rinverdimento, lunghezza 80 m.`

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Caratteristiche dell'intervento — superficie

### ATTENZIONE ! Inserire la superficie complessiva.

**Dove si trova**: Sezione **"Caratteristiche dell'intervento"** → dichiarazione 1) → campo mq accanto a "superficie complessiva di mq"

**Causa**: Non hai inserito la superficie complessiva dell'area oggetto degli interventi.

**Soluzione**: Inserisci la superficie in metri quadrati nel campo **"superficie complessiva di mq"** (es. `350`, `1200.5`). Il valore può essere intero o decimale.

---

## 5. Caratteristiche dell'intervento — movimenti di terra o roccia

### ATTENZIONE ! Non è stata selezionata nessuna voce per i movimenti di terra o roccia.

**Dove si trova**: Sezione **"Caratteristiche dell'intervento"** → dichiarazione 2) → radio button "movimenti di terra o roccia"

**Causa**: Non hai dichiarato le modalità di esecuzione o la natura dei movimenti di terra o roccia.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"verranno effettuati adottando ogni cautela necessaria ad evitare alterazioni idrogeologiche dell'area oggetto dei lavori... in assoluta conformità al progetto presentato"** — per interventi futuri regolari
- ⚪ **"sono stati eseguiti abusivamente nell'area sottoposta a vincolo idrogeologico ma non hanno pregiudicato né sono suscettibili di pregiudicare l'assetto idrogeologico dei luoghi"** — per interventi abusivi in sanatoria

{: .note }
> La scelta tra le due opzioni ha rilevanza legale: la prima è per interventi da eseguire in conformità al progetto, la seconda è per interventi già realizzati in assenza di autorizzazione che non hanno causato danni idrogeologici. Scegliere la voce corrispondente alla situazione reale.

---

## 6. Caratteristiche dell'intervento — vincoli del sito

### ATTENZIONE ! Non è stata selezionata nessuna voce per i vincoli a cui è sottoposto il sito oggetto di intervento.

**Dove si trova**: Sezione **"Caratteristiche dell'intervento"** → dichiarazione 3) → checkbox vincoli

**Causa**: Non hai spuntato nessuno dei tre checkbox che identificano i vincoli gravanti sul sito.

**Soluzione**: Spunta **almeno uno** dei tre vincoli e compila la relativa descrizione:
- ☑ **"Ambientale"** → inserisci la descrizione nel campo di testo che si attiva
- ☑ **"Area Protetta"** → inserisci la descrizione nel campo di testo che si attiva
- ☑ **"Altro"** → inserisci la descrizione nel campo di testo che si attiva

È possibile spuntare più di un vincolo se il sito è soggetto a vincoli multipli.

---

### ATTENZIONE ! Inserire la descrizione del vincolo ambientale.

**Causa**: Hai spuntato il checkbox **"Ambientale"** ma non hai compilato il campo di testo della descrizione.

**Soluzione**: Inserisci la descrizione del vincolo ambientale nel campo di testo che si attiva accanto al checkbox (es. `Vincolo paesaggistico ai sensi dell'art. 142 D.Lgs. 42/2004 - fascia fluviale`, `Zona SIC - Sito di Importanza Comunitaria IT1180025`).

---

### ATTENZIONE ! Inserire la descrizione del vincolo di area protetta.

**Causa**: Hai spuntato il checkbox **"Area Protetta"** ma non hai compilato il campo di testo della descrizione.

**Soluzione**: Inserisci la descrizione dell'area protetta nel campo di testo che si attiva (es. `Parco Naturale Regionale del Po Piemontese`, `Riserva Naturale Orientata Bosco della Partecipanza`).

---

### ATTENZIONE ! Inserire la descrizione del vincolo di altro tipo.

**Causa**: Hai spuntato il checkbox **"Altro"** ma non hai compilato il campo di testo della descrizione.

**Soluzione**: Inserisci la descrizione dell'ulteriore vincolo nel campo di testo che si attiva (es. `Vincolo idrogeologico forestale R.D. 3267/1923`, `Fascia di rispetto cimiteriale`, `Zona di rispetto pozzi idropotabili`).

---

## 7. Caratteristiche dell'intervento — aree a rischio PAI

### ATTENZIONE ! Non è stata selezionata nessuna voce per le aree a rischio.

**Dove si trova**: Sezione **"Caratteristiche dell'intervento"** → dichiarazione 4) → radio button aree a rischio PAI

**Causa**: Non hai dichiarato se il sito ricade o meno in aree censite come "aree a rischio" nei Piani di Assetto Idrogeologico (PAI).

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"ricade"** all'interno o in prossimità di aree censite come "aree a rischio" nei Piani di Assetto Idrogeologico
- ⚪ **"non ricade"** all'interno o in prossimità di aree a rischio PAI

{: .note }
> L'informazione sulla classificazione PAI è reperibile sul sito dell'Autorità di Bacino competente per il territorio (es. Autorità di Bacino Distrettuale del Fiume Po per il Piemonte) o attraverso il Geoportale Nazionale del Ministero dell'Ambiente.

---

## Consigli pratici AVI Nazionale

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (menu a discesa + radio button)
- [ ] Seleziona il **tipo di intervento** ("esegue" o "conserva")
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **superficie complessiva** in mq
- [ ] Seleziona la dichiarazione sui **movimenti di terra/roccia** (una delle 2 opzioni)
- [ ] Spunta **almeno un vincolo** del sito (Ambientale, Area Protetta o Altro)
- [ ] Per ogni vincolo spuntato: inserisci la **descrizione** nel campo di testo corrispondente
- [ ] Seleziona la dichiarazione sulle **aree a rischio PAI** (una delle 2 opzioni)
- [ ] **Salva** frequentemente

### Errori frequenti AVI Nazionale 🔍

1. **Bug Titolarità/Tipo Intervento** → in caso di errore su questi due campi il focus può fallire o generare eccezione; compilarli sempre prima di validare per evitare comportamenti anomali
2. **Nessun vincolo spuntato** → obbligatorio spuntare almeno uno dei tre checkbox; anche "Altro" è valido se i vincoli non rientrano nelle categorie standard
3. **Vincolo spuntato senza descrizione** → ogni checkbox spuntato attiva il campo di testo corrispondente che diventa obbligatorio
4. **Superficie mancante** → campo di testo inline nella dichiarazione 1), visivamente integrato nel testo; facile da non notare
5. **PAI dimenticato** → l'ultimo radio button della sezione Caratteristiche; posizionato in fondo dopo i vincoli, spesso saltato

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
**Fonte**: Analisi codice `ValidaDatiAVINaz` e `DatiAVINaz.ascx`
