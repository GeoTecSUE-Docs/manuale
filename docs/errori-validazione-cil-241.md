---
title: Errori Comunicazione di Inizio Lavori (C.I.L.) - Regione Liguria
parent: Errori di validazione
nav_order: 59
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori (CIL) - Regione Liguria (art. 6 c. 1 lett. e-bis D.P.R. 380/2001, n. 26 Tabella A Sez. II D.Lgs. 222/2016)
keywords: [CIL, comunicazione inizio lavori, Liguria, opere temporanee, 90 giorni, data inizio lavori, data fine lavori, parti comuni, impresa esecutrice, sicurezza lavoro]
IDRegione: 3
IDTipoPratica: 241
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Inizio Lavori (C.I.L.)
## Regione Liguria

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori (CIL)** per opere dirette a soddisfare obiettive esigenze contingenti e temporanee, da rimuovere entro 90 giorni — ai sensi dell'art. 6, comma 1, lettera e-bis) del D.P.R. 6 giugno 2001, n. 380 e del n. 26 della Tabella A, Sezione II del D.Lgs. 25 novembre 2016, n. 222 — Regione Liguria.

{: .note }
> La CIL Liguria è una delle pratiche più semplici del sistema, ma ha una caratteristica specifica: la sezione "Comunicazione di inizio dei lavori" usa **due checkbox indipendenti** (data inizio lavori e data fine lavori) anziché campi sempre visibili. Ciascuna, se spuntata, attiva la validazione del campo data corrispondente. Se entrambe sono spuntate, il sistema verifica anche la **coerenza temporale** tra le due date e il **limite dei 90 giorni**. La data di inizio non può essere antecedente alla data di inoltro della pratica. La sezione sicurezza ha solo **3 livelli** annidati (a differenza di altre pratiche che ne hanno 4 — la checkbox "allega notifica" non è validata). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Comunicazione di inizio dei lavori — date e descrizione](#3-comunicazione-di-inizio-dei-lavori--date-e-descrizione)
4. [Localizzazione dell'intervento](#4-localizzazione-dellintervento)
5. [Altre comunicazioni contestuali](#5-altre-comunicazioni-contestuali)
6. [Impresa esecutrice dei lavori](#6-impresa-esecutrice-dei-lavori)
7. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#7-sicurezza-sul-lavoro-dlgs-812008)
8. [Imprese nei soggetti coinvolti](#8-imprese-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` è presente ma **non validato**.

---

## 2. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Nessun radio button `$Opere` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **b_1** — "non riguardano parti comuni"
- ⚪ **b_2** — "riguardano le parti comuni di un fabbricato condominiale"
- ⚪ **b_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ⚪ **b_4** — "riguardano parti dell'edificio di proprietà comune ma non necessitano di assenso (art. 1102 c.c.)"

---

## 3. Comunicazione di inizio dei lavori — date e descrizione

La sezione "COMUNICA L'INIZIO DEI LAVORI" contiene **due checkbox indipendenti** per la data di inizio e la data di fine lavori. Almeno una deve essere spuntata. Se entrambe sono spuntate, il sistema verifica la coerenza tra le date. La descrizione delle opere è sempre obbligatoria indipendentemente dalle checkbox.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione di inizio dei lavori'.

**Dove si trova**: Sezione "COMUNICA L'INIZIO DEI LAVORI" → le 2 checkbox `chkPresCILc_1` e `chkPresCILc_2`

**Causa**: Nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle due checkbox:
- ☐ **chkPresCILc_1** — "i lavori avranno inizio in data ___" → inserisci la data di inizio lavori (GG/MM/AAAA, non può essere antecedente alla data di inoltro)
- ☐ **chkPresCILc_2** — "i lavori termineranno in data ___" → inserisci la data di fine lavori (GG/MM/AAAA, non superiore a 90 giorni dall'inizio)

---

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: `chkPresCILc_1` è spuntata ma il campo `txtDataInizioLavori` è vuoto.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data di inizio lavori non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/06/2026`).

---

### ATTENZIONE ! La data di inizio non può essere inferiore alla data di inoltro.

**Causa**: La data di inizio lavori inserita è **antecedente alla data odierna** (data di inoltro della pratica). Il controllo `DateDiff("d", DataI, CDate(Now)) > 0` verifica che la data di inizio non sia nel passato.

**Soluzione**: Inserisci una data di inizio lavori **uguale o successiva a oggi**.

{: .note }
> Questo è uno dei pochi controlli del sistema che verifica la data rispetto alla data corrente (data di inoltro). La CIL è una comunicazione di **inizio** lavori, quindi non è possibile indicare una data già trascorsa. Se i lavori sono già iniziati, verificare con l'ufficio SUE la procedura corretta.

---

### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Causa**: `chkPresCILc_2` è spuntata ma il campo `txtDataFineLavori` è vuoto.

**Soluzione**: Inserisci la data prevista di fine lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori)

**Causa**: La data di fine lavori non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! La data di fine non può essere inferiore alla data di inizio.

**Causa**: Entrambe le checkbox c_1 e c_2 sono spuntate, ma la data di fine lavori è **antecedente alla data di inizio** (`DateDiff("d", DataF, DataI) > 0`).

**Soluzione**: Correggi la data di fine lavori in modo che sia **uguale o successiva** alla data di inizio.

{: .note }
> Questo controllo si attiva solo quando **entrambe** le checkbox c_1 e c_2 sono spuntate e `txtDataInizioLavori` è già stato compilato correttamente. Se è spuntata solo c_2 (fine lavori) senza c_1 (inizio lavori), il confronto non viene eseguito.

---

### ATTENZIONE ! La data di fine non può essere superiore di 90 giorni rispetto alla data di inizio.

**Causa**: Entrambe le checkbox c_1 e c_2 sono spuntate, ma l'intervallo tra data inizio e data fine supera i **90 giorni** (`DateDiff("d", DataI, DataF) > 90`).

**Soluzione**: Riduci la data di fine lavori in modo che l'intervallo dalla data di inizio non superi **90 giorni** (3 mesi circa).

{: .note }
> Il limite di 90 giorni è previsto dall'art. 6, comma 1, lettera e-bis) del D.P.R. 380/2001: le opere temporanee oggetto della CIL devono essere rimosse entro questo termine. Si tratta di un vincolo normativo direttamente implementato nel validatore — non è possibile presentare una CIL per opere temporanee con durata superiore a 90 giorni.

---

### ATTENZIONE ! Campo obbligatorio 'Descrizione opere' non inserito.

**Dove si trova**: Campo multiriga `txtDescrLavori` "le opere consistono in:" (max 300 caratteri)

**Causa**: Il campo descrizione delle opere è vuoto. Viene validato **dopo** l'intero blocco delle date, indipendentemente da quali checkbox siano spuntate.

**Soluzione**: Inserisci la descrizione delle opere temporanee nel campo multiriga (max **300 caratteri**).

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

## 5. Altre comunicazioni contestuali

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito.

**Dove si trova**: Sezione "Altre comunicazioni, segnalazioni e asseverazioni eventualmente necessarie alla realizzazione delle opere presentate contestualmente alla comunicazione di inizio lavori" → campo `txtTipologiaAttoe_1` o `txtTipologiaAttoe_2`

**Causa**: Una delle 2 checkbox `chkPresCILe_1` o `chkPresCILe_2` è spuntata ma il campo "Comunicazioni, segnalazioni, etc." corrispondente è vuoto.

**Soluzione**: Inserisci la tipologia dell'atto (comunicazione, segnalazione o asseverazione contestuale) nel campo testo "Comunicazioni, segnalazioni, etc." affiancato alla checkbox spuntata.

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito.

**Causa**: Una checkbox `chkPresCILe_1` o `chkPresCILe_2` è spuntata e il campo "Comunicazioni, segnalazioni, etc." è compilato, ma il campo "Autorità competente" (`txtAutCompe_N`) è vuoto.

**Soluzione**: Inserisci l'ente o autorità a cui è destinata la comunicazione contestuale nel campo "Autorità competente" affiancato alla checkbox spuntata.

{: .note }
> La sezione "Altre comunicazioni contestuali" ha 2 righe (`chkPresCILe_1` e `chkPresCILe_2`), ciascuna con due campi: "Comunicazioni, segnalazioni, etc." e "Autorità competente". Se si spunta una riga, entrambi i campi diventano obbligatori. Il validatore scorre le righe in sequenza e si ferma al primo campo mancante.

---

## 6. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **f_1** — "che i lavori sono/saranno eseguiti dalla impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'" → deve essere presente almeno un'impresa nei soggetti
- ⚪ **f_2** — "che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"

---

## 7. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessun radio button `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **g_1** — "non ricade nell'ambito di applicazione delle norme [...] (d.lgs. n. 81/2008)"
- ⚪ **g_2** — "ricade nell'ambito di applicazione [...] e pertanto" → seleziona la documentazione imprese; se g_2_2: seleziona il radio notifica
- ⚪ **g_3** — "ricade [...] ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato g_2 ma nessuno dei 2 radio button `$ImpEs` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_2_1** — "entità presunta del cantiere inferiore a 200 uomini-giorno e lavori senza rischi particolari (Allegato XI)"
- ⚪ **g_2_2** — "entità presunta del cantiere pari o superiore a 200 uomini-giorno o lavori con rischi particolari (Allegato XI)" → seleziona il radio notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato g_2_2 ma nessuno dei 2 radio button `$Notifica` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_2_2_1** — "l'intervento non è soggetto all'invio della notifica"
- ⚪ **g_2_2_2** — "l'intervento è soggetto all'invio della notifica e" → la checkbox `chkAllegag_3_2_1` ("allega la notifica") è presente ma **non validata**

{: .note }
> La sezione sicurezza della CIL Liguria ha **3 livelli** annidati (AmbitoRicade → ImpEs → Notifica), a differenza di altre pratiche come la SCIA alt PdC o il PdC Nazionale che ne hanno 4 (con il livello `$Allega` per la modalità di trasmissione della notifica). Il 4° livello nella CIL è rappresentato dalla checkbox `chkAllegag_3_2_1` ("allega la notifica"), ma questa non viene validata dal codice.

---

## 8. Imprese nei soggetti coinvolti

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato `rdbImpresaf_1` ("lavori eseguiti da impresa") ma nessuna impresa è presente nella griglia dei soggetti coinvolti (`DSImprese.Tables(0).Rows.Count = 0`).

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice dei lavori, oppure seleziona f_2 se i lavori vengono eseguiti direttamente dal titolare.

---

## Consigli pratici — CIL Liguria

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona le **opere su parti comuni** (b_1..b_4)
- [ ] Spunta almeno una checkbox tra **data inizio** e **data fine** lavori; se c_1: inserisci data ≥ oggi; se c_2: inserisci data entro 90 giorni dall'inizio; se entrambe: data fine ≥ data inizio
- [ ] Inserisci la **descrizione delle opere** (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Se si spuntano le comunicazioni contestuali e/f: compila **tipologia** e **autorità competente** per ciascuna riga spuntata
- [ ] Seleziona il **radio impresa** (f_1/f_2); se f_1: aggiungi almeno un'impresa nei soggetti
- [ ] Seleziona la **sicurezza** (g_1/g_2/g_3); se g_2: compila i 3 livelli

### Campi presenti ma non validati ℹ️

- **`cmbTitoloSuImm`**: non validato
- **`chkAllegag_3_2_1`** ("allega la notifica"): checkbox presente ma non validata — il 4° livello sicurezza non è implementato
- **Privacy**: solo testo informativo
- **`txtData` e `txtLuogo`** (data e luogo firma): facoltativi

### Logica date — schema riassuntivo ⚠️

Se spuntata solo **c_1**: data inizio deve essere ≥ oggi.

Se spuntata solo **c_2**: data fine deve essere nel formato GG/MM/AAAA; nessun confronto con altra data.

Se spuntate **entrambe c_1 e c_2**: data inizio ≥ oggi; data fine ≥ data inizio; data fine − data inizio ≤ 90 giorni.

### Errori frequenti 🔍

1. **Data inizio nel passato** → il validatore rifiuta date antecedenti a oggi; inserire la data prevista reale di inizio
2. **Intervallo superiore a 90 giorni** → vincolo normativo; le opere temporanee da CIL non possono durare oltre 90 giorni; ridurre la data di fine
3. **Nessuna checkbox spuntata** → almeno una tra data inizio e data fine deve essere spuntata; il campo descrizione rimane comunque obbligatorio
4. **Comunicazione contestuale senza autorità** → se si spunta una riga e/f, entrambi i campi (tipologia e autorità) sono richiesti; spuntare solo se necessario
5. **Impresa f_1 senza soggetti** → aggiungere l'impresa prima di validare, oppure scegliere f_2 per lavori in economia diretta

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
**Fonte**: Analisi codice ValidaDatiCILLiguria e DatiCILLiguria.ascx
