---
title: Errori Attività Edilizia Libera - Tutte le regioni
parent: Errori di validazione
nav_order: 31
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori per Attività Edilizia Libera (AEL) - art. 6 c. 1 D.P.R. 380/2001
keywords: [attività edilizia libera, AEL, CIL, comunicazione inizio lavori libera, art. 6 DPR 380/2001, edilizia libera, data inizio lavori futura, impresa esecutrice]
IDRegione: Tutte
IDTipoPratica: 9928
Fonte: Manuale
---

# Errori di validazione - Attività Edilizia Libera (AEL)
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori per Attività di Edilizia Libera** ai sensi dell'art. 6, comma 1, del D.P.R. 6 giugno 2001, n. 380.

{: .note }
> L'AEL (Attività Edilizia Libera) è la comunicazione per opere eseguibili senza titolo abilitativo ai sensi dell'art. 6, c. 1, D.P.R. 380/2001. Ha due caratteristiche esclusive rispetto a tutte le altre pratiche della piattaforma: la **data di inizio lavori è condizionata a una checkbox** (non è un campo autonomo) e deve essere una **data futura** — il sistema verifica che non sia precedente alla data odierna. Nessun'altra pratica nella piattaforma esegue questo controllo. Sono presenti le sezioni **Titolarità**, **Opere su parti comuni**, **Impresa esecutrice** (obbligatoria con radio button), ma non la sezione Tecnici (commentata nel codice). La privacy è solo informativa, senza checkbox obbligatoria. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Comunicazione di inizio lavori — checkbox e data](#3-comunicazione-di-inizio-lavori--checkbox-e-data)
4. [Descrizione delle opere](#4-descrizione-delle-opere)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Impresa esecutrice dei lavori](#6-impresa-esecutrice-dei-lavori)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Non hai compilato il menu a discesa iniziale né selezionato il radio button sulla titolarità.

**Soluzione**: Compila il menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"** e seleziona una delle due opzioni:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva... ma di disporre comunque della dichiarazione di assenso dei terzi"**

---

## 2. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Non hai dichiarato se i lavori riguardano parti comuni dell'edificio.

**Soluzione**: Seleziona **una delle quattro opzioni**:
- ⚪ **"non riguardano parti comuni"**
- ⚪ **"riguardano le parti comuni di un fabbricato condominiale"**
- ⚪ **"riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"** (richiede assenso dei comproprietari allegato)
- ⚪ **"riguardano parti dell'edificio di proprietà comune ma non necessitano di assenso"** (art. 1102 c.c.)

---

## 3. Comunicazione di inizio lavori — checkbox e data

Questa sezione ha una struttura unica rispetto a tutte le altre pratiche: la data di inizio lavori non è un campo autonomo sempre obbligatorio, ma è attivata da una **checkbox che deve essere spuntata per prima**. Solo se la checkbox è spuntata diventano obbligatorie la data e la sua validità.

---

### ATTENZIONE ! Necessario spuntare la voce di inizio lavori.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → checkbox **"i lavori avranno inizio in data ___"**

**Causa**: Non hai spuntato la checkbox che attiva la comunicazione di inizio lavori. Il sistema richiede che questa dichiarazione venga esplicitamente confermata prima di inserire la data.

**Soluzione**:
1. Trova la sezione **"COMUNICA L'INIZIO DEI LAVORI"**
2. Spunta la checkbox ☑ **"i lavori avranno inizio in data"**
3. Inserisci la data di inizio lavori nel campo che si attiva a destra
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La checkbox è obbligatoria: non è possibile salvare la comunicazione senza averla spuntata. A differenza delle altre pratiche dove la data è un campo sempre visibile e obbligatorio, nell'AEL la checkbox funge da dichiarazione esplicita di intendere iniziare i lavori.

---

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: Hai spuntato la checkbox ma non hai inserito la data.

**Soluzione**: Inserisci la data di inizio lavori nel campo accanto alla checkbox nel formato **GG/MM/AAAA** (es. `20/06/2026`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data di inizio lavori è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `20/06/2026` ✅. Errati: `20-06-2026` ❌, `20/06/26` ❌.

---

### ATTENZIONE ! La data di inizio non può essere inferiore alla data odierna.

**Dove si trova**: Campo data accanto alla checkbox di inizio lavori

**Causa**: Hai inserito una data passata nel campo data di inizio lavori. L'AEL è una comunicazione preventiva di inizio lavori: la data deve essere **oggi o nel futuro**.

**Soluzione**:
1. Verifica la data inserita: deve essere uguale o successiva alla **data odierna** (oggi è il 04/05/2026)
2. Se i lavori iniziano oggi: inserisci la data odierna (`04/05/2026`)
3. Se i lavori iniziano in futuro: inserisci la data prevista di inizio
4. Se i lavori sono già iniziati: l'AEL non è la pratica corretta per questa situazione; contatta l'ufficio SUE

{: .warning }
> **Controllo esclusivo dell'AEL**: questo è l'**unico caso in tutta la piattaforma** in cui il sistema verifica che la data non sia nel passato. Tutte le altre pratiche accettano date passate senza segnalare errori. La logica riflette la natura preventiva della comunicazione: l'AEL deve essere presentata **prima** dell'inizio dei lavori. Se i lavori sono già iniziati senza comunicazione preventiva, occorre valutare con il SUE la procedura applicabile.

---

## 4. Descrizione delle opere

### ATTENZIONE ! Campo obbligatorio 'Descrizione opere' non inserito.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → campo di testo **"le opere consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere di edilizia libera oggetto della comunicazione.

**Soluzione**:
1. Trova il campo di testo **"le opere consistono in:"** sotto la checkbox di inizio lavori
2. Inserisci una descrizione chiara e sintetica delle opere (max **300 caratteri**)
3. Esempi di opere di edilizia libera (art. 6, c. 1, D.P.R. 380/2001):
   - `Manutenzione ordinaria interna: tinteggiatura pareti e soffitti di appartamento al 2° piano.`
   - `Installazione di impianto di aria condizionata split con unità esterna su parete laterale.`
   - `Sostituzione di infissi interni con materiali e dimensioni identici agli esistenti.`
   - `Installazione di pergolato in legno di mq 15 nel giardino privato, senza strutture in muratura.`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 5. Localizzazione dell'intervento

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

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali usando "Aggiungi Fabbricato" o "Aggiungi Terreno", compila i campi e salva con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 6. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai dichiarato chi eseguirà i lavori.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"che i lavori sono/saranno eseguiti dalla impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'"** → l'impresa diventa obbligatoria nei soggetti coinvolti
- ⚪ **"che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"**

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato "i lavori saranno eseguiti da impresa" ma non hai aggiunto nessuna impresa tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Imprese"**
2. Clicca **"Aggiungi Impresa"**
3. Compila i dati dell'impresa e salva
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Se i lavori sono di piccola entità e li esegui personalmente senza affidare a ditte esterne, seleziona la seconda opzione: in questo caso non è necessario aggiungere nessuna impresa nei soggetti coinvolti.

---

## Consigli pratici Attività Edilizia Libera

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (menu a discesa + radio button)
- [ ] Seleziona le **opere su parti comuni** (una delle 4 opzioni)
- [ ] **Spunta la checkbox** "i lavori avranno inizio in data"
- [ ] Inserisci la **data di inizio lavori** nel formato GG/MM/AAAA — deve essere oggi o nel futuro
- [ ] Inserisci la **descrizione delle opere** (max 300 caratteri)
- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona l'**impresa esecutrice** (una delle 2 opzioni)
- [ ] Se "lavori da impresa": aggiungi l'**impresa** nei soggetti coinvolti
- [ ] **Salva** frequentemente

### Caratteristica esclusiva: data non nel passato ⚠️

L'AEL è l'**unica pratica nella piattaforma** con verifica che la data di inizio lavori non sia nel passato. Il controllo usa `DateDiff("d", DataI, CDate(Now)) > 0`: se la differenza in giorni tra la data inserita e oggi è positiva (cioè la data è precedente a oggi), il sistema blocca la validazione. Una data uguale a oggi è accettata. Se i lavori sono già iniziati senza comunicazione preventiva, questa comunicazione non è presentabile con data retroattiva: contatta il SUE per valutare la situazione.

### Errori frequenti AEL 🔍

1. **Checkbox non spuntata** → il campo data non è autonomo: senza spuntare la checkbox il sistema non riesce a verificare la data e restituisce l'errore "necessario spuntare"
2. **Data nel passato** → errore esclusivo dell'AEL; inserire la data di oggi se i lavori iniziano oggi
3. **Descrizione opere vuota** → campo separato dalla checkbox/data, più in basso nella stessa sezione
4. **Impresa non aggiunta nei soggetti** → scegliere il radio "lavori da impresa" obbliga ad aggiungere l'impresa nella scheda Soggetti coinvolti; se l'impresa non è ancora nota usare il secondo radio

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
**Fonte**: Analisi codice ValidaDatiAELNaz e DatiAELNaz.ascx
