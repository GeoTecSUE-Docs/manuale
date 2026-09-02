---
title: Errori Comunicazione di Inizio Lavori (C.I.L.) - Regione Lombardia
parent: Errori di validazione
nav_order: 64
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori (CIL) - Regione Lombardia (art. 6 c. 1 lett. e-bis D.P.R. 380/2001, Lr 12/05)
keywords: [CIL, comunicazione inizio lavori, Lombardia, opere temporanee, 90 giorni, 180 giorni, parti comuni, coordinate UTM, WGS84, impresa esecutrice, sicurezza lavoro, privacy checkbox]
IDRegione: 4
IDTipoPratica: 424
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Inizio Lavori (C.I.L.)
## Regione Lombardia

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori (CIL)** per opere temporanee e stagionali — Regione Lombardia, ai sensi dell'art. 6, comma 1, lettera e-bis) del D.P.R. 380/2001 (come sostituita dall'art. 10, c. 1, lett. c) del D.L. 76/2020 conv. con modificazioni dalla L. 120/2020) e dell'art. 62, c. 1-ter della L.R. 11 marzo 2005, n. 12.

{: .note }
> La CIL Lombardia è simile alla [CIL Liguria](errori-validazione-cil-241.html) per la logica delle date (stessi controlli su inizio lavori ≥ oggi e fine ≤ 90 giorni dall'inizio) ma ha differenze strutturali importanti: la sezione "Opere su parti comuni" usa una **struttura radio + checkbox** a 2 livelli (radio "non riguardano" / "riguardano" → se "riguardano": almeno una delle 3 checkbox); sono presenti le **coordinate UTM WGS84 32N** con validazione degli intervalli (come tutte le pratiche Lombardia); la sezione comunicazioni contestuali ha **5 righe** invece di 2; la **privacy è una checkbox obbligatoria** da spuntare. Il campo `txtSpecifTitolarita1` ("Specificare se altro") è visibile nel modulo ma **non viene validato** — a differenza di altre pratiche Lombardia. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Date lavori e descrizione](#3-date-lavori-e-descrizione)
4. [Localizzazione dell'intervento](#4-localizzazione-dellintervento)
5. [Coordinate UTM WGS84 32N](#5-coordinate-utm-wgs84-32n)
6. [Comunicazioni contestuali](#6-comunicazioni-contestuali)
7. [Impresa esecutrice dei lavori](#7-impresa-esecutrice-dei-lavori)
8. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#8-sicurezza-sul-lavoro-dlgs-812008)
9. [Privacy](#9-privacy)
10. [Imprese nei soggetti coinvolti](#10-imprese-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` e il campo "Specificare se altro" (`txtSpecifTitolarita1`) sono presenti nel modulo ma **non vengono validati** — a differenza di alcune altre pratiche Lombardia (es. SCA Lombardia). Non generano errori se non compilati.

---

## 2. Opere su parti comuni o modifiche esterne

La CIL Lombardia usa una struttura a **2 livelli** per le opere su parti comuni: prima un radio group, poi (se si sceglie "riguardano") almeno una checkbox tra tre opzioni.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'. (radio mancante)

**Causa**: Nessuno dei 2 radio button `$OpereComuni` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbOpereComunid_1** — "non riguardano opere comuni"
- ⚪ **rdbOpereComunid_2** — "riguardano" → spunta almeno una delle 3 checkbox sottostanti

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'. (checkbox mancante)

**Causa**: Hai selezionato `rdbOpereComunid_2` ("riguardano") ma nessuna delle 3 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 3 checkbox che si attivano dopo aver selezionato "riguardano":
- ☐ **chkOpereb_2** — "le parti comuni di un fabbricato condominiale" (l'amministratore deve disporre della delibera assembleare)
- ☐ **chkOpereb_3** — "parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ☐ **chkOpereb_4** — "parti dell'edificio di proprietà comune ma non necessitano di assenso dei comproprietari perché, secondo l'art. 1102 c.c., apportano le modificazioni necessarie per il miglior godimento delle parti comuni"

{: .note }
> Le 3 checkbox sono abilitate solo dopo la selezione di `rdbOpereComunid_2` — se non sono cliccabili, verificare di aver selezionato il radio "riguardano" e che la pagina si sia aggiornata. Il messaggio di errore per il radio mancante e per le checkbox mancanti è identico — il validatore distingue i due casi internamente ma mostra lo stesso testo.

---

## 3. Date lavori e descrizione

La sezione "COMUNICA — Qualificazione dell'intervento" contiene 2 checkbox indipendenti per le date e il campo descrizione. Almeno una checkbox deve essere spuntata.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione di inizio dei lavori'.

**Causa**: Nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkPresCILc_1** — "i lavori avranno inizio in data ___" → inserisci data ≥ oggi (GG/MM/AAAA)
- ☐ **chkPresCILc_2** — "i lavori termineranno in data ___" → inserisci data fine (GG/MM/AAAA)

---

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: `chkPresCILc_1` è spuntata ma `txtDataInizioLavori` è vuoto.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data di inizio non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! La data di inizio non può essere inferiore alla data di inoltro.

**Causa**: La data di inizio lavori è antecedente a oggi.

**Soluzione**: Inserisci una data di inizio lavori **uguale o successiva a oggi**.

---

### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Causa**: `chkPresCILc_2` è spuntata ma `txtDataFineLavori` è vuoto.

**Soluzione**: Inserisci la data prevista di fine lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori)

**Causa**: La data di fine non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! La data di fine non può essere inferiore alla data di inizio.

**Causa**: Entrambe le checkbox sono spuntate ma la data fine è antecedente alla data inizio.

**Soluzione**: Correggi la data di fine in modo che sia **uguale o successiva** alla data di inizio.

---

### ATTENZIONE ! La data di fine non può essere superiore di 90 giorni rispetto alla data di inizio.

**Causa**: Entrambe le checkbox sono spuntate ma l'intervallo supera i **90 giorni**.

**Soluzione**: Riduci la data di fine lavori entro 90 giorni dalla data di inizio.

{: .note }
> Il modulo descrive le opere come quelle "da rimuovere entro un termine non superiore a **centottanta giorni**" (180 giorni, ai sensi del D.L. 76/2020 conv. L. 120/2020) mentre il validatore continua a usare il **limite di 90 giorni** — discrepanza tra il testo normativo nel modulo e il controllo implementato nel codice. Se la vostra opera dura tra 91 e 180 giorni, contattare l'ufficio SUE per verificare la procedura corretta da seguire in attesa di aggiornamento del sistema.

---

### ATTENZIONE ! Campo obbligatorio 'Descrizione opere' non inserito.

**Dove si trova**: Campo multiriga `txtDescrIntervento` "le opere consistono in:" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto.

**Soluzione**: Inserisci la descrizione delle opere temporanee (max **300 caratteri**).

---

## 4. Localizzazione dell'intervento

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

## 5. Coordinate UTM WGS84 32N

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Causa**: Il campo `txtCoordinateX` è vuoto.

**Soluzione**: Inserisci la coordinata X (asse Est) nel sistema UTM WGS84 32N. Deve essere compresa tra **430.000 e 700.000** metri.

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: Il valore della coordinata X è fuori intervallo o non numerico.

**Soluzione**: Verifica che la coordinata X sia un numero tra **430.000 e 700.000**. Usa il punto come separatore decimale.

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo `txtCoordinateY` è vuoto.

**Soluzione**: Inserisci la coordinata Y (asse Nord) nel sistema UTM WGS84 32N. Deve essere compresa tra **4.800.000 e 5.700.000** metri.

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Il valore della coordinata Y è fuori intervallo o non numerico.

**Soluzione**: Verifica che la coordinata Y sia un numero tra **4.800.000 e 5.700.000**. Usa il punto come separatore decimale.

{: .note }
> Gli intervalli di validazione (X: 430k-700k; Y: 4800k-5700k) sono identici a quelli delle altre pratiche Lombardia (CILA, SCIA, PdC, SCA, DS). Per trovare le coordinate puoi usare il bottone "Calcola Coordinate" se disponibile, oppure un GIS o la cartografia comunale.

---

## 6. Comunicazioni contestuali

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito.

**Dove si trova**: Sezione "Altre comunicazioni, segnalazioni e asseverazioni eventualmente necessarie alla realizzazione delle opere presentate contestualmente alla comunicazione di inizio lavori" → una delle 5 righe (chkPres3_1..chkPres3_5) → campo `txtTipologiaAtto3_N`

**Causa**: Una delle 5 checkbox (`chkPres3_1`..`chkPres3_5`) è spuntata ma il campo "Comunicazioni, segnalazioni, etc." della riga corrispondente è vuoto.

**Soluzione**: Inserisci la tipologia dell'atto comunicativo contestuale nel campo "Comunicazioni, segnalazioni, etc." della riga spuntata.

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito.

**Causa**: Una checkbox `chkPres3_N` è spuntata e il campo tipologia è compilato, ma il campo "Autorità competente" (`txtAutComp3_N`) è vuoto.

**Soluzione**: Inserisci l'ente destinatario della comunicazione contestuale nel campo "Autorità competente".

{: .note }
> La CIL Lombardia ha **5 righe** di comunicazioni contestuali (chkPres3_1..5) invece delle 2 della CIL Liguria. Per ciascuna riga spuntata sono obbligatori entrambi i campi: tipologia e autorità competente. Il validatore scorre le righe in sequenza e si ferma al primo campo mancante.

---

## 7. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **f_1** — "che i lavori sono/saranno eseguiti dalla impresa/e indicata/e alla sezione imprese esecutrici dei 'Soggetti coinvolti'" → deve essere presente almeno un'impresa
- ⚪ **f_2** — "che, in quanto opere di modesta entità [...] i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"

---

## 8. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessun radio button `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **g_1** — "non ricade nell'ambito di applicazione [...] (d.lgs. n. 81/2008)"
- ⚪ **g_2** — "ricade [...] e pertanto" → seleziona documentazione imprese; se g_2_2: seleziona il radio notifica
- ⚪ **g_3** — "ricade [...] ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato g_2 ma nessuno dei 2 radio button `$ImpEs` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_2_1** — "entità presunta del cantiere inferiore a 200 uomini-giorno e lavori senza rischi particolari (Allegato XI)"
- ⚪ **g_2_2** — "entità presunta del cantiere pari o superiore a 200 uomini-giorno o con rischi particolari" → seleziona il radio notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato g_2_2 ma nessuno dei 2 radio button `$Notifica` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_2_2_1** — "l'intervento non è soggetto all'invio della notifica"
- ⚪ **g_2_2_2** — "l'intervento è soggetto all'invio della notifica e" → la checkbox `chkAllegal1_1_4_1` (notifica su Ge.CA) è presente ma **non validata**

{: .note }
> Come la [CIL Liguria](errori-validazione-cil-241.html), la sicurezza della CIL Lombardia si ferma a **3 livelli** di validazione — la checkbox della notifica Ge.CA (`chkAllegal1_1_4_1`) e la checkbox "di essere a conoscenza" (`chkConoscenza`) sono presenti nel modulo ma non vengono validate dal codice.

---

## 9. Privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione "Rispetto della normativa sulla privacy" → checkbox `chkPrivacy` "di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune"

**Causa**: La checkbox `chkPrivacy` non è spuntata.

**Soluzione**: Spunta la checkbox privacy.

{: .warning }
> Come nella [DS Lombardia](errori-validazione-ds-417.html), la privacy è una **checkbox obbligatoria** da spuntare attivamente — non è solo un testo informativo. Viene validata come penultimo controllo, prima solo della verifica imprese nei soggetti.

---

## 10. Imprese nei soggetti coinvolti

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato `rdbImpresaf_1` ma nessuna impresa è presente nei soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice, oppure seleziona f_2 per lavori in economia diretta.

---

## Consigli pratici — CIL Lombardia

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona le **opere su parti comuni**: "non riguardano" (d_1) oppure "riguardano" (d_2) → se d_2: spunta almeno una delle 3 checkbox (b_2/b_3/b_4)
- [ ] Spunta almeno una delle 2 checkbox date; se c_1: data ≥ oggi (GG/MM/AAAA); se c_2: data fine; se entrambe: data fine ≥ inizio E ≤ 90 giorni dall'inizio
- [ ] Inserisci la **descrizione delle opere** (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci **coordinata X** (430.000 – 700.000) e **coordinata Y** (4.800.000 – 5.700.000)
- [ ] Se si spuntano le comunicazioni contestuali: compila **tipologia** e **autorità competente** per ciascuna riga (fino a 5 righe disponibili)
- [ ] Seleziona il **radio impresa** (f_1/f_2); se f_1: aggiungi almeno un'impresa nei soggetti
- [ ] Seleziona la **sicurezza** (g_1/g_2/g_3); se g_2: compila i 3 livelli
- [ ] Spunta la **checkbox Privacy**

### Campi e sezioni non validati ℹ️

Il radio `$TipoComunicazioneCIL` (tipo CIL: opere temporanee / serre mobili) è presente con il primo radio preselezionato ma **non validato**. Il campo `txtSpecifTitolarita1` ("Specificare se altro") non viene validato. Le checkbox `chkAllegal1_1_4_1` (notifica Ge.CA) e `chkConoscenza` (consapevolezza sospensione efficacia) non vengono validate.

### Differenze rispetto alla CIL Liguria ⚠️

La CIL Lombardia si differenzia dalla CIL Liguria per: struttura opere comuni a 2 livelli (radio + 3 checkbox) invece di 4 radio; presenza delle coordinate UTM obbligatorie; 5 righe comunicazioni contestuali invece di 2; checkbox privacy obbligatoria; limite 90 giorni per la data fine (disallineato rispetto ai 180 giorni citati nel testo del modulo ai sensi della L. 120/2020).

### Errori frequenti 🔍

1. **d_2 selezionato senza checkbox** → dopo aver scelto "riguardano", bisogna spuntare almeno una delle 3 checkbox che si abilitano
2. **Privacy non spuntata** → ultimo controllo prima delle imprese soggetti; ricordarsi di spuntarla
3. **Coordinate fuori intervallo** → usare il punto come separatore decimale; X tra 430000 e 700000; Y tra 4800000 e 5700000
4. **Data fine >90 giorni dall'inizio** → il validatore usa 90 giorni anche se il modulo cita 180 giorni; per opere tra 91 e 180 giorni contattare il SUE

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Vedi anche [CIL Liguria](errori-validazione-cil-241.html) per confronto
3. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiCILLombardia e DatiCILLombardia.ascx
