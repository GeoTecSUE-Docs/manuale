---
title: Errori Regolarizzazione Opere Interne - Regione Liguria
parent: Errori di validazione
nav_order: 37
description: Errori di validazione specifici per la Regolarizzazione Opere Interne (ROI) - Regione Liguria (art. 22 L.R. 16/2008)
keywords: [regolarizzazione opere interne, ROI, Liguria, LR 16/2008, art. 22, opere abusive interne, ante 1985, ante 2005, versamento 172.15, titolari aggiuntivi]
IDRegione: 3
IDTipoPratica: 61
Fonte: Analisi codice
---

# Errori di validazione - Regolarizzazione Opere Interne (ROI)
## Regione Liguria

Guida completa agli errori specifici per la **Regolarizzazione Opere Interne** ai sensi dell'art. 22 della L.R. Liguria 6 giugno 2008, n. 16, relativa alla **Regione Liguria**.

{: .note }
> La ROI Liguria è una pratica snella, specifica della regione, che consente la regolarizzazione amministrativa di opere interne abusive (ai sensi dell'art. 22 c. 2 L.R. 16/2008). La sezione più critica è il **tipo di intervento**: la scelta tra a.1 (opere ante 17/03/1985) e a.2 (opere post 17/03/1985 e ante 01/01/2005) determina se è richiesta la **data di versamento di € 172,15**. La sezione tecnici è solo dichiarativa (testo statico), senza campi da compilare o validare. Anche privacy e diritti di terzi sono testi informativi, non checkbox. La principale particolarità rispetto ad altre pratiche è il controllo dei **titolari aggiuntivi**: se si dichiara di non avere titolarità esclusiva, nella griglia dei soggetti coinvolti deve essere presente almeno un altro titolare. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Tipo di intervento](#1-tipo-di-intervento)
2. [Titolarità dell'intervento](#2-titolarità-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)

---

## 1. Tipo di intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo di intervento'.

**Causa**: Non hai selezionato nessuno dei 2 radio button che qualificano la collocazione temporale delle opere interne.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **a.1** — Opere realizzate **prima del 17 marzo 1985** (art. 22, c. 1, L.R. 16/2008) → nessun campo aggiuntivo
- ⚪ **a.2** — Opere realizzate **successivamente al 17 marzo 1985 e prima del 1° gennaio 2005** (art. 22, c. 3, L.R. 16/2008) → inserisci la data del versamento di € 172,15

{: .note }
> L'art. 22 c. 2 L.R. 16/2008 definisce le "opere interne" che possono essere regolarizzate: si tratta di interventi interni a unità immobiliari che non modificano la struttura portante, non creano nuove unità, non aumentano la superficie e non cambiano la destinazione d'uso. La scelta tra a.1 e a.2 dipende esclusivamente dalla **data di realizzazione** delle opere abusive, non dal tipo di intervento.

---

### ATTENZIONE ! Inserire la data. (versamento € 172,15)

**Dove si trova**: Sezione "Tipo di intervento" → campo data in linea nel testo dell'opzione a.2 "il versamento della somma di € 172,15 è stato effettuato in data ___"

**Causa**: Hai selezionato a.2 (opere post 17/03/1985) ma non hai inserito la data di versamento.

**Soluzione**: Inserisci la data del versamento di € 172,15 nel campo data nel formato **GG/MM/AAAA**.

{: .note }
> Il versamento di € 172,15 è richiesto dalla legge per le opere realizzate dopo il 17 marzo 1985 e prima del 1° gennaio 2005 (art. 22 c. 3 L.R. 16/2008). La ricevuta di versamento deve essere allegata alla comunicazione.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (versamento)

**Causa**: La data inserita per il versamento non rispetta il formato richiesto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/03/2018`).

---

### ATTENZIONE ! Inserire la Descrizione dell'intervento.

**Dove si trova**: Campo multiriga "che consistono in" nella sezione "Tipo di intervento", sotto i radio button.

**Causa**: Il campo descrizione (`txtDescrizioneIntervento`) è vuoto.

**Soluzione**: Inserisci la descrizione delle opere interne nel campo multiriga (max **300 caratteri**). La descrizione deve essere sufficientemente dettagliata da identificare le opere oggetto di regolarizzazione (es. `Realizzazione di tramezzatura interna per la separazione del locale cucina dal soggiorno`).

{: .warning }
> La descrizione è sempre obbligatoria, sia per a.1 che per a.2. Non dimenticare di compilarla anche se la pratica sembra semplice.

---

## 2. Titolarità dell'intervento

### ATTENZIONE ! Inserire la Titolarità dell'intervento.

**Causa**: Hai selezionato "altro" (`altron`) dal menu a discesa della titolarità ma non hai compilato il campo "Specificare se altro".

**Soluzione**: Inserisci la descrizione del titolo giuridico nel campo **"(Specificare se altro)"** (es. `Enfiteuta`, `Usufruttuario`, `Titolare di diritto reale di godimento`).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Non hai selezionato nessuno dei 2 radio button della titolarità.

**Soluzione**: Dopo aver selezionato il titolo giuridico dal menu a discesa, seleziona **una delle due opzioni**:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"** → è obbligatorio inserire almeno un titolare aggiuntivo nei soggetti coinvolti

---

### ATTENZIONE ! Non è stato inserito nessun Titolare aggiuntivo.

**Dove si trova**: Controllo eseguito automaticamente dopo la sezione titolarità, quando è selezionata l'opzione b.2 ("non avere titolarità esclusiva")

**Causa**: Hai dichiarato di non avere titolarità esclusiva ma la griglia dei titolari aggiuntivi (`GdvSoggTitolari`) è vuota.

**Soluzione**: Vai alla sezione **"Soggetti coinvolti"** → **"Titolari"** (o usa il pulsante "Aggiungi Titolare" se visibile) → aggiungi almeno un altro soggetto titolare dei diritti sull'immobile.

{: .note }
> Questo controllo è specifico della ROI Liguria e di poche altre pratiche liguri: quando si dichiara di non avere la titolarità esclusiva, il sistema verifica che nella griglia dei soggetti coinvolti sia presente almeno un altro titolare. Non è sufficiente allegare la dichiarazione di assenso — occorre anche registrare il soggetto nel sistema.

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato "Toponimo mancante" ma non hai compilato il campo testo.

**Soluzione**: Inserisci il toponimo nel campo di testo accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: "Toponimo mancante" non è spuntato e nessun indirizzo è selezionato dal menu a discesa.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure spunta "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP (es. `16100`).

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila i dati e salvalo con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso" (usa Ctrl+click per selezionare più voci).

---

## Consigli pratici ROI Liguria

### Prima di validare ✅

- [ ] Seleziona il **tipo di intervento** (a.1 ante 1985 o a.2 post 1985/ante 2005)
- [ ] Se a.2: inserisci la **data di versamento** di € 172,15 nel formato GG/MM/AAAA
- [ ] Compila la **descrizione** delle opere interne (obbligatoria, max 300 caratteri)
- [ ] Seleziona il **titolo giuridico** dal menu (se "altro": compila specificazione)
- [ ] Seleziona il **radio button titolarità** (esclusiva o non esclusiva)
- [ ] Se titolarità non esclusiva: aggiungi almeno un **titolare aggiuntivo** nei soggetti coinvolti
- [ ] Seleziona l'**indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**

### Sezioni non validate (solo informative) ℹ️

La ROI Liguria è una delle pratiche più snelle della piattaforma. Le seguenti sezioni sono presenti nel modulo come testo informativo ma **non generano errori di validazione** perché non contengono campi obbligatori da compilare:

- **Tecnici incaricati** — testo statico che dichiara l'incarico del progettista/rilevatore indicato nei soggetti coinvolti; nessun campo data, nessun radio button
- **Rispetto della normativa sulla privacy** — testo informativo statico, non una checkbox da spuntare
- **Informativa sulla privacy** — pannello espandibile con il testo completo dell'informativa D.Lgs. 196/2003

### Differenze principali ROI vs altre pratiche liguri ⚠️

Rispetto alle altre pratiche liguri (CILA, SCIA, PdC), la ROI è notevolmente semplificata: non ha sezione sicurezza D.Lgs. 81/2008, non ha sezione contributo, non ha sezione regolarità urbanistica, non ha sezione opere su parti comuni, non ha sezione descrizione sintetica separata (la descrizione è integrata nel tipo intervento), non ha data incarico tecnico obbligatoria. Il controllo del titolare aggiuntivo è invece più stringente rispetto ad altre pratiche dove si dichiara solo assenso documentale.

### Errori frequenti ROI Liguria 🔍

1. **Data versamento mancante per a.2** → se le opere sono post 17/03/1985, la data di versamento € 172,15 è sempre richiesta; controllare di aver già effettuato il versamento prima di presentare la pratica
2. **Descrizione vuota** → il campo multiriga "che consistono in" è facilmente ignorato poiché visivamente integrato nel testo della sezione; scorri la pagina verso il basso per trovarlo
3. **Titolare aggiuntivo non inserito** → chi dichiara titolarità non esclusiva deve aggiungere il co-titolare nella sezione soggetti coinvolti, non solo allegare un documento

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
**Fonte**: Analisi codice ValidaDatiROI_Liguria e DatiROILiguria.ascx
