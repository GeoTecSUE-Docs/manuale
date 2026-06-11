---
title: Errori Comunicazione di Agibilità - Regione Piemonte
parent: Errori di validazione
nav_order: 65
description: Errori di validazione specifici per la Comunicazione di Agibilità (CAGI) - Regione Piemonte (art. 25 c. 5-bis D.P.R. 380/2001)
keywords: [comunicazione agibilità, CAGI, Piemonte, art. 25 DPR 380, permesso costruire, SCIA, DIA, CILA, variante in corso d'opera, oggetto agibilità, impianti, abitabilità, agibilità parziale]
IDRegione: 2
IDTipoPratica: 11
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Agibilità (C.A.GI.)
## Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione di Agibilità (CAGI)** ai sensi dell'art. 25, comma 5-bis del D.P.R. 6 giugno 2001, n. 380 e ss.mm.ii. — Regione Piemonte.

{: .note }
> La CAGI Piemonte ha una struttura completamente diversa dalle altre pratiche del sistema. Non ha radio Titolarità, radio Impresa, radio Sicurezza o Contributo. Si articola in due blocchi: **DICHIARA** (titoli abilitativi di riferimento con eventuali varianti, descrizione, localizzazione) e **TRASMETTE** (oggetto dell'agibilità e documentazione allegata in 13 punti). La sezione "Titolarità" è basata su checkbox per i titoli edilizi (PdC, DIA, SCIA, CILA) ciascuna con una sotto-checkbox per la variante in corso d'opera — ogni checkbox spuntata richiede numero e data. Le checkbox dei titoli **non hanno un obbligo minimo** — tutte possono essere lasciate vuote senza errore. La sezione documentazione valida solo i 3 gruppi impianti (punto 12) e il punto 13 (precedente abitabilità/agibilità). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titoli abilitativi edilizi — sezione Titolarità](#1-titoli-abilitativi-edilizi--sezione-titolarità)
2. [Descrizione dell'intervento](#2-descrizione-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Oggetto dell'agibilità](#4-oggetto-dellagibilità)
5. [Documentazione — Punto 12 (Sicurezza impianti)](#5-documentazione--punto-12-sicurezza-impianti)
6. [Documentazione — Punto 13 (Precedente abitabilità/agibilità)](#6-documentazione--punto-13-precedente-abitabilitàagibilità)

---

## 1. Titoli abilitativi edilizi — sezione Titolarità

La sezione "Titolarità" contiene 4 checkbox principali per i titoli edilizi (PdC, DIA, SCIA, CILA), ciascuna con una sotto-checkbox per la variante in corso d'opera. Ogni checkbox principale spuntata attiva i campi numero e data obbligatori. Se anche la variante è spuntata, aggiunge un secondo blocco numero/data.

{: .note }
> Nessuna delle 8 checkbox ha un obbligo minimo: è tecnicamente possibile inviare la CAGI senza spuntare alcun titolo edilizio. Il validatore verifica solo che, **se** si spunta una checkbox, i relativi campi siano compilati correttamente.

---

### Permesso di Costruire (chkPdC1)

#### ATTENZIONE ! Inserire il numero. (PdC)

**Causa**: `chkPdC1` è spuntata ma `txtNPdC` è vuoto.

**Soluzione**: Inserisci il numero della pratica di Permesso di Costruire nel campo "n."

---

#### ATTENZIONE ! Inserire la data. (PdC)

**Causa**: `chkPdC1` è spuntata e il numero è compilato, ma `txtDataPdC` è vuoto.

**Soluzione**: Inserisci la data di presentazione del PdC nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (PdC)

**Causa**: La data del PdC non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire il numero. (PdC variante)

**Causa**: `chkPdC1` è spuntata ed è stata compilata, e anche `chkPdCVar` è spuntata, ma `txtNPdCVar` è vuoto.

**Soluzione**: Inserisci il numero della pratica di variante in corso d'opera al PdC.

---

#### ATTENZIONE ! Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (PdC variante)

**Causa**: `chkPdCVar` è spuntata ma `txtDataPdCVar` è vuoto o nel formato errato.

**Soluzione**: Inserisci la data della variante nel formato **GG/MM/AAAA**.

---

### Denuncia di Inizio Attività (chkDIA1)

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (DIA)

**Causa**: `chkDIA1` è spuntata ma mancano numero o data.

**Soluzione**: Compila il numero nel campo "n." e la data nel formato **GG/MM/AAAA** della D.I.A.

---

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (DIA variante)

**Causa**: `chkDIA1` è compilata e `chkDIAVar` è spuntata ma mancano numero o data della variante.

**Soluzione**: Compila numero e data (GG/MM/AAAA) della D.I.A. varianti in corso d'opera.

---

### S.C.I.A. (chkSCIA1)

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (SCIA)

**Causa**: `chkSCIA1` è spuntata ma mancano numero o data.

**Soluzione**: Compila il numero e la data (GG/MM/AAAA) della S.C.I.A.

---

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (SCIA variante)

**Causa**: `chkSCIA1` è compilata e `chkSCIAVar` è spuntata ma mancano numero o data.

**Soluzione**: Compila numero e data (GG/MM/AAAA) della S.C.I.A. varianti in corso d'opera.

---

### C.I.L.A. (chkCILA1)

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (CILA)

**Causa**: `chkCILA1` è spuntata ma mancano numero o data.

**Soluzione**: Compila il numero e la data (GG/MM/AAAA) della C.I.L.A.

---

#### ATTENZIONE ! Inserire il numero. / Inserire la data. / Inserire la data nel formato gg/mm/aaaa. (CILA variante)

**Causa**: `chkCILA1` è compilata e `chkCILAVar` è spuntata ma mancano numero o data.

**Soluzione**: Compila numero e data (GG/MM/AAAA) della C.I.L.A. varianti in corso d'opera.

{: .note }
> Il messaggio "ATTENZIONE ! Inserire il numero." e "ATTENZIONE ! Inserire la data." sono identici per tutti i titoli e le varianti — il sistema si ferma al primo campo mancante e non indica quale titolo specifico è incompleto. Verificare sistematicamente tutte le checkbox spuntate.

---

## 2. Descrizione dell'intervento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Titolarità" → campo multiriga `txtDescrizioneIntervento` "relativi all'intervento di" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto. Viene validato dopo il blocco dei titoli edilizi e prima della localizzazione.

**Soluzione**: Inserisci la descrizione dell'intervento edilizio (max **300 caratteri**).

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

## 4. Oggetto dell'agibilità

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Oggetto'.

**Dove si trova**: Sezione "TRASMETTE — Oggetto" → 5 radio button `$OggAgibilita`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei cinque radio button**:
- ⚪ **3_1** — "per tutta la costruzione" → nessun campo aggiuntivo
- ⚪ **3_2** — "per singole porzioni della costruzione (indicare quali)" → inserisci le porzioni nel campo `txtOggAgibilita3_2_1`
- ⚪ **3_3** — "per singole unità immobiliari (indicare gli estremi catastali)" → inserisci gli estremi catastali nel campo `txtOggAgibilita3_3_1`
- ⚪ **3_4** — "tutti gli edifici" → nessun campo aggiuntivo
- ⚪ **3_5** — "per i soli edifici (indicare quali)" → inserisci la specifica nel campo `txtOggAgibilita3_5_1`

---

### ATTENZIONE ! Inserire le singole porzioni della costruzione.

**Causa**: Hai selezionato 3_2 ma `txtOggAgibilita3_2_1` è vuoto.

**Soluzione**: Inserisci nel campo testo la specificazione delle porzioni della costruzione oggetto della comunicazione di agibilità (es. "piano terra, piano primo").

---

### ATTENZIONE ! Inserire le singole unità immobiliari.

**Causa**: Hai selezionato 3_3 ma `txtOggAgibilita3_3_1` è vuoto.

**Soluzione**: Inserisci gli estremi catastali delle singole unità immobiliari (es. "Foglio 12, Mappale 345, Sub. 1 e Sub. 2").

---

### ATTENZIONE ! Inserire i soli edifici.

**Causa**: Hai selezionato 3_5 ma `txtOggAgibilita3_5_1` è vuoto.

**Soluzione**: Inserisci la specificazione degli edifici a cui si riferisce la comunicazione.

---

## 5. Documentazione — Punto 12 (Sicurezza impianti)

Il punto 12 della documentazione da trasmettere riguarda le dichiarazioni di conformità degli impianti. Contiene 3 checkbox principali (`chkd_12_1`, `chkd_12_2`, `chkd_12_3`), ciascuna con 7 sotto-checkbox corrispondenti alle tipologie di impianto. Se si spunta una delle 3 checkbox principali, almeno una delle 7 sotto-checkbox deve essere selezionata.

---

### ATTENZIONE ! Selezionare almeno una voce. (chkd_12_1)

**Dove si trova**: Punto 12 → prima checkbox → "dichiarazioni di conformità dei seguenti impianti realizzati o modificati nelle **parti comuni** e attestazione di collaudo ove previsto"

**Causa**: `chkd_12_1` è spuntata ma nessuna delle 7 sotto-checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 7 tipologie di impianto nelle parti comuni:

Impianti elettrici, protezione scariche atmosferiche e automazione porte/cancelli/barriere; impianti radiotelevisivi, antenne ed elettronici; impianti di riscaldamento, climatizzazione, condizionamento e refrigerazione; impianti idrici e sanitari; impianti per la distribuzione e l'utilizzazione di gas; impianti di sollevamento (ascensori, montacarichi, scale mobili); impianti di protezione antincendio.

---

### ATTENZIONE ! Selezionare almeno una voce. (chkd_12_2)

**Dove si trova**: Punto 12 → seconda checkbox → "dichiarazioni di conformità dei seguenti impianti, essendo stati modificati o realizzati nel corso dei lavori nelle **singole unità immobiliari** e attestazione di collaudo ove previsto"

**Causa**: `chkd_12_2` è spuntata ma nessuna delle 7 sotto-checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 7 tipologie di impianto nelle singole unità immobiliari (stesse tipologie del punto 12_1).

---

### ATTENZIONE ! Selezionare almeno una voce. (chkd_12_3)

**Dove si trova**: Punto 12 → terza checkbox → "dichiarazione di rispondenza, per i seguenti impianti presenti, qualora le dichiarazioni di conformità non siano state prodotte o non siano più reperibili, per gli impianti eseguiti **prima dell'entrata in vigore del D.M. 37/2008**"

**Causa**: `chkd_12_3` è spuntata ma nessuna delle 7 sotto-checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 7 tipologie di impianto per la dichiarazione di rispondenza.

{: .note }
> Le sotto-checkbox dei 3 gruppi (12_1, 12_2, 12_3) si abilitano solo dopo aver spuntato la rispettiva checkbox principale. Se le sotto-checkbox non sono cliccabili, verificare di aver spuntato la checkbox principale del gruppo. Il messaggio d'errore "ATTENZIONE ! Selezionare almeno una voce." è identico per tutti e 3 i gruppi.

---

## 6. Documentazione — Punto 13 (Precedente abitabilità/agibilità)

### ATTENZIONE ! Inserire il numero della pratica.

**Dove si trova**: Punto 13 → "di precedente certificato di Abitabilità/Agibilità" → campo `txtNPraticad_13_1` "Pratica n."

**Causa**: `chkd_13_1` è spuntata ma il campo del numero pratica è vuoto.

**Soluzione**: Inserisci il numero della pratica del precedente certificato di abitabilità o agibilità.

---

### ATTENZIONE ! Inserire la data della pratica.

**Causa**: `chkd_13_1` è spuntata e il numero è compilato, ma il campo `txtDataPraticad_13_1` "rilasciato in data" è vuoto.

**Soluzione**: Inserisci la data di rilascio del precedente certificato di abitabilità/agibilità.

{: .note }
> A differenza dei campi data dei titoli edilizi (sezione 1), la data del punto 13 (`txtDataPraticad_13_1`) non viene verificata nel formato GG/MM/AAAA — il validatore controlla solo che il campo non sia vuoto. È presente il datepicker nel modulo, ma non è obbligatorio usarlo.

---

## Consigli pratici — CAGI Piemonte

### Prima di validare ✅

- [ ] Per ogni checkbox titolo spuntata (PdC, DIA, SCIA, CILA): inserisci **numero** e **data** (GG/MM/AAAA)
- [ ] Per ogni checkbox variante spuntata: inserisci **numero** e **data** (GG/MM/AAAA)
- [ ] Inserisci la **descrizione dell'intervento** (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona l'**oggetto dell'agibilità** (3_1..3_5); se 3_2/3_3/3_5: inserisci la specificazione nel campo testo
- [ ] Per ogni checkbox 12_1/12_2/12_3 spuntata: seleziona **almeno una tipologia di impianto**
- [ ] Se `chkd_13_1` spuntata: inserisci **numero pratica** e **data rilascio**

### Struttura della sezione documentazione ℹ️

La sezione TRASMETTE ha 13 punti di documentazione. Di questi, il validatore controlla **solo**:

I 3 gruppi del punto 12 (impianti): se la checkbox principale (12_1, 12_2 o 12_3) è spuntata, almeno una delle 7 sotto-checkbox deve essere selezionata.

Il punto 13 (precedente abitabilità/agibilità): se `chkd_13_1` è spuntata, numero pratica e data sono obbligatori.

Tutti gli altri punti (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11 e le singole checkbox delle sotto-sezioni) **non vengono validati** — sono informativi e facoltativi dal punto di vista del sistema.

### Ordine di validazione ⚠️

Titoli edilizi (PdC → DIA → SCIA → CILA, con relative varianti) → Descrizione → Localizzazione → Oggetto agibilità → Documentazione 12_1 → 12_2 → 12_3 → 13

### Errori frequenti 🔍

1. **Messaggio "Inserire il numero" senza indicare quale** → il validatore scorre i titoli in sequenza; se compare questo errore, controllare sistematicamente tutte le checkbox spuntate (PdC, PdCVar, DIA, DIAVar, SCIA, SCIAVar, CILA, CILAVar) e verificare che abbiano numero e data compilati
2. **Spuntato 12_1/12_2/12_3 senza sotto-checkbox** → le sotto-checkbox sono disabilitate di default; si abilitano solo dopo aver spuntato la checkbox principale; assicurarsi che la pagina si aggiorni e poi spuntare almeno una tipologia
3. **Oggetto con campo testo vuoto** → le opzioni 3_2, 3_3 e 3_5 richiedono specificazione obbligatoria; l'opzione 3_1 e 3_4 non richiedono testo
4. **Variante spuntata senza aver compilato il titolo principale** → il validatore controlla prima il titolo principale (se spuntato), poi la variante (se spuntata) — ma non richiede che il titolo principale sia spuntato per spuntare la variante; verificare di aver compilato correttamente l'intero blocco

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
**Fonte**: Analisi codice ValidaDatiComunicazioneAgibilita e DatiCAGI.ascx
