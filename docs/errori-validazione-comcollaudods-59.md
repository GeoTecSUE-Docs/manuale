---
title: Errori Comunicazione Collaudo DS - Regione Piemonte
parent: Errori di validazione
nav_order: 11
description: Errori di validazione specifici per la Comunicazione del Certificato di Collaudo Strutturale o della Dichiarazione di Regolare Esecuzione della Denuncia Sismica - Regione Piemonte
keywords: [collaudo strutturale, dichiarazione regolare esecuzione, denuncia sismica, CCDS, comunicazione collaudo, art. 67 DPR 380, zona PRG]
IDRegione: 2
IDTipoPratica: 59
Fonte: Manuale
---

# Errori di validazione - Comunicazione Collaudo o Dichiarazione di Regolare Esecuzione
## Denuncia Sismica — Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione del Certificato di Collaudo Strutturale o della Dichiarazione di Regolare Esecuzione** della Denuncia Sismica ai sensi dell'art. 67 del D.P.R. 06/06/2001 n. 380, relativa alla **Regione Piemonte**.

{: .note }
> Questa pratica **trasmette** al Comune o allo Sportello Unico uno dei due documenti conclusivi delle procedure sismiche: il **Certificato di Collaudo Strutturale** (art. 67 c. 7, per interventi ordinari) oppure la **Dichiarazione di Regolare Esecuzione** resa dal Direttore dei Lavori (art. 67 c. 8-bis, riservata agli interventi di riparazione o locali su edificio esistente). I due documenti sono mutuamente esclusivi. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Riferimento alla Denuncia Sismica](#1-riferimento-alla-denuncia-sismica)
2. [Documento trasmesso — Collaudo o Dichiarazione di Regolare Esecuzione](#2-documento-trasmesso--collaudo-o-dichiarazione-di-regolare-esecuzione)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Data della dichiarazione](#4-data-della-dichiarazione)

---

## 1. Riferimento alla Denuncia Sismica

Come nella Fine Lavori DS, i campi **Numero Pratica** e **Data Pratica** sono abilitati solo se il collegamento alla DS originaria non avviene automaticamente dal sistema.

{: .note }
> Se i campi numero e data della pratica appaiono disabilitati (grigi), il sistema ha già collegato automaticamente la Comunicazione Collaudo alla Denuncia Sismica originaria. I controlli seguenti non vengono eseguiti e puoi procedere direttamente alla sezione successiva.

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

## 2. Documento trasmesso — Collaudo o Dichiarazione di Regolare Esecuzione

Questa è la sezione centrale della pratica. Nella sezione **"TRASMETTE"** devi spuntare **una delle due checkbox** e compilare la relativa data. I due documenti corrispondono a due casistiche distinte previste dall'art. 67 del D.P.R. 380/2001.

{: .warning }
> Le due checkbox non sono mutuamente esclusive a livello di interfaccia, ma nella pratica si spunta **solo una** delle due: o si trasmette il collaudo strutturale (art. 67 c. 7) oppure la dichiarazione di regolare esecuzione (art. 67 c. 8-bis). Spuntarle entrambe è incoerente con le disposizioni normative.

---

### Opzione 1 — Certificato di collaudo strutturale (art. 67 c. 7)

Spunta questa checkbox se stai trasmettendo il **certificato di collaudo strutturale** rilasciato dal collaudatore nominato, previsto per gli interventi ordinari soggetti a Denuncia Sismica.

#### ATTENZIONE ! Campo obbligatorio 'Data certificato collaudo strutturale' non inserito.

**Dove si trova**: Campo data accanto alla checkbox **"certificato di collaudo strutturale in data ... previsto dall'art. 67, comma 7 del D.P.R. n. 380/2001"**

**Causa**: Hai spuntato ☑ la checkbox del collaudo strutturale ma non hai inserito la data del certificato.

**Soluzione**:
1. Trova il campo data che si abilita dopo aver spuntato la checkbox del collaudo strutturale
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `20/03/2026`)
4. Inserisci la data del certificato di collaudo strutturale
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La data del certificato di collaudo è quella in cui il collaudatore ha firmato il documento, non la data di trasmissione allo Sportello Unico.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data collaudo strutturale)

**Causa**: La data del certificato di collaudo strutturale è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `20/03/2026` ✅. Esempi errati: `20-03-2026` ❌, `2026/03/20` ❌.

---

### Opzione 2 — Dichiarazione di Regolare Esecuzione (art. 67 c. 8-bis)

Spunta questa checkbox se stai trasmettendo la **dichiarazione di regolare esecuzione** resa dal Direttore dei Lavori, riservata agli **interventi di riparazione o locali su edificio esistente** che non richiedono la nomina del collaudatore.

#### ATTENZIONE ! Campo obbligatorio 'Data dichiarazione regolare esecuzione' non inserito.

**Dove si trova**: Campo data accanto alla checkbox **"dichiarazione di regolare esecuzione resa dal direttore dei lavori in data ... ai sensi dell'art. 67, comma 8-bis del D.P.R. n. 380/2001"**

**Causa**: Hai spuntato ☑ la checkbox della dichiarazione di regolare esecuzione ma non hai inserito la data della dichiarazione.

**Soluzione**:
1. Trova il campo data che si abilita dopo aver spuntato la checkbox della dichiarazione di regolare esecuzione
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `20/03/2026`)
4. Inserisci la data in cui il Direttore dei Lavori ha firmato la dichiarazione
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La Dichiarazione di Regolare Esecuzione (DRE) è prevista dall'art. 67 c. 8-bis per gli interventi che nella Denuncia Sismica originaria erano stati dichiarati come **"interventi locali"** (quelli che non necessitano del collaudatore). Se nella DS hai dichiarato che l'intervento necessita di collaudo, devi usare l'Opzione 1.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data dichiarazione regolare esecuzione)

**Causa**: La data della dichiarazione di regolare esecuzione è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `20/03/2026` ✅. Esempi errati: `20-03-2026` ❌, `2026/03/20` ❌.

---

## 3. Localizzazione dell'intervento

I controlli sulla localizzazione sono identici a quelli della Fine Lavori DS e delle altre pratiche della suite sismica. Sono presenti anche i campi **Zona PRG vigente** e **Zona PRG adottato** (validazione solo lato client).

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

## 4. Data della dichiarazione

### ATTENZIONE ! Campo obbligatorio 'Data' non inserito.

**Dove si trova**: Campo **"Data"** in fondo al modulo, nella sezione **"TRASMETTE"**

**Causa**: La data della trasmissione (firma del tecnico o del collaudatore) è vuota. Questo campo è sempre obbligatorio, indipendentemente da quale delle due checkbox è stata spuntata.

**Soluzione**:
1. Trova il campo **"Data"** in fondo al modulo
2. Inserisci la data odierna (o la data di firma) nel formato **GG/MM/AAAA**
3. Usa l'**icona calendario** oppure inserisci manualmente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Questo campo è la **data della trasmissione**, distinta dalla data del certificato di collaudo o della dichiarazione di regolare esecuzione. Di norma coincide con la data di compilazione del modulo.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data trasmissione)

**Causa**: La data della trasmissione è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `09/04/2026` ✅. Esempi errati: `09-04-2026` ❌, `2026/04/09` ❌.

---

## Consigli pratici Comunicazione Collaudo Denuncia Sismica

### Prima di validare ✅

- [ ] Verifica che il campo **"n."** della denuncia strutturale di riferimento sia compilato (se abilitato)
- [ ] Verifica che la **data della Denuncia Sismica originaria** sia compilata nel formato GG/MM/AAAA (se abilitata)
- [ ] Spunta **una sola checkbox** tra collaudo strutturale e dichiarazione di regolare esecuzione
- [ ] Inserisci la **data del documento** corrispondente alla checkbox spuntata (collaudo o DRE) nel formato GG/MM/AAAA
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] Compila la **Zona PRG vigente** e la **Zona PRG adottato**
- [ ] Inserisci la **data della trasmissione** in fondo al modulo nel formato GG/MM/AAAA
- [ ] **Salva** frequentemente

### Quale documento trasmettere? ⚖️

La scelta tra le due opzioni dipende da quanto dichiarato nella **Denuncia Sismica originaria** alla sezione "Collaudo delle opere":

- Se nella DS è stato dichiarato **"necessita di nomina del collaudatore"** → trasmetti il **Certificato di Collaudo Strutturale** (art. 67 c. 7), spunta la prima checkbox
- Se nella DS è stato dichiarato **"non necessita di nomina del collaudatore"** (intervento locale) → trasmetti la **Dichiarazione di Regolare Esecuzione** del DL (art. 67 c. 8-bis), spunta la seconda checkbox

### Errori frequenti Comunicazione Collaudo Denuncia Sismica 🔍

1. **Nessuna checkbox spuntata** → il sistema non mostra un errore esplicito per questa mancanza, ma la pratica risulta incompleta; ricordati di spuntare almeno una delle due opzioni
2. **Data del documento mancante** → dopo aver spuntato una checkbox il campo data si abilita; non dimenticare di compilarlo
3. **Formato data errato** → tutti i campi data richiedono il formato GG/MM/AAAA
4. **Data pratica DS disabilitata** → se appare grigia il collegamento è automatico, non serve compilarla
5. **Confusione tra le tre date** → il modulo ha fino a tre campi data distinti: data della DS originaria (se abilitata) + data del collaudo/DRE + data della trasmissione finale

### Differenze rispetto alla Fine Lavori Denuncia Sismica ⚠️

| Aspetto | Fine Lavori Denuncia Sismica | Comunicazione Collaudo Denuncia Sismica |
|---|---|---|
| Dicitura sezione principale | **CERTIFICA** | **TRASMETTE** |
| Cosa si comunica | Data ultimazione lavori strutturali | Certificato collaudo o DRE |
| Riferimento normativo | Modello 5 procedure sismiche | Art. 67 c. 7 o c. 8-bis D.P.R. 380/2001 |
| Campi data nel modulo | 2 (ultimazione + dichiarazione) | 2 o 3 (collaudo/DRE + trasmissione, + eventuale DS) |
| Momento di presentazione | Dopo l'ultimazione dei lavori | Dopo il collaudo o la DRE |

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
**Fonte**: Analisi codice ValidaDatiComunicazCollaudoDS e DatiComunicazCollaudoDS.ascx
