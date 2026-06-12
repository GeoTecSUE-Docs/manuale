---
title: Errori Autorizzazione allo Scarico - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 62
description: Errori di validazione specifici per l'Autorizzazione allo Scarico di acque reflue domestiche (AS) - Tutte le regioni (D.Lgs. 152/2006)
keywords: [autorizzazione scarico, AS, acque reflue domestiche, D.Lgs. 152/2006, corpo idrico superficiale, strati superficiali sottosuolo, numero scarichi, titolarità, tutte le regioni]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 2, Prat: 79 }  # Piemonte - Autorizzazione allo scarico
  - { Reg: 1, Prat: 179 }  # Valle d'Aosta - Autorizzazione allo scarico
  - { Reg: 3, Prat: 379 } # Liguria - Autorizzazione allo scarico
  - { Reg: 4, Prat: 479 } # Lombardia - Autorizzazione allo scarico
  - { Reg: 6, Prat: 679 } # Veneto - Autorizzazione allo scarico
  - { Reg: 8, Prat: 879 } # Emilia-Romagna - Autorizzazione allo scarico
  - { Reg: 12, Prat: 1279 } # Lazio - Autorizzazione allo scarico
  - { Reg: 13, Prat: 1379 } # Abruzzo - Autorizzazione allo scarico
  - { Reg: 15, Prat: 1579 } # Campania - Autorizzazione allo scarico
  - { Reg: 16, Prat: 1679 } # Basilicata - Autorizzazione allo scarico
  - { Reg: 17, Prat: 1779 } # Puglia - Autorizzazione allo scarico
  - { Reg: 18, Prat: 1879 } # Calabria - Autorizzazione allo scarico
  - { Reg: 19, Prat: 1979 } # Sicilia - Autorizzazione allo scarico
Fonte: Manuale
---

# Errori di validazione - Autorizzazione allo Scarico (A.S.)
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per l'**Autorizzazione allo Scarico di acque reflue domestiche (AS)** ai sensi del D.Lgs. 3 aprile 2006, n. 152 (Codice dell'Ambiente) e delle norme statali e regionali di settore.

{: .note }
> L'Autorizzazione allo Scarico è una delle pratiche più snelle del sistema e strutturalmente unica: non ha sezioni di qualificazione, regolarità urbanistica, contributo, tecnici, impresa o sicurezza. Il nucleo della validazione è la sezione **"Recapito finale"** con 3 campi numerici legati da un **vincolo aritmetico preciso**: il numero totale di scarichi deve essere uguale alla somma degli scarichi in corpo idrico superficiale e in strati superficiali del sottosuolo. Se i tre numeri non si bilanciano, la validazione si blocca con un messaggio specifico. La sezione Titolarità è presente solo come menu a discesa — senza radio group. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Recapito finale — numero scarichi](#2-recapito-finale--numero-scarichi)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Specificare la titolarità dell'intervento.

**Dove si trova**: Sezione "Titolarità Intervento" → campo `txtSpecifTitolarita1` "Specificare se altro"

**Causa**: Il menu `cmbTitoloSuImm` ha il valore "altron" (opzione "altro") selezionato ma il campo di specificazione `txtSpecifTitolarita1` è vuoto.

**Soluzione**: Inserisci la specificazione del titolo di proprietà sull'immobile nel campo "Specificare se altro".

{: .note }
> La sezione Titolarità della pratica AS ha solo il **menu `cmbTitoloSuImm`** — non ci sono radio button Titolarita (a differenza di quasi tutte le altre pratiche del sistema). L'unico controllo è il caso in cui si seleziona "altro": in quel caso il campo di specificazione diventa obbligatorio. Per tutti gli altri valori del menu (proprietario, usufruttuario, ecc.) non viene eseguita nessuna validazione sulla titolarità.

---

## 2. Recapito finale — numero scarichi

Questa è la sezione specifica dell'Autorizzazione allo Scarico. Contiene 3 campi numerici che devono soddisfare un preciso vincolo aritmetico: il totale degli scarichi deve essere uguale alla somma degli scarichi per ciascun recapito finale.

Il validatore elabora i tre campi **in sequenza**: prima `txtNumeroScarichi`, poi `txtCorpoIdricoSup`, poi `txtStratiSupSottoSuolo`, e infine verifica la coerenza aritmetica. L'elaborazione si interrompe al primo campo mancante.

---

### ATTENZIONE ! Inserire il numero di scarichi.

**Dove si trova**: Sezione "CHIEDE — Recapito finale" → campo `txtNumeroScarichi` "a n° ___ scarico/chi di acque reflue domestiche"

**Causa**: Il campo del numero totale di scarichi è vuoto.

**Soluzione**: Inserisci il numero totale di scarichi di acque reflue domestiche per cui si richiede l'autorizzazione.

---

### ATTENZIONE ! Inserire il numero di corpo idrico superficiale.

**Causa**: `txtNumeroScarichi` è compilato ma il campo `txtCorpoIdricoSup` (scarichi con recapito in corpo idrico superficiale) è vuoto.

**Soluzione**: Inserisci il numero di scarichi con recapito finale in **corpo idrico superficiale**. Se nessuno scarico recapita in corpo idrico superficiale, inserisci **0**.

{: .note }
> Il validatore non ammette il campo vuoto anche se il valore è zero: inserire `0` esplicitamente se non sono previsti scarichi in corpo idrico superficiale.

---

### ATTENZIONE ! Inserire il numero di strati superficiali del sottosuolo.

**Causa**: `txtNumeroScarichi` e `txtCorpoIdricoSup` sono compilati ma il campo `txtStratiSupSottoSuolo` (scarichi con recapito negli strati superficiali del sottosuolo) è vuoto.

**Soluzione**: Inserisci il numero di scarichi con recapito finale negli **strati superficiali del sottosuolo**. Se nessuno scarico recapita nel sottosuolo, inserisci **0**.

---

### ATTENZIONE ! Il numero di scarichi totali non coincide con la somma di 'Corpo idrico superficiale' e 'Strati superficiali del sottosuolo'.

**Causa**: Tutti e tre i campi sono compilati ma la verifica aritmetica fallisce: `txtNumeroScarichi ≠ txtCorpoIdricoSup + txtStratiSupSottoSuolo`.

**Soluzione**: Correggi i tre valori in modo che la somma dei recapiti coincida con il totale. Esempi:

- Totale `2`, corpo idrico `1`, sottosuolo `1` → ✅ (1 + 1 = 2)
- Totale `3`, corpo idrico `2`, sottosuolo `0` → ✅ (2 + 0 = 2 ≠ 3) → ❌ — correggi il totale a `2` o aumenta un recapito
- Totale `1`, corpo idrico `0`, sottosuolo `0` → ❌ (0 + 0 = 0 ≠ 1) — inserire almeno 1 in uno dei recapiti

{: .warning }
> Questo è il controllo aritmetico più caratteristico dell'AS — unico nel sistema GeoTecSUE. Il validatore usa `Val()` per convertire i testi in numeri, quindi valori non numerici nei campi potrebbero causare errori imprevisti. Usare solo cifre intere nei tre campi.

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
> Il campo "Coordinate" è presente nel codice sorgente del modulo ma commentato (`<%-- --%>`) — non appare nel modulo e non viene validato.

---

## Consigli pratici — AS Nazionale

### Prima di validare ✅

- [ ] Se `cmbTitoloSuImm = "altro"`: compila il campo **"Specificare se altro"**
- [ ] Inserisci il **numero totale di scarichi** (`txtNumeroScarichi`)
- [ ] Inserisci gli scarichi in **corpo idrico superficiale** (`txtCorpoIdricoSup`), anche `0` se non applicabile
- [ ] Inserisci gli scarichi in **strati superficiali del sottosuolo** (`txtStratiSupSottoSuolo`), anche `0` se non applicabile
- [ ] Verifica che **totale = corpo idrico + sottosuolo** prima di inviare
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**

### Campi e sezioni non validati ℹ️

L'AS è la pratica con il numero minore di controlli del sistema. Non sono presenti e non vengono validati: radio Titolarita, qualificazione intervento, descrizione, regolarità urbanistica, contributo, tecnici, impresa, sicurezza, privacy (solo testo informativo), coordinate (commentate nel modulo).

### Calcolo scarichi — schema ⚠️

Il vincolo da rispettare è sempre: **N° scarichi totali = N° corpo idrico superficiale + N° strati superficiali sottosuolo**

Esempi di combinazioni valide:
- 1 scarico totale, tutti in corpo idrico: `1 = 1 + 0`
- 1 scarico totale, tutti nel sottosuolo: `1 = 0 + 1`
- 3 scarichi totali, misti: `3 = 2 + 1` oppure `3 = 1 + 2`
- Se lo scarico è unico e va in entrambi i recapiti: non è possibile — ogni scarico recapita in uno solo dei due.

### Errori frequenti 🔍

1. **Campo recapito vuoto invece di zero** → se non ci sono scarichi in un recapito, inserire `0`; lasciare il campo vuoto genera l'errore "Inserire il numero..."
2. **Somma sbagliata** → rileggere i tre valori prima di validare; es. 2 scarichi totali ma si inserisce 1+0=1 dimenticando il secondo
3. **Titolarità "altro" senza specificazione** → l'unico controllo sulla titolarità è il campo specificazione quando si sceglie "altro" nel menu

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
**Fonte**: Analisi codice ValidaDatiAS e DatiAS.ascx
