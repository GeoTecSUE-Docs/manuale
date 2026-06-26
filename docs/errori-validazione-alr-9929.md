---
title: Errori Attività Libera Fonti Rinnovabili - Tutte le regioni
parent: Errori di validazione
nav_order: 35
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori per Attività Libera per la Produzione di Energia da Fonti Rinnovabili (ALR) - Tutte le regioni
keywords: [attività libera fonti rinnovabili, ALR, D.Lgs. 190/2024, energia rinnovabile, nuova costruzione, impianti esistenti, variante in corso d'opera, comunicazione inizio lavori, data inizio lavori futura, impresa esecutrice, altri atti di assenso]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9928
IDTarget:
  - { Reg: 2, Prat: 28 }   # Piemonte - ALR
  - { Reg: 1, Prat: 128 }   # Valle d'Aosta - ALR
  - { Reg: 3, Prat: 328 }   # Liguria - ALR
  - { Reg: 4, Prat: 428 }   # Lombardia - ALR
  - { Reg: 6, Prat: 628 }   # Veneto - ALR
  - { Reg: 8, Prat: 828 }   # Emilia-Romagna - ALR
  - { Reg: 12, Prat: 1228 }  # Lazio - ALR
  - { Reg: 13, Prat: 1328 }  # Abruzzo - ALR
  - { Reg: 15, Prat: 1528 }  # Campania - ALR
  - { Reg: 16, Prat: 1628 }  # Basilicata - ALR
  - { Reg: 17, Prat: 1728 }  # Puglia - ALR
  - { Reg: 18, Prat: 1828 }  # Calabria - ALR
  - { Reg: 19, Prat: 1928 }  # Sicilia - ALR
Fonte: Manuale
---

# Errori di validazione - Attività Libera per la Produzione di Energia da Fonti Rinnovabili (ALR)
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori per Attività Libera per la Produzione di Energia da Fonti Rinnovabili** ai sensi del D.Lgs. 190/2024 (Allegato A, Sezioni I e II).

{: .note }
> L'ALR condivide con l'AEL la struttura "checkbox + data futura obbligatoria" per l'inizio lavori, con lo stesso messaggio e la stessa logica VB (`DateDiff("d", DataI, CDate(Now)) > 0`). Rispetto all'AEL presenta alcune sezioni aggiuntive specifiche: la **tipologia di intervento** ai sensi del D.Lgs. 190/2024 (tre radio button, due con campo comma/lettera obbligatorio e uno — variante — con numero e data della comunicazione precedente), e la sezione **"Altri atti di assenso"** con la stessa logica della sezione "Altre comunicazioni" della C.I.L. ma con prefisso corretto (`chkPres4_` = `txtPres4_` = `txtAutComp4_`). La **sezione Impresa** ha un unico radio button senza alternativa "lavori in proprio": l'impresa è quindi sempre obbligatoria. La **sezione Tecnici** è commentata nel codice e non viene validata. La privacy è solo informativa. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Opere su parti comuni o modifiche esterne](#2-opere-su-parti-comuni-o-modifiche-esterne)
3. [Comunicazione di inizio lavori — checkbox e data](#3-comunicazione-di-inizio-lavori--checkbox-e-data)
4. [Descrizione delle opere](#4-descrizione-delle-opere)
5. [Tipo di intervento D.Lgs. 190/2024](#5-tipo-di-intervento-dlgs-1902024)
6. [Localizzazione dell'intervento](#6-localizzazione-dellintervento)
7. [Impresa esecutrice dei lavori](#7-impresa-esecutrice-dei-lavori)
8. [Altri atti di assenso](#8-altri-atti-di-assenso)

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

## 3. Comunicazione di inizio lavori — checkbox e data

### ATTENZIONE ! Necessario spuntare la voce di inizio lavori.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → checkbox **"i lavori avranno inizio in data ___"**

**Causa**: Non hai spuntato la checkbox che attiva la comunicazione di inizio lavori.

**Soluzione**:
1. Trova la sezione **"COMUNICA L'INIZIO DEI LAVORI"** → voce **"di opere di attività libera"**
2. Spunta la checkbox ☑ **"i lavori avranno inizio in data"**
3. Inserisci la data nel campo che si attiva, nel formato **GG/MM/AAAA**
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Come nell'AEL, la checkbox è obbligatoria e il campo data si abilita solo dopo averla spuntata. A differenza della C.I.L., nell'ALR non è presente una seconda checkbox per la data di fine lavori: solo la data di inizio è richiesta.

---

### ATTENZIONE ! Campo obbligatorio 'Data inizio lavori' non inserito.

**Causa**: Hai spuntato la checkbox ma non hai inserito la data di inizio lavori.

**Soluzione**: Inserisci la data nel campo accanto alla checkbox nel formato **GG/MM/AAAA** (es. `20/07/2026`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data di inizio lavori è in un formato non riconosciuto.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `20/07/2026` ✅. Errati: `20-07-2026` ❌, `20/07/26` ❌.

---

### ATTENZIONE ! La data di inizio non può essere inferiore alla data odierna.

**Dove si trova**: Campo data accanto alla checkbox di inizio lavori

**Causa**: Hai inserito una data di inizio lavori precedente alla data odierna.

**Soluzione**:
1. Verifica la data inserita: deve essere uguale o successiva alla **data odierna**
2. Se i lavori iniziano oggi: inserisci la data odierna
3. Se i lavori sono già iniziati: questa comunicazione non è presentabile con data retroattiva; contatta l'ufficio SUE

{: .warning }
> **Controllo data futura condiviso con AEL**: come nell'AEL, il sistema verifica che la data di inizio non sia nel passato (`DateDiff("d", DataI, CDate(Now)) > 0`). La C.I.L. usa invece la dicitura "data di inoltro" nel messaggio (il controllo VB è identico). Una data uguale a oggi è accettata in entrambe le pratiche.

---

## 4. Descrizione delle opere

### ATTENZIONE ! Campo obbligatorio 'Descrizione opere' non inserito.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → campo di testo **"le opere consistono in:"**

**Causa**: Non hai inserito la descrizione delle opere per la produzione di energia da fonti rinnovabili.

**Soluzione**: Inserisci una descrizione chiara e sintetica nel campo **"le opere consistono in:"** (max **300 caratteri**). Esempi:
- `Installazione impianto fotovoltaico su falda tetto, potenza 6 kWp, n. 15 pannelli da 400W.`
- `Installazione mini-eolico da 3 kW su palo h 10m in area agricola di proprietà.`
- `Sostituzione caldaia a gas con pompa di calore aria-acqua 12 kW per riscaldamento domestico.`

---

## 5. Tipo di intervento D.Lgs. 190/2024

### ATTENZIONE ! Non è stata selezionata nessuna voce per il tipo di intervento.

**Dove si trova**: Sezione **"COMUNICA L'INIZIO DEI LAVORI"** → radio button sotto **"e riguardano:"**

**Causa**: Non hai selezionato la tipologia di intervento prevista dal D.Lgs. 190/2024.

**Soluzione**: Seleziona **uno dei tre tipi di intervento**:
- ⚪ **e.1** — interventi di **nuova costruzione** indicati alla Sezione I - Allegato A del D.Lgs. 190/2024, di cui all'art. 1 comma ___ → richiede l'indicazione della lettera del comma
- ⚪ **e.2** — interventi **su impianti esistenti** indicati alla Sezione II - Allegato A del D.Lgs. 190/2024, di cui all'art. 1 comma ___ → richiede l'indicazione della lettera del comma
- ⚪ **e.4** — **variante in corso d'opera** il cui intervento risulta precedentemente comunicato → richiede numero e data della comunicazione precedente

---

### ATTENZIONE ! Inserire il comma. *(nuova costruzione — e.1)*

**Dove si trova**: Campo lettera accanto al radio button e.1

**Causa**: Hai selezionato il tipo "nuova costruzione" (e.1) ma non hai indicato la lettera del comma dell'art. 1 del D.Lgs. 190/2024, Sezione I, Allegato A.

**Soluzione**: Inserisci la lettera del comma applicabile nel campo **"(inserire la lettera relativa)"** che si attiva accanto al radio button e.1 (es. `a`, `b`, `c`, ecc.). Consulta l'Allegato A, Sezione I, del D.Lgs. 190/2024 per individuare la categoria di intervento corretta.

{: .note }
> Il campo è etichettato nell'interfaccia come "inserire la lettera relativa" e il messaggio di errore recita "Inserire il comma": si tratta della lettera identificativa della fattispecie del comma, non del numero del comma in senso stretto. Il campo `txtNCComma` raccoglie la lettera (es. `a`) che qualifica la tipologia di nuova costruzione.

---

### ATTENZIONE ! Inserire il comma. *(impianti esistenti — e.2)*

**Dove si trova**: Campo lettera accanto al radio button e.2

**Causa**: Hai selezionato il tipo "impianti esistenti" (e.2) ma non hai indicato la lettera del comma dell'art. 1 del D.Lgs. 190/2024, Sezione II, Allegato A.

**Soluzione**: Inserisci la lettera del comma applicabile nel campo **"(inserire la lettera relativa)"** accanto al radio button e.2. Consulta l'Allegato A, Sezione II, del D.Lgs. 190/2024.

---

### ATTENZIONE ! Inserire il numero della comunicazione. *(variante — e.4)*

**Dove si trova**: Campo numero accanto al radio button e.4

**Causa**: Hai selezionato il tipo "variante in corso d'opera" (e.4) ma non hai inserito il numero della comunicazione precedente a cui la presente è in variante.

**Soluzione**: Inserisci il numero della comunicazione originaria nel campo **"comunicazione n."** che si attiva accanto al radio button e.4.

---

### ATTENZIONE ! Inserire la data della comunicazione. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(variante — e.4)*

**Dove si trova**: Campo data accanto al radio button e.4 → **"del"**

**Causa**: Hai selezionato la variante (e.4) e inserito il numero della comunicazione precedente, ma il campo data è vuoto oppure contiene una data in formato non valido.

**Soluzione**: Inserisci la data della comunicazione originaria nel campo **"del"** nel formato **GG/MM/AAAA**.

---

## 6. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

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

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 7. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai selezionato il radio button relativo all'impresa esecutrice.

**Soluzione**: Seleziona l'unica opzione disponibile:
- ⚪ **"che i lavori sono/saranno eseguiti dalla impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'"**

Quindi aggiungi l'impresa nella scheda **"Soggetti coinvolti"** → sezione **"Imprese"**.

{: .warning }
> **Differenza rispetto ad AEL e C.I.L.**: nell'ALR la sezione Impresa ha **un solo radio button** senza l'alternativa "lavori eseguiti in prima persona". L'indicazione dell'impresa esecutrice nei Soggetti coinvolti è quindi **sempre obbligatoria**: non è possibile dichiarare di eseguire i lavori autonomamente senza ditte esterne.

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato il radio button ma non hai aggiunto nessuna impresa tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → **"Imprese"**
2. Clicca **"Aggiungi Impresa"**
3. Compila i dati dell'impresa e salva
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

## 8. Altri atti di assenso

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito.

**Dove si trova**: Sezione **"Altri atti di assenso"** → campo **"Tipologia di atto"** accanto a una checkbox spuntata

**Causa**: Hai spuntato una delle checkbox nella sezione "Altri atti di assenso" ma non hai compilato il campo **"Tipologia di atto"** della riga corrispondente.

**Soluzione**: Per ogni checkbox spuntata, compila obbligatoriamente entrambi i campi della stessa riga:
- **"Tipologia di atto"** (es. `Autorizzazione paesaggistica`, `Nulla osta idrogeologico`, `Parere ASL`)
- **"Autorità competente al rilascio"** (es. `Soprintendenza`, `Regione`, `ASL`)

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito.

**Causa**: Hai spuntato una checkbox e compilato la tipologia ma hai lasciato vuoto il campo **"Autorità competente al rilascio"** della stessa riga.

**Soluzione**: Inserisci l'autorità competente al rilascio dell'atto nella stessa riga della tipologia già compilata.

{: .note }
> A differenza della C.I.L. nazionale (dove esiste una disallineamento tra i prefissi dei checkbox nell'ASCX e nel codice VB), nell'ALR i checkbox della sezione "Altri atti di assenso" usano il prefisso `chkPres4_` che **corrisponde correttamente** ai campi `txtPres4_N` e `txtAutComp4_N` dell'ASCX. La validazione di questa sezione funziona regolarmente per tutte le 5 righe disponibili (`chkPres4_1` … `chkPres4_5`).

---

## Consigli pratici ALR

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (menu a discesa + radio button)
- [ ] Seleziona le **opere su parti comuni** (una delle 4 opzioni)
- [ ] **Spunta la checkbox** "i lavori avranno inizio in data"
- [ ] Inserisci la **data di inizio lavori** nel formato GG/MM/AAAA — deve essere oggi o futura
- [ ] Inserisci la **descrizione delle opere** (max 300 caratteri)
- [ ] Seleziona il **tipo di intervento D.Lgs. 190/2024** (e.1, e.2 o e.4)
- [ ] **Se e.1 (nuova costruzione)**: inserisci la **lettera del comma** Sezione I, Allegato A
- [ ] **Se e.2 (impianti esistenti)**: inserisci la **lettera del comma** Sezione II, Allegato A
- [ ] **Se e.4 (variante)**: inserisci **numero** e **data** della comunicazione originaria (GG/MM/AAAA)
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **radio button Impresa** e aggiungi l'**impresa** nei Soggetti coinvolti
- [ ] Se compilata, verifica che ogni checkbox spuntata in "Altri atti di assenso" abbia **Tipologia** e **Autorità competente**
- [ ] **Salva** frequentemente

### Confronto ALR con pratiche simili ⚠️

| Caratteristica | AEL | C.I.L. | ALR |
|---|---|---|---|
| Checkbox inizio lavori obbligatoria | ☑ Sì | ☑ Sì | ☑ Sì |
| Data inizio = futura | ☑ Sì | ☑ Sì (= oggi accettato) | ☑ Sì (= oggi accettato) |
| Checkbox fine lavori | ✗ No | ☑ Sì (max 90 gg) | ✗ No |
| Tipo intervento con lettera/comma | ✗ No | ✗ No | ☑ Sì (D.Lgs. 190/2024) |
| Impresa "in proprio" alternativa | ✗ No | ☑ Sì | ✗ No |
| Sezione Sicurezza D.Lgs. 81/2008 | ✗ No | ☑ Sì | ✗ No |
| Altri atti di assenso validati | ✗ No | ✗ No (bug prefisso) | ☑ Sì (funzionante) |
| Tecnici obbligatori | ✗ No | ✗ No | ✗ No (commentato) |

### Errori frequenti ALR 🔍

1. **Checkbox inizio lavori non spuntata** → il campo data non è autonomo: senza checkbox il sistema blocca prima ancora di verificare la data
2. **Data nel passato** → uguale all'AEL: deve essere oggi o futura; i lavori già iniziati non sono presentabili con questa comunicazione
3. **Tipo intervento senza lettera comma** → selezionare e.1 o e.2 abilita il campo lettera ma non lo pre-compila; la lettera va inserita manualmente
4. **Variante senza numero o data** → selezionare e.4 abilita entrambi i campi; sono entrambi obbligatori con validazione formato data
5. **Impresa non aggiunta nei soggetti** → nell'ALR non esiste l'opzione "lavori in proprio"; l'impresa è sempre obbligatoria nei Soggetti coinvolti

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
**Fonte**: Analisi codice `ValidaDatiALR` e `DatiALR.ascx`
