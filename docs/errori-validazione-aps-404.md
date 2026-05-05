---
title: Errori Autorizzazione Paesaggistica Semplificata - Regione Lombardia
parent: Errori di validazione
nav_order: 33
description: Errori di validazione specifici per l'Autorizzazione Paesaggistica Semplificata (APS) - Regione Lombardia (art. 3 DPR 13/02/2017 n. 31, L.R. 12/2005)
keywords: [autorizzazione paesaggistica semplificata, APS, Lombardia, DPR 31/2017, allegato B, vincolo paesaggistico, art. 136, art. 142, coordinate UTM, intervento variante]
IDRegione: 4
IDTipoPratica: 404
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Semplificata (APS)
## Regione Lombardia

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Semplificata** ai sensi dell'art. 3 del D.P.R. 13 febbraio 2017, n. 31, relativa alla **Regione Lombardia**.

{: .note }
> L'APS Lombardia è un'istanza per interventi di lieve entità in zona vincolata. Rispetto all'APS Piemonte (già documentata) presenta alcune differenze significative: la **titolarità** è gestita solo tramite menu a discesa (senza radio button aggiuntivi), il campo "Specificare se altro" si attiva quando il valore selezionato è `"altron"` anziché tramite checkbox. Le **coordinate UTM** sono obbligatorie come nelle altre pratiche lombarde. La sezione **dichiarazioni vincolo paesaggistico** ha 4 checkbox con struttura molto articolata (Vincolo1 richiede 3 campi, Vincolo2 ne richiede 5), ma il codice **non verifica che almeno una sia spuntata** — ogni checkbox è facoltativa, ma se spuntata attiva campi obbligatori. La sezione **intervento variante** è una checkbox facoltativa con 3 campi condizionali inclusa una data con verifica formato. Nessuna sezione imprese. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento e coordinate UTM](#2-localizzazione-dellintervento-e-coordinate-utm)
3. [Descrizione dell'intervento e voce Allegato B](#3-descrizione-dellintervento-e-voce-allegato-b)
4. [Dichiarazioni vincolo paesaggistico](#4-dichiarazioni-vincolo-paesaggistico)
5. [Intervento di variante — campi condizionali](#5-intervento-di-variante--campi-condizionali)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

---

### ATTENZIONE ! Specificare la titolarità dell'intervento.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo di testo **"Specificare se altro"**

**Causa**: Hai selezionato la voce "altro" (valore `altron`) dal menu a discesa **"di avere titolo alla presentazione di questa pratica edilizia in quanto"**, ma non hai compilato il campo di testo che specifica il tipo di titolarità.

**Soluzione**:
1. Trova la sezione "Titolarità dell'intervento"
2. Se hai selezionato "altro" dal menu, compila il campo **"Specificare se altro"** con la descrizione della tua titolarità (es. `Usufruttuario`, `Conduttore con contratto registrato`, `Titolare di diritto di superficie`)
3. Altrimenti, torna al menu e seleziona una delle voci standard (proprietario, ecc.)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Nella APS Lombardia la titolarità è gestita **solo dal menu a discesa**, senza i radio button aggiuntivi presenti in altre pratiche. Il campo "Specificare se altro" si attiva automaticamente solo quando il menu restituisce il valore interno `"altron"`. Le altre voci del menu non richiedono specificazione aggiuntiva.

---

## 2. Localizzazione dell'intervento e coordinate UTM

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

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `20121`).

{: .warning }
> **CRITICO**: CAP errato blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Numero civico mancante.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila i dati e salva con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Dove si trova**: Campo **"Coord. asse X"** nella sezione Coordinate (UTM – WGS 84 32N)

**Causa**: Il campo coordinata X è vuoto.

**Soluzione**: Inserisci la coordinata X nel campo corrispondente. Deve essere compresa tra **430.000 e 700.000** (es. `514500`). Usa il punto come separatore decimale, non la virgola.

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: La coordinata X è fuori dal range valido oppure contiene caratteri non numerici o usa la virgola come separatore.

**Soluzione**: Verifica che la coordinata X sia un numero compreso tra **430.000 e 700.000**. Usa il punto come separatore decimale (es. `514500.5` ✅ — `514500,5` ❌).

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo coordinata Y è vuoto.

**Soluzione**: Inserisci la coordinata Y: un numero compreso tra **4.800.000 e 5.700.000** (es. `5034200`).

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: La coordinata Y è fuori dal range valido oppure in formato errato.

**Soluzione**: Verifica che la coordinata Y sia compresa tra **4.800.000 e 5.700.000**. Usa il punto come separatore decimale.

---

## 3. Descrizione dell'intervento e voce Allegato B

Questa sezione contiene due campi sempre obbligatori, verificati in sequenza.

---

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione **"Descrizione sintetica dell'intervento"** → campo di testo **"che i lavori per i quali viene inoltrata la richiesta consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere oggetto della richiesta di autorizzazione paesaggistica.

**Soluzione**: Inserisci una descrizione sintetica dei lavori nel campo di testo (max **300 caratteri**). Esempi:
- `Tinteggiatura delle facciate esterne con cambio cromatico in zona soggetta a vincolo ex art. 136 D.Lgs. 42/2004.`
- `Sostituzione di serramenti con modifica di materiale in edificio ricadente in fascia di rispetto fluviale.`
- `Installazione di pergolato in legno nel giardino privato in zona assoggettata a vincolo paesaggistico.`

---

### ATTENZIONE ! Inserire la voce di riferimento dell'allegato B.

**Dove si trova**: Campo **"riconducibile alla voce ___ dell'allegato B"** subito sotto la descrizione

**Causa**: Non hai indicato a quale voce dell'Allegato B del D.P.R. 31/2017 è riconducibile l'intervento.

**Soluzione**: Inserisci il numero della voce dell'Allegato B del D.P.R. 13 febbraio 2017, n. 31 corrispondente all'intervento (es. `A.2`, `A.6`, `B.14`). L'Allegato B elenca gli interventi ammissibili al procedimento semplificato di autorizzazione paesaggistica.

{: .note }
> L'Allegato B del D.P.R. 31/2017 definisce le tipologie di intervento di lieve entità ammissibili al procedimento semplificato. Se non sei sicuro della voce corretta, consulta il testo del decreto prima di compilare il modulo. Il campo accetta solo poche decine di caratteri (campo piccolo, 50px di larghezza nel modulo).

---

## 4. Dichiarazioni vincolo paesaggistico

La sezione "DICHIARAZIONI" contiene 4 checkbox per indicare la base normativa del vincolo paesaggistico applicabile. Il codice **non verifica che almeno una sia spuntata**: le checkbox sono tutte facoltative ai fini della validazione automatica. Tuttavia, **se una checkbox è spuntata**, i campi di testo correlati diventano obbligatori.

{: .note }
> La sezione vincoli dell'APS Lombardia è diversa da quella dell'APS Piemonte (dove era richiesta almeno una selezione) e dall'ACP Piemonte (14 checkbox con almeno una obbligatoria). Nell'APS Lombardia il validatore non controlla la presenza del vincolo, ma controlla la completezza dei campi qualora la checkbox sia stata spuntata.

---

### Vincolo 1 — Art. 136 D.Lgs. 42/2004 (3 campi obbligatori se spuntato)

#### ATTENZIONE ! Inserire lettera relativa art. 136 comma 1.

**Dove si trova**: Primo campo di testo (70px) subito dopo "all'art. 136, comma 1 lettera"

**Causa**: Hai spuntato la checkbox Vincolo1 ma non hai indicato la lettera della classificazione (a, b, c o d) prevista dall'art. 136, c. 1, del D.Lgs. 42/2004.

**Soluzione**: Inserisci la lettera corrispondente alla tipologia di immobile/area vincolata (es. `a`, `b`, `c` o `d`).

---

#### ATTENZIONE ! Inserire provvedimento DM.

**Causa**: Hai spuntato Vincolo1 ma non hai inserito il riferimento al Decreto Ministeriale che ha istituito il vincolo.

**Soluzione**: Inserisci il riferimento al DM nel campo **"DM"** (es. `12/03/1975`, `DM 1975`, `DM 30/12/1975`).

---

#### ATTENZIONE ! Inserire provvedimento DGR.

**Causa**: Hai spuntato Vincolo1 ma non hai inserito il riferimento alla Delibera di Giunta Regionale.

**Soluzione**: Inserisci il riferimento alla DGR nel campo **"DGR"** (es. `DGR 8/6415 del 27/12/2007`, `DGR 2024-01`).

---

### Vincolo 2 — Art. 142 D.Lgs. 42/2004 (5 campi obbligatori se spuntato)

#### ATTENZIONE ! Inserire lettera relativa art. 142 comma 1.

**Dove si trova**: Primo campo di testo dopo "all'art. 142, comma 1, lettera"

**Causa**: Hai spuntato Vincolo2 ma non hai indicato la lettera della categoria di vincolo ex art. 142, c. 1, D.Lgs. 42/2004.

**Soluzione**: Inserisci la lettera corrispondente (es. `a` per coste, `b` per laghi, `c` per fiumi, `d` per montagne, ecc.).

---

#### ATTENZIONE ! Campo obbligatorio non inserito. (Vincolo2 — distanza)

**Dove si trova**: Secondo campo di testo dopo "in quanto ricadenti entro"

**Causa**: Non hai inserito la distanza o la misura della fascia di rispetto applicabile.

**Soluzione**: Inserisci la dimensione della fascia (es. `300 m`, `150 m`).

---

#### ATTENZIONE ! Fascia di rispetto non inserita.

**Dove si trova**: Terzo campo di testo (dopo "fasce di rispetto del")

**Causa**: Non hai indicato il corso d'acqua, il lago, la costa o l'elemento geografico di cui si tratta la fascia di rispetto.

**Soluzione**: Inserisci il nome dell'elemento geografico soggetto a fascia di rispetto (es. `fiume Po`, `lago di Como`, `mare Adriatico`).

---

#### ATTENZIONE ! Parco non inserito.

**Dove si trova**: Quarto campo di testo (dopo "Parco")

**Causa**: Non hai indicato il nome del parco applicabile.

**Soluzione**: Inserisci il nome del parco o della riserva (es. `Parco Naturale della Valle del Lambro`, `n/a` se non applicabile). Il campo è obbligatorio anche se il vincolo non è relativo a un parco: in tal caso inserisci un riferimento convenzionale o la dicitura `n.a.`.

---

#### ATTENZIONE ! Campo obbligatorio non inserito. (Vincolo2 — ultimo campo)

**Dove si trova**: Quinto campo di testo (dopo "ambiti boscati ;")

**Causa**: Non hai compilato l'ultimo campo della descrizione del Vincolo2, relativo ad altri ambiti (es. ambiti boscati, altre categorie).

**Soluzione**: Inserisci la descrizione dell'ambito residuale applicabile (es. `ambiti boscati`, `zone di interesse archeologico`, `n.a.`).

---

### Vincolo 3 — Art. 134, c. 1, lett. c) D.Lgs. 42/2004 (nessun campo aggiuntivo)

Il Vincolo3 (`chkVincolo3`) è una checkbox semplice senza campi di testo associati: **non genera errori di validazione se spuntato o non spuntato**. Non è richiesta nessuna specificazione.

---

### Vincolo 4 — Art. 80, c. 3, L.R. 12/2005 (1 campo obbligatorio se spuntato)

#### ATTENZIONE ! Inserire vincoli per intervento proposto.

**Dove si trova**: Campo di testo dopo "ai sensi dell'art. 80, comma 3, lettera" → campo piccolo accanto alla checkbox Vincolo4

**Causa**: Hai spuntato il Vincolo4 (competenza dell'Amministrazione ai sensi della L.R. 12/2005) ma non hai inserito la lettera dell'articolo 80, c. 3, L.R. 12/2005 applicabile.

**Soluzione**: Inserisci la lettera corrispondente alla competenza (es. `a`, `b`, `c`).

---

## 5. Intervento di variante — campi condizionali

La sezione "intervento di variante" è identificata dalla checkbox **"Il sottoscritto dichiara altresì che per precedenti interventi su tale immobile è stata rilasciata dall'Ente..."**. È completamente facoltativa, ma se spuntata attiva 3 campi obbligatori inclusa una data con verifica del formato.

---

### ATTENZIONE ! Inserire l'Ente che ha rilasciato l'autorizzazione.

**Causa**: Hai spuntato la checkbox "intervento variante" ma non hai indicato quale ente ha rilasciato la precedente autorizzazione paesaggistica.

**Soluzione**: Inserisci il nome dell'ente nel campo di testo accanto alla checkbox (es. `Comune di Milano`, `Città Metropolitana di Milano`, `Soprintendenza Belle Arti e Paesaggio per le Province di Milano`).

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione rilasciata.

**Causa**: Hai spuntato la checkbox "intervento variante" e inserito l'ente, ma non hai indicato il numero dell'autorizzazione paesaggistica precedentemente rilasciata.

**Soluzione**: Inserisci il numero dell'autorizzazione paesaggistica nel campo **"l'autorizzazione paesaggistica n."** (es. `AP-2020-42`, `123/2019`).

---

### ATTENZIONE ! Inserire la data di rilascio dell'autorizzazione.

**Causa**: Hai compilato ente e numero ma non hai inserito la data di rilascio dell'autorizzazione precedente.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/06/2020`).

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (intervento variante)

**Causa**: La data di rilascio dell'autorizzazione precedente è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `15/06/2020` ✅ — `15-06-2020` ❌ — `15/06/20` ❌).

{: .note }
> La data dell'intervento variante è l'**unica data dell'APS Lombardia soggetta a verifica del formato**. Tutte le altre date eventualmente presenti nel modulo (es. nei campi vincolo) non vengono verificate.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Dove si trova**: Sezione **"Soggetti coinvolti"** → Tecnici

**Causa**: Non hai aggiunto nessun tecnico tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Compila i dati del tecnico e seleziona il ruolo (il codice non richiede un ruolo specifico)
4. Clicca l'**icona ✅** per salvare
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il modulo include anche una sezione anagrafica del redattore del progetto (`txtRedattore`, `txtComuneSede`, `txtViaSede`, ecc.) con un pulsante "Carica Professionista" che permette di importare i dati dall'anagrafica. Questi campi **non sono verificati dal codice di validazione**: possono essere compilati facoltativamente. Il requisito obbligatorio è la presenza di almeno un tecnico nei Soggetti coinvolti.

---

## Consigli pratici APS Lombardia

### Prima di validare ✅

- [ ] Compila il menu a discesa **"di avere titolo"** nella sezione Titolarità
- [ ] Se selezioni "altro" (valore `altron`): compila **"Specificare se altro"**
- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci le **coordinate UTM** (X: 430.000–700.000; Y: 4.800.000–5.700.000), separatore decimale con punto
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Inserisci la **voce Allegato B** del D.P.R. 31/2017 (es. `A.2`)
- [ ] Per ogni **checkbox vincolo** spuntata: compila tutti i campi testo richiesti (Vincolo1: 3 campi; Vincolo2: 5 campi; Vincolo3: nessuno; Vincolo4: 1 campo)
- [ ] Se "intervento variante" spuntato: inserisci **ente**, **numero** e **data** (formato GG/MM/AAAA)
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti
- [ ] **Salva** frequentemente

### Differenze principali APS Lombardia vs APS Piemonte ⚠️

Le due APS condividono la base normativa (D.P.R. 31/2017) ma differiscono nell'implementazione. L'APS Lombardia ha la titolarità solo con **menu a discesa** (senza radio button), mentre Piemonte usa il classico schema menu + radio. L'APS Lombardia ha le **coordinate UTM obbligatorie**, Piemonte no. L'APS Lombardia non verifica che **almeno un vincolo sia spuntato**, mentre nel sistema Piemonte la pressione implicita del modulo porta l'utente a spuntarne almeno uno. Il **Vincolo2** dell'APS Lombardia ha 5 campi obbligatori se spuntato — struttura più complessa rispetto ai 14 checkbox semplici di Piemonte. L'APS Lombardia ha la sezione **"intervento variante"** con data verificata, Piemonte no.

### Errori frequenti APS Lombardia 🔍

1. **"Specificare se altro" non compilato** → compare solo se si seleziona la voce "altro" dal menu titolarità; non è un campo sempre visibile
2. **Coordinate fuori range o con virgola** → errore comune a tutte le pratiche lombarde; usare il punto come separatore decimale
3. **Voce Allegato B non inserita** → campo piccolo (50px) inline nella frase; facile da saltare
4. **Vincolo2 con campi incompleti** → il Vincolo2 ha 5 campi obbligatori; compilarne 3 o 4 non è sufficiente; ogni campo mancante genera un errore diverso
5. **"Parco non inserito"** → terzo campo del Vincolo2; se il vincolo non riguarda un parco, inserire comunque un valore convenzionale (`n.a.`)
6. **Data intervento variante in formato errato** → unica data con verifica formato in tutta la pratica

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
**Fonte**: Analisi codice ValidaDatiAPSLombardia e DatiAPSLombardia.ascx
