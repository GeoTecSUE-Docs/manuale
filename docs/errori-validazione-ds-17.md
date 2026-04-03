---
title: Errori Denuncia Sismica - Regione Piemonte
parent: Errori di validazione
nav_order: 6
description: Errori di validazione specifici per la Denuncia Sismica (DS) Regione Piemonte - Guida dettagliata campo per campo
keywords: [denuncia sismica, DS, errori denuncia sismica, validazione sismica, progettista strutturale, direttore lavori strutturali, collaudo, vincolo idrogeologico]
---

# Errori di validazione - Denuncia Sismica Regione Piemonte

Guida completa agli errori specifici per la **Denuncia Sismica (DS)** ai sensi degli artt. 65 e 93 del D.P.R. 06/06/2001 n. 380, relativa alla **Regione Piemonte**.

{: .note }
> Questa guida copre tutti i controlli di validazione della Denuncia Sismica. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Struttura della Denuncia Sismica

La DS è strutturalmente diversa dalle altre pratiche della suite: non usa il sistema "Soggetti coinvolti" ma richiede la compilazione diretta e obbligatoria di **quattro schede professionisti** (Progettista architettonico, Direttore lavori architettonici, Progettista strutturale, Direttore lavori strutturali) e della scheda **Costruttore**, con tutti i dati anagrafici inline nel modulo.

---

## Indice sezioni Denuncia Sismica

1. [Titolo abilitativo di riferimento](#1-titolo-abilitativo-di-riferimento)
2. [Descrizione sintetica dell'intervento](#2-descrizione-sintetica-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Dati dei quattro professionisti](#4-dati-dei-quattro-professionisti)
5. [Dati del Costruttore](#5-dati-del-costruttore)
6. [Strumento urbanistico esecutivo](#6-strumento-urbanistico-esecutivo)
7. [Vincolo idrogeologico](#7-vincolo-idrogeologico)
8. [Precedenti lavori sul fabbricato](#8-precedenti-lavori-sul-fabbricato)
9. [Collaudo delle opere](#9-collaudo-delle-opere)
10. [Dichiarazione del progettista strutturale](#10-dichiarazione-del-progettista-strutturale)

---

## 1. Titolo abilitativo di riferimento

### ATTENZIONE ! Inserire il procedimento edilizio/titolo abilitativo.

**Dove si trova**: Sezione **"Titolare del seguente procedimento edilizio/titolo abilitativo in corso di validità"** → campo **"Procedimento edilizio/titolo abilitativo"**

**Causa**: Non hai indicato la tipologia del titolo edilizio collegato alla denuncia sismica.

**Soluzione**:
1. Vai alla sezione **"Titolare del seguente procedimento edilizio/titolo abilitativo in corso di validità"**
2. Trova il campo di testo **"Procedimento edilizio/titolo abilitativo (PdC, SCIA, Delibera GC...)"**
3. Inserisci la tipologia del titolo (es. `Permesso di Costruire`, `SCIA`, `Delibera GC`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La Denuncia Sismica è sempre collegata a un titolo edilizio in corso di validità che ha autorizzato i lavori strutturali.

---

### ATTENZIONE ! Inserire il numero del procedimento edilizio/titolo abilitativo.

**Dove si trova**: Campo **"N. Procedimento abilitativo"** nella sezione del titolo

**Causa**: Hai indicato la tipologia del titolo ma non hai inserito il numero.

**Soluzione**:
1. Trova il campo **"N. Procedimento abilitativo"**
2. Inserisci il numero del titolo (es. `PDC-123/2025`, `SCIA-456/2024`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data del procedimento edilizio/titolo abilitativo.

**Dove si trova**: Campo **"Data"** nella sezione del titolo abilitativo

**Causa**: Tipologia e numero del titolo inseriti, ma data mancante.

**Soluzione**:
1. Trova il campo **"Data"** nella stessa riga del titolo abilitativo
2. Clicca sull'**icona calendario** oppure inserisci manualmente
3. Formato: **GG/MM/AAAA** (es. `10/05/2025`)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data titolo abilitativo)

**Causa**: La data del titolo abilitativo è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA** (es. `10/05/2025`). Esempi errati: `10-05-2025` ❌, `2025/05/10` ❌.

---

## 2. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione **"Descrizione sintetica dell'intervento"** → campo di testo multiriga

**Causa**: Il campo descrizione è vuoto.

**Soluzione**:
1. Vai alla sezione **"Descrizione sintetica dell'intervento"**
2. Inserisci una descrizione chiara e sintetica dei lavori strutturali
3. Esempi:
   - `Nuova costruzione di fabbricato residenziale in muratura portante su due piani fuori terra.`
   - `Ristrutturazione strutturale con inserimento di nuovi setti portanti in c.a. e rinforzo fondazioni.`
   - `Sopraelevazione di un piano sul fabbricato esistente con struttura in acciaio.`
4. Massimo **300 caratteri**
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo testo (visibile con "Toponimo mancante" spuntato)

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**:
1. Compila il campo di testo accanto a "Toponimo mancante" (es. `Via Roma`, `Strada Provinciale 12`)
2. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Dove si trova**: Menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**

**Causa**: Nessun indirizzo selezionato dal menu e "Toponimo mancante" non spuntato.

**Soluzione**:
1. Seleziona la via dal menu a discesa
2. Se non è presente: spunta ☑ **"Toponimo mancante"** e inseriscila manualmente
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il CAP non è stato inserito.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`).

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il numero civico non è stato inserito.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (es. `15`, `22/A`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non hai inserito almeno un mappale catastale.

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Clicca l'**icona ✅** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso"** (usa **CTRL+click** per più voci).

---

### ATTENZIONE ! Inserire la zona PRG vigente.

**Dove si trova**: Campo **"Zona PRG vigente"** nella sezione Localizzazione

**Causa**: Il campo zona PRG vigente è vuoto.

**Soluzione**:
1. Trova il campo **"Zona PRG vigente"**
2. Inserisci la zona urbanistica prevista dal PRG vigente del Comune
3. Esempi: `Zona B2`, `Zone omogenea C1`, `Zona agricola E`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La zona PRG si trova nel certificato di destinazione urbanistica o consultando il PRG del Comune sul sito dell'ente.

---

### ATTENZIONE ! Inserire la zona PRG adottato.

**Dove si trova**: Campo **"Zona PRG adottato"** nella sezione Localizzazione

**Causa**: Il campo zona PRG adottato è vuoto.

**Soluzione**:
1. Trova il campo **"Zona PRG adottato"**
2. Inserisci la zona prevista dal PRG adottato (se diverso da quello vigente) oppure ripeti la stessa zona del PRG vigente se non ci sono varianti adottate
3. Esempi: `Zona B2`, `Nessuna variante adottata`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la classe di sintesi della pericolosità geomorfologica.

**Dove si trova**: Campo **"Classe di sintesi della pericolosità geomorfologica"** nella sezione Localizzazione

**Causa**: Il campo pericolosità geomorfologica è vuoto.

**Soluzione**:
1. Trova il campo **"Classe di sintesi della pericolosità geomorfologica"**
2. Inserisci la classe di pericolosità geomorfologica dell'area
3. Esempi: `Classe I`, `Classe II`, `Classe IIIa`, `Classe IIIb`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La classe di pericolosità geomorfologica si ricava dalla **Carta di Sintesi della pericolosità geomorfologica e dell'idoneità all'utilizzo urbanistico** del Comune, allegata al PRG. Per molti Comuni piemontesi è disponibile online sul Geoportale regionale.

---

### ATTENZIONE ! Inserire la latitudine.

**Dove si trova**: Campo **"Latitudine"** nelle **"Coordinate geografiche dell'intervento (ETRF89/WGS84)"**

**Causa**: Le coordinate geografiche non sono state inserite — manca la latitudine.

**Soluzione**:
1. Trova il campo **"Latitudine"**
2. Inserisci la latitudine in gradi decimali nel sistema ETRF89/WGS84
3. Esempio per Piemonte: `44.123456` (valore tipico tra 44° e 46°)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> **Come trovare le coordinate**: usa il portale cartografico del Comune, il Geoportale Piemonte o Google Maps (click destro sulla posizione → copia coordinate). Assicurati di usare il sistema ETRF89/WGS84 (coincide praticamente con WGS84 per applicazioni pratiche).

---

### ATTENZIONE ! Inserire la longitudine.

**Dove si trova**: Campo **"Longitudine"** nelle coordinate geografiche

**Causa**: Manca la longitudine.

**Soluzione**:
1. Trova il campo **"Longitudine"**
2. Inserisci la longitudine in gradi decimali nel sistema ETRF89/WGS84
3. Esempio per Piemonte: `7.654321` (valore tipico tra 6° e 9°)
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 4. Dati dei quattro professionisti

La Denuncia Sismica richiede la compilazione **obbligatoria e completa** delle schede di quattro professionisti tecnici. Il sistema verifica gli stessi campi per tutti e quattro, nell'ordine:

1. **Professionista 1** — Progettista delle opere architettoniche
2. **Professionista 2** — Direttore dei lavori architettonici
3. **Professionista 3** — Progettista delle strutture
4. **Professionista 4** — Direttore dei lavori strutturali

Per ciascuno vengono verificati in sequenza i campi elencati di seguito. Il messaggio di errore appare sul **primo campo mancante** del primo professionista incompleto.

{: .note }
> Puoi usare il pulsante **"Carica Soggetto"** per pre-compilare i dati da un soggetto già presente in anagrafica. Seleziona prima il tipo di soggetto, poi il soggetto specifico, quindi clicca "Carica Soggetto".

{: .warning }
> Tutti e quattro i professionisti sono **sempre obbligatori**, indipendentemente dall'intervento. Non è possibile presentare la Denuncia Sismica con meno di quattro tecnici compilati.

---

### ATTENZIONE ! Inserire il cognome del professionista.

**Dove si trova**: Campo **"Cognome"** nella scheda del professionista indicato

**Causa**: Il campo Cognome è vuoto per uno dei quattro professionisti.

**Soluzione**:
1. Identifica quale professionista ha il campo vuoto (il sistema si ferma al primo incompleto)
2. Vai alla scheda corrispondente: **"Progettista delle opere architettoniche"**, **"Direttore dei lavori architettonici"**, **"Progettista delle strutture"** o **"Direttore dei lavori strutturali"**
3. Inserisci il cognome nel campo **"Cognome"**
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire il nome del professionista.

**Dove si trova**: Campo **"Nome"** nella scheda del professionista

**Causa**: Il campo Nome è vuoto.

**Soluzione**: Inserisci il nome nel campo **"Nome"** della scheda del professionista indicato.

---

### ATTENZIONE ! Inserire il codice fiscale del professionista.

**Dove si trova**: Campo **"Cod. Fiscale"** nella scheda del professionista

**Causa**: Il codice fiscale è vuoto.

**Soluzione**:
1. Inserisci il codice fiscale nel campo **"Cod. Fiscale"**
2. Il CF è composto da **16 caratteri** alfanumerici
3. Esempio: `RSSMRA80A01L219F`

---

### ATTENZIONE ! Inserire la data di nascita del professionista.

**Dove si trova**: Campo **"Data Nascita"** nella scheda del professionista

**Causa**: La data di nascita è vuota.

**Soluzione**:
1. Trova il campo **"Data Nascita"**
2. Inserisci la data di nascita nel formato **GG/MM/AAAA**
3. Usa l'**icona calendario** oppure inserisci manualmente

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data nascita professionista)

**Causa**: La data di nascita del professionista è in formato errato.

**Soluzione**: Riscrivi la data di nascita nel formato **GG/MM/AAAA** (es. `01/03/1975`).

---

### ATTENZIONE ! Inserire il comune di nascita del professionista.

**Dove si trova**: Campo **"Comune Nascita"** nella scheda del professionista

**Causa**: Il comune di nascita è vuoto.

**Soluzione**: Inserisci il comune di nascita (es. `Torino`, `Milano`). Per nati all'estero, inserisci la città estera e compila il campo **"Stato"**.

---

### ATTENZIONE ! Inserire la provincia di nascita del professionista.

**Dove si trova**: Campo **"Provincia"** (nascita) nella scheda del professionista

**Causa**: La provincia di nascita è vuota.

**Soluzione**: Inserisci la **sigla** della provincia di nascita (2 caratteri, es. `TO`, `MI`, `RM`). Per nati all'estero, lascia vuoto e compila il campo **"Stato"**.

---

### ATTENZIONE ! Inserire la città di residenza del professionista.

**Dove si trova**: Campo **"Città"** nella sottosezione **"Residenza"**

**Causa**: La città di residenza è vuota.

**Soluzione**: Inserisci il comune di residenza del professionista (es. `Torino`, `Biella`).

---

### ATTENZIONE ! Inserire la provincia di residenza del professionista.

**Dove si trova**: Campo **"Provincia"** nella sottosezione **"Residenza"**

**Causa**: La provincia di residenza è vuota.

**Soluzione**: Inserisci la **sigla** della provincia di residenza (es. `TO`, `BI`).

---

### ATTENZIONE ! Inserire l'indirizzo di residenza del professionista.

**Dove si trova**: Campo **"Indirizzo"** nella sottosezione **"Residenza"**

**Causa**: L'indirizzo di residenza è vuoto.

**Soluzione**: Inserisci l'indirizzo di residenza (es. `Via Roma`).

---

### ATTENZIONE ! Inserire il civico di residenza del professionista.

**Dove si trova**: Campo **"Civico"** nella sottosezione **"Residenza"**

**Causa**: Il numero civico di residenza è vuoto.

**Soluzione**: Inserisci il numero civico (es. `15`, `22/A`).

---

### ATTENZIONE ! Inserire il CAP di residenza del professionista.

**Dove si trova**: Campo **"CAP"** nella sottosezione **"Residenza"**

**Causa**: Il CAP di residenza è vuoto.

**Soluzione**: Inserisci il CAP di residenza: esattamente **5 cifre** (es. `10121`).

---

### ATTENZIONE ! Inserire e-mail del professionista.

**Dove si trova**: Campo **"E-Mail"** nella scheda del professionista

**Causa**: L'indirizzo e-mail ordinario è vuoto.

**Soluzione**: Inserisci l'indirizzo e-mail del professionista (es. `mario.rossi@studio.it`).

---

### ATTENZIONE ! Inserire e-mail certificata del professionista.

**Dove si trova**: Campo **"E-Mail Certificata"** nella scheda del professionista

**Causa**: L'indirizzo PEC è vuoto.

**Soluzione**:
1. Trova il campo **"E-Mail Certificata"**
2. Inserisci l'indirizzo PEC del professionista (es. `mario.rossi@pec.ingpec.eu`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La PEC è obbligatoria per tutti i professionisti. Se il professionista non ha PEC personale, può usare la PEC dello studio associato.

---

### ATTENZIONE ! Selezionare l'ordine/collegio del professionista.

**Dove si trova**: Menu a discesa **"Iscritto all'ordine/collegio"** nella scheda del professionista

**Causa**: Non hai selezionato l'ordine o collegio professionale di appartenenza.

**Soluzione**:
1. Trova il menu a discesa **"Iscritto all'ordine/collegio"**
2. Seleziona l'ordine/collegio dal menu
3. Esempi: `Ordine degli Ingegneri`, `Ordine degli Architetti`, `Collegio dei Geometri`, `Collegio dei Periti Industriali`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire albo di appartenenza del professionista.

**Dove si trova**: Campo **"di"** nella riga dell'albo (sede dell'ordine)

**Causa**: Hai selezionato l'ordine ma non hai indicato la sede (provincia dell'ordine).

**Soluzione**:
1. Trova il campo **"di"** accanto al menu dell'ordine/collegio
2. Inserisci la **provincia** della sede dell'ordine (es. `Torino`, `Biella`, `Novara`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire numero di albo del professionista.

**Dove si trova**: Campo **"al n."** nella riga dell'albo

**Causa**: Hai indicato l'ordine e la sede ma non hai inserito il numero di iscrizione.

**Soluzione**:
1. Trova il campo **"al n."**
2. Inserisci il numero di iscrizione all'albo/ordine del professionista (es. `1234`, `A567`)
3. Lo trovi sulla **tessera professionale** o sul sito dell'ordine competente
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 5. Dati del Costruttore

Dopo i quattro professionisti, il sistema verifica i dati del **Costruttore** (impresa che esegue i lavori strutturali).

### ATTENZIONE ! Inserire la denominazione o ragione sociale del Costruttore.

**Dove si trova**: Campo **"Denominazione o ragione sociale"** nella sezione **"Costruttore"**

**Causa**: La ragione sociale dell'impresa costruttrice è vuota.

**Soluzione**:
1. Vai alla sezione **"Costruttore"**
2. Inserisci la ragione sociale o denominazione dell'impresa (es. `Rossi Costruzioni S.r.l.`, `Impresa Edile Bianchi`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire il codice fiscale del Costruttore.

**Dove si trova**: Campo **"Codice fiscale"** nella sezione Costruttore

**Causa**: Il codice fiscale dell'impresa è vuoto.

**Soluzione**: Inserisci il codice fiscale dell'impresa (per le società coincide spesso con la Partita IVA, es. `12345678901`).

---

### ATTENZIONE ! Inserire la Partita IVA del Costruttore.

**Dove si trova**: Campo **"Partita IVA"** nella sezione Costruttore

**Causa**: La Partita IVA è vuota.

**Soluzione**: Inserisci la Partita IVA dell'impresa: esattamente **11 cifre** (es. `12345678901`).

---

### ATTENZIONE ! Inserire il cognome del Legale Rappresentante del Costruttore.

**Dove si trova**: Campo **"Legale rappresentante Cognome"** nella sezione Costruttore

**Causa**: Il cognome del legale rappresentante è vuoto.

**Soluzione**: Inserisci il cognome del legale rappresentante dell'impresa (es. `Rossi`).

---

### ATTENZIONE ! Inserire il nome del Legale Rappresentante del Costruttore.

**Dove si trova**: Campo **"Legale rappresentante Nome"** nella sezione Costruttore

**Causa**: Il nome del legale rappresentante è vuoto.

**Soluzione**: Inserisci il nome del legale rappresentante (es. `Mario`).

---

### ATTENZIONE ! Inserire il comune della sede legale del Costruttore.

**Dove si trova**: Campo **"Comune"** nella sottosezione **"Con sede legale in"**

**Causa**: Il comune della sede legale è vuoto.

**Soluzione**: Inserisci il comune della sede legale dell'impresa (es. `Torino`).

---

### ATTENZIONE ! Inserire la provincia della sede legale del Costruttore.

**Dove si trova**: Campo **"Provincia"** nella sottosezione **"Con sede legale in"**

**Causa**: La provincia della sede legale è vuota.

**Soluzione**: Inserisci la **sigla** della provincia (es. `TO`, `BI`).

---

### ATTENZIONE ! Inserire l'indirizzo della sede legale del Costruttore.

**Dove si trova**: Campo **"Indirizzo"** nella sottosezione **"Con sede legale in"**

**Causa**: L'indirizzo della sede legale è vuoto.

**Soluzione**: Inserisci l'indirizzo della sede legale (es. `Via Roma`).

---

### ATTENZIONE ! Inserire il civico della sede legale del Costruttore.

**Dove si trova**: Campo **"Civico"** nella sottosezione **"Con sede legale in"**

**Causa**: Il numero civico della sede legale è vuoto.

**Soluzione**: Inserisci il numero civico (es. `15`, `22/A`).

---

### ATTENZIONE ! Inserire il CAP della sede legale del Costruttore.

**Dove si trova**: Campo **"CAP"** nella sottosezione **"Con sede legale in"**

**Causa**: Il CAP della sede legale è vuoto.

**Soluzione**: Inserisci il CAP della sede legale: esattamente **5 cifre** (es. `10121`).

---

### ATTENZIONE ! Inserire l'E-mail del Costruttore.

**Dove si trova**: Campo **"E-Mail"** nella sezione Costruttore

**Causa**: L'indirizzo e-mail dell'impresa è vuoto.

**Soluzione**: Inserisci l'e-mail dell'impresa costruttrice (es. `info@rossiconstruzioni.it`).

---

### ATTENZIONE ! Inserire l'E-mail Certificata del Costruttore.

**Dove si trova**: Campo **"E-Mail Certificata"** nella sezione Costruttore

**Causa**: L'indirizzo PEC dell'impresa è vuoto.

**Soluzione**: Inserisci la PEC dell'impresa (es. `rossiconstruzioni@pec.it`).

{: .note }
> La PEC dell'impresa è obbligatoria. Tutte le imprese iscritte alla CCIAA hanno una PEC; se non la conosci, cercala sul **Registro Imprese** (www.registroimprese.it).

---

## 6. Strumento urbanistico esecutivo

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Strumento Urbanistico Esecutivo'.

**Dove si trova**: Sezione **"DICHIARA"** → punto **a)** — **"che l'area oggetto dell'atto di assenso"**

**Causa**: Non hai selezionato se l'area è soggetta o meno a strumento urbanistico esecutivo.

**Soluzione**:
1. Vai alla sezione **"DICHIARA"** → punto **a)**
2. Seleziona **una delle due opzioni**:
   - ⚪ **"non è soggetta a strumento urbanistico esecutivo"** → caso più comune per interventi su singoli lotti
   - ⚪ **"è soggetta a strumento urbanistico esecutivo"** → l'area ricade in un Piano Esecutivo Convenzionato, Lottizzazione, ecc.; compila numero e data deliberazione
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire numero Deliberazione Comunale.

**Dove si trova**: Campo **"Deliberazione Comunale n."** (visibile dopo selezione "è soggetta a strumento urbanistico esecutivo")

**Causa**: Hai selezionato che l'area è soggetta a strumento urbanistico esecutivo ma non hai inserito il numero della deliberazione comunale che lo ha approvato.

**Soluzione**:
1. Trova il campo **"Deliberazione Comunale n."**
2. Inserisci il numero della deliberazione (es. `45/2020`, `GC 123/2019`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la data della Deliberazione Comunale.

**Dove si trova**: Campo **"Data"** accanto al numero della deliberazione

**Causa**: Numero deliberazione inserito ma data mancante.

**Soluzione**: Inserisci la data della deliberazione nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data deliberazione)

**Causa**: La data della deliberazione comunale è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**.

---

## 7. Vincolo idrogeologico

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Vincolo Idrogeologico'.

**Dove si trova**: Sezione **"DICHIARA"** → punto **b)** — **"che l'area interessata"**

**Causa**: Non hai dichiarato se l'area è soggetta a vincolo idrogeologico.

**Soluzione**:
1. Vai al punto **b)**
2. Seleziona **una delle tre opzioni**:
   - ⚪ **"non è sottoposta a vincolo idrogeologico"** → area libera da vincolo
   - ⚪ **"è sottoposta a vincolo idrogeologico e che l'autorizzazione è stata rilasciata da"** → vincolo presente, autorizzazione già ottenuta; compila Comune/Regione, n. protocollo e data
   - ⚪ **"è sottoposta a vincolo idrogeologico e l'intervento rientra nei casi eseguibili senza autorizzazione"** → vincolo presente ma non richiede autorizzazione specifica
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Verifica la presenza del vincolo idrogeologico sul Geoportale della Regione Piemonte o nel certificato di destinazione urbanistica.

---

### ATTENZIONE ! Inserire Comune/Regione. (autorizzazione vincolo idrogeologico)

**Dove si trova**: Campo **"Comune/Regione"** dopo selezione "è sottoposta a vincolo idrogeologico e l'autorizzazione è stata rilasciata da"

**Causa**: Hai selezionato che esiste il vincolo con autorizzazione ma non hai indicato chi l'ha rilasciata.

**Soluzione**:
1. Trova il campo **"Comune/Regione"**
2. Inserisci l'ente che ha rilasciato l'autorizzazione idrogeologica (es. `Comune di Torino`, `Regione Piemonte`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire numero protocollo. (autorizzazione vincolo idrogeologico)

**Dove si trova**: Campo **"Protocollo n."** nella sezione dell'autorizzazione idrogeologica

**Causa**: Comune/Regione inserito ma numero di protocollo mancante.

**Soluzione**: Inserisci il numero di protocollo dell'autorizzazione idrogeologica.

---

### ATTENZIONE ! Inserire data protocollo. (autorizzazione vincolo idrogeologico)

**Dove si trova**: Campo **"Data"** nella sezione dell'autorizzazione idrogeologica

**Causa**: Numero di protocollo inserito ma data mancante.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data autorizzazione idrogeologica)

**Causa**: La data dell'autorizzazione idrogeologica è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**.

---

## 8. Precedenti lavori sul fabbricato

Questa sezione è **opzionale**: il controllo si attiva solo se viene spuntata la checkbox **"ai sensi del D.P.R. 06/06/2001 n. 380, sono stati denunciati a"** al punto **c)**.

### ATTENZIONE ! Inserire Comune/Regione. (precedenti lavori)

**Dove si trova**: Campo **"Comune/Regione"** dopo spunta della checkbox dei precedenti lavori (punto c)

**Causa**: Hai spuntato "precedenti lavori già realizzati sul fabbricato" ma non hai indicato a chi sono stati denunciati.

**Soluzione**:
1. Trova il campo **"Comune/Regione"** nella riga dei precedenti lavori
2. Inserisci l'ente a cui è stata presentata la denuncia dei precedenti lavori (es. `Comune di Torino`, `Regione Piemonte`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire numero protocollo. (precedenti lavori)

**Dove si trova**: Campo **"Protocollo n."** nella sezione precedenti lavori

**Causa**: Comune inserito ma numero di protocollo mancante.

**Soluzione**: Inserisci il numero di protocollo della precedente denuncia sismica.

---

### ATTENZIONE ! Inserire data protocollo. (precedenti lavori)

**Dove si trova**: Campo **"Data"** nella sezione precedenti lavori

**Causa**: Numero protocollo inserito ma data mancante.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data precedenti lavori)

**Causa**: La data della precedente denuncia è in formato errato.

**Soluzione**: Riscrivi la data nel formato **GG/MM/AAAA**.

---

## 9. Collaudo delle opere

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Collaudo Opere'.

**Dove si trova**: Sezione **"DICHIARA"** → punto **e)** — **"con riferimento al collaudo delle opere"**

**Causa**: Non hai dichiarato se la denuncia necessita della nomina del collaudatore.

**Soluzione**:
1. Vai al punto **e)**
2. Seleziona **una delle due opzioni**:
   - ⚪ **"la presente denuncia non necessita di nomina del collaudatore"** → l'intervento rientra nel campo di applicazione dell'art. 67 c. 8-bis del D.P.R. 380/2001 (intervento locale); il direttore lavori strutturale depositerà la Dichiarazione di Regolare Esecuzione (DRE)
   - ⚪ **"la presente denuncia necessita di nomina del collaudatore"** → per interventi non locali; compila le sotto-opzioni
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> **Quando NON serve il collaudatore?** Per gli "interventi locali" ai sensi delle Norme Tecniche per le Costruzioni (NTC 2018), ossia interventi di riparazione o intervento locale su singoli elementi strutturali (art. 67 c. 8-bis d.P.R. 380/2001). In tutti gli altri casi il collaudatore è obbligatorio.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Nomina Collaudatore'.

**Dove si trova**: Sotto-opzioni dopo selezione **"necessita di nomina del collaudatore"**

**Causa**: Hai dichiarato che è necessaria la nomina del collaudatore ma non hai indicato le modalità di nomina.

**Soluzione**:
1. Dopo aver selezionato "necessita di nomina del collaudatore"
2. Seleziona **una delle tre sotto-opzioni**:
   - ⚪ **"e allega la dichiarazione di nomina e accettazione del collaudatore"** → il collaudatore è già stato scelto e ha accettato l'incarico; allega la dichiarazione di nomina
   - ⚪ **"e dichiara che il collaudatore verrà scelto tra una terna di professionisti indicati dall'Ordine"** → lavori in economia diretta; il collaudatore sarà indicato dall'Ordine degli Ingegneri/Architetti su richiesta già inoltrata
   - ⚪ **"e che l'intervento in progetto è riconducibile ad opera pubblica"** → opera pubblica; il committente presenterà nomina e atti prima dell'inizio lavori
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> **IMPORTANTE**: Le tre sotto-opzioni di nomina del collaudatore sono mutuamente esclusive. Selezionane solo una. In particolare, la richiesta di terna all'Ordine è prevista solo per lavori "in economia diretta" (committente = costruttore). Se selezioni "allega la dichiarazione di nomina", ricorda di caricare effettivamente il documento tra gli allegati.

---

## 10. Dichiarazione del progettista strutturale

### ATTENZIONE ! Inserire il cognome del progettista.

**Dove si trova**: Campo **"Cognome"** nella sezione **"Il progettista strutturale"** (in fondo al modulo)

**Causa**: Il cognome del progettista strutturale nella sezione dichiarazioni è vuoto.

**Soluzione**:
1. Vai alla sezione **"Il progettista strutturale"** in fondo al modulo
2. Inserisci il **cognome** nel campo corrispondente

{: .note }
> Questa sezione è separata dalla scheda "Progettista delle strutture" compilata nella sezione COMUNICA. Si tratta della **dichiarazione finale** del progettista strutturale che attesta la conformità del progetto alle norme tecniche. I dati del progettista strutturale qui inseriti devono coincidere con quelli del Professionista 3 (Progettista delle strutture).

---

### ATTENZIONE ! Inserire il nome del progettista.

**Dove si trova**: Campo **"Nome"** nella sezione **"Il progettista strutturale"**

**Causa**: Il nome è vuoto nella sezione dichiarazioni del progettista strutturale.

**Soluzione**: Inserisci il **nome** del progettista strutturale.

---

### ATTENZIONE ! Inserire il codice fiscale del progettista.

**Dove si trova**: Campo **"Codice Fiscale"** nella sezione **"Il progettista strutturale"**

**Causa**: Il codice fiscale è vuoto nella sezione dichiarazioni.

**Soluzione**: Inserisci il **codice fiscale** del progettista strutturale (16 caratteri).

---

## Consigli pratici Denuncia Sismica

### Prima di validare ✅

- [ ] Compila il **titolo abilitativo** (tipologia, numero, data)
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] Compila la **localizzazione** (indirizzo, CAP, civico, mappali, destinazione d'uso)
- [ ] Inserisci **Zona PRG vigente** e **Zona PRG adottato**
- [ ] Inserisci la **classe di sintesi della pericolosità geomorfologica**
- [ ] Inserisci **latitudine** e **longitudine** (ETRF89/WGS84)
- [ ] Compila **tutti e quattro i professionisti** con tutti i dati richiesti (cognome, nome, CF, data nascita, comune nascita, provincia nascita, residenza completa, e-mail, PEC, ordine, sede ordine, numero albo)
- [ ] Compila il **Costruttore** (ragione sociale, CF, PIVA, legale rappresentante, sede legale completa, e-mail, PEC)
- [ ] Seleziona la voce **strumento urbanistico esecutivo** (punto a)
- [ ] Seleziona la voce **vincolo idrogeologico** (punto b) e compila i campi se richiesto
- [ ] Spunta e compila la sezione **precedenti lavori** se applicabile (punto c)
- [ ] Seleziona la voce **collaudo opere** (punto e) e le sotto-opzioni se richiesto
- [ ] Compila la sezione **dichiarazione del progettista strutturale** (cognome, nome, CF)
- [ ] **Salva** frequentemente

### Errori frequenti Denuncia Sismica 🔍

1. **Professionista incompleto** → Il sistema itera su tutti e quattro; il primo errore si ferma al primo campo mancante del primo professionista incompleto. Compila tutte e quattro le schede dall'inizio alla fine
2. **PEC mancante** → Obbligatoria per tutti i professionisti e per il costruttore
3. **Coordinate geografiche mancanti** → Usa il Geoportale Piemonte o Google Maps per ricavarle
4. **Zona PRG/pericolosità mancanti** → Dati urbanistici esclusivi della DS, non presenti nelle altre pratiche
5. **Collaudo non dichiarato** → Obbligatorio indicare se è necessario il collaudatore
6. **Nomina collaudatore non selezionata** → Se dichiari "necessita collaudatore", devi specificare le modalità
7. **Dati costruttore incompleti** → Tutti i campi della sede legale e i contatti sono obbligatori
8. **Dichiarazione progettista strutturale** → Sezione in fondo al modulo spesso dimenticata (diversa dalla scheda Progettista 3)

### Campi esclusivi della Denuncia Sismica ⚠️

Questi campi non esistono nelle altre pratiche e sono spesso dimenticati:

- Zona PRG vigente e adottato
- Classe di sintesi della pericolosità geomorfologica
- Coordinate geografiche (latitudine e longitudine in ETRF89/WGS84)
- Dati completi di quattro professionisti (con data nascita, comune nascita, residenza, PEC, numero albo)
- Dati del Costruttore con sede legale completa e PEC
- Strumento urbanistico esecutivo (dichiarazione a)
- Vincolo idrogeologico (dichiarazione b)
- Precedenti lavori (dichiarazione c — opzionale)
- Collaudo opere con sotto-opzioni nomina collaudatore (dichiarazione e)
- Dichiarazione finale del progettista strutturale (cognome, nome, CF)

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
**Fonte**: Analisi codice ValidaDatiDS e DatiDS.ascx
