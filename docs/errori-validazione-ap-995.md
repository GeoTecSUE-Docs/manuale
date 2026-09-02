---
title: Errori Autorizzazione Paesaggistica Ordinaria - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 69
description: Errori di validazione per l'Autorizzazione Paesaggistica Ordinaria (AP) Nazionale - Tutte le regioni (art. 146 D.Lgs. 42/2004, D.P.R. 31/2017)
keywords: [autorizzazione paesaggistica, AP, ordinaria, nazionale, tutte le regioni, art. 146 D.Lgs. 42/2004, art. 136, art. 142, art. 134, vincolo paesaggistico, precedenti autorizzazioni, stato immobile]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 105 }  # Valle d'Aosta - Autorizzazione Paesaggistica
  - { Reg: 6, Prat: 605 } # Veneto - Autorizzazione Paesaggistica
  - { Reg: 8, Prat: 805 } # Emilia-Romagna - Autorizzazione Paesaggistica
  - { Reg: 12, Prat: 1205 } # Lazio - Autorizzazione Paesaggistica
  - { Reg: 13, Prat: 1305 } # Abruzzo - Autorizzazione Paesaggistica
  - { Reg: 15, Prat: 1505 } # Campania - Autorizzazione Paesaggistica
  - { Reg: 16, Prat: 1605 } # Basilicata - Autorizzazione Paesaggistica
  - { Reg: 17, Prat: 1705 } # Puglia - Autorizzazione Paesaggistica
  - { Reg: 18, Prat: 1805 } # Calabria - Autorizzazione Paesaggistica
  - { Reg: 19, Prat: 1905 } # Sicilia - Autorizzazione Paesaggistica
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Ordinaria (A.P.)
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Ordinaria (AP) Nazionale** ai sensi dell'art. 146 del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio).

{: .note }
> L'AP Nazionale si distingue dalle versioni regionali ([AP Piemonte](errori-validazione-ap-5.html), [AP Lombardia](errori-validazione-ap-405.html), [AP Liguria](errori-validazione-ap-55.html)) per la presenza della sezione **"Estremi di precedenti autorizzazioni paesaggistiche rilasciate"** con radio e_1/e_2 e checkbox condizionali, e per le **4 opzioni di vincolo** (incluso "altro"). Non ha sezioni di contributo, impresa o sicurezza. Il modulo ha un **bug nel codice** del Focus della Titolarità (tenta di agire su un controllo di un'altra istanza) e un secondo bug nel Focus della data pratica e_1_3 (punta su `txtDataPrat1_2` invece di `txtDataPrat1_3`): il messaggio di errore viene comunque mostrato correttamente ma il campo che riceve il cursore potrebbe non essere quello corretto. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Descrizione sintetica dell'intervento](#3-descrizione-sintetica-dellintervento)
4. [Stato precedenti autorizzazioni paesaggistiche](#4-stato-precedenti-autorizzazioni-paesaggistiche)
5. [Tipo di vincolo paesaggistico](#5-tipo-di-vincolo-paesaggistico)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .warning }
> **Bug nel codice**: quando viene visualizzato questo errore, il sistema tenta di spostare il cursore sul campo `rdbTitolaritaa_1` di un'istanza diversa (`DatiAP1` invece di `DatiAPNaz1`). Il messaggio d'errore appare correttamente ma il cursore potrebbe non posizionarsi nel campo atteso. Ignorare il comportamento del cursore e procedere a selezionare il radio button manualmente.

{: .note }
> Il menu `cmbTitoloSuImm` ("di avere titolo alla presentazione di questa pratica edilizia in quanto") e il campo "Specificare se altro" (`txtSpecifTitolarita1`) sono presenti ma **non validati**.

---

## 2. Localizzazione dell'intervento

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
> Il campo "Coordinate" è commentato nel modulo sorgente (`<%-- --%>`) e non appare nell'interfaccia.

---

## 3. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga `txtDescrIntervento` (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione sintetica dei lavori per cui si richiede l'autorizzazione paesaggistica ordinaria (max **300 caratteri**).

---

## 4. Stato precedenti autorizzazioni paesaggistiche

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Estremi di precedenti autorizzazioni paesaggistiche rilasciate'.

**Dove si trova**: Sezione "Estremi di precedenti autorizzazioni paesaggistiche rilasciate" → 2 radio button `$Stato`

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **e_1** — "pienamente conforme alla documentazione dello stato di fatto legittimato dalle seguenti autorizzazioni paesaggistiche:" → spunta almeno una delle 2 checkbox sottostanti con numero e data
- ⚪ **e_2** — "non sono state reperite precedenti autorizzazioni paesaggistiche essendo l'immobile di remota costruzione e non interessato successivamente da interventi edilizi per i quali era necessario munirsi di autorizzazione paesaggistica"

---

### Opzione e_1 — Pienamente conforme

#### ATTENZIONE ! Non è stata selezionata nessun tipo di autorizzazione paesaggistica.

**Causa**: Hai selezionato e_1 ma nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoe_1_1** — "autorizzazione paesaggistica" → inserisci numero e data
- ☐ **chkStatoe_1_2** — "accertamento di compatibilità paesaggistica" → inserisci numero e data

---

#### ATTENZIONE ! Inserire il numero di pratica. (chkStatoe_1_1)

**Causa**: `chkStatoe_1_1` è spuntata ma `txtNPrat1_1` è vuoto.

**Soluzione**: Inserisci il numero dell'autorizzazione paesaggistica.

---

#### ATTENZIONE ! Inserire la data della pratica. (chkStatoe_1_1)

**Causa**: `chkStatoe_1_1` è spuntata e il numero è compilato, ma `txtDataPrat1_1` è vuoto.

**Soluzione**: Inserisci la data dell'autorizzazione paesaggistica nel campo "del".

{: .note }
> Le date delle pratiche precedenti **non vengono verificate nel formato** GG/MM/AAAA — il validatore controlla solo che il campo non sia vuoto. Il datepicker è presente ma non è obbligatorio usarlo.

---

#### ATTENZIONE ! Inserire il numero di pratica. (chkStatoe_1_2)

**Causa**: `chkStatoe_1_2` è spuntata ma `txtNPrat1_2` è vuoto.

**Soluzione**: Inserisci il numero dell'accertamento di compatibilità paesaggistica.

---

#### ATTENZIONE ! Inserire la data della pratica. (chkStatoe_1_2)

**Causa**: `chkStatoe_1_2` è spuntata e il numero è compilato, ma `txtDataPrat1_2` è vuoto.

**Soluzione**: Inserisci la data dell'accertamento di compatibilità paesaggistica.

---

### Checkbox e_1_3 — Pratiche in corso (indipendente da e_1/e_2)

La checkbox "per lo stesso immobile sono in corso interventi/sono state presentate pratiche per interventi di ___" (`chkStatoe_1_3`) è **indipendente** dalla scelta del radio e_1/e_2 — può essere spuntata in qualsiasi momento e richiede tipo pratica, numero e data.

---

#### ATTENZIONE ! Inserire il tipo di pratica.

**Causa**: `chkStatoe_1_3` è spuntata ma `txtTipoPrat1_3` è vuoto.

**Soluzione**: Inserisci il tipo di pratica edilizia in corso (es. "SCIA", "Permesso di Costruire", "CILA") nel campo testo affiancato alla checkbox.

---

#### ATTENZIONE ! Inserire il numero di pratica. (chkStatoe_1_3)

**Causa**: Il campo `txtNPrat1_3` è vuoto.

**Soluzione**: Inserisci il numero della pratica in corso.

---

#### ATTENZIONE ! Inserire la data della pratica. (chkStatoe_1_3)

**Causa**: Il campo `txtDataPrat1_3` è vuoto.

**Soluzione**: Inserisci la data della pratica in corso nel campo "del".

{: .warning }
> **Bug nel codice**: quando manca la data della pratica e_1_3, il messaggio "ATTENZIONE ! Inserire la data della pratica." viene visualizzato correttamente, ma il sistema tenta di spostare il cursore su `txtDataPrat1_2` invece di `txtDataPrat1_3`. Il campo da compilare è sempre `txtDataPrat1_3` (riga della checkbox e_1_3), non il campo della pratica precedente.

---

## 5. Tipo di vincolo paesaggistico

### ATTENZIONE ! Selezionare almeno un tipo di vincolo.

**Dove si trova**: Sezione "Tipo di vincolo in cui ricade l'intervento" → 4 checkbox

**Causa**: Nessuna delle 4 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 4 opzioni:
- ☐ **chkVincolo1** — "art. 136, comma 1, lettera ___) del d.lgs. n. 42/2004" → inserisci lettera (`txtLettera1`) e estremi del provvedimento (`txtVincolo1`)
- ☐ **chkVincolo2** — "art. 142, comma 1, lettera ___) del d.lgs. n. 42/2004" → inserisci la lettera (`txtLettera2`)
- ☐ **chkVincolo3** — "art. 134, comma 1, lettera c) del d.lgs. n. 42/2004 (specificare ___)" → inserisci il dettaglio (`txtVincolo3`)
- ☐ **chkVincolo4** — "altro (specificare ___)" → inserisci il dettaglio (`txtVincolo4`)

{: .note }
> La AP Nazionale ha **4 opzioni vincolo** rispetto alle 3 delle versioni regionali, con l'aggiunta di "altro (specificare)". Come nella [AP Piemonte](errori-validazione-ap-5.html) e nella [AP Liguria](errori-validazione-ap-55.html), è possibile spuntare più checkbox contemporaneamente se l'immobile ricade in più ambiti di tutela.

---

### ATTENZIONE ! Inserire la lettera del vincolo. (chkVincolo1)

**Causa**: `chkVincolo1` è spuntata ma `txtLettera1` è vuoto.

**Soluzione**: Inserisci la lettera della fattispecie dell'art. 136 c. 1 del D.Lgs. 42/2004 (a = bellezze naturali; b = ville/giardini/parchi; c = complessi di cose immobili; d = bellezze panoramiche).

---

### ATTENZIONE ! Inserire il dettaglio del vincolo. (chkVincolo1)

**Causa**: `chkVincolo1` è spuntata e la lettera è compilata, ma `txtVincolo1` è vuoto.

**Soluzione**: Inserisci gli estremi del provvedimento che ha dichiarato il bene di notevole interesse pubblico (es. "d.m. 15/04/1960" o "d.g.r. n. 123 del 01/01/2000").

---

### ATTENZIONE ! Inserire la lettera del vincolo. (chkVincolo2)

**Causa**: `chkVincolo2` è spuntata ma `txtLettera2` è vuoto.

**Soluzione**: Inserisci la lettera della fattispecie dell'art. 142 c. 1 del D.Lgs. 42/2004 che identifica l'area tutelata per legge (es. b = laghi; c = fiumi e torrenti; g = boschi; h = montagne sopra 1600/1200 m; ecc.).

{: .note }
> A differenza dell'[APS Nazionale](errori-validazione-aps-9954.html) dove `txtVincolo2` (lettera dell'art. 142) non è validata, nell'AP Nazionale la lettera dell'art. 142 (`txtLettera2`) è **obbligatoria** se `chkVincolo2` è spuntata.

---

### ATTENZIONE ! Inserire il dettaglio del vincolo. (chkVincolo3)

**Causa**: `chkVincolo3` è spuntata ma `txtVincolo3` è vuoto.

**Soluzione**: Inserisci la specificazione del vincolo dell'art. 134 c. 1 lett. c) del D.Lgs. 42/2004 (beni tutelati dai piani paesaggistici regionali).

---

### ATTENZIONE ! Inserire il dettaglio del vincolo. (chkVincolo4)

**Causa**: `chkVincolo4` ("altro") è spuntata ma `txtVincolo4` è vuoto.

**Soluzione**: Inserisci la specificazione del tipo di vincolo paesaggistico non rientrante nelle categorie precedenti.

---

## Consigli pratici — AP Nazionale

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione** dell'intervento (max 300 caratteri)
- [ ] Seleziona lo **stato precedenti autorizzazioni** (e_1/e_2); se e_1: spunta almeno una checkbox (chkStatoe_1_1 o chkStatoe_1_2) con numero e data
- [ ] Se `chkStatoe_1_3` spuntata: inserisci **tipo pratica**, **numero** e **data**
- [ ] Spunta almeno una delle 4 **checkbox vincolo** (art. 136/142/134/altro); per ciascuna compilare i campi richiesti (lettera e/o dettaglio)

### Ordine di validazione ⚠️

Titolarità → Localizzazione → Descrizione → Stato precedenti autorizzazioni (e_1/e_2 + chkStatoe_1_3) → Vincolo (4 checkbox)

### Campi presenti ma non validati ℹ️

`cmbTitoloSuImm` (titolarità menu), `txtSpecifTitolarita1` ("Specificare se altro"), sezione "Qualificazione dell'intervento" (solo testo), coordinate (commentate nel modulo), privacy (solo testo informativo).

### Differenze rispetto alle versioni regionali ⚠️

Rispetto alle versioni regionali ([AP Piemonte](errori-validazione-ap-5.html) con 4 opzioni stato e 14 checkbox vincolo, [AP Lombardia](errori-validazione-ap-405.html) con 4 checkbox vincolo, [AP Liguria](errori-validazione-ap-55.html) con 14 checkbox vincolo): la versione Nazionale ha una sezione "Stato precedenti autorizzazioni" con radio e_1/e_2 + checkbox condizionali assente nelle versioni regionali; solo 4 opzioni vincolo invece di 14; inclusa la voce "altro" (chkVincolo4); la lettera dell'art. 142 (`txtLettera2`) è obbligatoria qui, non lo era nell'APS Nazionale.

### Bug noti ⚠️

Due bug di Focus nel codice di questa pratica: (1) Titolarità: il Focus tenta di agire su `DatiAP1` invece di `DatiAPNaz1` — il messaggio appare correttamente ma il cursore può non andare al posto giusto; (2) Data pratica e_1_3: quando `txtDataPrat1_3` è vuoto, il Focus va su `txtDataPrat1_2` — il campo da compilare rimane sempre `txtDataPrat1_3`.

### Errori frequenti 🔍

1. **Radio stato non selezionato** → scegliere e_1 (conforme a precedenti autorizzazioni) o e_2 (nessuna precedente); se e_1: spuntare almeno una checkbox con numero e data
2. **chkStatoe_1_3 senza dati** → richiede 3 campi (tipo pratica + n. + data); il bug del Focus non pregiudica la validazione ma può disorientare
3. **Nessun vincolo spuntato** → almeno una delle 4 checkbox obbligatoria; per art. 136: lettera + estremi; per art. 142: lettera; per art. 134 e "altro": dettaglio
4. **Lettera art. 142 vuota** → a differenza dell'APS Nazionale, nell'AP Nazionale la lettera dell'art. 142 è obbligatoria

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Vedi le versioni regionali: [AP Piemonte](errori-validazione-ap-5.html) — [AP Lombardia](errori-validazione-ap-405.html) — [AP Liguria](errori-validazione-ap-55.html)
3. Vedi [APS Nazionale](errori-validazione-aps-9954.html) per la versione semplificata
4. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
5. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiAPNaz e DatiAPNaz.ascx
