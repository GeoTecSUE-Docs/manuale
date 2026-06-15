---
title: Errori C.I.L. - Tutte le regioni
parent: Errori di validazione
nav_order: 32
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori (C.I.L.) - art. 6 c. 1 lett. e-bis D.P.R. 380/2001
keywords: [CIL, comunicazione inizio lavori, art. 6 DPR 380/2001, data inizio lavori, data fine lavori, 90 giorni, impresa esecutrice, sicurezza lavoro, d.lgs. 81/2008, notifica preliminare]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 124 }   # Valle d'Aosta - CIL
  - { Reg: 6, Prat: 624 }   # Veneto - CIL
  - { Reg: 8, Prat: 824 }   # Emilia-Romagna - CIL
  - { Reg: 12, Prat: 1224 }  # Lazio - CIL
  - { Reg: 13, Prat: 1324 }  # Abruzzo - CIL
  - { Reg: 15, Prat: 1524 }  # Campania - CIL
  - { Reg: 16, Prat: 1624 }  # Basilicata - CIL
  - { Reg: 17, Prat: 1724 }  # Puglia - CIL
  - { Reg: 18, Prat: 1824 }  # Calabria - CIL
  - { Reg: 19, Prat: 1924 }  # Sicilia - CIL
Fonte: Analisi codice
---

# Errori di validazione - C.I.L.
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori** ai sensi dell'art. 6, comma 1, lett. e-bis, del D.P.R. 6 giugno 2001, n. 380.

{: .note }
> La C.I.L. è la comunicazione per opere dirette a soddisfare esigenze contingenti e temporanee, da rimuovere entro 90 giorni. Rispetto all'AEL presenta due sezioni aggiuntive obbligatorie: la **data di fine lavori** (con il vincolo dei 90 giorni dalla data di inizio) e l'intera sezione **Sicurezza sul lavoro (D.Lgs. 81/2008)**, con logica a cascata su documentazione imprese e notifica preliminare. Le date di inizio e fine lavori sono entrambe attivate da checkbox indipendenti. Il controllo sulla data di inizio verifica che non sia **antecedente alla data di inoltro** (non che sia futura in senso stretto, a differenza dell'AEL). Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Comunicazione di inizio e fine lavori — checkbox e date](#3-comunicazione-di-inizio-e-fine-lavori--checkbox-e-date)
4. [Descrizione delle opere](#4-descrizione-delle-opere)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Altre comunicazioni e segnalazioni](#6-altre-comunicazioni-e-segnalazioni)
7. [Impresa esecutrice dei lavori](#7-impresa-esecutrice-dei-lavori)
8. [Sicurezza sul lavoro — D.Lgs. 81/2008](#8-sicurezza-sul-lavoro--dlgs-812008)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Non hai compilato il menu a discesa iniziale né selezionato il radio button sulla titolarità.

**Soluzione**: Compila il menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"** e seleziona una delle due opzioni:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva... ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"**

---

## 2. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Non hai dichiarato se i lavori riguardano parti comuni dell'edificio.

**Soluzione**: Seleziona **una delle quattro opzioni**:
- ⚪ **"non riguardano parti comuni"**
- ⚪ **"riguardano le parti comuni di un fabbricato condominiale"**
- ⚪ **"riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"** (richiede assenso dei comproprietari allegato)
- ⚪ **"riguardano parti dell'edificio di proprietà comune ma non necessitano di assenso"** (art. 1102 c.c.)

---

## 3. Comunicazione di inizio e fine lavori — checkbox e date

Questa sezione gestisce due date indipendenti, ciascuna attivata dalla propria checkbox. Almeno una delle due deve essere spuntata. Se entrambe sono spuntate, il sistema verifica anche la coerenza tra le due date.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione di inizio dei lavori'.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"**

**Causa**: Non hai spuntato nessuna delle due checkbox (né "i lavori avranno inizio in data" né "i lavori termineranno in data").

**Soluzione**:
1. Trova la sezione **"COMUNICA L'INIZIO DEI LAVORI"**
2. Spunta almeno una delle due checkbox:
   - ☑ **"i lavori avranno inizio in data"** → inserisci la data di inizio
   - ☑ **"i lavori termineranno in data"** → inserisci la data di fine
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: Hai spuntato la checkbox di inizio lavori ma non hai inserito la data.

**Soluzione**: Inserisci la data di inizio lavori nel campo accanto alla checkbox nel formato **GG/MM/AAAA** (es. `20/06/2026`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data inserita (di inizio o di fine) ha un formato non riconosciuto dal sistema.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `20/06/2026` ✅. Errati: `20-06-2026` ❌, `20/06/26` ❌. Il messaggio può comparire sia per la data di inizio sia per quella di fine: verifica entrambe.

---

### ATTENZIONE ! La data di inizio non può essere inferiore alla data di inoltro.

**Dove si trova**: Campo data accanto alla checkbox "i lavori avranno inizio in data"

**Causa**: Hai inserito una data di inizio lavori precedente alla data odierna.

**Soluzione**:
1. Verifica la data inserita: deve essere uguale o successiva alla **data odierna**
2. Se i lavori iniziano oggi: inserisci la data odierna
3. Se i lavori sono già iniziati: la C.I.L. deve essere presentata prima dell'inizio; contatta l'ufficio SUE per valutare la procedura applicabile

{: .warning }
> **Differenza con l'AEL**: il messaggio di errore recita "data di inoltro" (non "data odierna"), ma la logica è equivalente — il controllo VB usa `DateDiff("d", DataI, CDate(Now)) > 0`, che blocca qualsiasi data precedente al giorno corrente. Una data uguale a oggi è accettata.

---

### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Causa**: Hai spuntato la checkbox "i lavori termineranno in data" ma non hai inserito la data di fine.

**Soluzione**: Inserisci la data di fine lavori nel campo accanto alla checkbox nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! La data di fine non può essere inferiore alla data di inizio.

**Causa**: La data di fine lavori è precedente alla data di inizio lavori (entrambe inserite).

**Soluzione**: Correggi la data di fine in modo che sia **uguale o successiva** alla data di inizio.

---

### ATTENZIONE ! La data di fine non può essere superiore di 90 giorni rispetto alla data di inizio.

**Causa**: L'intervallo tra data di inizio e data di fine supera i 90 giorni di calendario.

**Soluzione**: La C.I.L. riguarda opere temporanee da rimuovere entro 90 giorni (art. 6, c. 1, lett. e-bis, D.P.R. 380/2001). Riduci la data di fine lavori in modo che l'intervallo non superi i **90 giorni** dalla data di inizio.

{: .note }
> Il controllo VB usa `DateDiff("d", DataI, DataF) > 90`: un intervallo esatto di 90 giorni è accettato, 91 o più viene bloccato. La data di fine viene verificata **solo se anche la data di inizio è compilata**: se la checkbox di inizio non è spuntata, il limite dei 90 giorni non viene controllato.

---

## 4. Descrizione delle opere

### ATTENZIONE ! Campo obbligatorio 'Descrizione opere' non inserito.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → campo di testo **"le opere consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere temporanee oggetto della comunicazione.

**Soluzione**:
1. Trova il campo di testo **"le opere consistono in:"** nella sezione date/lavori
2. Inserisci una descrizione chiara e sintetica delle opere (max **300 caratteri**)
3. Esempi di opere soggette a C.I.L. (art. 6, c. 1, lett. e-bis, D.P.R. 380/2001):
   - `Installazione di struttura temporanea in legno per riparo cantiere, da rimuovere entro 90 giorni.`
   - `Posa di recinzione mobile di cantiere per lavori stradali, con rimozione entro 60 giorni.`
   - `Allestimento di ponteggio leggero per lavori di tinteggiatura facciata, durata stimata 45 giorni.`
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 5. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente nel campo di testo.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non è stato inserito nessun mappale catastale né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅ (tasto verde con spunta)

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata nella ListBox.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Per selezionare più voci tieni premuto CTRL mentre clicchi.

---

## 6. Altre comunicazioni e segnalazioni

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito.

**Causa**: Hai spuntato una delle checkbox nella sezione "Altre comunicazioni, segnalazioni e asseverazioni" ma non hai compilato il campo "Comunicazioni, segnalazioni, etc." corrispondente.

**Soluzione**: Per ogni checkbox spuntata, compila obbligatoriamente entrambi i campi della stessa riga: **"Comunicazioni, segnalazioni, etc."** e **"Autorità competente"**.

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito.

**Causa**: Hai spuntato una checkbox e compilato la tipologia ma hai lasciato vuoto il campo "Autorità competente" della stessa riga.

**Soluzione**: Inserisci l'autorità competente per la comunicazione/segnalazione indicata nella stessa riga.

{: .warning }
> **Anomalia nel codice**: il ciclo di validazione cerca checkbox con ID contenente `chkPresCILe_`, ma nell'ASCX i checkbox della sezione sono dichiarati come `chkPres3_1` … `chkPres3_5`. Se questa discrepanza non è risolta nel code-behind, **la validazione della sezione 6 non viene mai eseguita** e i campi rimangono facoltativi de facto. Segnalare al team di sviluppo.

---

## 7. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai dichiarato chi eseguirà i lavori.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"che i lavori sono/saranno eseguiti dalla impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'"** → l'impresa diventa obbligatoria nei soggetti coinvolti
- ⚪ **"che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"**

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato "i lavori saranno eseguiti da impresa" ma non hai aggiunto nessuna impresa tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Imprese"**
2. Clicca **"Aggiungi Impresa"**
3. Compila i dati dell'impresa e salva
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Se i lavori sono di piccola entità e li esegui personalmente senza affidare a ditte esterne, seleziona la seconda opzione: in questo caso non è necessario aggiungere nessuna impresa nei soggetti coinvolti.

---

## 8. Sicurezza sul lavoro — D.Lgs. 81/2008

Questa sezione ha una logica a cascata: la selezione del primo radio button determina se i controlli successivi diventano obbligatori.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Non hai dichiarato se i lavori ricadono nell'ambito di applicazione del D.Lgs. 81/2008.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **"non ricade nell'ambito di applicazione"** → nessun altro campo obbligatorio in questa sezione
- ⚪ **"ricade nell'ambito di applicazione"** → si attivano i controlli su documentazione imprese e notifica
- ⚪ **"ricade… ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"**

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato "ricade nell'ambito di applicazione" ma non hai dichiarato la dimensione del cantiere.

**Soluzione**: Seleziona **una delle due opzioni** che compaiono nella sottosezione "relativamente alla documentazione delle imprese esecutrici":
- ⚪ **"entità presunta del cantiere inferiore a 200 uomini-giorno"** e nessun rischio particolare All. XI
- ⚪ **"entità presunta del cantiere pari o superiore a 200 uomini-giorno"** o lavori con rischi particolari All. XI

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato "cantiere ≥ 200 uomini-giorno o rischi particolari" ma non hai dichiarato se è prevista la notifica preliminare (art. 99 D.Lgs. 81/2008).

**Soluzione**: Seleziona **una delle due opzioni** nella sottosezione "relativamente alla notifica preliminare":
- ⚪ **"l'intervento non è soggetto all'invio della notifica"**
- ⚪ **"l'intervento è soggetto all'invio della notifica"** → allega la notifica tramite la checkbox **"allega"**

{: .note }
> La sezione Sicurezza è l'unica con tre livelli di validazione annidati: AmbitoRicade → ImpEs → Notifica. Ogni livello viene controllato solo se il livello precedente ha attivato il ramo corrispondente. Selezionando "non ricade" o "si riserva" al primo livello, i controlli successivi vengono saltati interamente.

---

## Consigli pratici C.I.L.

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (menu a discesa + radio button)
- [ ] Seleziona le **opere su parti comuni** (una delle 4 opzioni)
- [ ] Spunta almeno una checkbox: **"i lavori avranno inizio in data"** e/o **"i lavori termineranno in data"**
- [ ] Inserisci la **data di inizio lavori** nel formato GG/MM/AAAA — deve essere oggi o successiva
- [ ] Se compilata, inserisci la **data di fine lavori** nel formato GG/MM/AAAA — non oltre 90 giorni dall'inizio
- [ ] Inserisci la **descrizione delle opere** (max 300 caratteri)
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Se compilata, verifica che ogni checkbox spuntata nella sezione "Altre comunicazioni" abbia **Tipologia** e **Autorità competente**
- [ ] Seleziona l'**impresa esecutrice** (una delle 2 opzioni)
- [ ] Se "lavori da impresa": aggiungi l'**impresa** nei soggetti coinvolti
- [ ] Seleziona il **regime D.Lgs. 81/2008** (una delle 3 opzioni)
- [ ] Se "ricade nell'ambito": seleziona la **documentazione imprese** e, se necessario, la **notifica preliminare**
- [ ] **Salva** frequentemente

### Logica date: differenza con l'AEL ⚠️

| | AEL | C.I.L. |
|---|---|---|
| Data di inizio | Checkbox obbligatoria, data futura | Checkbox opzionale, data ≥ oggi |
| Data di fine | Non presente | Checkbox opzionale, ≤ 90 giorni dall'inizio |
| Messaggio data inizio nel passato | "inferiore alla data odierna" | "inferiore alla data di inoltro" |
| Controllo 90 giorni | Non presente | Presente (solo se entrambe le date sono inserite) |

### Errori frequenti C.I.L. 🔍

1. **Nessuna checkbox spuntata** → almeno una tra inizio e fine deve essere spuntata; il campo data non è autonomo
2. **Data inizio nel passato** → il sistema blocca date precedenti al giorno corrente, come per l'AEL
3. **Fine oltre i 90 giorni** → errore esclusivo della C.I.L.; ridurre la data di fine o ricalcolare l'intervallo
4. **Sezione 81/2008 non compilata** → spesso dimenticata perché è in fondo al modulo; è obbligatoria indipendentemente dalla dimensione del cantiere
5. **Impresa non aggiunta nei soggetti** → scegliere il radio "lavori da impresa" obbliga ad aggiungere l'impresa nella scheda Soggetti coinvolti

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

**Ultima revisione**: Giugno 2026
**Fonte**: Analisi codice `ValidaDatiCILNazionale` e `DatiCILNaz.ascx`
