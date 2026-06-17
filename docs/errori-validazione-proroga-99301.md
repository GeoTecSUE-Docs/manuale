---
title: Errori Proroga Termini - Tutte le regioni
parent: Errori di validazione
nav_order: 33
description: Errori di validazione specifici per la Comunicazione di Proroga dei Termini di inizio e/o ultimazione lavori - Tutte le regioni
keywords: [proroga termini, proroga lavori, 48 mesi, quarantotto mesi, permesso di costruire, convenzione lottizzazione, piano attuativo, SCIA, data inizio lavori, data fine lavori, verifiche effettuate, denominazione]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 99301
IDTarget:
  - { Reg: 2, Prat: 301 }   # Piemonte - Proroga
  - { Reg: 1, Prat: 1301 }   # Valle d'Aosta - Proroga
  - { Reg: 3, Prat: 3301 }   # Liguria - Proroga
  - { Reg: 4, Prat: 4301 }   # Lombardia - Proroga
  - { Reg: 6, Prat: 6301 }   # Veneto - Proroga
  - { Reg: 8, Prat: 8301 }   # Emilia-Romagna - Proroga
  - { Reg: 12, Prat: 12301 }  # Lazio - Proroga
  - { Reg: 13, Prat: 13301 }  # Abruzzo - Proroga
  - { Reg: 15, Prat: 15301 }  # Campania - Proroga
  - { Reg: 16, Prat: 16301 }  # Basilicata - Proroga
  - { Reg: 17, Prat: 17301 }  # Puglia - Proroga
  - { Reg: 18, Prat: 18301 }  # Calabria - Proroga
  - { Reg: 19, Prat: 19301 }  # Sicilia - Proroga
Fonte: Analisi codice
---

# Errori di validazione - Proroga dei Termini
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Proroga dei Termini** di inizio e/o ultimazione lavori di 48 mesi, applicabile a permessi di costruire, SCIA, SCIA alternative al PdC, autorizzazioni paesaggistiche, convenzioni di lottizzazione e piani attuativi.

{: .note }
> La Proroga ha una struttura compatta ma con alcune caratteristiche peculiari. La scelta tra proroga di inizio e proroga di fine lavori avviene tramite **due checkbox indipendenti** (almeno una obbligatoria), ciascuna con la propria data originale da compilare. La **nuova data** (proroga di 48 mesi calcolata automaticamente) e il relativo campo `txtDataInizioNuova`/`txtDataFineNuova` sono attualmente **commentati nel codice** e non compaiono nell'interfaccia: il sistema non richiede né calcola la nuova data, ma registra solo la data originale. La sezione **"Verifiche effettuate"** ha logica condizionale: se si sceglie il secondo radio button (convenzioni di lottizzazione), diventa obbligatorio indicare la denominazione dell'atto. La privacy in questa pratica è solo **informativa**, non genera errori di validazione. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Proroga termini — selezione e date originali](#1-proroga-termini--selezione-e-date-originali)
2. [Pratica edilizia di riferimento](#2-pratica-edilizia-di-riferimento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Verifiche effettuate](#4-verifiche-effettuate)

---

## 1. Proroga termini — selezione e date originali

### ATTENZIONE ! Selezionare almeno una proroga dei termini.

**Dove si trova**: Sezione **"Proroga termini"** → le due checkbox in cima al modulo

**Causa**: Non hai spuntato nessuna delle due checkbox di proroga disponibili.

**Soluzione**: Spunta **almeno una** delle due opzioni:
- ☑ **"la proroga di quarantotto mesi della data di inizio dei lavori attualmente prevista al ___"** → inserisci la data originale di inizio lavori nel campo che si attiva
- ☑ **"la proroga di quarantotto mesi della data di ultimazione dei lavori attualmente prevista al ___"** → inserisci la data originale di fine lavori nel campo che si attiva

È possibile spuntare entrambe se si richiede la proroga sia dell'inizio sia della fine dei lavori.

{: .note }
> La proroga dell'inizio lavori (prima checkbox) è **valida solo per permessi di costruire, convenzioni di lottizzazione e piani attuativi**, come indicato nel testo della checkbox stessa. Per SCIA e altri titoli, la proroga applicabile è solo quella della data di ultimazione lavori (seconda checkbox).

---

### ATTENZIONE ! Selezionare la data originale di inizio lavori.

**Dove si trova**: Prima checkbox → campo data **"attualmente prevista al"** accanto al testo di proroga inizio

**Causa**: Hai spuntato la checkbox di proroga inizio lavori ma non hai inserito la data originale di inizio lavori.

**Soluzione**:
1. Spunta la checkbox ☑ **"la proroga di quarantotto mesi della data di inizio dei lavori"**
2. Il campo data accanto a **"attualmente prevista al"** si attiva
3. Inserisci la data originale di inizio lavori nel formato **GG/MM/AAAA** (es. `15/03/2024`)
4. Puoi usare l'icona calendario o digitare direttamente

{: .note }
> Il campo data si abilita solo dopo aver spuntato la checkbox. Se il campo appare disabilitato (grigio), verifica di aver spuntato la checkbox corrispondente prima di tentare di inserire la data.

---

### ATTENZIONE ! Selezionare la data originale di fine lavori.

**Dove si trova**: Seconda checkbox → campo data **"attualmente prevista al"** accanto al testo di proroga fine

**Causa**: Hai spuntato la checkbox di proroga fine lavori ma non hai inserito la data originale di ultimazione lavori.

**Soluzione**:
1. Spunta la checkbox ☑ **"la proroga di quarantotto mesi della data di ultimazione dei lavori"**
2. Il campo data accanto a **"attualmente prevista al"** si attiva
3. Inserisci la data originale di ultimazione lavori nel formato **GG/MM/AAAA**

---

### ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Una delle date originali (inizio o fine lavori) è in un formato non riconosciuto dal sistema.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `15/03/2024` ✅. Errati: `15-03-2024` ❌, `15/03/24` ❌. Il messaggio può comparire per la data di inizio o per quella di fine: verifica entrambe le checkbox spuntate.

{: .warning }
> **Funzionalità commentata — nuova data non richiesta**: nel codice sorgente sono presenti (ma commentati) i campi `txtDataInizioNuova` e `txtDataFineNuova` e la logica di calcolo che verificava che la nuova data fosse successiva all'originale e non oltre 48 mesi. Questi controlli **non sono attivi**: il sistema attualmente accetta qualsiasi data originale valida nel formato GG/MM/AAAA, senza calcolare né richiedere la nuova data prorogata. Era anche presente un controllo che bloccava date nuove oltre 48 mesi dall'originale, anch'esso disattivato.

---

## 2. Pratica edilizia di riferimento

### ATTENZIONE ! Indicare la tipologia di pratica.

**Dove si trova**: Sezione **"Proroga termini"** → campo **"Tipo pratica"**

**Causa**: Non hai indicato la tipologia della pratica edilizia per cui si richiede la proroga.

**Soluzione**: Inserisci la tipologia nel campo **"Tipo pratica"** (es. `Permesso di Costruire`, `SCIA`, `Convenzione di Lottizzazione`, `Piano Attuativo`).

---

### ATTENZIONE ! Indicare il numero di pratica.

**Dove si trova**: Sezione **"Proroga termini"** → campo **"n."**

**Causa**: Non hai inserito il numero della pratica edilizia oggetto di proroga.

**Soluzione**: Inserisci il numero della pratica nel campo **"n."** accanto al tipo pratica.

---

### ATTENZIONE ! Indicare la data della pratica.

**Dove si trova**: Sezione **"Proroga termini"** → campo **"del"** (data pratica)

**Causa**: Non hai inserito la data della pratica edilizia di riferimento.

**Soluzione**: Inserisci la data della pratica nel campo **"del"** nel formato **GG/MM/AAAA**.

---

### ATTENZIONE! Inserire la data nel formato gg/mm/aaaa. *(pratica di riferimento)*

**Causa**: La data della pratica edilizia di riferimento è in un formato non riconosciuto.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `10/06/2022` ✅. Errati: `10-06-2022` ❌, `2022/06/10` ❌.

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

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

**Causa**: Nessun mappale catastale inserito né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Verifiche effettuate

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Verifiche effettuate'.

**Dove si trova**: Sezione **"Verifiche effettuate"**

**Causa**: Non hai dichiarato a quale tipologia di titolo si riferisce la proroga.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"relativamente a permessi di costruire, SCIA, SCIA alternative al PdC, autorizzazioni paesaggistiche, dichiarazioni e autorizzazioni ambientali comunque denominate"** — dichiari che:
  1. i termini di inizio e/o ultimazione lavori non sono ancora decorsi
  2. il titolo è stato rilasciato o si è formato **entro il 31 dicembre 2025**
  3. il titolo non risulta in contrasto con nuovi strumenti urbanistici o piani di tutela (D.Lgs. 42/2004)
- ⚪ **"relativamente a convenzioni di lottizzazione e relativi piani attuativi, altro atto ad essi propedeutico"** → si attiva il campo **"denominazione"** obbligatorio (vedi sotto)

{: .warning }
> **Data limite nel modulo**: il testo delle verifiche effettuate riporta la data **31 dicembre 2025** come termine entro cui il titolo abilitativo deve essersi formato. Questa data è trascorsa rispetto al momento attuale (giugno 2026). Se il titolo si è formato successivamente al 31/12/2025, verificare con l'ufficio SUE la procedura applicabile prima di presentare questa comunicazione, in quanto il modulo potrebbe non essere aggiornato alla normativa vigente. Segnalare al team di sviluppo per aggiornamento del testo.

---

### ATTENZIONE ! Indicare la denominazione.

**Dove si trova**: Sezione **"Verifiche effettuate"** → campo di testo **"denominazione"** accanto al secondo radio button

**Causa**: Hai selezionato il radio button relativo a convenzioni di lottizzazione e piani attuativi ma non hai inserito la denominazione dell'atto propedeutico.

**Soluzione**:
1. Seleziona il secondo radio button ⚪ **"relativamente a convenzioni di lottizzazione e relativi piani attuativi, altro atto ad essi propedeutico di seguito denominato"**
2. Il campo di testo accanto al radio button si attiva
3. Inserisci la denominazione dell'atto propedeutico (es. `Convenzione di lottizzazione "Parco Nord"`, `Piano di Recupero approvato con delibera n. 45/2020`)

{: .note }
> Il campo denominazione è **abilitato solo dopo aver selezionato il secondo radio button**. Se il campo appare disabilitato (grigio), verifica di aver selezionato la voce corretta tra i due radio button delle verifiche effettuate.

---

## Consigli pratici Proroga Termini

### Prima di validare ✅

- [ ] Spunta **almeno una** delle due checkbox di proroga (inizio lavori e/o fine lavori)
- [ ] Se spunti proroga **inizio lavori**: inserisci la **data originale di inizio** nel formato GG/MM/AAAA
- [ ] Se spunti proroga **fine lavori**: inserisci la **data originale di fine** nel formato GG/MM/AAAA
- [ ] Inserisci la **tipologia** della pratica edilizia di riferimento
- [ ] Inserisci il **numero** della pratica
- [ ] Inserisci la **data** della pratica nel formato GG/MM/AAAA
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona la **tipologia di verifica** (uno dei due radio button)
- [ ] Se selezioni "convenzioni di lottizzazione": inserisci la **denominazione** dell'atto propedeutico
- [ ] **Salva** frequentemente

### Struttura delle due checkbox di proroga ⚠️

| Checkbox | Data richiesta | Applicabile a |
|---|---|---|
| Proroga **inizio** lavori | Data originale di inizio (`txtDataInizioOrig`) | Solo permessi di costruire, convenzioni di lottizzazione, piani attuativi |
| Proroga **fine** lavori | Data originale di fine (`txtDataFineOrig`) | Tutti i titoli (PdC, SCIA, convenzioni, piani attuativi) |

Entrambe le checkbox possono essere spuntate contemporaneamente se si richiede la proroga sia dell'inizio sia della fine. La nuova data prorogata (inizio + 48 mesi, fine + 48 mesi) non è attualmente richiesta dal sistema — i relativi campi e controlli sono disattivati nel codice.

### Errori frequenti Proroga 🔍

1. **Nessuna checkbox spuntata** → almeno una tra proroga inizio e proroga fine è obbligatoria
2. **Campo data disabilitato** → i campi data si abilitano solo dopo aver spuntato la checkbox corrispondente; se la data non si inserisce, verificare che la checkbox sia attiva
3. **Tipo pratica vuoto** → campo testuale libero, non un menu a discesa; va compilato manualmente con la tipologia del titolo
4. **Secondo radio "verifiche" senza denominazione** → selezionare il radio relativo a convenzioni/piani attuativi attiva obbligatoriamente il campo denominazione
5. **Data limite 31/12/2025** → il testo del modulo riporta una data già scaduta; per titoli formati dopo tale data, consultare il SUE prima di procedere

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
**Fonte**: Analisi codice `ValidaDatiProroga` e `DatiProroga.ascx`
