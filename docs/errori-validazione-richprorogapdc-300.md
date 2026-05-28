---
title: Errori Richiesta di Proroga Termini Permesso di Costruire - Regione Piemonte
parent: Errori di validazione
nav_order: 48
description: Errori di validazione specifici per la Richiesta di Proroga dei Termini del Permesso di Costruire - Regione Piemonte (art. 15 D.P.R. 380/2001)
keywords: [proroga termini, permesso di costruire, PdC, Piemonte, art. 15 DPR 380/2001, inizio lavori, fine lavori, motivazioni, scadenza permesso]
IDRegione: 2
IDTipoPratica: 300
Fonte: Manuale
---

# Errori di validazione - Richiesta di Proroga Termini Permesso di Costruire
## Regione Piemonte

Guida completa agli errori specifici per la **Richiesta di Proroga dei Termini del Permesso di Costruire** ai sensi dell'art. 15 del D.P.R. 380/2001 — Regione Piemonte. La proroga può riguardare il termine di inizio lavori, il termine di fine lavori, o entrambi.

{: .note }
> La Proroga Termini PdC è una delle pratiche più semplici del sistema, con poche sezioni da compilare. La caratteristica principale è che la sezione **Proroga termini** viene validata **prima** della localizzazione: indicare il tipo di proroga e i relativi mesi — con valore necessariamente numerico — e collegare almeno un Permesso di Costruire esistente. La sezione **Motivazioni** è obbligatoria e richiede l'esposizione per iscritto dei fatti sopravvenuti che giustificano la proroga. La **privacy** è presente come testo informativo statico ma **non genera errori** se non spuntata. Non sono richiesti tecnici, imprese o coordinate. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Proroga termini — tipo e durata](#1-proroga-termini--tipo-e-durata)
2. [Proroga termini — pratiche edilizie di riferimento](#2-proroga-termini--pratiche-edilizie-di-riferimento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Motivazioni della proroga](#4-motivazioni-della-proroga)

---

## 1. Proroga termini — tipo e durata

### ATTENZIONE ! Selezionare almeno una proroga dei termini.

**Dove si trova**: Sezione "Proroga termini" → 2 checkbox in cima al modulo

**Causa**: Nessuna delle due checkbox di tipo proroga è spuntata — non hai indicato se la proroga riguarda il termine di inizio lavori, di fine lavori o entrambi.

**Soluzione**: Spunta **almeno una** tra le due checkbox:
- ☐ **chkProrogaa_1** — "la proroga del termine di inizio lavori di mesi ___" (massimo 12)
- ☐ **chkProrogaa_2** — "la proroga del termine di fine lavori di mesi ___" (massimo 12)

Le due checkbox non sono mutuamente esclusive: è possibile richiedere sia la proroga del termine di inizio che quella di fine lavori nella stessa istanza.

---

### ATTENZIONE ! Selezionare la durata della proroga del termine di inizio lavori.

**Causa**: Hai spuntato `chkProrogaa_1` (proroga inizio lavori) ma il campo `txtProrogaInizio` è vuoto.

**Soluzione**: Inserisci nel campo affiancato il numero di mesi di proroga richiesti per il termine di inizio lavori. Il valore deve essere un numero intero (es. `6`, `12`). Il modulo indica un massimo di **12 mesi**.

---

### ATTENZIONE ! La durata della proroga del termine di inizio lavori deve essere un valore numerico.

**Causa**: Hai compilato il campo `txtProrogaInizio` ma il valore inserito non è riconosciuto come numero (contiene lettere, simboli o testo).

**Soluzione**: Inserisci solo cifre nel campo della durata (es. `6`, `12`). Non inserire la parola "mesi", unità di misura o altri testi.

---

### ATTENZIONE ! Selezionare la durata della proroga del termine di fine lavori.

**Causa**: Hai spuntato `chkProrogaa_2` (proroga fine lavori) ma il campo `txtProrogaFine` è vuoto.

**Soluzione**: Inserisci nel campo affiancato il numero di mesi di proroga richiesti per il termine di fine lavori. Il valore deve essere un numero intero (massimo **12 mesi**).

---

### ATTENZIONE ! La durata della proroga del termine di fine lavori deve essere un valore numerico.

**Causa**: Il campo `txtProrogaFine` contiene un valore non numerico.

**Soluzione**: Inserisci solo cifre nel campo (es. `6`, `12`).

{: .note }
> Il validatore usa la funzione `IsNumeric` di VB.NET, che accetta interi e decimali (es. `6.5` è accettato). Tuttavia, il modulo indica valori interi di mesi; inserire un decimale potrebbe essere accettato tecnicamente ma non è corretto ai fini della richiesta. Inserire valori come `6 mesi`, `sei`, `12+` genera l'errore "deve essere un valore numerico". Il sistema non verifica che il valore non superi 12: la nota "(massimo 12)" è solo informativa nel modulo.

---

## 2. Proroga termini — pratiche edilizie di riferimento

### ATTENZIONE ! Selezionare almeno una pratica edilizia.

**Dove si trova**: Sezione "Proroga termini" → testo "per le seguenti pratiche edilizie:" → 3 checkbox "permesso di costruire"

**Causa**: Nessuna delle 3 checkbox delle pratiche edilizie è spuntata.

**Soluzione**: Spunta **almeno una** delle 3 checkbox "permesso di costruire" (chkProrogaa_3, a_4, a_5) e compila i campi numero e data del PdC corrispondente.

{: .note }
> Il modulo prevede fino a **3 Permessi di Costruire** a cui collegare la proroga — tutte e tre le righe sono etichettate identicamente "permesso di costruire". Questa struttura serve per i casi in cui la proroga riguarda più PdC correlati (es. varianti o fasi distinte). Nella maggior parte dei casi si spunta solo la prima checkbox (a_3) con il PdC principale.

---

### ATTENZIONE ! Selezionare il numero del permesso di costruire.

**Causa**: Hai spuntato una delle 3 checkbox "permesso di costruire" ma non hai inserito il numero nel campo "numero" affiancato.

**Soluzione**: Inserisci il numero del Permesso di Costruire nel campo "numero" corrispondente alla checkbox spuntata (es. `45/2021`, `PdC n. 123`).

Il messaggio è identico per tutte e 3 le checkbox (a_3, a_4, a_5).

---

### ATTENZIONE ! Selezionare la data del permesso di costruire.

**Causa**: Hai compilato il numero del PdC ma il campo data è vuoto.

**Soluzione**: Inserisci la data del Permesso di Costruire nel campo "del" nel formato **GG/MM/AAAA**.

Il messaggio è identico per tutte e 3 le checkbox.

{: .note }
> A differenza di molte altre pratiche GeoTecSUE, le date dei Permessi di Costruire in questa sezione **non vengono verificate nel formato GG/MM/AAAA**: il validatore controlla solo che il campo non sia vuoto. Un valore come `2021` o `marzo 2021` supera la validazione. È comunque buona prassi inserire la data nel formato standard GG/MM/AAAA per la correttezza documentale.

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inseriscilo nel campo testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

---

## 4. Motivazioni della proroga

### ATTENZIONE ! Inserire le motivazioni della proroga.

**Dove si trova**: Sezione "Motivazioni" → campo multiriga sotto "che non potrà rispettare i termini indicati nel Permesso di Costruire per i seguenti fatti sopravvenuti estranei alla volontà del titolare del permesso di seguito riportati"

**Causa**: Il campo `txtMotivazioni` è vuoto.

**Soluzione**: Inserisci nel campo multiriga la descrizione dei fatti sopravvenuti che giustificano la richiesta di proroga. La proroga dei termini del PdC ai sensi dell'art. 15 del D.P.R. 380/2001 è concessa dal Comune quando i ritardi siano dovuti a fatti estranei alla volontà del titolare (es. contenzioso in corso, difficoltà di reperimento materiali, eventi meteorologici eccezionali, procedure autorizzative di enti terzi).

{: .note }
> Non è indicato un limite di caratteri per il campo motivazioni nel codice VB — il validatore verifica solo che non sia vuoto. Ai fini procedurali, la motivazione deve essere sufficientemente dettagliata e documentata. Il Comune valuterà la fondatezza dei motivi esposti prima di accogliere la proroga.

---

## Consigli pratici — Proroga Termini PdC

### Prima di validare ✅

- [ ] Spunta almeno una checkbox tra **inizio lavori** e **fine lavori** e inserisci la durata in **mesi** (valore numerico, max 12)
- [ ] Spunta almeno una checkbox **"permesso di costruire"** e compila il **numero** e la **data** del PdC
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci le **motivazioni** della proroga nel campo multiriga

### Campi presenti ma non validati ℹ️

- **Privacy**: la sezione "Rispetto della normativa sulla privacy" e "Informativa sulla privacy" sono presenti come testo informativo statico — **non c'è nessuna checkbox `chkPrivacy`** e nessun errore viene generato
- **Tecnici e imprese**: non sono richiesti per questa pratica
- **Coordinate**: non sono richieste
- **Formato date PdC**: le date dei permessi di costruire vengono verificate solo come "non vuoto" — il formato GG/MM/AAAA non è validato; inserire il formato corretto è comunque buona prassi

### Ordine di validazione ⚠️

A differenza della maggior parte delle pratiche, la validazione della proroga segue questo ordine: tipo proroga (inizio/fine) → durata mesi → pratiche PdC → localizzazione → motivazioni. Gli errori sulla proroga appaiono quindi prima di qualsiasi errore sulla localizzazione.

### Errori frequenti 🔍

1. **Durata mesi non numerica** → inserire `6 mesi` o `sei` genera l'errore "deve essere un valore numerico"; inserire solo la cifra (`6`)
2. **Nessuna checkbox PdC spuntata** → dopo aver indicato il tipo di proroga, è necessario spuntare anche la riga del PdC a cui si riferisce; le due sezioni sono indipendenti e l'una non attiva automaticamente l'altra
3. **Numero PdC compilato ma data vuota** → per ogni PdC spuntato, sia numero che data sono obbligatori; compilare uno solo non è sufficiente
4. **Motivazioni vuote** → il campo motivazioni è l'ultimo controllato dal validatore e può essere dimenticato; è obbligatorio e non ha un limite minimo di caratteri, ma deve contenere almeno qualcosa

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
**Fonte**: Analisi codice ValidaDatiProrogaTerminiPDC e DatiProrogaTerminiPDC.ascx
