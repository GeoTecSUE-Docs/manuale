---
title: Errori Variante Lavori Zona Sismica - Regione Piemonte
parent: Errori di validazione
nav_order: 39
description: Errori di validazione specifici per la Variante Lavori in Zona Sismica - Regione Piemonte (art. 93-94 D.P.R. 380/2001)
keywords: [variante lavori zona sismica, denuncia sismica, variante sismica, Piemonte, art. 93 DPR 380/2001, art. 94 DPR 380/2001, zona sismica, 4 professionisti, costruttore, strumento urbanistico esecutivo, vincolo idrogeologico, referente PA, titolo abilitativo, procedimento edilizio, collaudo, collaudatore]
IDRegione: 2
IDTipoPratica: 60
Fonte: Manuale
---

# Errori di validazione - Variante Lavori Zona Sismica
## Regione Piemonte

Guida completa agli errori specifici per la **Variante Lavori in Zona Sismica** ai sensi degli artt. 93–94 del D.P.R. 6 giugno 2001, n. 380, relativa alla **Regione Piemonte**.

{: .note }
> La Variante Lavori Zona Sismica è una delle pratiche più articolate della piattaforma. A differenza delle altre pratiche, le schede dei **4 professionisti** (Progettista opere architettoniche, Direttore lavori architettonici, Progettista strutture, Direttore lavori strutturali) e del **Costruttore** sono **integrate direttamente nel modulo** come campi inline — non si usano i soggetti coinvolti della sezione tecnici. Il numero e la data della pratica originale di denuncia lavori sono **condizionali** (abilitati solo se la pratica è collegata a una denuncia precedente). Le sezioni "Strumento Urbanistico Esecutivo" e "Vincolo Idrogeologico" hanno campi che diventano obbligatori in base al radio button selezionato. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Descrizione sintetica dell'intervento](#1-descrizione-sintetica-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Titolare del procedimento edilizio/titolo abilitativo in corso di validità](#3-titolare-del-procedimento-ediliziotitolo-abilitativo-in-corso-di-validità)
4. [Denuncia — Ente, pratica originale e tipo intervento](#4-denuncia--ente-pratica-originale-e-tipo-intervento)
5. [I quattro professionisti](#5-i-quattro-professionisti)
6. [Costruttore](#6-costruttore)
7. [Referente per i rapporti con la pubblica amministrazione](#7-referente-per-i-rapporti-con-la-pubblica-amministrazione)
8. [Strumento urbanistico esecutivo](#8-strumento-urbanistico-esecutivo)
9. [Vincolo idrogeologico](#9-vincolo-idrogeologico)
10. [Denuncia lavori precedente (punto c)](#10-denuncia-lavori-precedente-punto-c)
11. [Collaudo delle opere (punto e)](#11-collaudo-delle-opere-punto-e)
12. [Data, firma dichiarante e firma costruttore](#12-data-firma-dichiarante-e-firma-costruttore)
13. [Dichiarazione di conformità](#13-dichiarazione-di-conformità)

---

## 1. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Causa**: Il campo descrizione è vuoto.

**Soluzione**: Inserisci la descrizione dei lavori nel campo multiriga "che i lavori per i quali viene inoltrata la presente consistono in:" (max **300 caratteri**).

{: .note }
> Nella stessa sezione è presente il menu a discesa **Zona Sismica** (valori: 3, 3S, 4). Questo campo **non è validato** dal codice — non genera errori se rimane sul valore di default — ma è importante selezionare la zona corretta per la correttezza del procedimento.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato "Toponimo mancante" ma non hai compilato il campo testo.

**Soluzione**: Inserisci il toponimo nel campo di testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure spunta "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

{: .note }
> La sezione localizzazione include anche i campi **"Zona PRG vigente"** e **"Classe di sintesi della pericolosità geomorfologica"**: entrambi sono contrassegnati come campi obbligatori nel modulo ma **non sono validati** dal codice. Non generano errori se vuoti, ma è corretto compilarli.

---

## 3. Titolare del procedimento edilizio/titolo abilitativo in corso di validità

Subito dopo la sezione "Localizzazione dell'intervento" il modulo richiede gli estremi del procedimento edilizio/titolo abilitativo attualmente in corso di validità sull'immobile (es. PdC, SCIA, Delibera GC...). I tre campi sono compilati inline in questa sezione.

---

### ATTENZIONE ! Campo obbligatorio 'Procedimento Edilizio/Titolo abilitativo' non inserito.

**Dove si trova**: Campo nel testo "Procedimento edilizio/titolo abilitativo (PdC, SCIA, Delibera GC...)"

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la tipologia del procedimento edilizio/titolo abilitativo in corso di validità (es. `PdC`, `SCIA`, `Delibera GC`).

---

### ATTENZIONE ! Campo obbligatorio 'N. Procedimento abilitativo' non inserito.

**Dove si trova**: Campo "N. Procedimento abilitativo"

**Causa**: Il numero del procedimento abilitativo è vuoto.

**Soluzione**: Inserisci il numero del procedimento/titolo abilitativo.

---

### ATTENZIONE ! Campo obbligatorio 'Data' (del procediemento edilizio) non inserito.

**Dove si trova**: Campo "Data" accanto al procedimento edilizio/titolo abilitativo

**Causa**: Il campo data è attivo ma non compilato.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** con il datepicker associato.

{: .note }
> Il campo data del procedimento edilizio è **condizionale**: viene validato solo se risulta abilitato. Se il sistema lo mostra disabilitato (grigio), non è richiesto in questa pratica specifica.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (procedimento edilizio)

**Causa**: La data inserita per il procedimento edilizio/titolo abilitativo non è nel formato corretto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/03/2022`).

---

## 4. Denuncia — Ente, pratica originale e tipo intervento

### ATTENZIONE ! Campo obbligatorio 'Ente/Regione' non inserito.

**Dove si trova**: Sezione "DENUNCIA" → campo testo nel testo "a codesto Ufficio... di voler procedere alla variante dei lavori già denunciati a ___"

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci il nome dell'Ente/Regione a cui è stata presentata la denuncia originale (es. `Regione Piemonte`, `Provincia di Torino`).

---

### ATTENZIONE ! Campo obbligatorio 'Numero Pratica' non inserito.

**Dove si trova**: Campo nel testo "(Prot n. ___)" della sezione DENUNCIA

**Causa**: Il campo numero pratica è attivo ma non compilato.

**Soluzione**: Inserisci il numero di protocollo della denuncia originale.

{: .note }
> Questo campo è condizionale: viene validato **solo se risulta attivo**. Se il sistema lo mostra disabilitato (grigio), non è richiesto in questa pratica specifica.

---

### ATTENZIONE ! Campo obbligatorio 'Data Pratica' non inserito.

**Causa**: Il campo data pratica originale è abilitato ma non compilato.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** nel campo "del" accanto al numero pratica.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica)

**Causa**: La data inserita per la pratica originale non è nel formato corretto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/03/2022`).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Intervento'.

**Dove si trova**: Sezione DENUNCIA → 3 radio button sotto i dati della pratica originale

**Causa**: Non hai selezionato il tipo di procedura sismica applicabile.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **"l'intervento è sottoposto a denuncia e autorizzazione preventiva (artt. 93 e 94 D.P.R. 380/2001)"**
- ⚪ **"l'intervento è sottoposto a denuncia e controllo a campione (art. 93 D.P.R. 380/2001)"**
- ⚪ **"l'intervento è sottoposto a denuncia (art. 93 D.P.R. 380/2001)"**

{: .note }
> La distinzione tra le tre opzioni dipende dalla zona sismica e dal tipo di costruzione: la denuncia con autorizzazione preventiva (artt. 93-94) è obbligatoria nelle zone sismiche 1 e 2; il controllo a campione si applica in zone 3 e 3S; la sola denuncia riguarda la zona 4. Verifica con il tecnico strutturista quale opzione è applicabile.

---

## 5. I quattro professionisti

Il modulo contiene **quattro schede professionisti** compilate inline (non tramite soggetti coinvolti). Per ciascuna scheda il validatore controlla gli stessi tre campi obbligatori, nell'ordine: **Cognome**, **Nome**, **Cod. Fiscale**.

Le quattro schede sono:
- **Scheda 1** — Progettista delle opere architettoniche
- **Scheda 2** — Direttore dei lavori architettonici
- **Scheda 3** — Progettista delle strutture
- **Scheda 4** — Direttore dei lavori strutturali

---

### ATTENZIONE ! Inserire il cognome del professionista.

**Causa**: Il campo cognome di una delle quattro schede professionisti è vuoto.

**Soluzione**: Scorri il modulo fino alla scheda corrispondente e inserisci il **cognome** del professionista nel campo "Cognome". Controlla tutte e quattro le schede: il messaggio appare per la prima scheda incompleta trovata nell'ordine 1→4.

---

### ATTENZIONE ! Inserire il nome del professionista.

**Causa**: Il campo nome di una delle quattro schede è vuoto.

**Soluzione**: Inserisci il **nome** del professionista nella scheda incompleta.

---

### ATTENZIONE ! Inserire il codice fiscale del professionista.

**Causa**: Il campo codice fiscale di una delle quattro schede è vuoto.

**Soluzione**: Inserisci il **codice fiscale** (16 caratteri) del professionista nella scheda incompleta.

{: .note }
> Ogni scheda ha un selettore di caricamento rapido ("Seleziona il tipo di soggetto" + "Seleziona il soggetto" + pulsante "Carica Soggetto") che permette di pre-compilare i campi da un soggetto già presente in anagrafica. Una volta caricato il soggetto, verifica che i campi cognome, nome e CF siano effettivamente compilati prima di procedere. Gli altri campi di ogni scheda (residenza di lavoro, via, n. civico, tel.) non sono validati dal codice.

---

## 6. Costruttore

Anche il Costruttore è compilato inline nel modulo (non tramite soggetti coinvolti). È prevista **una sola impresa costruttrice**.

---

### ATTENZIONE ! Inserire il cognome del Costruttore.

**Causa**: Il campo Cognome è vuoto.

**Soluzione**: Scorri fino alla sezione **"Costruttore"** e inserisci il cognome (o la ragione sociale per persone giuridiche) nel campo "Cognome".

---

### ATTENZIONE ! Inserire il nome del Costruttore.

**Causa**: Il campo Nome è vuoto.

**Soluzione**: Inserisci il nome nel campo "Nome" della sezione Costruttore.

---

### ATTENZIONE ! Inserire il codice fiscale del Costruttore.

**Causa**: Il campo Cod. Fiscale è vuoto.

**Soluzione**: Inserisci il codice fiscale (o partita IVA per soggetti giuridici) nel campo "Cod. Fiscale" della sezione Costruttore.

---

## 7. Referente per i rapporti con la pubblica amministrazione

### ATTENZIONE ! Referente per i rapporti con pubblica amministrazione non indicato.

**Dove si trova**: Menu a discesa nel testo "designando tra di essi il ___ quale referente, per i rapporti con la pubblica amministrazione"

**Causa**: Il menu è rimasto sull'opzione vuota iniziale.

**Soluzione**: Seleziona dal menu **uno dei due ruoli**:
- **Progettista delle opere architettoniche**
- **Progettista delle strutture**

Il referente designato deve corrispondere a uno dei professionisti compilati nelle schede della sezione d).

---

## 8. Strumento urbanistico esecutivo

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Strumento Urbanistico Esecutivo'.

**Dove si trova**: Sezione dichiarazioni → punto a) "l'area oggetto dell'atto di assenso ___ soggetta a strumento urbanistico esecutivo"

**Causa**: Non hai selezionato né "è" né "non è".

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"è"** → l'area è soggetta a SUE → compilare obbligatoriamente i 3 campi aggiuntivi
- ⚪ **"non è"** → l'area non è soggetta a SUE → nessun campo aggiuntivo richiesto

---

### ATTENZIONE ! Inserire descrizione Strumento Urbanistico Esecutivo.

**Causa**: Hai selezionato "è" ma non hai inserito la descrizione del tipo di strumento urbanistico.

**Soluzione**: Inserisci nel campo di testo la descrizione dello strumento (es. `Piano Particolareggiato`, `Piano di Lottizzazione`, `Piano di Recupero`).

---

### ATTENZIONE ! Inserire il numero della deliberazione comunale.

**Causa**: Hai selezionato "è" ma non hai inserito il numero della delibera comunale di approvazione.

**Soluzione**: Inserisci il numero nel campo "approvato con Deliberazione Comunale n ___" (es. `45`, `123/2020`).

---

### ATTENZIONE ! Inserire la data della deliberazione comunale.

**Causa**: Hai selezionato "è" ma non hai inserito la data della delibera.

**Soluzione**: Inserisci la data nel campo "del" accanto al numero della delibera, nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (strumento urbanistico)

**Causa**: La data della delibera non è nel formato corretto.

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA**.

---

## 9. Vincolo idrogeologico

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Vincolo Idrogeologico'.

**Dove si trova**: Sezione dichiarazioni → punto b) "l'area interessata ___ sottoposta a vincolo idrogeologico"

**Causa**: Non hai selezionato né "è" né "non è".

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"è"** → l'area è soggetta a vincolo idrogeologico → compilare obbligatoriamente i 3 campi dell'autorizzazione
- ⚪ **"non è"** → l'area non è soggetta a vincolo idrogeologico → nessun campo aggiuntivo

---

### ATTENZIONE ! Inserire descrizione dell'Ente rilasciante Autorizzazione.

**Causa**: Hai selezionato "è" ma non hai indicato l'ente che ha rilasciato l'autorizzazione idrogeologica.

**Soluzione**: Inserisci nel campo di testo il nome dell'ente (es. `Regione Piemonte - Settore Difesa del Suolo`).

---

### ATTENZIONE ! Inserire il numero di protocollo dell'Autorizzazione.

**Causa**: Hai selezionato "è" ma non hai inserito il numero di protocollo dell'autorizzazione.

**Soluzione**: Inserisci il numero nel campo "(Prot n. ___)" (es. `1234/2023`).

---

### ATTENZIONE ! Inserire la data di protocollo dell'Autorizzazione.

**Causa**: Hai selezionato "è" ma non hai inserito la data dell'autorizzazione.

**Soluzione**: Inserisci la data nel campo "del" accanto al numero di protocollo, nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (vincolo idrogeologico)

**Causa**: La data dell'autorizzazione idrogeologica non è nel formato corretto.

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA**.

---

## 10. Denuncia lavori precedente (punto c)

Il punto c) "i lavori già realizzati sul fabbricato... sono stati denunciati a" contiene tre campi (ente, numero di protocollo e data della denuncia precedente) che nel codice originale erano tutti validati come obbligatori ma sono stati **resi facoltativi** nella versione attuale. L'unico controllo rimasto attivo è la **verifica del formato della data**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (denuncia lavori precedente)

**Dove si trova**: Sezione dichiarazioni → punto c) → campo data

**Causa**: Hai inserito una data nel campo "del" della denuncia lavori precedente ma il formato non è corretto.

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA** oppure svuota il campo se non è rilevante.

{: .note }
> Il punto c) è l'unico in cui i campi ente, numero protocollo e data **non sono obbligatori** (il codice di validazione è commentato). Tuttavia la data, se inserita, viene sempre verificata nel formato. Se il fabbricato non ha denunce precedenti, è possibile lasciare il campo vuoto.

---

## 11. Collaudo delle opere (punto e)

Il punto e) "con riferimento al collaudo delle opere" richiede la selezione di una delle tre opzioni relative al collaudo. Se si seleziona la terza opzione, diventa a sua volta obbligatoria la scelta tra le tre sotto-opzioni relative alla nomina del collaudatore.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce in riferimento al collaudo delle opere.

**Dove si trova**: Sezione dichiarazioni → punto e) "con riferimento al collaudo delle opere"

**Causa**: Non hai selezionato nessuna delle tre opzioni sul collaudo.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **"che la presente denuncia non necessita di nomina del collaudatore in quanto rientra nel campo di applicazione dell'art. 67 - comma 8 bis - D.P.R. n. 380/2001 (intervento locale) e pertanto depositerà la dichiarazione di regolare esecuzione (DRE) resa dal direttore lavori strutturale"**
- ⚪ **"che la presente denuncia non necessita di nuova nomina del collaudatore in quanto è ancora valida e conforme la nomina già depositata con la denuncia originaria"**
- ⚪ **"che la presente denuncia necessita di nomina del collaudatore"** → se selezionata, compilare obbligatoriamente anche il blocco "nomina del collaudatore" sottostante

---

### ATTENZIONE ! Non è stata selezionata nessuna voce in riferimento alla nomina del collaudatore.

**Dove si trova**: Sotto-opzioni visibili solo se è selezionata la terza voce ("...necessita di nomina del collaudatore")

**Causa**: Hai selezionato "necessita di nomina del collaudatore" ma non hai indicato le modalità di nomina.

**Soluzione**: Seleziona **una delle tre sotto-opzioni**:
- ⚪ **"e allega la dichiarazione di nomina e accettazione del collaudatore (Dichiarazione di accettazione e nomina del collaudatore)"**
- ⚪ **"e dichiara che il collaudatore verrà scelto tra una terna di professionisti indicati dall'Ordine degli Ingegneri/Architetti in base a richiesta già inoltrata al detto Ordine"**
- ⚪ **"e che l'intervento in progetto è riconducibile ad opera pubblica..."** (nomina rimandata alla presentazione della copia dell'atto di approvazione del progetto esecutivo e degli estremi dell'aggiudicatario dei lavori)

{: .note }
> Questa sotto-scelta è **condizionale**: viene richiesta dal validatore solo quando è selezionato il terzo radio button relativo al collaudo delle opere. Se scegli la prima o la seconda opzione, il blocco "nomina del collaudatore" non viene validato.

---

## 12. Data, firma dichiarante e firma costruttore

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Riga "data / firma" sotto le dichiarazioni → campo "data"

**Causa**: Il campo data del dichiarante è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** nel campo "data" in fondo alla sezione DENUNCIA.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data dichiarante)

**Causa**: La data inserita non è nel formato corretto.

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la firma del dichiarante.

**Dove si trova**: Riga "data / firma" → campo "firma"

**Causa**: Il campo firma del dichiarante è vuoto.

**Soluzione**: Inserisci il nominativo del dichiarante nel campo "firma".

---

### ATTENZIONE ! Inserire la firma del Costruttore.

**Dove si trova**: Riga separata sotto la firma del dichiarante → campo "firma", nel testo "Firma del Costruttore per opere disciplinate dal D.P.R. n. 380 del 6/06/2001 art. 65"

**Causa**: Il campo firma del costruttore è vuoto.

**Soluzione**: Inserisci il nominativo del costruttore nel campo firma.

---

## 13. Dichiarazione di conformità

### ATTENZIONE ! Inserire il nominativo del sottoscritto.

**Dove si trova**: Sezione "DICHIARAZIONE DI CONFORMITA'" → campo nel testo "Il sottoscritto ___"

**Causa**: Il campo nome del dichiarante è vuoto.

**Soluzione**: Inserisci il nominativo del progettista che sottoscrive la dichiarazione di conformità.

---

### ATTENZIONE ! Tipo di progettista non indicato.

**Causa**: Il menu "in qualità di progettista" è rimasto sull'opzione vuota.

**Soluzione**: Seleziona **uno dei due ruoli** dal menu:
- **Progettista delle opere architettoniche**
- **Progettista delle strutture**

Il ruolo selezionato deve corrispondere al professionista indicato come sottoscritto.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolo Abitativo'.

**Dove si trova**: Sezione DICHIARAZIONE DI CONFORMITA' → radio button nel testo "in conformità al titolo abilitativo ___"

**Causa**: Non hai indicato se il titolo abilitativo è allegato o già rilasciato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"allegato"** — il titolo abilitativo viene allegato alla presente denuncia
- ⚪ **"rilasciato"** — il titolo abilitativo è già stato rilasciato

---

### ATTENZIONE ! Inserire nominativo firma del sottoscrittore.

**Dove si trova**: Campo "firma" nella riga finale in fondo al modulo

**Causa**: Il campo firma del progettista della dichiarazione di conformità è vuoto.

**Soluzione**: Inserisci il nominativo del progettista che firma la dichiarazione di conformità.

---

## Consigli pratici — Variante Lavori Zona Sismica

### Prima di validare ✅

- [ ] Inserisci la **descrizione** dell'intervento (max 300 caratteri)
- [ ] Seleziona la **Zona Sismica** (3, 3S o 4) — non obbligatorio ma importante
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci **tipologia**, **numero** e (se richiesta) **data** del procedimento edilizio/titolo abilitativo in corso di validità
- [ ] Inserisci l'**Ente/Regione** destinatario della denuncia
- [ ] Se richiesti: inserisci **numero** e **data pratica** originale (GG/MM/AAAA)
- [ ] Seleziona il **tipo di intervento** (radio denuncia/autorizzazione/controllo)
- [ ] Compila **tutte e quattro le schede professionisti**: cognome, nome, CF per ognuna
- [ ] Compila la scheda **Costruttore**: cognome, nome, CF
- [ ] Seleziona il **referente PA** dal menu
- [ ] Seleziona il radio **strumento urbanistico** (è / non è); se "è": compila descrizione, n. delibera, data
- [ ] Seleziona il radio **vincolo idrogeologico** (è / non è); se "è": compila ente, n. autorizzazione, data
- [ ] Se presente: verifica il **formato della data** punto c) (denuncia lavori precedente)
- [ ] Seleziona una delle tre opzioni per il **collaudo delle opere**; se "necessita di nomina del collaudatore": seleziona anche una delle tre sotto-opzioni
- [ ] Inserisci **data** e **firma dichiarante** in fondo alla sezione DENUNCIA
- [ ] Inserisci la **firma del Costruttore**
- [ ] Inserisci il **nominativo del sottoscritto** nella Dichiarazione di Conformità
- [ ] Seleziona il **tipo di progettista** nella Dichiarazione di Conformità
- [ ] Seleziona il **titolo abilitativo** (allegato / rilasciato)
- [ ] Inserisci la **firma del progettista** in fondo al modulo

### Differenze rispetto alla Denuncia Sismica standard ⚠️

La Variante Lavori Zona Sismica è strutturalmente molto simile alla Denuncia Sismica Piemonte, con le seguenti differenze. Il testo della sezione DENUNCIA è "variante dei lavori già denunciati" invece di "lavori"; i campi numero pratica e data pratica originale servono a riferirsi alla denuncia precedente; la sezione DENUNCIA non contiene le coordinate ETRF89/WGS84 (presenti invece nella Denuncia Sismica); è presente inoltre la sezione dedicata al **titolare del procedimento edilizio/titolo abilitativo in corso di validità** e la sezione **collaudo delle opere** (punto e) con relativa nomina del collaudatore, entrambe specifiche di questa pratica. La Dichiarazione di Conformità è comune a entrambe.

### Errori frequenti 🔍

1. **Una delle 4 schede professionisti incompleta** → il ciclo si ferma alla prima scheda con un campo mancante; scorri tutto il modulo e controlla tutte e quattro le schede, non solo la prima
2. **Titolare del procedimento edilizio non compilato** → i tre campi (tipologia, numero, data) si trovano subito dopo la sezione "Localizzazione" e vengono facilmente saltati perché precedono il blocco DENUNCIA vero e proprio
3. **Referente PA non selezionato** → il menu inizia su voce vuota e spesso viene saltato perché si trova nel mezzo del modulo tra le schede professionisti e le dichiarazioni
4. **Data in formato errato** → la data del procedimento edilizio, della delibera SUE, dell'autorizzazione idrogeologica e del dichiarante devono tutte essere nel formato GG/MM/AAAA; con il datepicker il formato è automatico, ma se si inserisce manualmente è facile sbagliare
5. **Collaudo delle opere non selezionato o incompleto** → si trova al punto e), dopo il punto c) sulla denuncia lavori precedente, e viene spesso trascurato; se si sceglie "necessita di nomina del collaudatore" ricordarsi di compilare anche la sotto-scelta sulle modalità di nomina
6. **Firma del costruttore dimenticata** → si trova separata dalla firma del dichiarante e viene spesso ignorata; cercala nel testo "Firma del Costruttore per opere disciplinate dal D.P.R. n. 380..."
7. **Tipo progettista non selezionato nella Dichiarazione di Conformità** → il menu "in qualità di progettista" è diverso dal menu del referente PA; entrambi devono essere compilati separatamente

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

**Ultima revisione**: Settembre 2026
**Fonte**: Analisi codice ValidaDatiVarianteLavoriZonaSismica e DatiVarLavoriZonaSis.ascx
