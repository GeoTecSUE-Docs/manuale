---
title: Errori Relazione Struttura Ultimata DS - Regione Piemonte
parent: Errori di validazione
nav_order: 12
description: Errori di validazione specifici per la Comunicazione della Relazione a Struttura Ultimata della Denuncia Sismica (Modello 6) - Regione Piemonte
keywords: [relazione struttura ultimata, denuncia sismica, modello 6, RSU, comunicazione struttura ultimata, zona PRG, procedure sismiche]
IDRegione: 2
IDTipoPratica: 58
Fonte: Manuale
---

# Errori di validazione - Relazione a Struttura Ultimata
## Denuncia Sismica — Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione della Relazione a Struttura Ultimata** della Denuncia Sismica, ai sensi delle procedure attuative di gestione e controllo delle attività urbanistico-edilizie ai fini della prevenzione del rischio sismico (Modello 6), relativa alla **Regione Piemonte**.

{: .note }
> La Relazione a Struttura Ultimata è il documento con cui il progettista strutturale **comunica** allo Sportello Unico la relazione redatta al termine dell'esecuzione delle strutture, allegando il **Modello 6** delle procedure sismiche. Si colloca cronologicamente dopo la Fine Lavori DS e prima (o contestualmente) alla Comunicazione Collaudo DS. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Riferimento alla Denuncia Sismica](#1-riferimento-alla-denuncia-sismica)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Data della relazione e data della comunicazione](#3-data-della-relazione-e-data-della-comunicazione)

---

## 1. Riferimento alla Denuncia Sismica

Come nelle altre pratiche della famiglia sismica (Fine Lavori DS, Comunicazione Collaudo DS), i campi **Numero Pratica** e **Data Pratica** sono abilitati solo se il collegamento alla DS originaria non avviene automaticamente dal sistema.

{: .note }
> Se i campi numero e data della pratica appaiono disabilitati (grigi), il sistema ha già collegato automaticamente la Relazione a Struttura Ultimata alla Denuncia Sismica originaria. I controlli seguenti non vengono eseguiti e puoi procedere direttamente alla sezione successiva.

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

I controlli sulla localizzazione sono identici a quelli delle altre pratiche della famiglia sismica. Sono presenti anche i campi **Zona PRG vigente** e **Zona PRG adottato** (validazione solo lato client, non controllati dal server).

{: .note }
> **Zona PRG vigente** e **Zona PRG adottato** sono contrassegnati come `CampoObbligatorio` nell'interfaccia ma non sono verificati dalla validazione server-side. Se il sistema ti blocca su questi campi, compilali con la zona urbanistica indicata nel certificato di destinazione urbanistica (es. `Zona B2`, `Zona C1`).

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

## 3. Data della relazione e data della comunicazione

Questa sezione contiene i due campi data della pratica: la data in cui il progettista strutturale ha redatto la relazione a struttura ultimata, e la data della comunicazione stessa (firma).

### ATTENZIONE ! Campo obbligatorio 'Data Fine Lavori' non inserito.

**Dove si trova**: Campo data nella riga **"che la relazione a struttura ultimata è stata redatta in data ..."** nella sezione **"COMUNICA"**

**Causa**: La data di redazione della relazione a struttura ultimata è vuota.

{: .note }
> Il campo si chiama tecnicamente `txtDataFineLavori` nel codice, ma nel modulo corrisponde alla **data di redazione della relazione a struttura ultimata**, non a una data di fine lavori in senso stretto. Il nome nel messaggio di errore può risultare fuorviante: si tratta della data in cui il progettista strutturale ha firmato e redatto la relazione allegata (Modello 6).

**Soluzione**:
1. Vai alla sezione **"COMUNICA"**
2. Trova il campo data accanto a **"che la relazione a struttura ultimata è stata redatta in data"**
3. Clicca sull'**icona calendario** oppure inserisci manualmente
4. Formato: **GG/MM/AAAA** (es. `20/03/2026`)
5. Inserisci la data in cui il progettista strutturale ha redatto la relazione
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data relazione)

**Causa**: La data di redazione della relazione a struttura ultimata è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `20/03/2026` ✅. Esempi errati: `20-03-2026` ❌, `2026/03/20` ❌.

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserito.

**Dove si trova**: Campo **"Data"** in fondo al modulo, nella sezione **"COMUNICA"**

**Causa**: La data della comunicazione (firma del tecnico) è vuota.

**Soluzione**:
1. Trova il campo **"Data"** in fondo al modulo
2. Inserisci la data odierna (o la data di firma) nel formato **GG/MM/AAAA**
3. Usa l'**icona calendario** oppure inserisci manualmente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Questo campo è la **data della comunicazione**, distinta dalla data di redazione della relazione. Di norma coincide con la data di presentazione allo Sportello Unico.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data comunicazione)

**Causa**: La data della comunicazione è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `09/04/2026` ✅. Esempi errati: `09-04-2026` ❌, `2026/04/09` ❌.

---

## Consigli pratici Relazione a Struttura Ultimata Denuncia Sismica

### Prima di validare ✅

- [ ] Verifica che il campo **"n."** della denuncia strutturale di riferimento sia compilato (se abilitato)
- [ ] Verifica che la **data della Denuncia Sismica originaria** sia compilata nel formato GG/MM/AAAA (se abilitata)
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] Compila la **Zona PRG vigente** e la **Zona PRG adottato**
- [ ] Inserisci la **data di redazione della relazione a struttura ultimata** nel formato GG/MM/AAAA
- [ ] Inserisci la **data della comunicazione** in fondo al modulo nel formato GG/MM/AAAA
- [ ] **Salva** frequentemente

### Errori frequenti Relazione a Struttura Ultimata Denuncia Sismica 🔍

1. **"Data Fine Lavori" non inserita** → nonostante il nome del campo nel messaggio di errore, si tratta della **data di redazione della relazione a struttura ultimata** (Modello 6), non di una data di fine lavori
2. **Data comunicazione mancante** → campo separato dalla data di redazione della relazione, in fondo al modulo
3. **Formato data errato** → tutti i campi data richiedono il formato GG/MM/AAAA
4. **Campi n. pratica e data DS disabilitati** → se appaiono grigi il collegamento è automatico, non serve compilarli

### Posizione nella sequenza delle pratiche sismiche ⚙️

Le pratiche della famiglia Denuncia Sismica si presentano in questo ordine cronologico:

1. **Denuncia Sismica** — alla presentazione del progetto strutturale, prima dell'inizio dei lavori
2. **Fine Lavori Denuncia Sismica** — alla conclusione dei lavori strutturali (Modello 5)
3. **Relazione a Struttura Ultimata DS** — dopo l'ultimazione delle strutture, con la relazione del progettista strutturale (Modello 6)
4. **Comunicazione Collaudo DS** — dopo il collaudo strutturale o la dichiarazione di regolare esecuzione (art. 67 D.P.R. 380/2001)

### Confronto con le altre pratiche sismiche ⚠️

| Aspetto | Fine Lavori DS | Relazione Struttura Ultimata DS | Comunicazione Collaudo DS |
|---|---|---|---|
| Dicitura sezione principale | **CERTIFICA** | **COMUNICA** | **TRASMETTE** |
| Modello allegato | Modello 5 | Modello 6 | — (collaudo o DRE) |
| Campo data principale | Data ultimazione lavori | Data redazione relazione | Data collaudo o DRE |
| Campi data totali | 2 | 2 | 2 o 3 |

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
**Fonte**: Analisi codice ValidaDatiRelazioneSU e DatiRelazioneSU.ascx
