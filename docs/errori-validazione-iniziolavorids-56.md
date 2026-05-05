---
title: Errori Inizio Lavori Denuncia Sismica - Regione Piemonte
parent: Errori di validazione
nav_order: 30
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori relativa alla Denuncia Sismica (Modello 4) - Regione Piemonte
keywords: [inizio lavori denuncia sismica, ILDS, modello 4, art. 93 DPR 380/2001, data inizio lavori, Piemonte, denuncia strutturale, zona PRG, sismica]
IDRegione: 2
IDTipoPratica: 56
Fonte: Analisi codice
---

# Errori di validazione - Inizio Lavori Denuncia Sismica (Modello 4)
## Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori relativa alla Denuncia Sismica** (Modello 4 delle procedure attuative di gestione e controllo delle attività urbanistico-edilizie ai fini della prevenzione del rischio sismico), presentata ai sensi dell'art. 93 del D.P.R. 6 giugno 2001, n. 380, relativa alla **Regione Piemonte**.

{: .note }
> L'Inizio Lavori Denuncia Sismica è una pratica di comunicazione tecnica collegata a una Denuncia Sismica già presentata. Ha una struttura molto semplice: localizzazione standard, riferimento alla denuncia strutturale madre, data di inizio lavori e data della comunicazione. Il modulo usa il verbo **"CERTIFICA"** (non COMUNICA o DICHIARA). I campi **Zona PRG vigente** e **Zona PRG adottato** sono visibili nel modulo ma **non vengono verificati** dal codice di validazione. Il campo **numero pratica** e il campo **data pratica** della denuncia strutturale sono normalmente pre-compilati automaticamente dal sistema e verificati solo se risultano modificabili (abilitati). Le **tre date** presenti nel modulo sono tutte soggette a verifica del formato GG/MM/AAAA. Non ci sono sezioni tecnici, imprese o sicurezza. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Riferimento alla denuncia strutturale](#1-riferimento-alla-denuncia-strutturale)
2. [Data di inizio lavori e data della comunicazione](#2-data-di-inizio-lavori-e-data-della-comunicazione)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)

---

## 1. Riferimento alla denuncia strutturale

Questa sezione contiene il numero e la data della Denuncia Sismica (strutturale) già depositata, alla quale questa comunicazione di inizio lavori fa riferimento. I campi sono normalmente pre-compilati automaticamente dal sistema quando la pratica viene aperta in collegamento con la DS madre: in questo caso non è possibile modificarli e il codice non li verifica. Vengono verificati solo se risultano abilitati alla modifica.

---

### ATTENZIONE ! Campo obbligatorio 'Numero Pratica' non inserito.

**Dove si trova**: Campo **"con riferimento alla denuncia strutturale n. ___"**

**Causa**: Il campo numero pratica della denuncia strutturale di riferimento è abilitato alla modifica ma non è stato compilato.

**Soluzione**: Inserisci il numero della Denuncia Sismica già depositata nel campo **"n."**. Se il campo non è modificabile (grigio), il sistema lo ha già compilato automaticamente: non è necessario intervenire.

{: .note }
> In condizioni normali questo campo è **pre-compilato e bloccato** (`Enabled="false"`) dal sistema quando si crea la comunicazione di inizio lavori partendo dalla pratica di Denuncia Sismica collegata. Compare come errore solo in casi eccezionali in cui il campo risulta sbloccato.

---

### ATTENZIONE ! Campo obbligatorio 'Data Pratica' non inserito.

**Dove si trova**: Campo **"presentata in data ___"** accanto al numero della denuncia strutturale

**Causa**: Il campo data della denuncia strutturale di riferimento è abilitato alla modifica ma non è stato compilato.

**Soluzione**: Inserisci la data di presentazione della Denuncia Sismica collegata nel formato **GG/MM/AAAA** (es. `10/01/2026`).

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica denuncia strutturale)

**Causa**: La data della denuncia strutturale è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `10/01/2026` ✅. Errati: `10-01-2026` ❌, `10/01/26` ❌.

---

## 2. Data di inizio lavori e data della comunicazione

Questa sezione contiene le due date principali della comunicazione: la data in cui i lavori sono effettivamente iniziati e la data della comunicazione stessa. Entrambe sono sempre obbligatorie e soggette a verifica del formato.

---

### ATTENZIONE ! Campo obbligatorio 'Data Inizio Lavori' non inserito.

**Dove si trova**: Sezione **"CERTIFICA"** → campo data nella frase **"che i lavori sono iniziati il ___"**

**Causa**: Non hai inserito la data in cui i lavori sono effettivamente iniziati.

**Soluzione**:
1. Trova il campo data nella sezione "CERTIFICA" (dopo la sezione denuncia strutturale)
2. Inserisci la data di inizio lavori nel formato **GG/MM/AAAA** (es. `15/04/2026`)
3. Puoi usare l'**icona calendario** accanto al campo oppure digitare direttamente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data di inizio lavori è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserito.

**Dove si trova**: Campo **"Data"** in fondo alla sezione CERTIFICA (data della comunicazione, distinta dalla data di inizio lavori)

**Causa**: Non hai inserito la data della comunicazione stessa (la data in cui viene redatta e trasmessa la presente comunicazione di inizio lavori).

**Soluzione**: Inserisci la data odierna o la data di trasmissione della comunicazione nel campo **"Data"** nel formato **GG/MM/AAAA** (es. `29/04/2026`).

{: .note }
> La Comunicazione di Inizio Lavori DS contiene **due date distinte**: la **data di inizio lavori** (quando i lavori sono effettivamente iniziati, nel passato o in data odierna) e la **data della comunicazione** (quando viene redatto e trasmesso il documento, generalmente la data odierna). Entrambe sono obbligatorie e soggette a verifica del formato.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data comunicazione)

**Causa**: La data della comunicazione è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

## 3. Localizzazione dell'intervento

{: .note }
> I campi **"Zona PRG vigente"** e **"Zona PRG adottato"**, visibili nel modulo, **non vengono verificati** dal codice di validazione: possono essere compilati facoltativamente senza impatto sulla validazione.

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

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`).

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

## Consigli pratici Inizio Lavori Denuncia Sismica

### Prima di validare ✅

- [ ] Verifica che il **numero della denuncia strutturale** e la **data pratica** siano presenti (di solito pre-compilati automaticamente)
- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data di inizio lavori** nel formato GG/MM/AAAA (sezione CERTIFICA)
- [ ] Inserisci la **data della comunicazione** nel formato GG/MM/AAAA (campo "Data" in fondo alla sezione CERTIFICA)
- [ ] **Salva** frequentemente

### Caratteristiche peculiari di questa pratica ⚠️

L'Inizio Lavori DS è una delle pratiche più semplici della piattaforma per numero di campi obbligatori, ma ha due caratteristiche che generano confusione. Il **collegamento automatico con la DS madre**: i campi numero pratica e data pratica sono normalmente bloccati perché il sistema li compila direttamente dalla Denuncia Sismica associata; se risultano vuoti e modificabili è probabile che la pratica non sia stata creata correttamente dalla DS di riferimento. Le **due date distinte**: la "data di inizio lavori" e la "data" finale sono due campi separati che il sistema verifica indipendentemente; compilarne solo uno non è sufficiente.

### Errori frequenti Inizio Lavori DS 🔍

1. **"Data" finale non compilata** → il campo "Data" in fondo alla sezione CERTIFICA è separato dalla "Data Inizio Lavori"; spesso chi compila la data di inizio lavori dimentica di compilare anche la data della comunicazione
2. **Formato data errato** → tutte e tre le date (`txtDataPratica`, `txtDataInizioLavori`, `txtData`) hanno verifica del formato; usare trattini invece di barre (`15-04-2026` invece di `15/04/2026`) genera errore
3. **Destinazione d'uso non selezionata** → lista a scorrimento, richiede almeno un clic di selezione
4. **Numero pratica DS mancante** → raro, accade se la comunicazione viene creata manualmente senza agganciare la DS madre

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
**Fonte**: Analisi codice ValidaDatiInizioLavoriDS e DatiInizioLavoriDS.ascx
