---
title: Errori Segnalazione Certificata di Agibilità - Regione Piemonte
parent: Errori di validazione
nav_order: 5
description: Errori di validazione specifici per la Segnalazione Certificata di Agibilità (SCA) Regione Piemonte - Guida dettagliata campo per campo
keywords: [agibilità, SCA, segnalazione certificata agibilità, errori agibilità, validazione agibilità, titolo abilitativo, fine lavori]
---

# Errori di validazione - Segnalazione Certificata di Agibilità Regione Piemonte

Guida completa agli errori specifici per la **Segnalazione Certificata di Agibilità (SCAGI)** relativa alla **Regione Piemonte**.

{: .note }
> Questa guida copre tutti i controlli di validazione della SCAGI. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni SCAGI

La validazione SCAGI è suddivisa in **sezioni tematiche**. Clicca per andare direttamente alla sezione:

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Titolo abilitativo edilizio](#2-titolo-abilitativo-edilizio)
3. [Dichiarazioni per fine lavori](#3-dichiarazioni-per-fine-lavori)
4. [Presentazione agibilità](#4-presentazione-agibilità)
5. [Data e luogo](#5-data-e-luogo)
6. [Informativa privacy](#6-informativa-privacy)
7. [Professionista incaricato nei soggetti coinvolti](#7-professionista-incaricato-nei-soggetti-coinvolti)

---

## 1. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo testo **"Indirizzo"** (visibile quando è spuntato "Toponimo mancante")

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**:
1. Vai a **"Localizzazione dell'intervento"**
2. Verifica di aver spuntato ☑ **"Toponimo mancante"**
3. Compila il campo di testo che appare (es. `Via Roma`, `Strada Provinciale 45`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Usa "Toponimo mancante" solo se la via non è presente nel menu a discesa del Comune.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Dove si trova**: Menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**

**Causa**: Non hai selezionato nessun indirizzo dal menu a discesa (e non hai spuntato "Toponimo mancante").

**Soluzione**:
1. Vai a **"Localizzazione dell'intervento"**
2. Clicca sul menu a discesa **"Indirizzo"** e seleziona la via corretta
3. Se la via non è presente: spunta ☑ **"Toponimo mancante"** e inseriscila manualmente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Dove si trova**: Campo **"CAP"** nella sezione Localizzazione

**Causa**: Il CAP non è stato inserito.

**Soluzione**:
1. Trova il campo **"CAP"**
2. Inserisci esattamente **5 cifre** (es. `10121`)
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
3. Compila i dati catastali:
   - **Sezione**: (se presente, altrimenti lascia vuoto)
   - **Foglio**: numero foglio catastale
   - **Mappale**: numero particella
   - **Subalterno**: (solo fabbricati, se esiste)
4. Clicca l'**icona ✅ verde** per salvare la riga
5. Verifica che la riga appaia nella tabella
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> I dati catastali devono corrispondere a quelli indicati nel titolo abilitativo originario (PdC, SCIA, CILA).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Dove si trova**: Campo **"Avente destinazione d'uso"** nella sezione Localizzazione

**Causa**: Non hai selezionato la destinazione d'uso dell'immobile.

**Soluzione**:
1. Trova il campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**
2. Seleziona almeno una destinazione d'uso (Residenziale, Produttivo, Commerciale, Agricolo, ecc.)
3. Per selezionare più voci: tieni premuto **CTRL** e clicca
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 2. Titolo abilitativo edilizio

Questa sezione permette di indicare il titolo edilizio (o i titoli) che hanno legittimato i lavori di cui si chiede l'agibilità. Esistono **due blocchi distinti**:

- **Blocco principale** (`cmbTitoliAbitEdilizi` + `txtNTitEdilizio` + `txtDataTitEdilizio`): per titoli **non presenti su GeoTecSUE**, da compilare manualmente
- **Blocco GeoTecSUE** (`cmbTitoliAbitEdilizi1` + `cmbTitoloRif1`): per titoli **già presenti su GeoTecSUE**, da selezionare dalla lista pratiche

È sufficiente compilare **uno dei due blocchi**. Il sistema richiede che almeno uno dei due menu principali abbia una selezione valida.

---

### ATTENZIONE ! Selezionare il titolo abitativo edilizio.

**Dove si trova**: Sezione **"DICHIARA"** → primo blocco — menu a discesa **"che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente (selezionare questa voce se il titolo non è presente su GeoTecSUE)"**

**Causa**: Nessuno dei due menu principali ha una selezione valida — né il menu del blocco manuale né quello del blocco GeoTecSUE.

**Soluzione**:

**Opzione A — Titolo non presente su GeoTecSUE** (compilazione manuale):
1. Trova il **primo menu a discesa** `cmbTitoliAbitEdilizi`
2. Seleziona la tipologia del titolo (es. `Permesso di Costruire`, `SCIA`, `CILA`, `Concessione Edilizia`)
3. Compila il campo **"prot. / n."** con il numero del titolo
4. Compila il campo **"del"** con la data nel formato **GG/MM/AAAA**
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

**Opzione B — Titolo presente su GeoTecSUE** (selezione dalla lista):
1. Trova il **secondo blocco** (visibile solo se abilitato dal sistema) con il menu `cmbTitoliAbitEdilizi1`
2. Seleziona la tipologia del titolo
3. Seleziona la pratica specifica dal menu `cmbTitoloRif1` che si popola automaticamente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> **Quale blocco usare?** Se la pratica edilizia originaria è stata gestita su GeoTecSUE (il gestionale del Comune), usa il blocco GeoTecSUE per collegare direttamente le pratiche. Se il titolo è precedente all'uso di GeoTecSUE o proviene da altro sistema, usa il blocco manuale.

---

### ATTENZIONE ! Selezionare il riferimento della pratica.

**Dove si trova**: Menu a discesa **`cmbTitoloRif1`** nel blocco GeoTecSUE

**Causa**: Hai selezionato la tipologia nel menu `cmbTitoliAbitEdilizi1` (blocco GeoTecSUE) ma non hai selezionato la pratica specifica dal secondo menu che si è popolato.

**Soluzione**:
1. Trova il menu a discesa **`cmbTitoloRif1`** (quello che si popola dopo la selezione del tipo)
2. Clicca sul menu e seleziona la pratica di riferimento dall'elenco
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il menu `cmbTitoloRif1` mostra le pratiche presenti su GeoTecSUE corrispondenti alla tipologia selezionata. Se non vedi la pratica attesa, verifica di aver selezionato la tipologia corretta nel primo menu.

---

### ATTENZIONE ! Inserire il numero.

**Dove si trova**: Campo **"prot. / n."** nel blocco manuale (accanto al primo menu `cmbTitoliAbitEdilizi`)

**Causa**: Hai selezionato la tipologia del titolo nel blocco manuale ma non hai inserito il numero di protocollo o il numero del titolo.

**Soluzione**:
1. Trova il campo **"prot. / n."** accanto al menu del titolo
2. Inserisci il numero del titolo abilitativo (es. `PDC-123/2022`, `SCIA-456/2023`, `45/2020`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Campo **"del"** nel blocco manuale (accanto a "prot. / n.")

**Causa**: Hai selezionato la tipologia e inserito il numero, ma non hai inserito la data del titolo.

**Soluzione**:
1. Trova il campo **"del"** accanto al campo "prot. / n."
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `10/05/2022`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data titolo abilitativo)

**Dove si trova**: Campo **"del"** nel blocco manuale del titolo abilitativo

**Causa**: La data del titolo è stata inserita in un formato non valido.

**Soluzione**:
1. Trova il campo data del titolo abilitativo
2. Verifica il formato: **GG/MM/AAAA**
3. Esempi **corretti**: `10/05/2022` ✅, `01/01/2020` ✅
4. Esempi **errati**: `10-05-2022` ❌, `2022/05/10` ❌, `10/5/22` ❌
5. Usa il **calendario** 📅 accanto al campo
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 3. Dichiarazioni per fine lavori

Questa sezione richiede di dichiarare se la fine lavori è già stata presentata separatamente oppure se viene comunicata contestualmente alla SCAGI.

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Dichiarazioni per fine lavori'.

**Dove si trova**: Seconda sezione **"DICHIARA"** → opzioni sulla comunicazione di fine lavori

**Causa**: Non hai selezionato nessuna delle due opzioni relative alla fine lavori.

**Soluzione**:
1. Vai alla sezione **"DICHIARA"** (seconda)
2. Seleziona **una delle due opzioni**:
   - ⚪ **"che la comunicazione di fine lavori è stata già presentata prot. / n. ... del ..."** → la fine lavori è stata protocollata separatamente; compila n. e data
   - ⚪ **"che la presente segnalazione vale come comunicazione di fine lavori e a tal fine attesta che gli stessi sono stati ultimati in data ..."** → la SCAGI incorpora anche la fine lavori; inserisci la data di ultimazione e la tipologia
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### Opzione 1 — Fine lavori già presentata

#### ATTENZIONE ! Inserire il prot. / n. di pratica.

**Dove si trova**: Campo **"prot. / n."** accanto alla prima opzione (fine lavori già presentata)

**Causa**: Hai selezionato "la comunicazione di fine lavori è stata già presentata" ma non hai inserito il numero di protocollo della fine lavori.

**Soluzione**:
1. Trova il campo **"prot. / n."** nella riga della prima opzione
2. Inserisci il numero di protocollo della comunicazione di fine lavori già presentata (es. `FL-78/2025`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

#### ATTENZIONE ! Campo obbligatorio 'Data pratica' non inserito.

**Dove si trova**: Campo **"del"** accanto al numero di protocollo della fine lavori già presentata

**Causa**: Numero di protocollo inserito ma data della fine lavori mancante.

**Soluzione**:
1. Trova il campo **"del"** accanto al numero della fine lavori
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA**
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data pratica fine lavori)

**Causa**: La data della comunicazione di fine lavori è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA** (es. `15/01/2026`).

---

### Opzione 2 — Fine lavori contestuale alla SCAGI

#### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Dove si trova**: Campo data accanto a **"gli stessi sono stati ultimati in data"** (seconda opzione)

**Causa**: Hai selezionato "la presente segnalazione vale come comunicazione di fine lavori" ma non hai inserito la data di ultimazione dei lavori.

**Soluzione**:
1. Trova il campo data accanto a "gli stessi sono stati ultimati in data"
2. Inserisci la data effettiva di ultimazione lavori nel formato **GG/MM/AAAA**
3. La data deve essere **passata**
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori contestuale)

**Causa**: La data di ultimazione lavori è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo ultimazione lavori'.

**Dove si trova**: Opzioni di completamento sotto il campo data fine lavori (seconda opzione)

**Causa**: Hai inserito la data di fine lavori ma non hai selezionato la modalità di completamento.

**Soluzione**:
1. Dopo aver inserito la data di ultimazione
2. Seleziona **una delle due opzioni**:
   - ⚪ **"completamente"** → I lavori sono terminati al 100%
   - ⚪ **"in forma parziale come da planimetria allegata"** → I lavori sono parzialmente conclusi (allega planimetria)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> Se selezioni "in forma parziale", ricorda di allegare la planimetria che individua le parti completate!

---

## 4. Presentazione agibilità

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione agibilità'.

**Dove si trova**: Sezione **"PRESENTA"** → opzioni SCIA / SCIA Unica

**Causa**: Non hai selezionato per quale tipo di agibilità stai presentando la SCAGI.

**Soluzione**:
1. Vai alla sezione **"PRESENTA"**
2. Seleziona **una delle sei opzioni** disponibili:

   **SCIA per:**
   - ⚪ **"l'agibilità relativa all'immobile oggetto dell'intervento edilizio"** → agibilità totale dell'intero immobile
   - ⚪ **"l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione"** (art. 24, comma 4, lett. a) → per complessi edilizi con più edifici o porzioni distinte
   - ⚪ **"l'agibilità parziale relativa a singole unità immobiliari"** (art. 24, comma 4, lett. b) → per singole U.I. nell'ambito di un intervento più ampio

   **SCIA Unica per:**
   - ⚪ **"l'agibilità relativa all'immobile oggetto dell'intervento edilizio"** → agibilità totale presentata con altre segnalazioni contestuali
   - ⚪ **"l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione"** (art. 24, comma 4, lett. a)
   - ⚪ **"l'agibilità parziale relativa a singole unità immobiliari"** (art. 24, comma 4, lett. b)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> **SCIA o SCIA Unica?** Usa la **SCIA** quando la segnalazione di agibilità è autonoma. Usa la **SCIA Unica** quando presenti contestualmente altre segnalazioni o comunicazioni necessarie (indicate nel quadro riepilogativo allegato).

---

## 5. Data e luogo

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Campo **"data"** nel riquadro finale

**Causa**: Il campo data della dichiarazione è vuoto.

**Soluzione**:
1. Scorri fino al riquadro finale con i campi **"data"** e **"luogo"**
2. Compila il campo **"data"** con la data odierna (o la data di firma)
3. Formato: **GG/MM/AAAA** (es. `26/03/2026`)
4. Usa l'**icona calendario** oppure inserisci manualmente
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data dichiarazione)

**Causa**: La data della dichiarazione finale è in formato errato.

**Soluzione**:
1. Trova il campo **"data"**
2. Verifica il formato: **GG/MM/AAAA**
3. Esempi **corretti**: `26/03/2026` ✅, `01/01/2026` ✅
4. Esempi **errati**: `26-03-2026` ❌, `2026/03/26` ❌, `26/3/26` ❌
5. Usa il **calendario** 📅 accanto al campo
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Campo **"luogo"** nel riquadro finale

**Causa**: Il campo luogo è vuoto.

**Soluzione**:
1. Trova il campo **"luogo"** accanto alla data
2. Inserisci il comune dove viene firmata la dichiarazione
3. Esempio: `Torino`, `Biella`, `Novara`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 6. Informativa privacy

### ATTENZIONE ! Selezionare la presa visione dell'informativa sul trattamento dei dati personali.

**Dove si trova**: Checkbox in fondo alla sezione **"INFORMATIVA SUL TRATTAMENTO DEI DATI PERSONALI"**

**Causa**: Non hai spuntato la checkbox di presa visione dell'informativa privacy (Reg. UE n. 2016/679).

**Soluzione**:
1. Scorri fino alla sezione **"INFORMATIVA SUL TRATTAMENTO DEI DATI PERSONALI"** in fondo al modulo
2. Leggi l'informativa
3. Spunta ☑ la checkbox: **"Il/la sottoscritto/a dichiara di aver letto l'informativa sul trattamento dei dati personali pubblicata sul sito istituzionale del SUAP/SUE"**
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> Questa è l'**unica pratica** della suite che richiede esplicitamente la spunta della privacy come condizione per la validazione. Nelle altre pratiche l'informativa è presente ma non ha un controllo attivo.

---

## 7. Professionista incaricato nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Professionista incaricato per Agibilità o come Direttore Lavori.

**Dove si trova**: Sezione **"Soggetti coinvolti"** → Tecnici

**Causa**: Non hai aggiunto nessun tecnico con ruolo **Tecnico Agibilità (TA)** o **Direttore Lavori (DR)** tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Compila i dati del professionista
4. Nel campo **"Ruolo"** seleziona:
   - **"Tecnico Agibilità" (TA)** → il professionista che assevera l'agibilità
   - oppure **"Direttore Lavori" (DR)** → se il DL coincide con il professionista dell'agibilità
5. Salva il tecnico
6. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Per la SCAGI è sufficiente che esista **almeno uno** tra TA e DR. Non è richiesto il Progettista (PR).

{: .warning }
> Il professionista che firma la **Sezione B** ("Attestazione del direttore dei lavori o del professionista abilitato") deve essere presente nei soggetti coinvolti con ruolo TA o DR.

---

## Consigli pratici SCAGI

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** (o spunta "Toponimo mancante" e inseriscilo manualmente)
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Seleziona la **destinazione d'uso** (CTRL+click per più voci)
- [ ] Indica il **titolo abilitativo** che ha legittimato i lavori (blocco manuale o GeoTecSUE)
- [ ] Se blocco manuale: compila **tipologia**, **numero** e **data** del titolo
- [ ] Se blocco GeoTecSUE: seleziona **tipologia** e poi la **pratica** dal secondo menu
- [ ] Seleziona la voce relativa alla **fine lavori** (già presentata o contestuale alla SCAGI)
- [ ] Se fine lavori già presentata: inserisci **n. protocollo** e **data**
- [ ] Se fine lavori contestuale: inserisci **data ultimazione** e seleziona **completamente / parziale**
- [ ] Seleziona la voce **"Presentazione agibilità"** (SCIA o SCIA Unica, totale o parziale)
- [ ] Inserisci **data** e **luogo** finali
- [ ] Spunta la **checkbox privacy** (obbligatoria per la SCAGI)
- [ ] Aggiungi almeno un tecnico con ruolo **TA** o **DR** nei soggetti coinvolti
- [ ] **Salva** frequentemente

### Errori frequenti SCAGI 🔍

1. **Nessun titolo abilitativo selezionato** → Compila il blocco manuale (tipologia + numero + data) oppure il blocco GeoTecSUE
2. **Riferimento GeoTecSUE mancante** → Dopo aver selezionato la tipologia nel blocco GeoTecSUE, seleziona anche la pratica dal secondo menu
3. **Fine lavori non dichiarata** → Scegli tra "già presentata" (con n. e data) o "contestuale" (con data ultimazione e tipo completamento)
4. **Tipo ultimazione mancante** → Se scegli la fine lavori contestuale, specifica sempre "completamente" o "parziale"
5. **Privacy non spuntata** → Scorri fino in fondo e spunta la checkbox dell'informativa
6. **Professionista agibilità assente** → Aggiungi tecnico con ruolo TA o DR nei soggetti coinvolti
7. **Presentazione agibilità non selezionata** → Scegli tra le 6 opzioni SCIA/SCIA Unica nella sezione PRESENTA

### Campi spesso dimenticati ⚠️

- Checkbox privacy in fondo al modulo (esclusiva della SCAGI)
- Riferimento pratica GeoTecSUE (secondo menu del blocco GeoTecSUE)
- Tipo ultimazione lavori (completamente / parziale) quando la fine lavori è contestuale
- Tecnico con ruolo TA o DR nei soggetti coinvolti
- Tipologia SCIA / SCIA Unica nella sezione PRESENTA

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

**Ultima revisione**: Marzo 2026
**Fonte**: Analisi codice ValidaDatiSegnalazioneCertAgibilita e DatiSCAGI.ascx
