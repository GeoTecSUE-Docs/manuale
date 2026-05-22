---
title: Errori Denuncia Sismica Postuma (Tardiva) - Regione Piemonte
parent: Errori di validazione
nav_order: 41
description: Errori di validazione specifici per la Denuncia Sismica Postuma (Tardiva) - Regione Piemonte (artt. 65 e/o 93 D.P.R. 380/2001 - lavori già eseguiti senza denuncia)
keywords: [denuncia sismica postuma, denuncia tardiva, art. 65 DPR 380/2001, art. 93 DPR 380/2001, zona sismica, collaudo, nomina collaudatore, progettista strutture, Piemonte, pericolosità geomorfologica, ETRF89, WGS84, lavori senza denuncia]
IDRegione: 2
IDTipoPratica: 19
Fonte: Manuale
---

# Errori di validazione - Denuncia Sismica Postuma (Tardiva)
## Regione Piemonte

Guida completa agli errori specifici per la **Denuncia Sismica Postuma** (Tardiva) ai sensi degli artt. 65 e/o 93 del D.P.R. 6 giugno 2001, n. 380, relativa alla **Regione Piemonte**. La pratica riguarda la regolarizzazione di lavori già eseguiti senza aver effettuato la denuncia preventiva prevista dalla normativa sismica.

{: .note }
> La Denuncia Sismica Postuma è strutturalmente diversa dalla Denuncia Sismica ordinaria. Descrive lavori **già realizzati** ("di aver realizzato lavori senza aver effettuato la prevista denuncia"). Ha caratteristiche uniche: la **doppia base normativa** (art. 65 e/o art. 93, almeno una obbligatoria); la **localizzazione estesa** con pericolosità geomorfologica e coordinate ETRF89/WGS84 tutte obbligatorie; il **loop professionisti che salta la scheda 2** (Direttore lavori architettonici — non validata); la sezione **Collaudo opere** con radio a due livelli; e la **sezione Progettista Strutturale finale** con nome, cognome e CF come dichiarante conclusivo. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Descrizione sintetica e normativa di riferimento](#1-descrizione-sintetica-e-normativa-di-riferimento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Professionisti — Schede 1 e 3](#3-professionisti--schede-1-e-3)
4. [Strumento urbanistico esecutivo — dichiarazione a)](#4-strumento-urbanistico-esecutivo--dichiarazione-a)
5. [Vincolo idrogeologico — dichiarazione b)](#5-vincolo-idrogeologico--dichiarazione-b)
6. [Lavori precedenti — dichiarazione c)](#6-lavori-precedenti--dichiarazione-c)
7. [Provvedimenti di sospensione — dichiarazione d)](#7-provvedimenti-di-sospensione--dichiarazione-d)
8. [Collaudo opere — dichiarazione e)](#8-collaudo-opere--dichiarazione-e)
9. [Periodo di esecuzione dei lavori — dichiarazione f)](#9-periodo-di-esecuzione-dei-lavori--dichiarazione-f)
10. [Progettista strutturale dichiarante](#10-progettista-strutturale-dichiarante)

---

## 1. Descrizione sintetica e normativa di riferimento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga "che i lavori per i quali viene inoltrata la presente consistono in:"

**Causa**: Il campo `txtDescrIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione dei lavori già realizzati nel campo multiriga (max **300 caratteri**).

---

### ATTENZIONE ! Selezionare almeno un articolo (65 oppure 93).

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → due checkbox sotto il campo descrizione

**Causa**: Non hai spuntato nessuna delle due checkbox che identificano la base normativa della denuncia.

**Soluzione**: Spunta **almeno una** tra le due opzioni (è possibile selezionarle entrambe):
- ☐ **"ai sensi dell'art. 65 del D.P.R. 06/06/2001 n. 380"** — deposito strutturale per cemento armato e strutture metalliche
- ☐ **"ai sensi dell'art. 93 del D.P.R. 06/06/2001 n. 380"** — denuncia sismica per costruzioni in zona sismica

{: .note }
> La scelta dipende dalla natura dei lavori. L'art. 65 riguarda le opere in conglomerato cementizio armato, normale e precompresso, e a struttura metallica. L'art. 93 riguarda le costruzioni in zone sismiche. Per interventi che ricadono in entrambe le categorie è possibile (e corretto) spuntare entrambe le checkbox.

---

## 2. Localizzazione dell'intervento

La localizzazione nella DST è più estesa rispetto alle altre pratiche: include campi aggiuntivi tutti obbligatori (Zone PRG, pericolosità geomorfologica, coordinate geografiche).

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inserisci il toponimo nel campo testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure spunta "Toponimo mancante".

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

---

### ATTENZIONE ! Inserire la zona PRG vigente.

**Dove si trova**: Campo `txtZonaPRGVigente` nella sezione localizzazione, dopo i mappali

**Causa**: Il campo "Zona PRG vigente" è vuoto.

**Soluzione**: Inserisci la zona del Piano Regolatore Generale vigente (es. `B1`, `C2`, `D`, `Zona agricola E`).

---

### ATTENZIONE ! Inserire la zona PRG adottato.

**Dove si trova**: Campo `txtZonaPRGAdottato` accanto al PRG vigente

**Causa**: Il campo "Zona PRG adottato" è vuoto.

**Soluzione**: Inserisci la zona del Piano Regolatore Generale adottato (es. `B1`, `Zona mista`). Se non esiste un PRG adottato diverso dal vigente, inserisci lo stesso valore del PRG vigente.

---

### ATTENZIONE ! Inserire la classe di sintesi della pericolosità geomorfologica.

**Dove si trova**: Campo `txtPericolositaGeoMorf` nella sezione localizzazione

**Causa**: Il campo "Classe di sintesi della pericolosità geomorfologica" è vuoto.

**Soluzione**: Inserisci la classe di pericolosità geomorfologica dell'area (es. `IIa`, `IIb`, `IIIa`, `IIIb`). Il valore si trova nella cartografia PAI (Piano per l'Assetto Idrogeologico) o negli elaborati di piano del Comune.

{: .note }
> La classe di pericolosità geomorfologica è un dato specifico della normativa sismica piemontese. Non riguarda la zona sismica (3, 3S, 4) ma la classificazione del rischio geomorfologico locale secondo il Piano per l'Assetto Idrogeologico dell'Autorità di Bacino. Il tecnico strutturista deve indicare il valore corretto ricavandolo dagli elaborati di piano.

---

### ATTENZIONE ! Inserire la latitudine.

**Dove si trova**: Sezione "Coordinate geografiche dell'intervento (ETRF89/WGS84)" → campo `txtLatitudine`

**Causa**: La latitudine delle coordinate geografiche è vuota.

**Soluzione**: Inserisci la latitudine in gradi decimali nel sistema di riferimento **ETRF89/WGS84** (es. `44.123456`). Le coordinate si ottengono dalla cartografia online (Google Maps, OpenStreetMap) o dagli elaborati di rilievo.

---

### ATTENZIONE ! Inserire la longitudine.

**Dove si trova**: Sezione "Coordinate geografiche dell'intervento (ETRF89/WGS84)" → campo `txtLongitudine`

**Causa**: La longitudine è vuota.

**Soluzione**: Inserisci la longitudine in gradi decimali nel sistema **ETRF89/WGS84** (es. `7.654321`).

{: .note }
> Le coordinate ETRF89/WGS84 coincidono praticamente con le coordinate geografiche standard (GPS/Google Maps) per l'Italia. Il sistema ETRF89 è il riferimento geodetico europeo, praticamente sovrapponibile al WGS84 per gli usi pratici nella documentazione edilizia.

---

## 3. Professionisti — Schede 1 e 3

Il modulo contiene 4 schede professionisti, ma il validatore le controlla con un ciclo `i = 0 To 2` con condizione `If i <> 1`. In pratica vengono validate solo la **scheda 1** (Progettista delle opere architettoniche, `i=0`) e la **scheda 3** (Progettista delle strutture, `i=2`). La scheda 2 (Direttore dei lavori architettonici) non è validata.

Per le schede 1 e 3 i campi obbligatori sono molti più rispetto alle altre pratiche — non solo cognome/nome/CF, ma anche dati anagrafici completi:

---

### ATTENZIONE ! Inserire il cognome del professionista.

**Causa**: Il campo cognome della scheda 1 o della scheda 3 è vuoto.

**Soluzione**: Inserisci il cognome nella scheda corrispondente ("Progettista delle opere architettoniche" o "Progettista delle strutture"). Il messaggio appare per la prima scheda incompleta trovata nell'ordine 1 → 3.

---

### ATTENZIONE ! Inserire il nome del professionista.

**Causa**: Il campo nome è vuoto nella scheda in esame.

**Soluzione**: Inserisci il nome del professionista nella scheda incompleta.

---

### ATTENZIONE ! Inserire il codice fiscale del professionista.

**Causa**: Il codice fiscale è vuoto.

**Soluzione**: Inserisci il codice fiscale (16 caratteri alfanumerici).

---

### ATTENZIONE ! Inserire la data di nascita del professionista.

**Causa**: Il campo data di nascita è abilitato (ha classe `CampoObbligatorio`) ma vuoto.

**Soluzione**: Inserisci la data di nascita nel formato **GG/MM/AAAA** utilizzando il datepicker o digitandola manualmente.

{: .note }
> La data di nascita è condizionale: viene validata solo se il campo ha la classe CSS `CampoObbligatorio`. Nella scheda 1 (Progettista opere architettoniche) il campo ha questa classe (`txtDataNascProf1`), quindi è sempre obbligatorio. Nella scheda 3 (Progettista strutture) analogamente. Nella scheda 2 (Direttore lavori architettonici) non è presente la classe, ed è per questo che quella scheda non viene validata.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data nascita professionista)

**Causa**: La data di nascita inserita non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/03/1975`).

---

### ATTENZIONE ! Inserire il comune di nascita del professionista.

**Soluzione**: Inserisci il comune di nascita nel campo "Comune Nascita" della scheda.

---

### ATTENZIONE ! Inserire la provincia di nascita del professionista.

**Soluzione**: Inserisci la sigla della provincia (2 caratteri, es. `TO`, `MI`, `GE`) nel campo "Provincia" accanto al comune di nascita.

---

### ATTENZIONE ! Inserire la città di residenza del professionista.

**Soluzione**: Inserisci la città di residenza nel campo "Città" della sezione **Residenza** della scheda.

---

### ATTENZIONE ! Inserire la provincia di residenza del professionista.

**Soluzione**: Inserisci la sigla della provincia di residenza (2 caratteri).

---

### ATTENZIONE ! Inserire l'indirizzo di residenza del professionista.

**Soluzione**: Inserisci via o piazza nel campo "Indirizzo" della sezione Residenza.

---

### ATTENZIONE ! Inserire il civico di residenza del professionista.

**Soluzione**: Inserisci il numero civico nel campo "Civico" della sezione Residenza.

---

### ATTENZIONE ! Inserire il CAP di residenza del professionista.

**Soluzione**: Inserisci le 5 cifre del CAP nel campo "CAP" della sezione Residenza.

---

### ATTENZIONE ! Inserire e-mail del professionista.

**Soluzione**: Inserisci l'indirizzo e-mail nel campo "E-Mail" della scheda.

---

### ATTENZIONE ! Inserire e-mail certificata del professionista.

**Soluzione**: Inserisci l'indirizzo PEC nel campo "E-Mail Certificata" della scheda.

---

### ATTENZIONE ! Selezionare l'ordine/collegio del professionista.

**Causa**: Il menu a discesa `cmbTipoRuoloProf` è rimasto sull'opzione vuota.

**Soluzione**: Seleziona il tipo di ordine o collegio professionale dal menu "Iscritto all'ordine/collegio" (es. Ingegneri, Architetti, Geometri, Periti industriali).

---

### ATTENZIONE ! Inserire albo di appartenenza del professionista.

**Soluzione**: Inserisci il nome della sede dell'ordine/collegio nel campo "di" (es. `Torino`, `Milano`).

---

### ATTENZIONE ! Inserire numero di albo del professionista.

**Soluzione**: Inserisci il numero di iscrizione all'albo nel campo "al n."

{: .note }
> **Campi della scheda 2 (Direttore dei lavori architettonici) non validati**: tutti i campi della seconda scheda — cognome, nome, CF, data nascita, residenza, email, ordine — **non generano errori** se vuoti. Questa scheda è compilabile ma non obbligatoria ai fini della validazione del modulo. Compilarla è comunque buona prassi documentale quando il direttore lavori è una figura distinta dal progettista.

---

## 4. Strumento urbanistico esecutivo — dichiarazione a)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Strumento Urbanistico Esecutivo'.

**Dove si trova**: Sezione "DICHIARA" → punto a) "che l'area interessata"

**Causa**: Non hai selezionato nessuno dei due radio button.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"non è soggetta a strumento urbanistico esecutivo"**
- ⚪ **"è soggetta a strumento urbanistico esecutivo"** → compilare n. delibera + data

---

### ATTENZIONE ! Inserire numero Deliberazione Comunale.

**Causa**: Hai selezionato "è soggetta" ma non hai inserito il numero della deliberazione comunale.

**Soluzione**: Inserisci il numero nel campo "Deliberazione Comunale n." (es. `45`, `123/2022`).

---

### ATTENZIONE ! Inserire la data della Deliberazione Comunale.

**Causa**: Hai selezionato "è soggetta" e hai inserito il numero ma non la data.

**Soluzione**: Inserisci la data nel campo "Data" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (deliberazione comunale)

**Causa**: La data della deliberazione non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 5. Vincolo idrogeologico — dichiarazione b)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Vincolo Idrogeologico'.

**Dove si trova**: Sezione "DICHIARA" → punto b) "che l'area interessata"

**Causa**: Non hai selezionato nessuno dei tre radio button.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **"non è sottoposta a vincolo idrogeologico"**
- ⚪ **"è sottoposta a vincolo idrogeologico e che l'autorizzazione è stata rilasciata da ___"** → compilare Comune/Regione + n. protocollo + data
- ⚪ **"è sottoposta a vincolo idrogeologico e l'intervento rientra nei casi eseguibili senza autorizzazione"**

---

### ATTENZIONE ! Inserire Comune/Regione. (vincolo idrogeologico)

**Causa**: Hai selezionato "è sottoposta con autorizzazione" (`rdbVincoloIdrogeologicob_2`) ma non hai indicato l'ente rilasciante.

**Soluzione**: Inserisci nel campo "Comune/Regione" il nome dell'ente che ha rilasciato l'autorizzazione idrogeologica (es. `Regione Piemonte`, `Comune di Torino`).

---

### ATTENZIONE ! Inserire numero protocollo. (vincolo idrogeologico)

**Causa**: Hai compilato il Comune/Regione ma non il numero di protocollo dell'autorizzazione.

**Soluzione**: Inserisci il numero di protocollo nel campo "Protocollo n."

---

### ATTENZIONE ! Inserire data protocollo. (vincolo idrogeologico)

**Causa**: Manca la data del protocollo dell'autorizzazione.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (vincolo idrogeologico)

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA**.

---

## 6. Lavori precedenti — dichiarazione c)

La sezione c) è opzionale: si attiva spuntando la checkbox `chkPrecLavori` ("ai sensi del D.P.R. 06/06/2001 n. 380, sono stati denunciati a"). Se non spuntata, nessun campo viene validato.

---

### ATTENZIONE ! Inserire Comune/Regione. (lavori precedenti)

**Causa**: Hai spuntato la checkbox "lavori precedenti" ma non hai indicato l'ente destinatario della denuncia precedente.

**Soluzione**: Inserisci il nome del Comune o della Regione destinatario della denuncia nel campo "Comune/Regione".

---

### ATTENZIONE ! Inserire numero protocollo. (lavori precedenti)

**Causa**: Hai compilato il Comune/Regione ma non il numero di protocollo della denuncia precedente.

**Soluzione**: Inserisci il numero nel campo "Protocollo n."

---

### ATTENZIONE ! Inserire data protocollo. (lavori precedenti)

**Causa**: Manca la data del protocollo della denuncia precedente.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (lavori precedenti)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 7. Provvedimenti di sospensione — dichiarazione d)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Provvedimenti di sospensione'.

**Dove si trova**: Sezione "DICHIARA" → punto d) "che sui lavori oggetto del citato assenso"

**Causa**: Non hai selezionato nessuno dei due radio button.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"non esistono provvedimenti di sospensione per violazione del D.P.R. 06/06/2001 n. 380 o delle leggi urbanistiche"**
- ⚪ **"sui lavori oggetto del citato atto di assenso esistono provvedimenti di sospensione..."** → compilare emesso da + n. provvedimento + data

---

### ATTENZIONE ! Inserire soggetto emissione.

**Causa**: Hai selezionato "esistono provvedimenti di sospensione" ma non hai indicato chi li ha emessi.

**Soluzione**: Inserisci nel campo "Emessi da" il soggetto che ha emesso il provvedimento (es. `Comune di Torino`, `Regione Piemonte`).

---

### ATTENZIONE ! Inserire numero provvedimento.

**Causa**: Hai indicato il soggetto emittente ma non il numero del provvedimento.

**Soluzione**: Inserisci il numero nel campo "Provvedimento n."

---

### ATTENZIONE ! Inserire data provvedimento.

**Causa**: Manca la data del provvedimento di sospensione.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (provvedimento sospensione)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 8. Collaudo opere — dichiarazione e)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Collaudo Opere'.

**Dove si trova**: Sezione "DICHIARA" → punto e) "con riferimento al collaudo delle opere"

**Causa**: Non hai selezionato nessuno dei due radio button principali.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **c_1** — "che la presente denuncia **non necessita** di nomina del collaudatore in quanto rientra nel campo di applicazione dell'art. 67 - comma 8 bis - D.P.R. n. 380/2021 (intervento locale) e pertanto depositerà la dichiarazione di regolare esecuzione (DRE) resa dal direttore lavori strutturale"
- ⚪ **c_2** — "che la presente denuncia **necessita** di nomina del collaudatore" → seleziona la modalità di nomina

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Nomina Collaudatore'.

**Causa**: Hai selezionato c_2 (necessita collaudatore) ma non hai indicato come verrà nominato.

**Soluzione**: Seleziona **uno dei tre radio button** della nomina collaudatore:
- ⚪ **d_1** — "e allega la dichiarazione di nomina e accettazione del collaudatore"
- ⚪ **d_2** — "e dichiara che il collaudatore verrà scelto tra una terna di professionisti indicati dall'Ordine degli Ingegneri/Architetti in base a richiesta già inoltrata"
- ⚪ **d_3** — "e che l'intervento in progetto è riconducibile ad opera pubblica..."

{: .note }
> Le tre opzioni di nomina del collaudatore sono **mutuamente esclusive**. La richiesta di terna è prevista solo se i lavori sono "in economia diretta" (quando non esiste il Committente ed il Costruttore esegue in proprio). Ai sensi dell'art. 67 c. 8-bis D.P.R. 380/2001, il collaudo non è dovuto per interventi locali/riparazioni secondo le NTC vigenti — in quel caso si usa l'opzione c_1.

---

## 9. Periodo di esecuzione dei lavori — dichiarazione f)

### ATTENZIONE ! Inserire data di inizio lavori.

**Dove si trova**: Sezione "DICHIARA" → punto f) "che i lavori sono stati realizzati nel periodo compreso" → campo "fra il"

**Causa**: Il campo `txtDataInizioLavori` è vuoto.

**Soluzione**: Inserisci la data di inizio dei lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire data di fine lavori.

**Dove si trova**: Campo "e il" accanto alla data di inizio

**Causa**: Il campo `txtDataFineLavori` è vuoto.

**Soluzione**: Inserisci la data di fine dei lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

{: .note }
> Il punto f) è la dichiarazione del periodo in cui i lavori già eseguiti sono stati realizzati. Trattandosi di denuncia postuma, entrambe le date sono nel passato. Inserire date future genererebbe una contraddizione logica con la natura della pratica, anche se il sistema non esegue verifiche di questo tipo.

---

## 10. Progettista strutturale dichiarante

### ATTENZIONE ! Inserire il cognome del progettista.

**Dove si trova**: Sezione finale "Il progettista strutturale" → campo `txtCognomePSDich`

**Causa**: Il campo cognome del progettista strutturale dichiarante è vuoto.

**Soluzione**: Inserisci il cognome del progettista strutturale che sottoscrive la dichiarazione di conformità del progetto alle norme vigenti all'epoca dei lavori.

---

### ATTENZIONE ! Inserire il nome del progettista.

**Causa**: Il campo `txtNomePSDich` è vuoto.

**Soluzione**: Inserisci il nome del progettista strutturale dichiarante.

---

### ATTENZIONE ! Inserire il codice fiscale del progettista.

**Causa**: Il campo `txtCodFiscPSDich` è vuoto.

**Soluzione**: Inserisci il codice fiscale del progettista strutturale dichiarante.

{: .note }
> La sezione "Il progettista strutturale" in fondo al modulo è la dichiarazione conclusiva in cui il progettista strutturale attesta che il progetto allegato è stato redatto nel rispetto delle prescrizioni normative vigenti all'epoca della realizzazione dei lavori. Questa sezione è **distinta e separata** dalle schede professionisti a inizio modulo: i dati di questa sezione sono solo cognome, nome e codice fiscale, senza gli altri dettagli anagrafici richiesti nelle schede.

---

## Consigli pratici — Denuncia Sismica Postuma

### Prima di validare ✅

- [ ] Inserisci la **descrizione** dei lavori già eseguiti (max 300 caratteri)
- [ ] Spunta almeno **una checkbox** normativa (art. 65 e/o art. 93)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci **Zona PRG vigente** e **Zona PRG adottato**
- [ ] Inserisci la **classe di pericolosità geomorfologica**
- [ ] Inserisci **Latitudine** e **Longitudine** (ETRF89/WGS84)
- [ ] Compila la **scheda 1** (Progettista opere architettoniche) con tutti i 14 campi obbligatori
- [ ] Compila la **scheda 3** (Progettista strutture) con tutti i 14 campi obbligatori
- [ ] Seleziona il radio **Strumento Urbanistico**; se "è soggetta": inserisci n. delibera + data
- [ ] Seleziona il radio **Vincolo Idrogeologico** (3 opzioni); se con autorizzazione: inserisci ente + n. + data
- [ ] Se presenti lavori precedenti: spunta `chkPrecLavori` e inserisci ente + n. + data
- [ ] Seleziona il radio **Provvedimenti di sospensione**; se esistono: inserisci ente + n. + data
- [ ] Seleziona il radio **Collaudo opere**; se necessario: seleziona la modalità di nomina
- [ ] Inserisci la **data di inizio lavori** (GG/MM/AAAA)
- [ ] Inserisci la **data di fine lavori** (GG/MM/AAAA)
- [ ] Inserisci **cognome, nome e CF** del progettista strutturale dichiarante

### Campi presenti ma non validati ℹ️

- **Scheda 2** (Direttore dei lavori architettonici) — nessun campo validato; compilarla è facoltativo
- **Titolarità** (`cmbTitoloSuImm`) — menu "In qualità di" non validato
- **Procedimento edilizio** (`txtProcEdilizio`, `txtNumProcEdilizio`, `txtDataProcEdilizio`) — dati del titolo abilitativo, non validati
- **Costruttore** (scheda 5) — tutti i campi non validati
- **Con studio in** (sezione delle schede 1 e 3) — città, indirizzo, telefono, cellulare non validati
- **Note aggiuntive** (`txtNote`) — facoltative

### Differenze principali DST vs Denuncia Sismica ordinaria ⚠️

La DST si distingue per la descrizione come lavori già realizzati. Aggiunge la doppia checkbox art. 65/93 (nella denuncia ordinaria è invece un radio button per il tipo di intervento). Richiede la pericolosità geomorfologica e le coordinate ETRF89/WGS84 obbligatorie. Ha la sezione Collaudo opere con nomina collaudatore (assente nella denuncia ordinaria). Ha la sezione Provvedimenti di sospensione. Le schede professionisti hanno 14 campi obbligatori anziché i 3 (cognome+nome+CF) della denuncia ordinaria.

### Errori frequenti DST 🔍

1. **Nessuna checkbox art. 65/93 spuntata** → le due checkbox si trovano sotto la descrizione; è l'unico errore della sezione descrizione oltre al testo vuoto
2. **Pericolosità geomorfologica dimenticata** → campo specifico piemontese, spesso non riconosciuto; si trova nella cartografia PAI, non è la zona sismica
3. **Coordinate geografiche mancanti** → latitudine e longitudine sono obbligatorie; usare Google Maps (clic destro → "Cosa c'è qui?") per ricavarle se non disponibili negli elaborati
4. **Scheda 3 (Progettista strutture) compilata parzialmente** → la scheda ha 14 campi obbligatori; spesso si compilano solo cognome/nome/CF omettendo residenza completa e dati ordine
5. **Collaudo: radio c_2 senza sotto-radio nomina** → selezionare "necessita collaudatore" attiva 3 sotto-radio inizialmente disabilitati che diventano cliccabili; la selezione è obbligatoria
6. **Sezione "Progettista strutturale" finale confusa con scheda 3** → sono due sezioni distinte; la scheda 3 è la scheda professionista completa nella sezione COMUNICA, mentre la sezione finale raccoglie solo i 3 campi identificativi del soggetto dichiarante

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
**Fonte**: Analisi codice ValidaDatiDST e DatiDST.ascx
