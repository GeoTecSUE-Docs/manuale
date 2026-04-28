---
title: Errori Denuncia Sismica Semplificata - Regione Piemonte
parent: Errori di validazione
nav_order: 28
description: Errori di validazione specifici per la Denuncia Sismica Semplificata (DSS) - Regione Piemonte (art. 93 D.P.R. 380/2001, D.M. 30/04/2020, D.G.R. n. 10-4161 del 26/11/2021)
keywords: [denuncia sismica semplificata, DSS, sismica, art. 93 DPR 380/2001, DGR 10-4161, professionista abilitato, relazione asseverazione, progettista strutturale, costruttore, zona PRG]
IDRegione: 2
IDTipoPratica: 18
Fonte: Manuale
---

# Errori di validazione - Denuncia Sismica Semplificata (DSS)
## Regione Piemonte

Guida completa agli errori specifici per la **Denuncia Sismica Semplificata** ai sensi dell'art. 93 del D.P.R. 6 giugno 2001, n. 380, del D.M. 30/04/2020 e della D.G.R. Piemonte n. 10-4161 del 26/11/2021, relativa alla **Regione Piemonte**.

{: .note }
> La Denuncia Sismica Semplificata (DSS) è strutturalmente diversa da tutte le altre pratiche. Non ha la sezione **Titolarità** (è una denuncia tecnica), né le sezioni **imprese esecutrici** nel senso ordinario né **sicurezza sul lavoro**. Include invece quattro schede professionista inline obbligatorie (**Progettista opere architettoniche, Direttore lavori architettonici, Progettista strutture, Direttore lavori strutturali**), una scheda **Costruttore** con i medesimi campi, e una sezione **Relazione di Asseverazione** con 12 campi dedicati al professionista abilitato strutturale, inclusa la verifica algoritmica del codice fiscale. La **Zona PRG vigente** e la **Zona PRG adottato** sono entrambe obbligatorie nella localizzazione. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Descrizione sintetica dell'intervento](#1-descrizione-sintetica-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Professionisti incaricati — 4 schede inline](#3-professionisti-incaricati--4-schede-inline)
4. [Costruttore](#4-costruttore)
5. [Data e firma del dichiarante](#5-data-e-firma-del-dichiarante)
6. [Relazione di Asseverazione — professionista strutturale](#6-relazione-di-asseverazione--professionista-strutturale)

---

## 1. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Prima sezione del modulo → campo di testo **"che i lavori per i quali viene inoltrata la presente consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere oggetto della denuncia sismica semplificata.

**Soluzione**:
1. Trova la sezione **"Descrizione sintetica dell'intervento"** in cima al modulo (prima della localizzazione)
2. Inserisci una descrizione chiara delle opere (max **300 caratteri**)
3. Esempi:
   - `Realizzazione di solaio in latero-cemento piano terra e primo piano di fabbricato residenziale bifamiliare.`
   - `Costruzione di muro di recinzione in c.a. con fondazione a platea su terreno in zona sismica 3.`
   - `Ristrutturazione edilizia con consolidamento strutturale di edificio esistente anni '60.`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 2. Localizzazione dell'intervento

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

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila i dati e salva con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

### ATTENZIONE ! Inserire la zona di PRG vigente.

**Dove si trova**: Campo **"Zona PRG vigente"** nella localizzazione, dopo i mappali

**Causa**: Non hai indicato la zona urbanistica del PRG vigente in cui si trova l'immobile.

**Soluzione**: Inserisci la zona del Piano Regolatore Generale vigente nel campo **"Zona PRG vigente"** (es. `B1`, `C2`, `E agricola`, `D produttiva`).

---

### ATTENZIONE ! Inserire la zona di PRG adottato.

**Dove si trova**: Campo **"Zona PRG adottato"** accanto alla Zona PRG vigente

**Causa**: Non hai indicato la zona urbanistica del PRG adottato (eventualmente diverso dal vigente).

**Soluzione**: Inserisci la zona del PRG adottato nel campo **"Zona PRG adottato"**. Se il PRG vigente e quello adottato coincidono, ripeti lo stesso valore (es. `B1`). Se non esiste un PRG adottato diverso da quello vigente, inserisci comunque il valore del vigente o la dicitura convenzionale usata dal Comune.

---

## 3. Professionisti incaricati — 4 schede inline

La DSS contiene **quattro schede professionista** compilate inline, ciascuna con gli stessi 7 campi obbligatori. Il sistema le valida in sequenza: prima tutti i campi del Professionista 1, poi del 2, poi del 3, poi del 4. I messaggi di errore sono identici per tutti e quattro, ma riguardano ruoli diversi.

Le quattro schede sono nell'ordine:
1. **Progettista delle opere architettoniche**
2. **Direttore dei lavori architettonici**
3. **Progettista delle strutture**
4. **Direttore dei lavori strutturali**

{: .note }
> Tutte e quattro le schede sono sempre obbligatorie. Non è possibile lasciarne vuota nessuna. Se per una DSS semplificata lo stesso professionista ricopre più ruoli, i suoi dati vanno ripetuti in ogni scheda corrispondente. Ogni scheda ha un pulsante **"Carica Soggetto"** che permette di importare automaticamente i dati da un soggetto già registrato nel sistema.

---

### ATTENZIONE ! Inserire il cognome del professionista.

**Dove si trova**: Campo **"Cognome"** nella scheda professionista corrente

**Causa**: Il campo Cognome è vuoto nella scheda del professionista che il sistema sta validando (1, 2, 3 o 4).

**Soluzione**: Inserisci il cognome del professionista nella scheda corrispondente, oppure usa il pulsante **"Carica Soggetto"** per importarlo automaticamente.

---

### ATTENZIONE ! Inserire il nome del professionista.

**Causa**: Il campo Nome è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci il nome del professionista, oppure usa **"Carica Soggetto"**.

---

### ATTENZIONE ! Inserire il codice fiscale del professionista.

**Causa**: Il campo Cod. Fiscale è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci il codice fiscale (16 caratteri) nella scheda corrispondente.

{: .note }
> Il codice fiscale dei 4 professionisti viene verificato solo per **presenza**, non per validità algoritmica. La verifica algoritmica del codice fiscale è applicata solo al professionista della Relazione di Asseverazione (sezione 6).

---

### ATTENZIONE ! Inserire la residenza del professionista.

**Causa**: Il campo **"con residenza di lavoro in"** (città) è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci la città di residenza professionale (studio/ufficio) del professionista nel campo **"con residenza di lavoro in"**.

---

### ATTENZIONE ! Inserire l'indirizzo del professionista.

**Causa**: Il campo **"via"** è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci la via dello studio/residenza professionale nel campo **"via"**.

---

### ATTENZIONE ! Inserire il numero civico del professionista.

**Causa**: Il campo **"n."** (numero civico) è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci il numero civico dello studio/residenza professionale nel campo **"n."**.

---

### ATTENZIONE ! Inserire il telefono del professionista.

**Causa**: Il campo **"tel. n"** è vuoto nella scheda del professionista corrente.

**Soluzione**: Inserisci il numero di telefono del professionista nel campo **"tel. n"** (es. `011 1234567`, `333 1234567`).

---

## 4. Costruttore

Il Costruttore è la quinta scheda anagrafica della DSS, strutturalmente identica alle quattro del professionista (stessi 7 campi: cognome, nome, CF, città lavoro, indirizzo, civico, telefono). I messaggi di errore hanno però testo differente ("del Costruttore" invece di "del professionista").

---

### ATTENZIONE ! Inserire il cognome del Costruttore.

**Dove si trova**: Sezione **"Costruttore"** → campo **"Cognome"**

**Causa**: Il cognome del Costruttore (o della persona fisica rappresentante dell'impresa) non è stato inserito.

**Soluzione**: Inserisci il cognome del titolare dell'impresa costruttrice nel campo **"Cognome"**, oppure usa il pulsante **"Carica Soggetto"**.

---

### ATTENZIONE ! Inserire il nome del Costruttore.

**Causa**: Il nome del Costruttore è mancante.

**Soluzione**: Inserisci il nome del titolare dell'impresa costruttrice.

---

### ATTENZIONE ! Inserire il codice fiscale del Costruttore.

**Causa**: Il codice fiscale del Costruttore è mancante.

**Soluzione**: Inserisci il codice fiscale del titolare (o della ragione sociale se persona giuridica) nel campo **"Cod. Fiscale"**.

---

### ATTENZIONE ! Inserire la residenza dell'impresa.

**Causa**: La città di residenza/sede dell'impresa costruttrice è mancante.

**Soluzione**: Inserisci la città della sede legale o operativa dell'impresa nel campo **"con residenza di lavoro in"**.

---

### ATTENZIONE ! Inserire l'indirizzo dell'impresa.

**Causa**: La via della sede dell'impresa è mancante.

**Soluzione**: Inserisci la via della sede dell'impresa costruttrice nel campo **"via"**.

---

### ATTENZIONE ! Inserire il numero civico dell'impresa.

**Causa**: Il numero civico della sede dell'impresa è mancante.

**Soluzione**: Inserisci il numero civico nel campo **"n."**.

---

### ATTENZIONE ! Inserire il telefono dell'impresa.

**Causa**: Il telefono dell'impresa costruttrice è mancante.

**Soluzione**: Inserisci il numero di telefono dell'impresa nel campo **"tel. n"**.

---

## 5. Data e firma del dichiarante

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Campo **"data"** dopo la sezione Costruttore, prima della Relazione di Asseverazione

**Causa**: Non hai inserito la data della dichiarazione.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `28/04/2026`). Il sistema verifica il formato: assicurati di usare il separatore `/` e l'anno a 4 cifre.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data inserita è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `28/04/2026` ✅. Errati: `28-04-2026` ❌, `28/04/26` ❌.

{: .note }
> La data della dichiarazione è l'**unico campo con verifica del formato data** in tutta la DSS. Gli altri campi data eventualmente presenti nel modulo non vengono controllati.

---

### ATTENZIONE ! Inserire la firma del dichiarante.

**Dove si trova**: Campo **"firma"** accanto alla data

**Causa**: Il campo firma del dichiarante (titolare della denuncia) è vuoto.

**Soluzione**: Inserisci il nome e cognome o la sigla del dichiarante nel campo **"firma"** (es. `Mario Rossi`, `M.R.`).

---

## 6. Relazione di Asseverazione — professionista strutturale

La **Relazione di Asseverazione** è la sezione finale della DSS, compilata dal professionista abilitato in qualità di progettista strutturale. Contiene 12 campi, tutti obbligatori. Il codice fiscale è l'unico soggetto a verifica algoritmica completa.

{: .note }
> I campi della Relazione di Asseverazione sono **distinti e separati** dai 4 professionisti inline sopra. Anche se il Progettista delle strutture (scheda 3) e il professionista della Relazione di Asseverazione sono spesso la stessa persona, i campi devono essere compilati due volte separatamente.

---

### ATTENZIONE ! Inserire il cognome del professionista abilitato.

**Dove si trova**: Sezione **"RELAZIONE DI ASSEVERAZIONE"** → campo **"Cognome"**

**Causa**: Il cognome del professionista abilitato (progettista strutturale asseverante) è mancante.

**Soluzione**: Inserisci il cognome del professionista abilitato nel campo **"Cognome"** della sezione Relazione di Asseverazione.

---

### ATTENZIONE ! Inserire il nome del professionista abilitato.

**Causa**: Il nome del professionista abilitato è mancante.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della sezione Relazione di Asseverazione.

---

### ATTENZIONE ! Inserire l'Ordine professionale del professionista abilitato.

**Dove si trova**: Campo **"iscritto all'Ordine professionale della Provincia di"**

**Causa**: La Provincia dell'Ordine professionale non è stata inserita.

**Soluzione**: Inserisci la provincia dell'Ordine/Collegio professionale di appartenenza del professionista (es. `Torino`, `Cuneo`, `Milano`).

---

### ATTENZIONE ! Inserire il numero dell'Ordine professionale del professionista abilitato.

**Dove si trova**: Campo **"al num."** accanto alla Provincia dell'Ordine

**Causa**: Il numero di iscrizione all'Ordine professionale non è stato inserito.

**Soluzione**: Inserisci il numero di iscrizione all'Ordine nel campo **"al num."** (es. `A-1234`, `5678`).

---

### ATTENZIONE ! Inserire la città dello studio del professionista abilitato.

**Dove si trova**: Campo **"con studio in"**

**Causa**: La città dello studio professionale è mancante.

**Soluzione**: Inserisci la città in cui si trova lo studio del professionista nel campo **"con studio in"** (es. `Torino`, `Cuneo`).

---

### ATTENZIONE ! Inserire la via dello studio del professionista abilitato.

**Causa**: La via dello studio professionale è mancante.

**Soluzione**: Inserisci la via dello studio nel campo **"Via"** (es. `Via Roma`, `Corso Vittorio Emanuele`).

---

### ATTENZIONE ! Inserire il numero civico dello studio del professionista abilitato.

**Causa**: Il numero civico dello studio professionale è mancante.

**Soluzione**: Inserisci il numero civico dello studio nel campo **"n."**.

---

### ATTENZIONE ! Inserire il codice fiscale dello studio del professionista abilitato.

**Dove si trova**: Campo **"codice fiscale"** nella Relazione di Asseverazione

**Causa**: Il codice fiscale del professionista abilitato non è stato inserito.

**Soluzione**: Inserisci il codice fiscale personale (16 caratteri) del professionista abilitato nel campo **"codice fiscale"**.

---

### ATTENZIONE ! Codice fiscale dello studio del professionista abilitato non valido.

**Causa**: Il codice fiscale è stato inserito ma non supera la verifica algoritmica del formato (checksum).

**Soluzione**:
1. Verifica che il codice fiscale sia esattamente **16 caratteri** (6 lettere + 2 cifre + 1 lettera + 2 cifre + 1 lettera + 3 cifre + 1 lettera)
2. Controlla che non ci siano spazi, trattini o altri caratteri estranei
3. Verifica la correttezza del codice su un calcolatore del codice fiscale prima di inserirlo
4. Se il codice è corretto ma continua a dare errore, contatta [Assistenza](assistenza-tecnica.html)

{: .note }
> Questo è l'**unico campo di tutta la DSS** soggetto a verifica algoritmica del codice fiscale. Il sistema usa la funzione `clsModuloAsp.CheckCodiceFiscale()` che verifica il checksum secondo le regole del Ministero dell'Economia. I codici fiscali delle persone fisiche devono rispettare l'algoritmo standard; non sono accettati codici fiscali di persone giuridiche (partite IVA o codici numerici a 11 cifre).

---

### ATTENZIONE ! Inserire il numero di telefono dello studio del professionista abilitato.

**Causa**: Il telefono del professionista abilitato è mancante.

**Soluzione**: Inserisci il numero di telefono nel campo **"recapito telefonico"** (es. `011 1234567`, `333 1234567`).

---

### ATTENZIONE ! Inserire l'e-mail del professionista abilitato.

**Causa**: L'indirizzo email del professionista abilitato è mancante.

**Soluzione**: Inserisci l'indirizzo email nel campo **"e-mail"** (es. `mario.rossi@studio.it`).

---

### ATTENZIONE ! Inserire la PEC del professionista abilitato.

**Causa**: L'indirizzo PEC del professionista abilitato è mancante.

**Soluzione**: Inserisci l'indirizzo PEC nel campo **"PEC"** (es. `mario.rossi@ingpec.eu`). La PEC è obbligatoria separatamente dall'email ordinaria.

---

### ATTENZIONE ! Inserire la descrizione dell'opera.

**Dove si trova**: Campo di testo **"che l'opera/intervento costituito da"** nella sezione Relazione di Asseverazione

**Causa**: Non hai descritto l'opera o l'intervento strutturale nella Relazione di Asseverazione.

**Soluzione**: Inserisci la descrizione dell'opera strutturale nel campo di testo (es. `Solaio in latero-cemento spessore 20+4 di circa 150 mq`, `Muro in c.a. fondato su platea spessore 40 cm`). Questo campo è distinto dalla descrizione sintetica dell'intervento nella sezione 1.

---

## Consigli pratici Denuncia Sismica Semplificata

### Prima di validare ✅

- [ ] Inserisci la **descrizione dell'intervento** (max 300 caratteri)
- [ ] Seleziona l'**indirizzo** della località, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **Zona PRG vigente**
- [ ] Inserisci la **Zona PRG adottato**
- [ ] Compila tutti e 7 i campi della scheda **Progettista opere architettoniche** (cognome, nome, CF, città lavoro, via, civico, tel.)
- [ ] Compila tutti e 7 i campi della scheda **Direttore lavori architettonici**
- [ ] Compila tutti e 7 i campi della scheda **Progettista delle strutture**
- [ ] Compila tutti e 7 i campi della scheda **Direttore dei lavori strutturali**
- [ ] Compila tutti e 7 i campi della scheda **Costruttore** (cognome, nome, CF, città, via, civico, tel.)
- [ ] Inserisci la **data** nel formato GG/MM/AAAA (con verifica formato)
- [ ] Inserisci la **firma del dichiarante**
- [ ] Compila la sezione **Relazione di Asseverazione**: cognome, nome, ordine (provincia), n. ordine, città studio, via, civico, **CF con verifica algoritmica**, telefono, email, PEC, opera
- [ ] **Salva** frequentemente

### Strategia "Carica Soggetto" per accelerare la compilazione ⚡

Ogni scheda professionista e la scheda Costruttore hanno il pulsante **"Carica Soggetto"** che permette di importare automaticamente tutti i dati anagrafici da un soggetto già presente in anagrafica. Per usarlo: seleziona il tipo di soggetto (persona fisica/giuridica), poi il nominativo dal secondo menu, poi clicca "Carica Soggetto". Tutti e 7 i campi della scheda si compilano automaticamente.

### Differenze principali DSS rispetto alla Denuncia Sismica ordinaria ⚠️

La DSS (tipo istanza 18) è completamente diversa dalla Denuncia Sismica ordinaria (tipo istanza 6 o 7 a seconda della variante). La DSS ha 4 professionisti inline + 1 costruttore inline come parte del modulo istanza, mentre la DS ordinaria usa i soggetti coinvolti standard. La DSS include la **Relazione di Asseverazione** integrata nel modulo con 12 campi specifici. La DSS ha la **Zona PRG** obbligatoria nella localizzazione. La DSS fa riferimento alla **D.G.R. n. 10-4161 del 26/11/2021** (denuncia semplificata), la DS ordinaria all'art. 93 senza il regime semplificato.

### Errori frequenti DSS 🔍

1. **Zona PRG vigente o adottato vuota** → campi dopo i mappali, spesso non visti perché il form scorre verso il basso
2. **Una delle 4 schede professionista con un campo mancante** → il sistema valida in sequenza: se la scheda 1 è completa e la 2 ha il telefono mancante, l'errore compare solo dopo aver compilato la 1
3. **Codice fiscale del professionista della Relazione di Asseverazione non valido** → unico campo con verifica algoritmica; un carattere errato (spazio incluso) causa il fallimento
4. **PEC e email della Relazione di Asseverazione entrambe obbligatorie** → non è sufficiente compilare solo l'email; la PEC è un campo separato e indipendente
5. **Opera/intervento nella Relazione di Asseverazione non compilata** → campo distinto dalla descrizione iniziale dell'intervento; il modulo è lungo e questo campo è quasi in fondo
6. **Firma del dichiarante dimenticata** → campo accanto alla data, spesso ignorato

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
**Fonte**: Analisi codice ValidaDatiDSS e DatiDSS.ascx
