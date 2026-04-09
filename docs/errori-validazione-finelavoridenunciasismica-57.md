---
title: Errori Fine Lavori Denuncia Sismica - Regione Piemonte
parent: Errori di validazione
nav_order: 11
description: Errori di validazione specifici per la Fine Lavori Denuncia Sismica (FLDS) Regione Piemonte - Guida dettagliata campo per campo
keywords: [fine lavori denuncia sismica, FLDS, errori fine lavori sismica, validazione fine lavori strutturale, modello 5, zona PRG]
---

# Errori di validazione - Fine Lavori Denuncia Sismica
## Regione Piemonte

Guida completa agli errori specifici per la **Fine Lavori Denuncia Sismica** ai sensi degli artt. 65 e 93 del D.P.R. 06/06/2001 n. 380, relativa alla **Regione Piemonte**.

{: .note }
> La Fine Lavori Denuncia Sismica è la pratica che certifica l'ultimazione dei lavori strutturali oggetto di una Denuncia Sismica già presentata. È una pratica snella — i controlli di validazione riguardano principalmente le date e la localizzazione. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni Fine Lavori DS

1. [Riferimento alla Denuncia Sismica](#1-riferimento-alla-denuncia-sismica)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Data di ultimazione lavori e data dichiarazione](#3-data-di-ultimazione-lavori-e-data-dichiarazione)

---

## 1. Riferimento alla Denuncia Sismica

Questa sezione collega la Fine Lavori alla Denuncia Sismica originaria. I campi **Numero Pratica** e **Data Pratica** sono abilitati solo se non vengono pre-compilati automaticamente dal sistema (es. quando la DS originaria non è presente su GeoTecSUE oppure viene inserita manualmente).

{: .note }
> Se i campi numero e data della pratica appaiono disabilitati (grigi), il sistema ha già collegato automaticamente la Fine Lavori alla Denuncia Sismica originaria. In questo caso i controlli seguenti non vengono eseguiti e puoi procedere direttamente alla sezione successiva.

---

### ATTENZIONE ! Campo obbligatorio 'Numero Pratica' non inserito.

**Dove si trova**: Campo **"n."** nella riga **"con riferimento alla denuncia strutturale n. ... presentata in data ..."**

**Causa**: Il campo del numero della Denuncia Sismica originaria è abilitato ma non è stato compilato.

**Soluzione**:
1. Trova il campo **"n."** nella sezione di riferimento alla denuncia strutturale
2. Inserisci il numero della Denuncia Sismica originaria (es. `DS-123/2024`, `456/2024`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Campo obbligatorio 'Data Pratica' non inserito.

**Dove si trova**: Campo data nella riga **"con riferimento alla denuncia strutturale n. ... presentata in data ..."**

**Causa**: Il numero della DS è stato inserito ma la data di presentazione della Denuncia Sismica originaria è vuota.

**Soluzione**:
1. Trova il campo **"presentata in data"** accanto al numero della denuncia
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `15/03/2024`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica)

**Causa**: La data di presentazione della Denuncia Sismica originaria è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `15/03/2024` ✅. Esempi errati: `15-03-2024` ❌, `2024/03/15` ❌.

---

## 2. Localizzazione dell'intervento

I controlli sulla localizzazione sono identici a quelli delle altre pratiche. La sezione include anche i campi **Zona PRG vigente** e **Zona PRG adottato**, presenti anche nella Denuncia Sismica originaria.

{: .note }
> **Zona PRG vigente** e **Zona PRG adottato** sono campi obbligatori (contrassegnati con `CampoObbligatorio` nel codice) ma il loro controllo è gestito dal sistema di validazione lato client prima della validazione server. Se il sistema ti blocca su questi campi, compilali con la zona urbanistica indicata nel certificato di destinazione urbanistica (es. `Zona B2`, `Zona C1`).

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Dove si trova**: Campo testo **"Indirizzo"** (visibile con "Toponimo mancante" spuntato)

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**: Compila il campo di testo che appare accanto a "Toponimo mancante" (es. `Via Roma`, `Strada Provinciale 12`).

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

**Causa**: Non hai inserito almeno un mappale catastale (fabbricato o terreno).

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione (se presente), Foglio, Mappale e Subalterno (solo fabbricati)
3. Clicca l'**icona ✅ verde** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> I dati catastali devono corrispondere a quelli indicati nella Denuncia Sismica originaria.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Tieni premuto **CTRL** per selezionarne più di una.

---

## 3. Data di ultimazione lavori e data dichiarazione

Questa sezione contiene i due campi data più importanti della Fine Lavori DS: la data in cui i lavori strutturali sono stati effettivamente ultimati e la data della dichiarazione stessa (firma del tecnico certificante).

### ATTENZIONE ! Campo obbligatorio 'Data Fine Lavori' non inserito.

**Dove si trova**: Campo data nella riga **"che i lavori sono stati ultimati il ..."** nella sezione **"CERTIFICA"**

**Causa**: La data di ultimazione dei lavori strutturali è vuota.

**Soluzione**:
1. Vai alla sezione **"CERTIFICA"**
2. Trova il campo data accanto a **"che i lavori sono stati ultimati il"**
3. Clicca sull'**icona calendario** oppure inserisci manualmente
4. Formato: **GG/MM/AAAA** (es. `20/03/2026`)
5. La data deve essere **passata** (i lavori sono già terminati)
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La data di ultimazione lavori deve essere successiva alla data di presentazione della Denuncia Sismica originaria e compatibile con i tempi di esecuzione delle opere strutturali dichiarate.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori)

**Causa**: La data di ultimazione dei lavori è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `20/03/2026` ✅. Esempi errati: `20-03-2026` ❌, `2026/03/20` ❌.

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserito.

**Dove si trova**: Campo **"Data"** in fondo al modulo, nella sezione di firma del tecnico certificante

**Causa**: La data della dichiarazione (firma del tecnico) è vuota.

**Soluzione**:
1. Trova il campo **"Data"** in fondo al modulo nella sezione **"CERTIFICA"**
2. Inserisci la data odierna (o la data di firma del tecnico) nel formato **GG/MM/AAAA**
3. Usa l'**icona calendario** oppure inserisci manualmente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Questo campo è la **data della dichiarazione** del tecnico certificante, distinta dalla data di ultimazione lavori. Di norma coincide con la data di compilazione/firma del modulo.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data dichiarazione)

**Causa**: La data della dichiarazione del tecnico è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `09/04/2026` ✅. Esempi errati: `09-04-2026` ❌, `2026/04/09` ❌.

---

## Consigli pratici Fine Lavori DS

### Prima di validare ✅

- [ ] Verifica che il campo **"n."** della denuncia strutturale di riferimento sia compilato (se abilitato)
- [ ] Verifica che la **data della Denuncia Sismica originaria** sia compilata nel formato GG/MM/AAAA (se abilitata)
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] Compila la **Zona PRG vigente** e la **Zona PRG adottato**
- [ ] Inserisci la **data di ultimazione lavori** nel formato GG/MM/AAAA
- [ ] Inserisci la **data della dichiarazione** nel formato GG/MM/AAAA
- [ ] **Salva** frequentemente

### Errori frequenti Fine Lavori DS 🔍

1. **Data Fine Lavori mancante** → il campo è nella sezione "CERTIFICA", non nella localizzazione
2. **Data dichiarazione mancante** → campo separato dalla data ultimazione lavori, spesso confusi
3. **Formato data errato** → tutti e tre i campi data (pratica DS, ultimazione lavori, dichiarazione) richiedono il formato GG/MM/AAAA
4. **Campi n. pratica e data DS disabilitati** → se appaiono grigi il collegamento è automatico, non serve compilarli

### Campi esclusivi della Fine Lavori DS ⚠️

Rispetto alla Fine Lavori ordinaria, questa pratica ha:
- Il **riferimento esplicito alla Denuncia Sismica originaria** (numero e data pratica)
- La **Zona PRG vigente** e **Zona PRG adottato** (come nella DS)
- La dicitura **"CERTIFICA"** (invece di "COMUNICA") con il richiamo al **Modello 5** delle procedure attuative di gestione e controllo delle attività urbanistico-edilizie ai fini della prevenzione del rischio sismico
- **Due campi data distinti**: data ultimazione lavori + data dichiarazione del tecnico

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
3. Contatta [Assistenza](assistenza-tecnica.html) con screenshot

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiFineLavoriDS e DatiFineLavoriDS.ascx
