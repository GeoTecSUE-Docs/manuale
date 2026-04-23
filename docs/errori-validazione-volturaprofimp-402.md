---
title: Errori Voltura Professionisti / Imprese - Regione Piemonte
parent: Errori di validazione
nav_order: 20
description: Errori di validazione specifici per la Voltura Professionisti/Imprese (variazione tecnici e/o imprese) - Regione Piemonte
keywords: [voltura, variazione tecnici, variazione imprese, voltura professionisti, sicurezza lavoro, Titolo IV, notifica preliminare, errori voltura]
IDRegione: 2
IDTipoPratica: 402
Fonte: Manuale
---

# Errori di validazione - Voltura Professionisti / Imprese
## Regione Piemonte

Guida completa agli errori specifici per la **Voltura Professionisti / Imprese**, ovvero la comunicazione di variazione dei tecnici incaricati e/o delle imprese esecutrici rispetto a una pratica edilizia già presentata, relativa alla **Regione Piemonte**.

{: .note }
> La Voltura Professionisti/Imprese non è una nuova pratica edilizia autonoma, ma una **comunicazione di variazione** che fa riferimento a una pratica preesistente. Il modulo è strutturato in tre blocchi principali: la sezione "Variazione" (con le checkbox per indicare cosa cambia e i riferimenti alla pratica originaria), la localizzazione dell'immobile, e la sezione "Tutela della salute e della sicurezza" che include un'**anagrafica completa** del committente/responsabile dei lavori compilata direttamente nel modulo. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Variazione — checkbox e date](#1-variazione--checkbox-e-date)
2. [Pratica edilizia di riferimento](#2-pratica-edilizia-di-riferimento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Tutela della salute — anagrafica committente/responsabile](#4-tutela-della-salute--anagrafica-committenteresponsabile)
5. [Tutela della salute — dichiarazione Titolo IV D.Lgs. 81/2008](#5-tutela-della-salute--dichiarazione-titolo-iv-dlgs-812008)
6. [Soggetti coinvolti — tecnici e imprese](#6-soggetti-coinvolti--tecnici-e-imprese)

---

## 1. Variazione — checkbox e date

### ATTENZIONE ! Selezionare la variazione tecnico e/o impresa da effettuare.

**Dove si trova**: Sezione **"Variazione"** → due checkbox in cima al modulo

**Causa**: Non hai spuntato nessuna delle due checkbox che indicano il tipo di variazione da comunicare.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"che in data ___ sono variati i tecnici incaricati"** → inserisci la data di variazione e aggiorna i soggetti coinvolti
- ☐ **"che in data ___ sono variate le imprese"** → inserisci la data di variazione e aggiorna i soggetti coinvolti

{: .note }
> Puoi spuntare entrambe le checkbox se la variazione riguarda contemporaneamente sia i tecnici sia le imprese. Ogni checkbox ha un proprio campo data indipendente.

---

### ATTENZIONE ! Inserire la data di variazione.

**Dove si trova**: Campo data accanto alla checkbox spuntata (tecnici o imprese)

**Causa**: Hai spuntato una o entrambe le checkbox ma non hai inserito la data in cui è avvenuta (o avverrà) la variazione.

**Soluzione**:
1. Trova il campo data nella riga della checkbox spuntata
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `20/04/2026`)
4. Il campo si attiva automaticamente spuntando la checkbox
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il messaggio "Inserire la data di variazione" è lo stesso per entrambe le checkbox (tecnici e imprese). Se hai spuntato entrambe, il sistema controlla prima la data tecnici e poi la data imprese: il primo campo vuoto che trova produce l'errore.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data variazione)

**Causa**: La data di variazione (tecnici o imprese) è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `20/04/2026` ✅. Esempi errati: `20-04-2026` ❌, `2026/04/20` ❌.

---

## 2. Pratica edilizia di riferimento

I tre campi della pratica di riferimento (**Tipo pratica**, **Numero**, **Data**) sono normalmente pre-compilati dal sistema con i dati della pratica a cui la voltura si collega, e hanno `Enabled="false"` nell'ASCX. Il codice VB li verifica **solo se risultano abilitati** (`If txtTipoPratica.Enabled Then`). In condizioni normali questi errori non si presentano; possono comparire in casi particolari di configurazione o accesso diretto al modulo.

---

### ATTENZIONE ! Non è stato inserito il Tipo di Pratica.

**Dove si trova**: Campo **tipo pratica** nella sezione Variazione → riga "per la seguente pratica edilizia"

**Causa**: Il campo tipo pratica è abilitato ma vuoto.

**Soluzione**: Se il campo risulta modificabile, inserisci il tipo della pratica di riferimento (es. `SCIA`, `PdC`, `CILA`). In condizioni normali questo campo è pre-compilato automaticamente. Se è vuoto e non modificabile, contatta l'assistenza tecnica.

---

### ATTENZIONE ! Non è stato inserito il Numero di Pratica.

**Dove si trova**: Campo **numero** nella riga della pratica edilizia di riferimento

**Causa**: Il campo numero pratica è abilitato ma vuoto.

**Soluzione**: Inserisci il numero della pratica edilizia originaria. In condizioni normali è pre-compilato automaticamente.

---

### ATTENZIONE ! Non è stato inserita la data della Pratica.

**Dove si trova**: Campo **del** (data) nella riga della pratica edilizia di riferimento

**Causa**: Il campo data della pratica è abilitato ma vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica di riferimento)

**Causa**: La data della pratica di riferimento è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**.

---

## 3. Localizzazione dell'intervento

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

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (es. `15`, `22/A`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non hai inserito almeno un mappale catastale.

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione (se presente), Foglio, Mappale e Subalterno (solo fabbricati)
3. Clicca l'**icona ✅ verde** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Tutela della salute — anagrafica committente/responsabile

La sezione **"Tutela della salute e della sicurezza nei luoghi di lavoro (D.Lgs. 81/2008)"** contiene un'anagrafica completa del committente o responsabile dei lavori compilata direttamente nel modulo. Tutti i campi anagrafici sono obbligatori. Il ruolo si seleziona dal menu a discesa accanto al nome.

{: .note }
> Il modulo offre un pulsante **"Carica Soggetto"** che permette di importare i dati anagrafici da un soggetto già presente nella pratica (committente, responsabile dei lavori, ecc.), evitando di reinserirli manualmente. Usa questa funzione selezionando il tipo di soggetto e il soggetto, poi clicca "Carica Soggetto".

---

### ATTENZIONE ! Inserire il Cognome.

**Dove si trova**: Campo **"Cognome"** nella sezione Tutela della salute

**Causa**: Il campo cognome del committente/responsabile dei lavori è vuoto.

**Soluzione**: Inserisci il cognome nel campo **"Cognome"**, oppure usa il pulsante **"Carica Soggetto"** per importare i dati da un soggetto già presente.

---

### ATTENZIONE ! Inserire il Nome.

**Causa**: Il campo nome è vuoto.

**Soluzione**: Inserisci il nome nel campo **"Nome"**.

---

### ATTENZIONE ! Inserire la Città.

**Dove si trova**: Campo **"Città"** nella sezione Residenza della Tutela

**Causa**: Il campo città di residenza è vuoto.

**Soluzione**: Inserisci il comune di residenza (es. `Torino`, `Biella`).

---

### ATTENZIONE ! Inserire la Provincia.

**Causa**: Il campo provincia è vuoto.

**Soluzione**: Inserisci la sigla della provincia (es. `TO`, `BI`, `CN`).

---

### ATTENZIONE ! Inserire l'Indirizzo.

**Causa**: Il campo indirizzo di residenza è vuoto.

**Soluzione**: Inserisci l'indirizzo di residenza (es. `Via Roma`).

---

### ATTENZIONE ! Inserire il Civico.

**Causa**: Il campo civico è vuoto.

**Soluzione**: Inserisci il numero civico (es. `15`, `22/A`).

---

### ATTENZIONE ! Inserire il CAP.

**Dove si trova**: Campo **"CAP"** nella sezione Residenza della Tutela

**Causa**: Il CAP di residenza del committente/responsabile è vuoto.

**Soluzione**: Inserisci il CAP a **5 cifre** (es. `10121`).

{: .note }
> Attenzione: questo CAP si riferisce alla **residenza del committente/responsabile**, non alla localizzazione dell'intervento. Sono due campi distinti.

---

### ATTENZIONE ! Inserire la PEC/Posta Elettronica.

**Causa**: Il campo email/PEC è vuoto.

**Soluzione**: Inserisci l'indirizzo di posta elettronica o PEC del committente/responsabile (es. `mario.rossi@pec.it`).

---

### ATTENZIONE ! Inserire il Telefono fisso/Cellulare.

**Causa**: Il campo telefono è vuoto.

**Soluzione**: Inserisci il numero di telefono fisso o cellulare (es. `0115551234`, `3331234567`).

---

## 5. Tutela della salute — dichiarazione Titolo IV D.Lgs. 81/2008

Dopo l'anagrafica, il committente/responsabile deve dichiarare se il cantiere rientra nell'ambito del Titolo IV del D.Lgs. 81/2008. La struttura è più articolata rispetto ad altre pratiche: la notifica, se soggetta, richiede una scelta aggiuntiva tra allegare la notifica o indicarne gli estremi.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tutela della salute e della sicurezza nei luoghi di lavoro'.

**Causa**: Non hai dichiarato se l'intervento rientra nell'ambito del Titolo IV del D.Lgs. 81/2008.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"non ricade nell'ambito di applicazione del Titolo IV del d.lgs. n. 81/2008"**
- ⚪ **"ricade nell'ambito di applicazione del Titolo IV del d.lgs. n. 81/2008 e pertanto:"** → compila le sotto-opzioni

{: .note }
> La Voltura usa il **Titolo IV** del D.Lgs. 81/2008 come riferimento normativo, a differenza delle altre pratiche (CILA, SCIA, ecc.) che usano il generico D.Lgs. 81/2008. Il Titolo IV riguarda specificamente i cantieri temporanei o mobili.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato "ricade nel Titolo IV" ma non hai indicato l'entità del cantiere.

**Soluzione**: Seleziona una delle due sotto-opzioni:
- ⚪ **"entità presunta inferiore a 200 uomini-giorno"** e senza rischi particolari (allegato XI D.Lgs. 81/2008)
- ⚪ **"entità pari o superiore a 200 uomini-giorno"** o con rischi particolari

Consulta la tabella riepilogativa degli adempimenti presente nella sezione per orientarti nella scelta corretta.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato cantiere ≥ 200 uomini-giorno ma non hai dichiarato se è richiesta la notifica preliminare (art. 99 D.Lgs. 81/2008).

**Soluzione**: Seleziona:
- ⚪ **"l'intervento non è soggetto all'invio della notifica"**
- ⚪ **"l'intervento è soggetto all'invio della notifica e pertanto"** → seleziona poi come gestisci la notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione/Estremi Notifica'.

**Causa**: Hai dichiarato che la notifica è soggetta ma non hai indicato se la allegi o se ne fornisci gli estremi.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"allega alla presente comunicazione la notifica"** → il contenuto sarà esposto in cantiere su apposita tabella
- ⚪ **"indica gli estremi della notifica, già trasmessa in data ___ con prot./cod. ___"** → inserisci data e protocollo

{: .warning }
> Questa ulteriore scelta sulla notifica è specifica della Voltura Professionisti/Imprese e non è presente nelle altre pratiche (CILA, SCIA, ecc.), dove la gestione della notifica si ferma al livello precedente.

---

### ATTENZIONE ! Campo obbligatorio 'Data estremi notifica' non inserito.

**Dove si trova**: Campo data accanto a **"indica gli estremi della notifica, già trasmessa in data"**

**Causa**: Hai selezionato "indica gli estremi della notifica" ma non hai inserito la data di trasmissione della notifica già inviata.

**Soluzione**: Inserisci la data in cui la notifica è stata trasmessa nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Campo obbligatorio 'Prot. estremi notifica' non inserito.

**Dove si trova**: Campo **"con prot./cod."** accanto agli estremi della notifica

**Causa**: Data inserita ma protocollo/codice della notifica mancante.

**Soluzione**: Inserisci il numero di protocollo o codice assegnato alla notifica già trasmessa (es. `PROT-2024-12345`, `NP/2024/001`).

---

## 6. Soggetti coinvolti — tecnici e imprese

### ATTENZIONE ! Non è stato selezionato nessun tecnico.

**Dove si trova**: Sezione **"Soggetti coinvolti"** → Tecnici

**Causa**: Hai spuntato la checkbox **"sono variati i tecnici incaricati"** ma non hai aggiunto nessun tecnico tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Compila i dati del nuovo tecnico e seleziona il ruolo
4. Clicca l'**icona ✅** per salvare
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il controllo scatta solo se hai spuntato la checkbox tecnici. Se hai spuntato solo quella delle imprese, il controllo tecnici non viene eseguito. I soggetti coinvolti devono riflettere la situazione **dopo** la variazione.

---

### ATTENZIONE ! Non è stata selezionata nessun impresa.

**Dove si trova**: Sezione **"Soggetti coinvolti"** → Imprese

**Causa**: Hai spuntato la checkbox **"sono variate le imprese"** ma non hai aggiunto nessuna impresa tra i soggetti coinvolti.

**Soluzione**:
1. Vai a **"Soggetti coinvolti"** → sezione **"Imprese"**
2. Clicca **"Aggiungi Impresa"**
3. Compila i dati della nuova impresa
4. Clicca l'**icona ✅** per salvare
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Analogamente ai tecnici, il controllo imprese scatta solo se hai spuntato la relativa checkbox. Se stai comunicando solo la variazione dei tecnici senza variare l'impresa, non è necessario inserire alcuna impresa nei soggetti coinvolti.

---

## Consigli pratici Voltura Professionisti / Imprese

### Prima di validare ✅

- [ ] Spunta **almeno una** delle due checkbox (tecnici e/o imprese)
- [ ] Per ogni checkbox spuntata, inserisci la **data di variazione** nel formato GG/MM/AAAA
- [ ] Verifica che i campi **pratica di riferimento** (tipo, numero, data) siano compilati
- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** dell'intervento (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Nella sezione Tutela: usa **"Carica Soggetto"** per importare l'anagrafica se già presente
- [ ] Compila tutti i campi anagrafici obbligatori: **Cognome, Nome, Città, Provincia, Indirizzo, Civico, CAP, PEC/Email, Telefono**
- [ ] Seleziona la **dichiarazione Titolo IV** (ricade / non ricade)
- [ ] Se ricade: seleziona **documentazione imprese** e **notifica preliminare**
- [ ] Se notifica soggetta: scegli tra **"allega"** o **"indica gli estremi"** (con data e protocollo)
- [ ] Se checkbox tecnici spuntata: aggiungi **almeno un tecnico** in Soggetti coinvolti
- [ ] Se checkbox imprese spuntata: aggiungi **almeno un'impresa** in Soggetti coinvolti
- [ ] **Salva** frequentemente

### Caratteristiche peculiari della Voltura ⚠️

La Voltura Professionisti/Imprese ha alcune caratteristiche che la distinguono da tutte le altre pratiche della piattaforma.

I campi della pratica di riferimento (tipo, numero, data) sono normalmente pre-compilati dal sistema e non modificabili: il codice li verifica solo se sono abilitati, quindi in condizioni normali questi errori non si presentano.

La sezione sicurezza usa il riferimento normativo **"Titolo IV del D.Lgs. 81/2008"** invece del generico "D.Lgs. 81/2008": è la stessa normativa sui cantieri, ma il riferimento al Titolo IV è più preciso perché riguarda esplicitamente i cantieri temporanei o mobili.

La gestione della notifica ha un livello in più rispetto alle altre pratiche: se la notifica è soggetta, occorre scegliere tra allegarla direttamente o indicarne gli estremi (data + protocollo) di una notifica già trasmessa. Questo ulteriore livello (`$Allega`) non esiste nella CILA, SCIA o CIL.

### Errori frequenti Voltura 🔍

1. **Nessuna checkbox spuntata** → obbligatorio indicare cosa si sta variando (tecnici, imprese o entrambi)
2. **Data di variazione mancante dopo aver spuntato la checkbox** → il campo data si attiva solo dopo aver spuntato la checkbox; verificare che sia compilato
3. **Anagrafica committente/responsabile incompleta** → tutti i 9 campi (cognome, nome, città, provincia, indirizzo, civico, CAP, email, telefono) sono obbligatori; usare "Carica Soggetto" per velocizzare
4. **"Comunicazione/Estremi Notifica" non selezionata** → quarto livello del ramo sicurezza, specifico di questa pratica
5. **Data e/o protocollo estremi notifica mancanti** → obbligatori solo se si sceglie "indica gli estremi della notifica già trasmessa"
6. **Soggetti coinvolti non aggiornati** → se si spunta la checkbox tecnici/imprese, i soggetti coinvolti devono contenere almeno un elemento del tipo corrispondente

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
**Fonte**: Analisi codice ValidaDatiVolturaProfImp e DatiVolturaProfImp.ascx
