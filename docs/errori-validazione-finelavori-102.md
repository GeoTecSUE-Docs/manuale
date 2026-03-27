---
title: Errori Fine Lavori - Regione Piemonte
parent: Errori di validazione
nav_order: 3
description: Errori di validazione specifici per la Comunicazione di Fine Lavori Regione Piemonte - Guida dettagliata campo per campo
keywords: [fine lavori, errori fine lavori, validazione fine lavori, ultimazione lavori, localizzazione, titolo abilitativo]
---

# Errori di validazione - Fine Lavori Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione di Fine Lavori** relativa alla **Regione Piemonte**.

{: .note }
> Questa guida copre tutti i controlli di validazione della Fine Lavori. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni Fine Lavori

La validazione Fine Lavori è suddivisa in **sezioni tematiche**. Clicca per andare direttamente alla sezione:

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Comunicazione di ultimazione lavori](#2-comunicazione-di-ultimazione-lavori)
3. [Titolo abilitativo di riferimento](#3-titolo-abilitativo-di-riferimento)
4. [Data e luogo](#4-data-e-luogo)

---

## 1. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo testo **"Indirizzo"** (visibile quando è spuntato "Toponimo mancante")

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente nel campo di testo.

**Soluzione**:
1. Vai a **"Localizzazione dell'intervento"**
2. Verifica di aver spuntato ☑ **"Toponimo mancante"**
3. Compila il campo di testo che appare (es. `Via Roma`, `Strada Provinciale 45`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Usa "Toponimo mancante" solo se la via non è presente nel menu a discesa del Comune.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**

**Causa**: Non hai selezionato nessun indirizzo dal menu a discesa (e non hai spuntato "Toponimo mancante").

**Soluzione**:
1. Vai a **"Localizzazione dell'intervento"**
2. Clicca sul menu a discesa **"Indirizzo"** e seleziona la via corretta
3. Se la via non è presente nel menu: spunta ☑ **"Toponimo mancante"** e inseriscila manualmente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Dove si trova**: Campo **"CAP"** nella sezione Localizzazione

**Causa**: Il CAP non è stato inserito.

**Soluzione**:
1. Trova il campo **"CAP"**
2. Inserisci il CAP: esattamente **5 cifre** (es. `10121`)
3. Nessuno spazio, nessun trattino
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Dove si trova**: Campo **"N. Civico"** nella sezione Localizzazione

**Causa**: Il numero civico non è stato inserito.

**Soluzione**:
1. Trova il campo **"N. Civico"**
2. Inserisci il numero civico dell'immobile (es. `15`, `22/A`, `8 bis`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Dove si trova**: Sezione **"Localizzazione"** → tabelle **"Fabbricati"** e **"Terreni"**

**Causa**: Non hai inserito almeno un mappale catastale (fabbricato o terreno).

**Soluzione**:
1. Vai a **"Localizzazione dell'intervento"**
2. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
3. Compila i dati catastali richiesti:
   - **Sezione**: (se presente, altrimenti lascia vuoto)
   - **Foglio**: numero foglio catastale
   - **Mappale**: numero particella
   - **Subalterno**: (solo fabbricati, se esiste)
4. Clicca l'**icona ✅ verde** per salvare la riga
5. Verifica che la riga appaia nella tabella
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> I dati catastali si trovano nella visura catastale dell'immobile (Agenzia delle Entrate o servizi online). Devono corrispondere a quelli indicati nel titolo abilitativo originario.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Dove si trova**: Campo **"Avente destinazione d'uso"** nella sezione Localizzazione

**Causa**: Non hai selezionato la destinazione d'uso dell'immobile.

**Soluzione**:
1. Trova il campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**
2. Seleziona almeno una destinazione d'uso (Residenziale, Produttivo, Commerciale, Agricolo, ecc.)
3. Per selezionare più voci: tieni premuto **CTRL** e clicca sulle voci desiderate
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 2. Comunicazione di ultimazione lavori

### ATTENZIONE ! Inserire la data di ultimazione lavori.

**Dove si trova**: Campo **"che in data ... i lavori sono stati ultimati"** nella sezione COMUNICA

**Causa**: Il campo data di ultimazione dei lavori è vuoto.

**Soluzione**:
1. Vai alla sezione **"COMUNICA"**
2. Trova il campo data accanto a **"che in data ... i lavori sono stati ultimati"**
3. Clicca sull'**icona calendario** oppure inserisci manualmente
4. Formato: **GG/MM/AAAA** (es. `15/03/2026`)
5. La data deve essere **passata** (i lavori sono già terminati)
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La data di ultimazione lavori deve essere coerente con la durata massima prevista dal titolo abilitativo originario (permesso di costruire, SCIA, ecc.).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Ultimazione lavori'.

**Dove si trova**: Sezione **"COMUNICA"** → opzioni sotto la data di ultimazione

**Causa**: Hai inserito la data ma non hai selezionato la modalità di completamento dei lavori.

**Soluzione**:
1. Dopo aver inserito la data di ultimazione
2. Seleziona **una delle tre opzioni**:
   - ⚪ **"completamente"** → I lavori sono terminati al 100%
   - ⚪ **"in forma parziale come da planimetria allegata"** → I lavori sono parzialmente conclusi (allega planimetria)
   - ⚪ **"esaustiva degli ambiti delle precedenti comunicazioni di fine lavori parziali e completa le precedenti fine lavori parziali"** → Chiusura di una o più fine lavori parziali precedenti (allega planimetria)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> Se selezioni la seconda o la terza opzione, ricorda di allegare la planimetria che individua le opere concluse!

---

## 3. Titolo abilitativo di riferimento

Questa sezione raccoglie i dati del titolo edilizio (permesso di costruire, SCIA, CILA, ecc.) che ha legittimato i lavori di cui si comunica la fine.

### ATTENZIONE ! Indicare il tipo di pratica.

**Dove si trova**: Campo di testo **"che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente:"**

**Causa**: Non hai indicato la tipologia del titolo abilitativo di riferimento.

**Soluzione**:
1. Trova il campo di testo nella sezione **"COMUNICA"**
2. Inserisci la tipologia del titolo che ha autorizzato i lavori
3. Esempi:
   - `Permesso di Costruire`
   - `SCIA`
   - `CILA`
   - `DIA`
   - `Concessione Edilizia`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Campo obbligatorio 'Prot. / N.' non inserito.

**Dove si trova**: Campo **"prot. / n."** nella sezione del titolo abilitativo

**Causa**: Non hai inserito il numero di protocollo o il numero del titolo abilitativo.

**Soluzione**:
1. Trova il campo **"prot. / n."**
2. Inserisci il numero del titolo abilitativo di riferimento
3. Esempi: `456/2022`, `SCIA-123/2023`, `PDC 78/2021`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il numero si trova nella ricevuta o nel provvedimento del titolo originario. Per le SCIA, usa il numero di protocollo assegnato dallo Sportello Unico al momento della presentazione.

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserita.

**Dove si trova**: Campo **"del"** accanto al numero di protocollo del titolo abilitativo

**Causa**: Hai inserito il tipo e il numero del titolo ma non hai inserito la data.

**Soluzione**:
1. Trova il campo **"del"** accanto al campo **"prot. / n."**
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `10/05/2022`)
4. Inserisci la data del titolo abilitativo originario
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 4. Data e luogo

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Campo **"data"** nel riquadro finale delle dichiarazioni

**Causa**: Il campo data della dichiarazione è vuoto.

**Soluzione**:
1. Scorri fino al riquadro finale con i campi **"data"** e **"luogo"**
2. Compila il campo **"data"** con la data odierna (o la data di firma)
3. Formato: **GG/MM/AAAA** (es. `26/03/2026`)
4. Usa l'**icona calendario** oppure inserisci manualmente
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Dove si trova**: Campo **"data"** nel riquadro finale

**Causa**: La data della dichiarazione è stata inserita in un formato non valido.

**Soluzione**:
1. Trova il campo **"data"**
2. Verifica il formato: **GG/MM/AAAA**
3. Esempi **corretti**: `01/01/2026` ✅, `26/03/2026` ✅, `31/12/2025` ✅
4. Esempi **errati**: `1/1/2026` ❌, `26-03-2026` ❌, `2026/03/26` ❌
5. Usa il **calendario** cliccando sull'icona 📅 accanto al campo
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Campo **"luogo"** nel riquadro finale delle dichiarazioni

**Causa**: Il campo luogo della dichiarazione è vuoto.

**Soluzione**:
1. Trova il campo **"luogo"** accanto alla data
2. Inserisci il comune dove viene firmata la dichiarazione
3. Di solito corrisponde al comune dell'intervento
4. Esempio: `Torino`, `Biella`, `Novara`
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## Consigli pratici Fine Lavori

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] Inserisci la **data di ultimazione lavori**
- [ ] Seleziona la **modalità di completamento** (completamente / parziale / esaustiva)
- [ ] Indica il **tipo di pratica** che ha legittimato i lavori
- [ ] Inserisci il **numero di protocollo** del titolo abilitativo
- [ ] Inserisci la **data** del titolo abilitativo
- [ ] Inserisci **data** e **luogo** finali della dichiarazione
- [ ] **Salva** frequentemente

### Errori frequenti Fine Lavori 🔍

1. **Data ultimazione lavori mancante** → Inserisci la data nel campo "che in data ... i lavori sono stati ultimati"
2. **Modalità completamento non selezionata** → Scegli tra completamente / parziale / esaustiva
3. **Tipo pratica non indicato** → Scrivi la tipologia del titolo (es. `Permesso di Costruire`, `SCIA`)
4. **Numero protocollo mancante** → Recuperalo dalla ricevuta del titolo abilitativo originario
5. **Data titolo mancante** → Inserisci la data nel campo "del" accanto al numero di protocollo
6. **Destinazione d'uso non selezionata** → Usa CTRL+click per selezionare dal menu

### Campi spesso dimenticati ⚠️

- Modalità di completamento (completamente / parziale / esaustiva)
- Tipo di pratica che ha legittimato i lavori
- Data del titolo abilitativo (campo "del" accanto al numero protocollo)
- Destinazione d'uso (menu multi-selezione con CTRL+click)

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla messaggio esatto)
2. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
3. Consulta [Compilare istanza](compilare-istanza.html)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Compilare un'istanza](compilare-istanza.html) - Guida completa compilazione
- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Marzo 2026
**Fonte**: Analisi codice ValidaDatiFineLavori e DatiFineLavori.ascx
