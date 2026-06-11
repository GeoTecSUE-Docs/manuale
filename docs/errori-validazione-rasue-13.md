---
title: Errori Richiesta Approvazione Strumento Urbanistico Esecutivo - Regione Piemonte
parent: Errori di validazione
nav_order: 66
description: Errori di validazione specifici per la Richiesta di Approvazione dello Strumento Urbanistico Esecutivo (RASUE) - Regione Piemonte (L.U.R. 5/12/1977 n. 56, L.R. 9/04/1996 n. 18)
keywords: [strumento urbanistico esecutivo, RASUE, SUE, Piemonte, piano particolareggiato, piano edilizia economica, piano di recupero, piano insediamenti produttivi, piano esecutivo convenzionato, programma integrato, LUR 56/1977, LR 18/1996]
IDRegione: 2
IDTipoPratica: 13
Fonte: Manuale
---

# Errori di validazione - Richiesta Approvazione Strumento Urbanistico Esecutivo (R.A.S.U.E.)
## Regione Piemonte

Guida completa agli errori specifici per la **Richiesta di Approvazione dello Strumento Urbanistico Esecutivo (RASUE)** — Regione Piemonte, ai sensi della Legge Urbanistica Regionale 5 dicembre 1977, n. 56 (artt. 38-44) e della L.R. 9 aprile 1996, n. 18.

{: .note }
> La RASUE è una delle pratiche più lineari del sistema — solo 5 controlli in sequenza, senza logiche condizionali complesse. L'ordine di validazione è però insolito rispetto alle altre pratiche: il primo controllo non riguarda la localizzazione o la titolarità, ma il **campo area normativa** (`txtSpecifAreaNormativa`), seguito dalla scelta dello strumento urbanistico. La descrizione dell'intervento è l'ultimo controllo, dopo la localizzazione. Non ci sono sezioni di impresa, sicurezza, contributo o tecnici da validare. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Area normativa e tipo di strumento urbanistico](#1-area-normativa-e-tipo-di-strumento-urbanistico)
2. [Titolarità dell'intervento](#2-titolarità-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Descrizione dello Strumento Urbanistico Esecutivo](#4-descrizione-dello-strumento-urbanistico-esecutivo)

---

## 1. Area normativa e tipo di strumento urbanistico

### ATTENZIONE !  Inserire la descrizione della normativa.

**Dove si trova**: Sezione "CHIEDE — Riferimenti allo Strumento Urbanistico Esecutivo" → campo testo `txtSpecifAreaNormativa` "in area normativa ___"

**Causa**: Il campo area normativa è vuoto. È il **primo controllo** del validatore — viene verificato prima della titolarità e della localizzazione. Il messaggio ha due spazi dopo il punto esclamativo.

**Soluzione**: Inserisci la descrizione dell'area normativa di riferimento per lo strumento urbanistico esecutivo (es. tipo di zona PRG: "residenziale B2", "produttiva D1", ecc.).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Strumento Urbanistico Esecutivo'.

**Dove si trova**: Sezione "CHIEDE — Riferimenti allo Strumento Urbanistico Esecutivo" → 8 radio button `$StrUrbEse`

**Causa**: Nessuno degli 8 radio button è selezionato.

**Soluzione**: Seleziona **uno degli otto radio button** corrispondente allo strumento urbanistico esecutivo da approvare:
- ⚪ **a_1** — "piano particolareggiato di cui all'art. 38 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_2** — "piano per l'edilizia economica e popolare di cui all'art. 41 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_3** — "piano di recupero del patrimonio edilizio esistente di cui all'art. 41 bis L.U.R. 5/12/1977 n. 56"
- ⚪ **a_4** — "piano delle aree per insediamenti produttivi di cui all'art. 42 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_5** — "piano esecutivo convenzionato di libera iniziativa di cui all'art. 43 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_6** — "piano di recupero di libera iniziativa di cui all'art. 43 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_7** — "piano esecutivo convenzionato obbligatorio di cui all'art. 44 L.U.R. 5/12/1977 n. 56"
- ⚪ **a_8** — "programma integrato di riqualificazione urbanistica, edilizia e ambientale di cui alla L.R. 9/04/1996 n. 18"

{: .note }
> La scelta dello strumento dipende dalla tipologia di intervento urbanistico e dalla classificazione del PRG comunale. Per interventi su aree residenziali o miste si usa tipicamente il piano particolareggiato (a_1) o il piano esecutivo convenzionato (a_5/a_7); per aree produttive il piano insediamenti produttivi (a_4); per il patrimonio edilizio esistente il piano di recupero (a_3/a_6). In caso di dubbio, consultare l'ufficio tecnico comunale.

---

## 2. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` ("di avere titolo alla presentazione di questa pratica edilizia in quanto") è presente nel modulo ma non viene validato. La checkbox `chkAllegaDichAssenso` (si allega la dichiarazione di assenso) è commentata nel codice sorgente — non compare nel modulo.

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

{: .note }
> Il campo "Coordinate" (`txtCoordinate`) è presente nel modulo ma non validato.

---

## 4. Descrizione dello Strumento Urbanistico Esecutivo

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dello Strumento Urbanistico Esecutivo" → campo multiriga `txtDescrIntervento` "che i lavori per i quali viene inoltrata la presente richiesta consistono in:" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto. È l'**ultimo controllo** del validatore, dopo la localizzazione. Il messaggio ha due spazi dopo il punto esclamativo.

**Soluzione**: Inserisci la descrizione sintetica dello strumento urbanistico esecutivo e dei lavori previsti (max **300 caratteri**).

---

## Consigli pratici — RASUE Piemonte

### Prima di validare ✅

- [ ] Inserisci l'**area normativa** nel campo testo (primo controllo)
- [ ] Seleziona il **tipo di strumento urbanistico esecutivo** (a_1..a_8)
- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione** dello strumento urbanistico (max 300 caratteri)

### Ordine di validazione ⚠️

Area normativa → Strumento Urbanistico Esecutivo → Titolarità → Localizzazione → Descrizione

L'ordine è insolito rispetto alle altre pratiche: l'area normativa e il tipo di strumento vengono verificati **prima** della titolarità e della localizzazione. Assicurarsi di compilare la sezione "CHIEDE" nella sua interezza prima di procedere.

### Campi presenti ma non validati ℹ️

`cmbTitoloSuImm` (qualità del titolare), `txtCoordinate`, `txtData`, `txtLuogo`, `txtNote`, sezione tecnici, diritti di terzi, privacy (solo testo informativo).

### Errori frequenti 🔍

1. **Campo area normativa vuoto** → essendo il primo controllo, blocca immediatamente anche se tutto il resto è compilato; inserire la designazione della zona urbanistica del PRG
2. **Strumento non selezionato** → selezionare il radio corrispondente alla tipologia di strumento prevista dalla LUR 56/1977 o dalla LR 18/1996 in base al tipo di intervento urbanistico
3. **Descrizione vuota** → essendo l'ultimo controllo, appare solo dopo che tutti gli altri campi sono corretti; non dimenticarla

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
**Fonte**: Analisi codice ValidaDatiRASUE e DatiRASUE.ascx
