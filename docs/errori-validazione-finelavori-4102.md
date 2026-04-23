---
title: Errori Fine Lavori - Regione Lombardia
parent: Errori di validazione
nav_order: 23
description: Errori di validazione specifici per la Comunicazione di Fine Lavori - Regione Lombardia
keywords: [fine lavori, comunicazione fine lavori, Lombardia, SCIA alternativa PdC, prestazione energetica, APE, risparmio energetico, anticaduta, coordinate UTM, privacy]
IDRegione: 4
IDTipoPratica: 4102
Fonte: Manuale
---

# Errori di validazione - Fine Lavori
## Regione Lombardia

Guida completa agli errori specifici per la **Comunicazione di Fine Lavori** relativa alla **Regione Lombardia**.

{: .note }
> Il Fine Lavori Lombardia è significativamente più articolato del Fine Lavori Piemonte. Include obbligatoriamente le **coordinate UTM WGS 84 32N**, tre dichiarazioni energetiche/strutturali con radio button (legittimazione da SCIA alt. PdC, prestazione energetica, risparmio energetico), la sezione **titolo edilizio** con cinque campi distinti, la **data di ultimazione** con modalità (completa/parziale), e la **Privacy** come checkbox obbligatoria. Le tre checkbox anticaduta sono facoltative. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Coordinate UTM](#2-coordinate-utm)
3. [Dichiarazioni sull'intervento](#3-dichiarazioni-sullintervento)
4. [Data di ultimazione e modalità](#4-data-di-ultimazione-e-modalità)
5. [Titolo edilizio di riferimento](#5-titolo-edilizio-di-riferimento)
6. [Normativa sulla privacy](#6-normativa-sulla-privacy)

---

## 1. Localizzazione dell'intervento

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**: Compila il campo di testo che appare accanto a "Toponimo mancante" (es. `Via Roma`, `Via Milano`).

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona la via dal menu a discesa, oppure spunta ☑ **"Toponimo mancante"** e inseriscila manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il CAP non è stato inserito.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `20121`). Nessuno spazio, nessun trattino.

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il numero civico non è stato inserito.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (es. `15`, `22/A`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non hai inserito almeno un mappale catastale.

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione (se presente), Foglio, Mappale e Subalterno (solo fabbricati)
3. Clicca l'**icona ✅ verde** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 2. Coordinate UTM

{: .warning }
> Le coordinate UTM WGS 84 32N sono **obbligatorie** nel Fine Lavori Lombardia. X deve essere tra 430.000 e 700.000, Y tra 4.800.000 e 5.700.000.

---

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Dove si trova**: Campo **"Coord. asse X"** nella sezione Coordinate dell'intervento

**Causa**: Il campo della coordinata X è vuoto.

**Soluzione**:
1. Trova la sezione **"Coordinate dell'intervento (UTM - WGS 84 32N)"** nella localizzazione
2. Inserisci la coordinata X nel campo **"Coord. asse X"**
3. La coordinata X deve essere compresa tra **430.000 e 700.000** (es. `514500`)
4. Usa il punto come separatore decimale (es. `514500.5`), non la virgola
5. Usa il pulsante **"Calcola Coordinate"** se disponibile per ricavarle dalla cartografia
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: La coordinata X inserita è fuori dal range valido, oppure contiene caratteri non numerici o usa la virgola come separatore decimale.

**Soluzione**: Verifica che la coordinata X sia un numero decimale compreso tra **430.000 e 700.000**. Usa il punto come separatore decimale, non la virgola.

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo della coordinata Y è vuoto.

**Soluzione**: Inserisci la coordinata Y: un numero compreso tra **4.800.000 e 5.700.000** (es. `5034200`).

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: La coordinata Y inserita è fuori dal range valido, oppure contiene caratteri non numerici.

**Soluzione**: Verifica che la coordinata Y sia un numero decimale compreso tra **4.800.000 e 5.700.000**. Usa il punto come separatore decimale.

---

## 3. Dichiarazioni sull'intervento

Questa sezione contiene tre coppie di radio button obbligatorie — tutte e tre devono essere compilate indipendentemente dall'una dall'altra. Seguono poi le tre checkbox anticaduta, che sono invece facoltative.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Legittimazione da SCIA'.

**Dove si trova**: Prima coppia di radio button nella sezione dichiarazioni → **"che l'intervento"**

**Causa**: Non hai dichiarato se l'intervento è legittimato da SCIA alternativa al Permesso di Costruire.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"non è legittimato da SCIA alternativa al permesso di costruire"**
- ⚪ **"è legittimato da SCIA alternativa al permesso di costruire"** → si allega il certificato di collaudo finale ai sensi dell'art. 23, comma 7, D.P.R. 380/2001

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Prestazione energetica degli edifici (D.Lgs. n. 192/2005)'.

**Dove si trova**: Seconda coppia di radio button → **"Prestazione energetica degli edifici (D.Lgs. n. 192/2005)"**

**Causa**: Non hai dichiarato se l'intervento è soggetto ai requisiti minimi di prestazione energetica.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"non è soggetto all'osservanza dei requisiti minimi di prestazione energetica"**
- ⚪ **"è soggetto all'osservanza dei requisiti minimi di prestazione energetica"** → si allega l'Attestato di Prestazione Energetica (APE) redatto da tecnico abilitato

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Risparmio energetico'.

**Dove si trova**: Terza coppia di radio button → **"Risparmio energetico"**

**Causa**: Non hai dichiarato se l'intervento è soggetto al deposito del progetto e della relazione tecnica sul risparmio energetico.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"non è soggetto al deposito del progetto e della relazione tecnica"** (art. 125 D.P.R. 380/2001 e D.Lgs. 192/2005)
- ⚪ **"è soggetto al deposito del progetto e della relazione tecnica"** → si allega dichiarazione asseverata di conformità delle opere realizzate rispetto al progetto e alla relazione tecnica

---

### Checkbox anticaduta (facoltative)

Le tre checkbox nella sezione **"Misure di prevenzione contro il rischio di caduta dall'alto"** (D.Lgs. 81/2008 e D.D.G. Sanità Regione Lombardia n. 119 del 14/1/2009) sono **completamente facoltative**: il codice di validazione non le controlla mai. Puoi spuntarle tutte, alcune o nessuna senza che la validazione produca errori.

Le tre opzioni disponibili sono: "non è soggetto alle disposizioni del D.Lgs. 81/2008", "è soggetto alle disposizioni del D.Lgs. 81/2008 e si allega il fascicolo dell'opera", e "si dichiara che l'installatore ha fornito attestazione di conformità dell'installazione". Consulta il tecnico per determinare quale o quali siano applicabili al tuo intervento.

Analogamente, la checkbox **"Modifiche rappresentazione cartografica"** (art. 42 c. 14 L.R. 12/2005) è facoltativa: va spuntata solo se l'intervento ha comportato modifiche alla rappresentazione cartografica del Database topografico.

---

## 4. Data di ultimazione e modalità

---

### ATTENZIONE ! Inserire la data di ultimazione lavori.

**Dove si trova**: Campo **"che in data ___ i lavori sono stati ultimati"**

**Causa**: Non hai inserito la data in cui i lavori sono stati completati.

**Soluzione**:
1. Trova il campo data accanto alla frase "che in data ___ i lavori sono stati ultimati"
2. Clicca sull'**icona calendario** oppure inserisci manualmente la data
3. Formato: **GG/MM/AAAA** (es. `15/03/2026`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il codice non verifica il formato della data di ultimazione lavori: se inserita in formato errato la pratica potrebbe essere salvata ma la data risulterà non valida nel sistema. Inserisci sempre la data nel formato GG/MM/AAAA.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Ultimazione lavori'.

**Dove si trova**: Sezione data ultimazione → due radio button sotto la data

**Causa**: Non hai dichiarato se i lavori sono stati ultimati completamente o solo parzialmente.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"completamente"**
- ⚪ **"in forma parziale come da planimetria allegata"** → assicurati di allegare la planimetria che documenta la parte completata

---

## 5. Titolo edilizio di riferimento

Questa sezione contiene cinque campi obbligatori che identificano il titolo edilizio (o comunicazione) che ha legittimato l'intervento. Tutti e cinque sono sempre richiesti.

{: .note }
> Il codice non verifica il formato della data (`txtDataProt`): se inserita in formato errato la pratica potrebbe essere salvata con data non valida. Inserisci sempre nel formato GG/MM/AAAA.

---

### ATTENZIONE ! Indicare il tipo di procedimento.

**Dove si trova**: Campo **"Tipo procedimento"** nella sezione "che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente"

**Causa**: Non hai inserito il tipo di procedimento edilizio che ha autorizzato i lavori.

**Soluzione**: Inserisci il tipo di procedimento nel campo **"Tipo procedimento"** (es. `CILA`, `SCIA`, `Permesso di Costruire`, `SCIA alternativa al PdC`).

---

### ATTENZIONE ! Indicare l'Ente Ricevente.

**Dove si trova**: Campo **"Ente ricevente"** accanto al tipo procedimento

**Causa**: Non hai indicato l'ente che ha ricevuto il titolo edilizio originario.

**Soluzione**: Inserisci il nome dell'ente nel campo **"Ente ricevente"** (es. `Comune di Milano`, `Comune di Bergamo SUE`).

---

### ATTENZIONE ! Campo obbligatorio 'Pratica edilizia' non inserito.

**Dove si trova**: Campo **"Pratica edilizia"** nella seconda riga della sezione titolo edilizio

**Causa**: Non hai indicato la tipologia o il riferimento della pratica edilizia.

**Soluzione**: Inserisci il riferimento alla pratica edilizia nel campo **"Pratica edilizia"** (es. `CILA 2024`, `SCIA n. 45/2023`, `PDC 12/2022`).

---

### ATTENZIONE ! Campo obbligatorio 'Prot. / N.' non inserito.

**Dove si trova**: Campo **"prot. / n."** nella riga della pratica edilizia

**Causa**: Non hai inserito il numero di protocollo o il numero assegnato al titolo edilizio.

**Soluzione**: Inserisci il numero di protocollo o il numero del titolo nel campo **"prot. / n."** (es. `PROT-2023-45678`, `123/2023`).

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserita.

**Dove si trova**: Campo **"del"** (data) nella riga della pratica edilizia

**Causa**: Non hai inserito la data del titolo edilizio.

**Soluzione**: Inserisci la data del titolo edilizio nel campo **"del"** nel formato **GG/MM/AAAA** (es. `15/06/2023`).

---

## 6. Normativa sulla privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione **"Rispetto della normativa sulla privacy"** → checkbox in fondo al modulo

**Causa**: Non hai dichiarato di aver letto l'informativa sul trattamento dei dati personali.

**Soluzione**: Spunta la checkbox **"di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune"**.

---

## Consigli pratici Fine Lavori Lombardia

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci le **coordinate UTM WGS 84 32N** (X tra 430.000–700.000, Y tra 4.800.000–5.700.000), separatore decimale con punto
- [ ] Seleziona la voce **"Legittimazione da SCIA"** (prima coppia di radio button)
- [ ] Seleziona la voce **"Prestazione energetica"** (seconda coppia di radio button)
- [ ] Seleziona la voce **"Risparmio energetico"** (terza coppia di radio button)
- [ ] Se applicabile: spunta le **checkbox anticaduta** (facoltative) e/o **"Modifiche rappresentazione cartografica"** (facoltativa)
- [ ] Inserisci la **data di ultimazione lavori** nel formato GG/MM/AAAA
- [ ] Seleziona la **modalità di ultimazione** (completamente / in forma parziale)
- [ ] Compila tutti e 5 i campi del **titolo edilizio**: Tipo procedimento, Ente ricevente, Pratica edilizia, Prot./N., Data
- [ ] Spunta la **checkbox Privacy**
- [ ] **Salva** frequentemente

### Differenze principali rispetto al Fine Lavori Piemonte ⚠️

Il Fine Lavori Lombardia è più complesso di quello Piemonte per diversi aspetti. Le **coordinate UTM** (X tra 430.000–700.000, Y tra 4.800.000–5.700.000) sono obbligatorie in Lombardia e assenti in Piemonte. Le **tre dichiarazioni energetiche** (legittimazione SCIA, prestazione energetica, risparmio energetico) sono specifiche della Lombardia. Il titolo edilizio ha **cinque campi distinti** (tipo procedimento, ente ricevente, pratica edilizia, prot./n., data) invece di un semplice n. e data. La **Privacy** è una checkbox obbligatoria in Lombardia, assente nel Fine Lavori Piemonte. Le **checkbox anticaduta** (D.Lgs. 81/2008 + D.D.G. 119/2009) sono facoltative e specifiche della Lombardia.

### Errori frequenti Fine Lavori Lombardia 🔍

1. **Coordinate UTM fuori range o con virgola** → usare il punto come separatore decimale (es. `514500.5` non `514500,5`)
2. **Una delle tre dichiarazioni energetiche non selezionata** → tutte e tre sono indipendenti e obbligatorie; il sistema le controlla in sequenza
3. **Data ultimazione mancante** → campo separato dai radio button, spesso saltato
4. **Tipo ultimazione non selezionato** → i due radio button (completamente / parziale) sotto la data sono obbligatori
5. **Uno dei cinque campi del titolo edilizio vuoto** → tutti e cinque obbligatori, il sistema li controlla in sequenza
6. **Privacy non spuntata** → checkbox in fondo al modulo, facile da dimenticare

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
**Fonte**: Analisi codice ValidaDatiFineLavoriLombardia e DatiFineLavoriLombardia.ascx
