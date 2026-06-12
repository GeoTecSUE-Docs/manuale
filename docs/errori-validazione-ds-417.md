---
title: Errori Denuncia Sismica - Regione Lombardia
parent: Errori di validazione
nav_order: 63
description: Errori di validazione specifici per la Denuncia Sismica (DS) - Regione Lombardia con coordinate UTM WGS84 32N, zona sismica e tipologia trasmissione
keywords: [denuncia sismica, DS, Lombardia, zona sismica, coordinate UTM, WGS84 32N, autorizzazione sismica, deposito sismico, procedimento edilizio, privacy checkbox]
IDRegione: 4
IDTipoPratica: 417
Fonte: Manuale
---

# Errori di validazione - Denuncia Sismica
## Regione Lombardia

Guida completa agli errori specifici per la **Denuncia Sismica (DS)** — Regione Lombardia.

{: .note }
> La DS Lombardia è una pratica con struttura originale rispetto alle altre denunce sismiche del sistema. Non ha le sezioni professionisti/costruttore in formato inline tipiche del Piemonte, ma presenta caratteristiche specifiche lombarde: la sezione **"In relazione a procedimento edilizio"** (3 opzioni con dati pratica obbligatori per la terza), le **coordinate UTM WGS84 32N** con validazione degli intervalli numerici (identica alle pratiche CILA/SCIA/PdC Lombardia), la **Zona Sismica** (4 livelli), la **tipologia di trasmissione** (autorizzazione sismica o deposito sismico in base alla zona) e la **checkbox Privacy** — obbligatoria da spuntare attivamente (a differenza di quasi tutte le altre pratiche dove la privacy è solo testo informativo). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Relazione a procedimento edilizio](#1-relazione-a-procedimento-edilizio)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Coordinate UTM WGS84 32N](#3-coordinate-utm-wgs84-32n)
4. [Zona Sismica](#4-zona-sismica)
5. [Tipologia di trasmissione](#5-tipologia-di-trasmissione)
6. [Descrizione dell'intervento](#6-descrizione-dellintervento)
7. [Privacy](#7-privacy)

---

## 1. Relazione a procedimento edilizio

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'In relazione a procedimento edilizio'.

**Dove si trova**: Sezione "In relazione a procedimento edilizio" → 3 radio button `$RelProcEdi`

**Causa**: Nessuno dei 3 radio button è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **rdbRelProcEdi_1** — "non ancora avviato e per il quale sarà presentata apposita documentazione"
- ⚪ **rdbRelProcEdi_2** — "avviato congiuntamente alla presente documentazione"
- ⚪ **rdbRelProcEdi_3** — "già avviato e per il quale è stata presentata apposita documentazione" → inserisci titolo, protocollo e data del procedimento edilizio

---

### Opzione rdbRelProcEdi_3 — Procedimento già avviato

#### ATTENZIONE !  Inserire il titolo del procedimento edilizio (o selezionarlo dalla chiave).

**Causa**: Hai selezionato rdbRelProcEdi_3 ma il campo `txtTitoloPE` "Titolo e/o comunicazione" è vuoto.

**Soluzione**: Inserisci il titolo del procedimento edilizio già avviato (es. `SCIA`, `Permesso di Costruire`, `CILA`). In alternativa, se la pratica originaria è stata compilata su GeoTecSUE, inserisci la chiave numerica nel campo apposito e clicca il tasto verde 🔄 per precompilare automaticamente tutti e tre i campi.

---

#### ATTENZIONE !  Inserire il protocollo del procedimento edilizio (o selezionarlo dalla chiave).

**Causa**: Hai selezionato rdbRelProcEdi_3 e inserito il titolo, ma il campo `txtProtocolloPE` "Protocollo numero" è vuoto.

**Soluzione**: Inserisci il numero di protocollo del procedimento edilizio già presentato.

---

#### ATTENZIONE !  Inserire la data del protocollo del procedimento edilizio (o selezionarlo dalla chiave).

**Causa**: Hai selezionato rdbRelProcEdi_3 e inserito titolo e protocollo, ma il campo `txtDataPE` "Data" è vuoto.

**Soluzione**: Inserisci la data di protocollo del procedimento edilizio nel campo "Data".

{: .note }
> Il validatore verifica solo che i tre campi non siano vuoti — **non controlla il formato della data** `txtDataPE`. È presente il datepicker nel modulo, quindi inserire la data tramite il calendario è sufficiente indipendentemente dal formato. Il campo `txtChiavePE` (chiave numerica GeoTecSUE a 20 cifre) non viene validato e può essere lasciato vuoto se si preferisce inserire manualmente titolo, protocollo e data.

---

## 2. Localizzazione dell'intervento

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

## 3. Coordinate UTM WGS84 32N

Le coordinate vengono validate subito dopo la localizzazione. Entrambe sono obbligatorie e devono rientrare negli intervalli numerici del sistema di riferimento UTM WGS84 Zona 32N per il territorio lombardo.

---

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Causa**: Il campo `txtCoordinateX` è vuoto.

**Soluzione**: Inserisci la coordinata X (asse Est) dell'intervento nel sistema UTM WGS84 32N. Il valore deve essere compreso tra **430.000 e 700.000** metri.

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: La coordinata X inserita è fuori dall'intervallo valido, oppure il valore inserito non è un numero.

**Soluzione**: Verifica che la coordinata X sia un valore numerico compreso tra **430.000 e 700.000**. Per trovare le coordinate dell'intervento puoi usare il bottone "Calcola Coordinate" presente nel modulo (se abilitato) o rilevare le coordinate da un GIS o dalla cartografia comunale.

{: .note }
> L'intervallo 430.000–700.000 per X corrisponde all'estensione in longitudine del territorio lombardo nel sistema UTM WGS84 Zona 32N. Valori fuori da questo intervallo indicano generalmente un errore di trasposizione (es. coordinate in un sistema di riferimento diverso, cifre scambiate o valore incompleto).

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo `txtCoordinateY` è vuoto.

**Soluzione**: Inserisci la coordinata Y (asse Nord) dell'intervento nel sistema UTM WGS84 32N. Il valore deve essere compreso tra **4.800.000 e 5.700.000** metri.

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: La coordinata Y inserita è fuori dall'intervallo valido, oppure il valore non è un numero.

**Soluzione**: Verifica che la coordinata Y sia un valore numerico compreso tra **4.800.000 e 5.700.000**.

{: .note }
> Gli intervalli di validazione delle coordinate (X: 430k-700k; Y: 4800k-5700k) sono identici a quelli usati nelle pratiche CILA, SCIA, PdC e SCA della Regione Lombardia. Per entrambe le coordinate il validatore usa `clsModuloAsp.GetDoubleNullable()` — se il valore inserito non è convertibile in numero (es. testo, virgola al posto del punto) viene trattato come fuori intervallo.

---

## 4. Zona Sismica

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Zona Sismica'.

**Dove si trova**: Sezione "Zona Sismica" → 4 radio button `$ZonaSismica`

**Causa**: Nessuno dei 4 radio button è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button** corrispondente alla zona sismica del Comune in cui si trova l'immobile:
- ⚪ **rdbZonaSismica_1** — "Zona 1 - Livello di pericolosità alto"
- ⚪ **rdbZonaSismica_2** — "Zona 2 - Livello di pericolosità medio"
- ⚪ **rdbZonaSismica_3** — "Zona 3 - Livello di pericolosità basso"
- ⚪ **rdbZonaSismica_4** — "Zona 4 - Livello di pericolosità molto basso"

{: .note }
> La classificazione sismica del Comune è stabilita dall'Ordinanza PCM 3274/2003 e aggiornata con le classificazioni regionali. Per la Lombardia, consultare la [pagina della Regione Lombardia sulla pericolosità sismica](https://www.regione.lombardia.it). La scelta della zona sismica è collegata alla tipologia di trasmissione obbligatoria: Zona 1 e 2 → autorizzazione sismica; Zona 3 e 4 → deposito sismico.

---

## 5. Tipologia di trasmissione

### ATTENZIONE ! Non è stata selezionata nessuna voce per la tipologia di trasmissione.

**Dove si trova**: Sezione "TRASMETTE" → 2 radio button `$Trasmissione`

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button** in base alla zona sismica del Comune:
- ⚪ **rdbTrasmissione_1** — "la documentazione relativa all'**istanza di autorizzazione sismica**" *(solo per i Comuni ricadenti in zona 1 e in zona 2)*
- ⚪ **rdbTrasmissione_2** — "la documentazione relativa alla **comunicazione di deposito sismico**" *(solo per i Comuni ricadenti in zona 3 e in zona 4)*

{: .note }
> Il validatore non verifica la coerenza tra la zona sismica selezionata nella sezione precedente e la tipologia di trasmissione scelta — è responsabilità del dichiarante selezionare la tipologia coerente con la zona. In zona 1-2 (pericolosità alta/media) è obbligatoria l'autorizzazione preventiva; in zona 3-4 (pericolosità bassa/molto bassa) è sufficiente il deposito della documentazione.

---

## 6. Descrizione dell'intervento

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Dichiarazioni" → campo multiriga `txtDescrIntervento` "Descrizione dell'intervento" (max 300 caratteri). Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice.

**Causa**: Il campo descrizione è vuoto.

**Soluzione**: Inserisci la descrizione dell'intervento strutturale nel campo multiriga (max **300 caratteri**).

{: .note }
> Il campo `txtNote` "Note aggiuntive ed eventuali comunicazioni" è presente sotto la descrizione ma non viene validato — è facoltativo.

---

## 7. Privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione "Rispetto della normativa sulla privacy" → checkbox `chkPrivacy` "di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune"

**Causa**: La checkbox `chkPrivacy` non è spuntata.

**Soluzione**: Spunta la checkbox "di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune".

{: .warning }
> La DS Lombardia è una delle poche pratiche del sistema in cui la **privacy è una checkbox obbligatoria** da spuntare attivamente — non è solo un testo informativo. Se si dimentica di spuntarla, la validazione fallisce sempre come ultimo controllo, anche se tutti gli altri campi sono corretti.

---

## Consigli pratici — DS Lombardia

### Prima di validare ✅

- [ ] Seleziona la **relazione a procedimento edilizio** (rdb_1/rdb_2/rdb_3); se rdb_3: inserisci **titolo**, **protocollo** e **data** del procedimento (o usa la chiave GeoTecSUE)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **coordinata X** (430.000 – 700.000)
- [ ] Inserisci la **coordinata Y** (4.800.000 – 5.700.000)
- [ ] Seleziona la **zona sismica** (1/2/3/4)
- [ ] Seleziona la **tipologia di trasmissione** (autorizzazione zone 1-2 / deposito zone 3-4)
- [ ] Inserisci la **descrizione dell'intervento** (max 300 caratteri)
- [ ] Spunta la **checkbox Privacy**

### Campi presenti ma non validati ℹ️

- **`cmbTitoloSuImm`** ("In qualità di"): menu titolare, non validato
- **`txtChiavePE`**: chiave GeoTecSUE a 20 cifre per precompilare i dati del procedimento edilizio — non validata, opzionale
- **`txtNote`**: note aggiuntive, facoltativo

### Ordine di validazione ⚠️

Procedimento edilizio → Localizzazione → Coordinate X → Coordinate Y → Zona Sismica → Trasmissione → Descrizione → Privacy

### Errori frequenti 🔍

1. **Privacy non spuntata** → essendo l'ultimo controllo, viene segnalata solo dopo che tutti gli altri campi sono corretti; ricordarsi di spuntarla prima di tentare la validazione
2. **Coordinate fuori intervallo o non numeriche** → inserire cifre intere o decimali con punto (non virgola); X tra 430000 e 700000; Y tra 4800000 e 5700000
3. **rdb_3 senza dati procedimento** → i tre campi titolo/protocollo/data sono tutti obbligatori; la chiave GeoTecSUE può precompilarli automaticamente
4. **Zona sismica e trasmissione non coerenti** → il sistema non verifica la coerenza tra zona e tipologia; fare attenzione a scegliere la tipologia corretta (autorizzazione per zone 1-2, deposito per zone 3-4)

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
**Fonte**: Analisi codice ValidaDatiDSLombardia e DatiDSLombardia.ascx
