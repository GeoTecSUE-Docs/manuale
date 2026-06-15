---
title: Errori Lavori in Abitati da Consolidare - Piemonte
parent: Errori di validazione
nav_order: 43
description: Errori di validazione specifici per i Lavori di Costruzione in Abitati da Consolidare (AC) - Regione Piemonte
keywords: [abitati da consolidare, AC, Piemonte, lavori costruzione, art. 61 DPR 380/2001, art. 30-bis L. 56/77, progettista architettonico, direttore lavori strutturali, costruttore, zona PRGC, vincolo idrogeologico, PEC, strumento urbanistico]
IDRegione: 2         # Piemonte
IDTipoPratica: 8
Fonte: Manuale
---

# Errori di validazione - Lavori in Abitati da Consolidare (AC)
## Regione Piemonte

Guida completa agli errori specifici per la **comunicazione di Lavori di Costruzione in Abitati da Consolidare** ai sensi dell'art. 61 del D.P.R. n. 380/2001 e dell'art. 30-bis della L. 56/77 — Regione Piemonte.

{: .note }
> Questa pratica è **esclusiva della Regione Piemonte** ed è la più articolata della piattaforma per numero di sezioni obbligatorie. Oltre ai campi comuni (indirizzo, mappali, destinazione d'uso), richiede: il **Comune del provvedimento edilizio**, la **tipologia di intervento** (manutenzione straordinaria o restauro), gli **estremi completi del titolo edilizio**, la **zona di PRGC**, i dati completi (cognome, nome, PEC, studio) di **quattro figure professionali** (progettista architettonico, direttore lavori architettonici, progettista strutture, direttore lavori strutturali) e del **costruttore**, le **dichiarazioni sullo strumento urbanistico** e sul **vincolo idrogeologico** con logica condizionale, e facoltativamente la dichiarazione sui **lavori già realizzati**. La PEC è validata con regex: un indirizzo formalmente errato genera un messaggio distinto rispetto al campo vuoto. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità e dati del provvedimento edilizio](#1-titolarità-e-dati-del-provvedimento-edilizio)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Progettista delle opere architettoniche](#3-progettista-delle-opere-architettoniche)
4. [Direttore dei lavori architettonici](#4-direttore-dei-lavori-architettonici)
5. [Progettista delle strutture](#5-progettista-delle-strutture)
6. [Direttore dei lavori strutturali](#6-direttore-dei-lavori-strutturali)
7. [Costruttore](#7-costruttore)
8. [Dichiarazioni — area soggetta e vincoli](#8-dichiarazioni--area-soggetta-e-vincoli)

---

## 1. Titolarità e dati del provvedimento edilizio

### ATTENZIONE ! Inserire il Comune.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo **"di essere titolare di istanza di Provvedimento Edilizio, depositato presso il Comune di"**

**Causa**: Non hai indicato il Comune presso cui è depositato il provvedimento edilizio.

**Soluzione**: Inserisci il nome del Comune nel campo di testo accanto alla dicitura "depositato presso il Comune di".

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per la tipologia dell'intervento.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → radio button tipologia

**Causa**: Non hai selezionato la tipologia dei lavori oggetto della comunicazione.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"Manutenzione straordinaria"**
- ⚪ **"Restauro e risanamento conservativo"**

---

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo di testo **"consistenti in:"**

**Causa**: Non hai descritto i lavori oggetto della comunicazione.

**Soluzione**: Inserisci una descrizione sintetica dei lavori nel campo **"consistenti in:"** (max 300 caratteri).

---

### ATTENZIONE ! Inserire gli estremi del titolo edilizio.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo **"Estremi del titolo edilizio (DIA/SCIA/PDC/CIL/CILA):"**

**Causa**: Non hai indicato la tipologia del titolo edilizio di riferimento.

**Soluzione**: Inserisci gli estremi del titolo edilizio nel campo apposito (es. `SCIA`, `Permesso di Costruire`, `CIL`, ecc.).

---

### ATTENZIONE ! Inserire il numero del titolo edilizio.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo **"numero"**

**Causa**: Non hai inserito il numero del titolo edilizio.

**Soluzione**: Inserisci il numero assegnato dal SUE al titolo edilizio di riferimento.

---

### ATTENZIONE ! Inserire la data del titolo edilizio.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo **"del"** (data titolo)

**Causa**: Non hai inserito la data del titolo edilizio.

**Soluzione**: Inserisci la data nel campo **"del"** nel formato **GG/MM/AAAA** (es. `10/04/2023`). Puoi usare l'icona calendario o digitare direttamente.

{: .note }
> A differenza di altre pratiche, la data del titolo edilizio non viene validata nel formato da questo modulo (non c'è `ControlloFormatoData` nella sezione a)): viene verificata solo la presenza. Inserisci comunque una data nel formato corretto GG/MM/AAAA per coerenza con gli altri campi del modulo.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente nel campo di testo.

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

**Causa**: Non è stato inserito nessun mappale catastale né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅ (tasto verde con spunta)

---

### ATTENZIONE ! Inserire la zona di PRG vigente.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo **"Zona di PRGC"**

**Causa**: Non hai indicato la zona del Piano Regolatore Generale Comunale in cui ricade l'intervento.

**Soluzione**: Inserisci la zona di PRGC nel campo apposito (es. `Zona A - Centro storico`, `Zona B2`, `Zona agricola E`). Il dato è reperibile sul certificato di destinazione urbanistica o sul portale cartografico del Comune.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata nella ListBox.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Per selezionare più voci tieni premuto CTRL mentre clicchi.

---

## 3. Progettista delle opere architettoniche

Ogni figura professionale richiede quattro campi: **Cognome**, **Nome**, **PEC** e **Studio**. La PEC viene validata con regex: non è sufficiente la presenza del simbolo `@`, il formato deve essere corretto.

{: .note }
> Per tutte le sezioni professionisti (3, 4, 5, 6) è disponibile il pulsante **"Carica Soggetto"**: seleziona prima il tipo di soggetto, poi il soggetto dall'elenco, e clicca il pulsante per precompilare automaticamente cognome, nome, PEC e studio. In questo modo si evitano errori di digitazione sulla PEC.

---

### ATTENZIONE ! Inserire il cognome del progettista delle opere architettoniche.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"** della sezione **"Progettista delle opere architettoniche"**.

---

### ATTENZIONE ! Inserire il nome del progettista delle opere architettoniche.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione **"Progettista delle opere architettoniche"**.

---

### ATTENZIONE ! Inserire la PEC del progettista delle opere architettoniche.

**Soluzione**: Inserisci l'indirizzo PEC nel campo **"PEC"** della sezione **"Progettista delle opere architettoniche"**.

---

### ATTENZIONE ! PEC del progettista delle opere architettoniche non valida.

**Causa**: Il campo PEC contiene un valore ma non è un indirizzo email formalmente valido.

**Soluzione**:
1. Verifica che l'indirizzo contenga il simbolo `@` e un dominio (es. `mario.rossi@pec.it`) ✅
2. Non sono accettati: spazi, caratteri speciali non consentiti, domini senza punto (es. `mario.rossi@pec`) ❌
3. Usa il pulsante **"Carica Soggetto"** per importare la PEC dal registro soggetti ed evitare errori di digitazione

---

### ATTENZIONE ! Inserire lo studio del progettista delle opere architettoniche.

**Soluzione**: Inserisci l'indirizzo dello studio nel campo **"Con studio in"** della sezione **"Progettista delle opere architettoniche"**.

---

## 4. Direttore dei lavori architettonici

### ATTENZIONE ! Inserire il cognome del direttore dei lavori architettonici.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"** della sezione **"Direttore dei lavori architettonici"**.

---

### ATTENZIONE ! Inserire il nome del direttore dei lavori architettonici.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione **"Direttore dei lavori architettonici"**.

---

### ATTENZIONE ! Inserire la PEC del direttore dei lavori architettonici.

**Soluzione**: Inserisci l'indirizzo PEC nel campo **"PEC"** della sezione **"Direttore dei lavori architettonici"**.

---

### ATTENZIONE ! PEC del direttore dei lavori architettonici non valida.

**Causa**: Il campo PEC contiene un valore ma non è un indirizzo email formalmente valido.

**Soluzione**: Verifica il formato (es. `mario.rossi@pec.it` ✅) oppure usa **"Carica Soggetto"** per importarlo automaticamente.

---

### ATTENZIONE ! Inserire lo studio del direttore dei lavori architettonici.

**Soluzione**: Inserisci l'indirizzo dello studio nel campo **"Con studio in"** della sezione **"Direttore dei lavori architettonici"**.

---

## 5. Progettista delle strutture

### ATTENZIONE ! Inserire il cognome del progettista delle strutture.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"** della sezione **"Progettista delle strutture"**.

---

### ATTENZIONE ! Inserire il nome del progettista delle strutture.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione **"Progettista delle strutture"**.

---

### ATTENZIONE ! Inserire la PEC del progettista delle strutture.

**Soluzione**: Inserisci l'indirizzo PEC nel campo **"PEC"** della sezione **"Progettista delle strutture"**.

---

### ATTENZIONE ! PEC del progettista delle strutture non valida.

**Causa**: Il campo PEC contiene un valore ma non è un indirizzo email formalmente valido.

**Soluzione**: Verifica il formato (es. `mario.rossi@pec.it` ✅) oppure usa **"Carica Soggetto"** per importarlo automaticamente.

---

### ATTENZIONE ! Inserire lo studio del progettista delle strutture.

**Soluzione**: Inserisci l'indirizzo dello studio nel campo **"Con studio in"** della sezione **"Progettista delle strutture"**.

---

## 6. Direttore dei lavori strutturali

### ATTENZIONE ! Inserire il cognome del direttore dei lavori strutturali.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"** della sezione **"Direttore dei lavori strutturali"**.

---

### ATTENZIONE ! Inserire il nome del direttore dei lavori strutturali.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione **"Direttore dei lavori strutturali"**.

---

### ATTENZIONE ! Inserire la PEC del direttore dei lavori strutturali.

**Soluzione**: Inserisci l'indirizzo PEC nel campo **"PEC"** della sezione **"Direttore dei lavori strutturali"**.

---

### ATTENZIONE ! PEC del direttore dei lavori strutturali non valida.

**Causa**: Il campo PEC contiene un valore ma non è un indirizzo email formalmente valido.

**Soluzione**: Verifica il formato (es. `mario.rossi@pec.it` ✅) oppure usa **"Carica Soggetto"** per importarlo automaticamente.

---

### ATTENZIONE ! Inserire lo studio del direttore dei lavori strutturali.

**Soluzione**: Inserisci l'indirizzo dello studio nel campo **"Con studio in"** della sezione **"Direttore dei lavori strutturali"**.

---

## 7. Costruttore

Il costruttore richiede solo tre campi: **Cognome**, **Nome** e **Sede** (non PEC, a differenza dei professionisti).

---

### ATTENZIONE ! Inserire il cognome del costruttore.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"** della sezione **"Costruttore"**.

---

### ATTENZIONE ! Inserire il nome del costruttore.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione **"Costruttore"**.

---

### ATTENZIONE ! Inserire lo studio del costruttore.

**Dove si trova**: Sezione **"Costruttore"** → campo **"Con sede in"**

**Causa**: Non hai inserito la sede del costruttore.

**Soluzione**: Inserisci l'indirizzo della sede nel campo **"Con sede in"** della sezione **"Costruttore"**.

{: .note }
> Il messaggio di errore recita "studio" ma il campo nell'ASCX è etichettato **"Con sede in"**: si riferisce alla sede dell'impresa costruttrice, non allo studio professionale. È la stessa variabile `txtSedeCostruttore`. Il messaggio è tecnicamente impreciso ma il campo a cui si riferisce è inequivocabile.

---

## 8. Dichiarazioni — area soggetta e vincoli

Questa sezione contiene due blocchi di radio button con logica condizionale indipendente, più una checkbox opzionale che attiva ulteriori campi obbligatori.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Area soggetta ad intervento'.

**Dove si trova**: Sezione **"Dichiarazioni"** → primo blocco radio button

**Causa**: Non hai dichiarato se l'area è soggetta a strumento urbanistico esecutivo.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"Non è soggetta"** a strumento urbanistico esecutivo → nessun campo aggiuntivo
- ⚪ **"È soggetta"** a strumento urbanistico esecutivo → si attivano tre campi obbligatori (vedi sotto)

---

### ATTENZIONE ! Inserire lo strumento urbanistico esecutivo.

**Causa**: Hai selezionato "È soggetta" ma non hai indicato il tipo di strumento urbanistico.

**Soluzione**: Inserisci il tipo di strumento urbanistico esecutivo nel campo che si attiva accanto al radio button (es. `Piano Particolareggiato`, `Piano di Lottizzazione`, `Piano di Recupero`).

---

### ATTENZIONE ! Inserire il numero.

**Causa**: Hai selezionato "È soggetta" ma non hai inserito il numero della deliberazione comunale di approvazione dello strumento.

**Soluzione**: Inserisci il numero nel campo **"approvato con Deliberazione Comunale numero"**.

{: .note }
> Il messaggio "Inserire il numero" è generico e può riferirsi a due contesti distinti: il numero della delibera urbanistica (sezione "Area soggetta") oppure il numero di protocollo dei lavori già realizzati (sezione "Lavori già realizzati", checkbox `chkLavoriRealizzati`). Controlla quale delle due sezioni hai attivato e quale campo è rimasto vuoto.

---

### ATTENZIONE ! Inserire la data.

**Causa**: Hai selezionato "È soggetta" ma non hai inserito la data della deliberazione comunale, oppure hai spuntato "Lavori già realizzati" ma non hai inserito la data di protocollo.

**Soluzione**:
- Se stai compilando la sezione **"Area soggetta"**: inserisci la data nel campo **"del"** accanto al numero della delibera, nel formato GG/MM/AAAA
- Se stai compilando la sezione **"Lavori già realizzati"**: inserisci la data nel campo **"del"** accanto al numero di protocollo, nel formato GG/MM/AAAA

{: .warning }
> Il messaggio "Inserire la data" è identico per tre campi data distinti presenti nella sezione Dichiarazioni: la data dello strumento urbanistico, la data dell'autorizzazione al vincolo idrogeologico e la data del protocollo dei lavori realizzati. Se il messaggio compare inaspettatamente, scorrere tutta la sezione Dichiarazioni e verificare tutti i campi data attivati.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Area interessata ad intervento'.

**Dove si trova**: Sezione **"Dichiarazioni"** → secondo blocco radio button

**Causa**: Non hai dichiarato se l'area è sottoposta a vincolo idrogeologico.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"Non è sottoposta"** a vincolo idrogeologico → nessun campo aggiuntivo
- ⚪ **"È sottoposta"** a vincolo idrogeologico → si attivano due campi obbligatori (numero e data dell'autorizzazione L.R. 45/89)

---

### ATTENZIONE ! Inserire il numero. *(vincolo idrogeologico)*

**Causa**: Hai selezionato "È sottoposta" a vincolo idrogeologico ma non hai inserito il numero dell'autorizzazione.

**Soluzione**: Inserisci il numero dell'autorizzazione ai sensi della L.R. 45/89 nel campo **"Aut. n."**.

---

### ATTENZIONE ! Inserire la data. *(vincolo idrogeologico)*

**Causa**: Hai selezionato "È sottoposta" a vincolo idrogeologico ma non hai inserito la data dell'autorizzazione.

**Soluzione**: Inserisci la data dell'autorizzazione nel campo **"del"** accanto al numero, nel formato GG/MM/AAAA.

---

### Campi attivati dalla checkbox "Lavori già realizzati"

**Dove si trova**: Sezione **"Dichiarazioni"** → checkbox **"Informa infine che i lavori già realizzati sul fabbricato in oggetto... sono stati denunciati"**

Se spunti questa checkbox, diventano obbligatori tre campi aggiuntivi:

| Campo | Messaggio di errore se vuoto |
|---|---|
| `txtUfficio` — "all'ufficio" | `ATTENZIONE ! Inserire l'ufficio.` |
| `txtNumero` — "al prot." | `ATTENZIONE ! Inserire il numero.` |
| `txtData` — "del" (data protocollo) | `ATTENZIONE ! Inserire la data.` |

**Soluzione**: Compila i tre campi con l'ufficio destinatario, il numero di protocollo e la data della denuncia precedente.

---

## Consigli pratici Lavori in Abitati da Consolidare

### Prima di validare ✅

- [ ] Inserisci il **Comune** del provvedimento edilizio
- [ ] Seleziona la **tipologia intervento** (manutenzione straordinaria o restauro)
- [ ] Inserisci la **descrizione** dei lavori (max 300 caratteri)
- [ ] Inserisci gli **estremi** del titolo edilizio (DIA/SCIA/PDC/CIL/CILA)
- [ ] Inserisci il **numero** del titolo edilizio
- [ ] Inserisci la **data** del titolo edilizio (GG/MM/AAAA)
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Inserisci la **zona di PRGC**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Compila **Progettista architettonico**: cognome, nome, PEC valida, studio
- [ ] Compila **Direttore lavori architettonici**: cognome, nome, PEC valida, studio
- [ ] Compila **Progettista strutture**: cognome, nome, PEC valida, studio
- [ ] Compila **Direttore lavori strutturali**: cognome, nome, PEC valida, studio
- [ ] Compila **Costruttore**: cognome, nome, sede
- [ ] Seleziona **area soggetta a strumento urbanistico** (una delle 2 opzioni)
- [ ] Se "È soggetta": inserisci tipo strumento, numero e data delibera
- [ ] Seleziona **area interessata da vincolo idrogeologico** (una delle 2 opzioni)
- [ ] Se "È sottoposta": inserisci numero e data autorizzazione L.R. 45/89
- [ ] Se spunti **"Lavori già realizzati"**: inserisci ufficio, numero protocollo e data
- [ ] **Salva** frequentemente

### Messaggi ambigui: "Inserire il numero" e "Inserire la data" ⚠️

Questi due messaggi sono identici per contesti diversi. Se compaiono inaspettatamente:

| Messaggio | Possibile origine |
|---|---|
| "Inserire il numero" | Numero delibera strumento urbanistico **oppure** numero protocollo lavori realizzati |
| "Inserire la data" | Data delibera strumento urbanistico **oppure** data autorizzazione vincolo idrogeologico **oppure** data protocollo lavori realizzati |

Scorrere tutta la sezione **Dichiarazioni** e verificare tutti i campi attivati da radio button o checkbox.

### Validazione PEC: differenza tra campo vuoto e formato errato 🔍

| Situazione | Messaggio |
|---|---|
| Campo PEC vuoto | `ATTENZIONE ! Inserire la PEC del [ruolo].` |
| Campo PEC compilato ma formato non valido | `ATTENZIONE ! PEC del [ruolo] non valida.` |

Il secondo messaggio usa `SettaMessaggioErrore` (non `pValidaDati`): potrebbe apparire in posizione diversa nell'interfaccia rispetto agli altri errori. La validazione usa una regex email completa, non solo il controllo del simbolo `@`.

### Errori frequenti Lavori AC Piemonte 🔍

1. **Data titolo edilizio** → non c'è controllo formato in questa sezione: inserire comunque GG/MM/AAAA per coerenza
2. **PEC non valida** → usare "Carica Soggetto" per evitare errori di digitazione; il messaggio appare in modo diverso rispetto agli altri errori
3. **Costruttore: campo "studio"** → il messaggio recita "studio" ma il campo è "Con sede in": si tratta della sede dell'impresa, non dello studio professionale
4. **Messaggi "Inserire numero/data" doppi** → tre campi data e due campi numero nella sezione Dichiarazioni usano lo stesso messaggio: scorrere tutta la sezione
5. **Quattro professionisti tutti obbligatori** → tutti e quattro i blocchi (progettista arch., DL arch., progettista strutt., DL strutt.) sono sempre obbligatori, non condizionali

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
**Fonte**: Analisi codice `ValidaDatiAC` e `DatiAC.ascx`
