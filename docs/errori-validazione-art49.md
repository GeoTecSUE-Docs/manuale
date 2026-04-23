---
title: Errori Parere art. 49 L.U.R. - Regione Piemonte
parent: Errori di validazione
nav_order: 22
description: Errori di validazione specifici per la richiesta di Parere ai sensi dell'art. 49 L.U.R. (L.R. 56/77) - Regione Piemonte
keywords: [parere art. 49, LUR, L.R. 56/77, L.R. 32/2008, PRG vigente, PRG adottato, parere urbanistico, errori art. 49]
IDRegione: 2
IDTipoPratica: 52
Fonte: Manuale
---

# Errori di validazione - Parere art. 49 L.U.R.
## Regione Piemonte

Guida completa agli errori specifici per la **richiesta di Parere ai sensi dell'art. 49, comma 7, della L.R. 56/77** (Legge Urbanistica Regionale), nonché della L.R. 32 del 01/12/2008 e s.m.i. e delle vigenti Norme Tecniche di Attuazione del P.R.G., relativa alla **Regione Piemonte**.

{: .note }
> La pratica Parere art. 49 L.U.R. è una richiesta di parere urbanistico per interventi ricadenti in specifiche aree soggette a tale prescrizione. È strutturalmente molto simile alla pratica [Zona UNESCO](errori-zona-unesco-piemonte.html) — stessa base normativa, stesso meccanismo di titolarità e stessi campi Zona PRG — con due differenze sostanziali: **non richiede la selezione della zona Core/Buffer** (assente in questa pratica), e include una sezione **"Note"** facoltativa. Non include sezioni tecnici, imprese, sicurezza o contributo. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Descrizione sintetica dell'intervento](#3-descrizione-sintetica-dellintervento)
4. [Note](#4-note)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Specificare la titolarità dell'intervento.

**Dove si trova**: Campo **"Specificare se altro"** nella sezione **"Titolarità Intervento"**

**Causa**: Hai selezionato dal menu a discesa la voce **"altro"** come titolo di presentazione della pratica, ma non hai compilato il campo di testo libero che specifica di quale titolo si tratta.

**Soluzione**:
1. Trova il campo **"Specificare se altro"** accanto al menu a discesa
2. Inserisci il tipo di titolo che hai sull'immobile (es. `Locatario con autorizzazione del proprietario`, `Amministratore di condominio delegato`, `Procuratore`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il campo "Specificare se altro" è normalmente disabilitato e si attiva automaticamente solo quando si seleziona la voce "altro" dal menu a discesa. Per tutte le altre voci (proprietario, usufruttuario, ecc.) questo campo non è richiesto e il controllo non viene eseguito.

---

## 2. Localizzazione dell'intervento

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**: Compila il campo di testo che appare accanto a "Toponimo mancante" (es. `Via Roma`, `Piazza Castello`).

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona la via dal menu a discesa, oppure spunta ☑ **"Toponimo mancante"** e inseriscila manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il CAP non è stato inserito.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`). Nessuno spazio, nessun trattino.

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il numero civico non è stato inserito.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (es. `15`, `snc`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non hai inserito almeno un mappale catastale.

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione (se presente), Foglio, Mappale e Subalterno (solo fabbricati)
3. Clicca l'**icona ✅ verde** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la zona di PRG vigente.

**Dove si trova**: Campo **"Zona PRG vigente"** nella sezione Localizzazione

**Causa**: Non hai inserito la zona del Piano Regolatore Generale vigente in cui ricade l'immobile.

**Soluzione**:
1. Trova il campo **"Zona PRG vigente"** nella sezione localizzazione
2. Inserisci la zona come indicata negli strumenti urbanistici del Comune (es. `Zona A - Centro storico`, `R3`, `Ambito di conservazione`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La zona PRG vigente si ricava dalla cartografia urbanistica comunale o dal Certificato di Destinazione Urbanistica (CDU). Puoi consultare il SIT (Sistema Informativo Territoriale) del tuo Comune o rivolgerti all'Ufficio Tecnico Comunale.

---

### ATTENZIONE ! Inserire la zona di PRG adottato.

**Dove si trova**: Campo **"Zona PRG adottato"** nella sezione Localizzazione

**Causa**: Non hai inserito la zona del Piano Regolatore Generale adottato (variante adottata ma non ancora vigente).

**Soluzione**:
1. Trova il campo **"Zona PRG adottato"** accanto al campo Zona PRG vigente
2. Inserisci la zona come indicata nel PRG adottato
3. Se non ci sono varianti in corso o il PRG adottato coincide con quello vigente, inserisci la stessa zona o una dicitura esplicativa (es. `coincidente con PRG vigente`, `nessuna variante adottata`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Entrambi i campi Zona PRG (vigente e adottato) sono **sempre obbligatori**. Se non ci sono varianti in corso, è comunque necessario compilare entrambi i campi: inserisci la stessa zona o la dicitura più appropriata per il tuo caso.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Tieni premuto **CTRL** per selezionarne più di una.

---

## 3. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Campo di testo nella sezione **"Descrizione sintetica dell'intervento"**

**Causa**: Non hai inserito la descrizione sintetica delle opere previste.

**Soluzione**:
1. Vai alla sezione **"Descrizione sintetica dell'intervento"**
2. Inserisci una sintesi chiara delle opere da eseguire (max **300 caratteri**)
3. La descrizione deve essere coerente con la relazione tecnica allegata, che contiene il dettaglio completo
4. Esempi:
   - `Restauro e risanamento conservativo della facciata esterna con pulitura e tinteggiatura.`
   - `Sostituzione infissi esterni con modelli conformi alle NTA del PRG vigente.`
   - `Ristrutturazione interna con eliminazione di tramezze non portanti, senza modifica dell'involucro esterno.`
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 4. Note

La sezione **"Note"** è completamente **facoltativa**: il campo `txtNote` non è soggetto ad alcun controllo di validazione nel codice VB. Puoi lasciarla vuota senza che la validazione produca errori.

Puoi utilizzarla per inserire informazioni aggiuntive utili all'istruttore della pratica che non trovano posto nella descrizione sintetica (es. riferimenti a precedenti pratiche, vincoli specifici, richieste particolari, note sulla tempistica).

---

## Consigli pratici Parere art. 49 L.U.R.

### Prima di validare ✅

- [ ] Compila il menu a discesa **titolarità** (proprietario, usufruttuario, ecc.)
- [ ] Se hai selezionato "altro": compila il campo **"Specificare se altro"**
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Inserisci la **Zona PRG vigente**
- [ ] Inserisci la **Zona PRG adottato** (entrambi obbligatori)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Le **Note** sono facoltative — compilale solo se hai informazioni aggiuntive utili
- [ ] **Salva** frequentemente

### Differenze rispetto alla pratica Zona UNESCO ⚠️

Il Parere art. 49 L.U.R. e la Zona UNESCO condividono la stessa base normativa (L.R. 32/2008, art. 49 c.7 L.R. 56/77) e la stessa struttura di validazione, ma presentano due differenze sostanziali.

La pratica Zona UNESCO richiede obbligatoriamente la selezione della zona di appartenenza (**Core Zone** o **Buffer Zone**) tramite radio button. Il Parere art. 49 L.U.R. **non ha questa sezione**: non c'è nessuna scelta Core/Buffer e il relativo errore non compare mai in questa pratica.

Il Parere art. 49 L.U.R. include invece una sezione **"Note"** con campo di testo libero, completamente assente nella Zona UNESCO. Le note sono facoltative e non vengono mai bloccanti in fase di validazione.

### Errori frequenti Parere art. 49 🔍

1. **"altro" selezionato senza specificare** → il campo "Specificare se altro" si attiva solo per quella voce; per le altre voci del menu non è richiesto
2. **Zona PRG adottato vuota** → spesso dimenticata perché si pensa sia opzionale; è invece sempre obbligatoria
3. **Descrizione sintetica vuota** → unico controllo sulla sezione c), obbligatorio

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
**Fonte**: Analisi codice ValidaDatiART49 e DatiArt49.ascx
