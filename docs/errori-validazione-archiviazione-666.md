---
title: Errori Archiviazione - Tutte le regioni
parent: Errori di validazione
nav_order: 15
description: Errori di validazione specifici per la Richiesta di Archiviazione (richiesta di annullamento pratica edilizia) - Guida dettagliata campo per campo
keywords: [archiviazione, annullamento pratica, richiesta archiviazione, rinuncia pratica edilizia, inefficacia pratica]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 2, Prat: 666 }  # Piemonte - Richiesta Archiviazione
  - { Reg: 1, Prat: 666 }  # Valle d'Aosta - Richiesta Archiviazione
  - { Reg: 3, Prat: 666 } # Liguria - Richiesta Archiviazione
  - { Reg: 4, Prat: 666 } # Lombardia - Richiesta Archiviazione
  - { Reg: 6, Prat: 666 } # Veneto - Richiesta Archiviazione
  - { Reg: 8, Prat: 666 } # Emilia-Romagna - Richiesta Archiviazione
  - { Reg: 12, Prat: 666 } # Lazio - Richiesta Archiviazione
  - { Reg: 13, Prat: 666 } # Abruzzo - Richiesta Archiviazione
  - { Reg: 15, Prat: 666 } # Campania - Richiesta Archiviazione
  - { Reg: 16, Prat: 666 } # Basilicata - Richiesta Archiviazione
  - { Reg: 17, Prat: 666 } # Puglia - Richiesta Archiviazione
  - { Reg: 18, Prat: 666 } # Calabria - Richiesta Archiviazione
  - { Reg: 19, Prat: 666 } # Sicilia - Richiesta Archiviazione
Fonte: Manuale
---

# Errori di validazione - Archiviazione
## Tutte le regioni

Guida completa agli errori specifici per la **Richiesta di Archiviazione**, la pratica con cui il titolare richiede l'annullamento e l'archiviazione di una pratica edilizia precedentemente presentata, valida per **tutte le regioni**.

{: .note }
> L'Archiviazione è una pratica autonoma con cui il titolare comunica allo Sportello Unico che intende rinunciare a una pratica edilizia già presentata. La richiesta determina automaticamente l'inefficacia della pratica originaria. È una pratica snella: i controlli di validazione riguardano solo la motivazione, i riferimenti alla pratica da archiviare e la localizzazione dell'immobile. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Motivazione e riferimento alla pratica da archiviare](#1-motivazione-e-riferimento-alla-pratica-da-archiviare)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)

---

## 1. Motivazione e riferimento alla pratica da archiviare

Questa sezione raccoglie la motivazione della richiesta di archiviazione e i riferimenti alla pratica edilizia originaria. I campi **Tipo di Pratica**, **Numero di Pratica** e **Data della Pratica** sono normalmente pre-compilati automaticamente dal sistema a partire dalla pratica originaria cui l'Archiviazione è collegata, e in quel caso appaiono disabilitati (grigi). Vengono controllati solo se abilitati.

{: .note }
> Se i campi Tipo Pratica, Numero e Data appaiono disabilitati e pre-compilati, il sistema ha già collegato la Richiesta di Archiviazione alla pratica originaria. Non è necessario compilarli manualmente e i relativi controlli non vengono eseguiti.

---

### ATTENZIONE ! Indicare la motivazione.

**Dove si trova**: Campo di testo **"per la seguente motivazione"** nella sezione **"Archiviazione"**

**Causa**: Il campo motivazione è vuoto. È l'unico campo sempre obbligatorio della sezione Archiviazione, indipendentemente da qualsiasi altra condizione.

**Soluzione**:
1. Vai alla sezione **"Archiviazione"**
2. Trova il campo di testo a più righe accanto a **"allo Sportello Unico per l'Edilizia che per la seguente motivazione"**
3. Inserisci la motivazione della richiesta di archiviazione
4. Esempi di motivazioni:
   - `Rinuncia all'intervento per sopravvenute ragioni economiche.`
   - `L'intervento non è più necessario a seguito di modifica del progetto originario.`
   - `Presentata in duplicato: la pratica corretta è la n. XXXX/2025.`
   - `La pratica è stata sostituita da una nuova presentazione con titolo diverso.`
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stato inserito il Tipo di Pratica.

**Dove si trova**: Campo **"Tipo di Pratica"** nella riga **"occorre procedere all'archiviazione della seguente pratica"**

**Causa**: Il campo tipo pratica è abilitato ma non è stato compilato.

**Soluzione**:
1. Trova il campo **"Tipo di Pratica"** nella sezione Archiviazione
2. Inserisci il tipo di pratica da archiviare (es. `CILA`, `SCIA`, `Permesso di Costruire`, `Denuncia Sismica`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stato inserito il Numero di Pratica.

**Dove si trova**: Campo **"numero"** nella riga della pratica da archiviare

**Causa**: Il campo del numero di pratica è abilitato ma non è stato compilato.

**Soluzione**:
1. Trova il campo **"numero"** accanto al tipo di pratica
2. Inserisci il numero di protocollo o identificativo della pratica da archiviare (es. `SCIA-123/2025`, `PDC-456/2024`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stato inserita la data della Pratica.

**Dove si trova**: Campo **"del"** nella riga della pratica da archiviare

**Causa**: Il campo data della pratica è abilitato e il numero è stato inserito, ma la data è vuota.

**Soluzione**:
1. Trova il campo **"del"** accanto al numero della pratica
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `15/03/2025`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica)

**Causa**: La data della pratica da archiviare è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**. Esempi corretti: `15/03/2025` ✅. Esempi errati: `15-03-2025` ❌, `2025/03/15` ❌.

---

## 2. Localizzazione dell'intervento

I controlli sulla localizzazione sono identici a quelli delle altre pratiche e si riferiscono all'immobile oggetto della pratica originaria da archiviare.

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
> I dati catastali devono corrispondere a quelli indicati nella pratica originaria che si intende archiviare.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Tieni premuto **CTRL** per selezionarne più di una.

---

## Consigli pratici Richiesta di Archiviazione

### Prima di validare ✅

- [ ] Compila la **motivazione** dell'archiviazione (campo testo libero — sempre obbligatorio)
- [ ] Verifica che il **tipo di pratica** sia indicato (se abilitato)
- [ ] Verifica che il **numero di pratica** sia indicato (se abilitato)
- [ ] Verifica che la **data della pratica** sia nel formato GG/MM/AAAA (se abilitata)
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] **Salva** frequentemente

### Errori frequenti Richiesta di Archiviazione 🔍

1. **Motivazione vuota** → è l'unico campo sempre obbligatorio e spesso dimenticato; inserisci almeno una frase che spieghi il motivo della rinuncia
2. **Campi pratica disabilitati** → se appaiono grigi il collegamento alla pratica originaria è automatico; non serve compilarli e il sistema non li controlla
3. **Campi pratica abilitati** → in rari casi il sistema non riesce a collegare automaticamente la pratica originaria; in questo caso tipo, numero e data sono tutti obbligatori

### Cosa succede dopo la validazione ⚠️

Il modulo riporta nel riquadro **"DICHIARA"** le conseguenze della Richiesta di Archiviazione:

1. Con riferimento alla pratica indicata, che **non è stato dato inizio ai lavori**
2. Che la comunicazione **sospende ogni istruttoria** eventualmente in corso e comporta automaticamente l'**inefficacia della pratica** inoltrata, salvo contraria comunicazione dello Sportello Unico
3. Che l'inefficacia è stata comunicata agli ulteriori soggetti coinvolti (titolari, tecnici incaricati, imprese esecutrici) indicati nella pratica originaria

{: .warning }
> Prima di procedere con l'Archiviazione verificare che i lavori non siano effettivamente iniziati. La dichiarazione mendace è soggetta alle sanzioni penali previste dagli artt. 483, 495 e 496 del Codice Penale e dall'art. 76 del D.P.R. n. 445/2000, oltre alla decadenza dai benefici conseguiti.

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
**Fonte**: Analisi codice ValidaDatiArchiviazione e DatiArchiviazione.ascx
