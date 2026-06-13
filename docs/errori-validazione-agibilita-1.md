---
title: Errori Richiesta di Agibilità - Regione Piemonte
parent: Errori di validazione
nav_order: 71
description: Errori di validazione per la Richiesta del Certificato di Agibilità - Regione Piemonte (art. 25 c. 1 D.P.R. 380/2001)
keywords: [agibilità, certificato agibilità, Piemonte, art. 25 DPR 380, titoli abilitativi, collaudo statico, urbanizzazione primaria, abitabilità, prevenzione incendi, sicurezza impianti, oggetto agibilità]
IDRegione: 2
IDTipoPratica: 1
Fonte: Manuale
---

# Errori di validazione - Richiesta di Agibilità
## Regione Piemonte

Guida completa agli errori specifici per la **Richiesta del Certificato di Agibilità** ai sensi dell'art. 25, comma 1 del D.P.R. 6 giugno 2001, n. 380 e ss.mm.ii. — Regione Piemonte.

{: .note }
> La Richiesta di Agibilità Piemonte è strutturalmente molto simile alla [Comunicazione di Agibilità (CAGI)](errori-comunicazione-agibilita-piemonte.html), con la stessa sezione "Titolarità" basata su checkbox di titoli edilizi (PdC/DIA/SCIA/CILA con varianti). La differenza principale è nella sezione documentazione: mentre la CAGI usa "TRASMETTE", questa usa "RICHIEDE" con "DICHIARA" e ha una struttura diversa delle checkbox di documentazione — in particolare la checkbox `chkd_12` (sicurezza impianti) ha 23 sotto-opzioni verificate dal validatore (contro le 3 "parent" della CAGI). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titoli abilitativi edilizi — sezione Titolarità](#1-titoli-abilitativi-edilizi--sezione-titolarità)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Oggetto dell'agibilità](#3-oggetto-dellagibilità)
4. [Documentazione — sicurezza statica (chkd_3)](#4-documentazione--sicurezza-statica-chkd_3)
5. [Documentazione — urbanizzazione primaria (chkd_4)](#5-documentazione--urbanizzazione-primaria-chkd_4)
6. [Documentazione — precedente abitabilità/agibilità (chkd_5)](#6-documentazione--precedente-abitabilitàagibilità-chkd_5)
7. [Documentazione — barriere architettoniche (chkd_6)](#7-documentazione--barriere-architettoniche-chkd_6)
8. [Documentazione — prevenzione incendi (chkd_8)](#8-documentazione--prevenzione-incendi-chkd_8)
9. [Documentazione — sicurezza impianti (chkd_12)](#9-documentazione--sicurezza-impianti-chkd_12)

---

## 1. Titoli abilitativi edilizi — sezione Titolarità

La sezione "Titolarità" contiene 4 checkbox principali per i titoli edilizi (PdC, DIA, SCIA, CILA), ciascuna con una sotto-checkbox per la variante in corso d'opera. Ogni checkbox spuntata attiva i campi numero e data obbligatori con verifica del formato.

{: .note }
> Come nella [CAGI Piemonte](errori-comunicazione-agibilita-piemonte.html#1-titoli-abilitativi-edilizi--sezione-titolarità), nessuna delle 8 checkbox ha un obbligo minimo — è tecnicamente possibile inviare la richiesta senza spuntare alcun titolo. Il validatore verifica solo che, **se** si spunta una checkbox, i relativi campi siano compilati correttamente nel formato GG/MM/AAAA.

---

### ATTENZIONE ! Inserire il numero. (PdC / PdCVar / DIA / DIAVar / SCIA / SCIAVar / CILA / CILAVar)

**Causa**: Una checkbox titolo è spuntata ma il campo numero (`txtNPdC`, `txtNDIA`, `txtNSCIA`, `txtNCILA` o la variante corrispondente) è vuoto.

**Soluzione**: Inserisci il numero della pratica edilizia nel campo "n." della riga corrispondente.

---

### ATTENZIONE ! Inserire la data. (per qualsiasi titolo o variante)

**Causa**: La checkbox è spuntata e il numero è compilato, ma il campo data è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (per qualsiasi titolo o variante)

**Causa**: Il campo data non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

{: .note }
> I messaggi "Inserire il numero", "Inserire la data" e "Inserire la data nel formato gg/mm/aaaa" sono identici per tutti e 8 i titoli/varianti. Se compare uno di questi errori, verificare sistematicamente tutte le checkbox spuntate. Il campo `txtVariantiCorsoOpera` (campo libero multiriga per ulteriori varianti) non viene validato.

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

## 3. Oggetto dell'agibilità

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Oggetto'.

**Dove si trova**: Sezione "RICHIEDE — Oggetto" → 5 radio button `$OggAgibilita`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei cinque radio button**:
- ⚪ **3_1** — "per tutta la costruzione"
- ⚪ **3_2** — "per singole porzioni della costruzione (indicare quali)" → inserisci le porzioni nel campo `txtOggAgibilita3_2_1`
- ⚪ **3_3** — "per singole unità immobiliari (indicare gli estremi catastali)" → inserisci gli estremi catastali nel campo `txtOggAgibilita3_3_1`
- ⚪ **3_4** — "tutti gli edifici"
- ⚪ **3_5** — "per i soli edifici (indicare quali)" → inserisci la specifica nel campo `txtOggAgibilita3_5_1`

---

### ATTENZIONE ! Inserire le singole porzioni della costruzione.

**Causa**: Hai selezionato 3_2 ma `txtOggAgibilita3_2_1` è vuoto.

**Soluzione**: Inserisci le porzioni della costruzione oggetto della richiesta (es. "piano terra, piano primo").

---

### ATTENZIONE ! Inserire le singole unità immobiliari.

**Causa**: Hai selezionato 3_3 ma `txtOggAgibilita3_3_1` è vuoto.

**Soluzione**: Inserisci gli estremi catastali delle singole unità immobiliari.

---

### ATTENZIONE ! Inserire i soli edifici.

**Causa**: Hai selezionato 3_5 ma `txtOggAgibilita3_5_1` è vuoto.

**Soluzione**: Inserisci la specificazione degli edifici.

---

## 4. Documentazione — sicurezza statica (chkd_3)

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'sicurezza statica'.

**Dove si trova**: Sezione "DICHIARA" → punto 3 "per la sicurezza statica" → 2 checkbox sotto-opzioni

**Causa**: `chkd_3` è spuntata ma `chkd_3_1` non è spuntata.

**Soluzione**: Spunta **almeno** la checkbox `chkd_3_1`:
- ☐ **chkd_3_1** — "certificato di collaudo statico (art. 25 comma 3 lett. a) del D.P.R. 380/2011 e ss.mm.ii.)"
- ☐ **chkd_3_2** — "relazione di verifica statica qualora non sia stata presentata la relativa denuncia strutturale"

{: .warning }
> **Bug nel codice**: il validatore verifica `chkd_3_1 = False AND chkd_3_1 = False` — la stessa checkbox due volte invece di `chkd_3_1 = False AND chkd_3_2 = False`. In pratica: se si spunta `chkd_3` senza spuntare `chkd_3_1`, compare l'errore; se si spunta `chkd_3_1` (indipendentemente da `chkd_3_2`), l'errore non compare. La checkbox `chkd_3_2` non viene mai verificata dal codice — può essere lasciata senza problemi ma non viene controllata. Per evitare l'errore è sufficiente spuntare `chkd_3_1`.

---

## 5. Documentazione — urbanizzazione primaria (chkd_4)

### ATTENZIONE ! Non è stata selezionata nessuna voce per le 'opere di urbanizzazione primaria'.

**Dove si trova**: Sezione "DICHIARA" → punto 4 "per le opere di urbanizzazione primaria" → 2 radio button `$UrbPrimaria`

**Causa**: `chkd_4` è spuntata ma nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbUrbPrimariad_4_1** — "per tutta la costruzione"
- ⚪ **rdbUrbPrimariad_4_2** — "dichiarazione del direttore dei lavori di funzionalità delle opere di urbanizzazione primaria rispetto all'edificio oggetto di agibilità parziale"

---

## 6. Documentazione — precedente abitabilità/agibilità (chkd_5)

### ATTENZIONE ! Inserire numero pratica.

**Dove si trova**: Sezione "DICHIARA" → punto 5 "di precedente certificato di Abitabilità/Agibilità" → campo `txtNPraticad_5` "Pratica n."

**Causa**: `chkd_5` è spuntata ma il campo numero pratica è vuoto.

**Soluzione**: Inserisci il numero della pratica del precedente certificato di abitabilità o agibilità.

---

### ATTENZIONE ! Inserire data pratica.

**Causa**: `chkd_5` è spuntata e il numero è compilato, ma `txtDataPraticad_5` è vuoto.

**Soluzione**: Inserisci la data di rilascio del precedente certificato.

{: .note }
> A differenza dei campi data della sezione Titolarità (che vengono verificati nel formato GG/MM/AAAA), la data del punto 5 (`txtDataPraticad_5`) **non viene verificata nel formato** — il validatore controlla solo che il campo non sia vuoto. Il radio group `$CertAbiAgi` (per/tutta la costruzione/DL funzionalità) è commentato nel codice e non appare nel modulo.

---

## 7. Documentazione — barriere architettoniche (chkd_6)

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'dichiarazione di conformità'.

**Dove si trova**: Sezione "DICHIARA" → punto 6 "dichiarazione di conformità delle opere realizzate alla normativa vigente in materia di accessibilità e superamento delle barriere architettoniche" → 2 radio button `$DichConf`

**Causa**: `chkd_6` è spuntata ma nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbDichConfd6_1** — "per edifici privati su autocertificazione"
- ⚪ **rdbDichConfd6_2** — "per edifici pubblici o privati aperti al pubblico, sotto forma di perizia giurata redatta da un tecnico abilitato, attestante il rispetto delle prescrizioni di cui all'art. 82 comma 1 del D.P.R. 380/2001 e ss.mm.ii."

---

## 8. Documentazione — prevenzione incendi (chkd_8)

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'prevenzione incendi'.

**Dove si trova**: Sezione "DICHIARA" → punto 8 "per la prevenzione incendi" → 2 radio button `$PrevIncendi`

**Causa**: `chkd_8` è spuntata ma nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbPrevIncendid_8_1** — "copia della ricevuta di presentazione della SCIA dal Comando Provinciale Vigili del Fuoco per le attività di cui all'allegato I del D.P.R. 151/2011"
- ⚪ **rdbPrevIncendid_8_2** — "autocertificazione attestante che nell'area/immobile non vi sono attività soggette a controllo di prevenzione incendi ai sensi del D.P.R. 151/2011"

---

## 9. Documentazione — sicurezza impianti (chkd_12)

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'sicurezza impianti'.

**Dove si trova**: Sezione "DICHIARA" → punto 12 "per la sicurezza impianti" → 23 checkbox sotto-opzioni (chkd_12_1..23)

**Causa**: `chkd_12` è spuntata ma nessuna delle 23 checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 23 checkbox. La struttura è a 3 gruppi:

**Gruppo 1 — chkd_12_1** (parti comuni): "dichiarazioni di conformità dei seguenti impianti realizzati o modificati nelle **parti comuni** e attestazione di collaudo ove previsto" + sotto-tipologie chkd_12_2..8: impianti elettrici/protezione scariche/automazione porte; impianti radiotelevisivi ed elettronici; impianti riscaldamento/climatizzazione/condizionamento/refrigerazione; impianti idrici e sanitari; impianti distribuzione/utilizzazione gas; impianti sollevamento (ascensori/montacarichi/scale mobili); impianti protezione antincendio.

**Gruppo 2 — chkd_12_9** (singole U.I.): "dichiarazioni di conformità dei seguenti impianti [...] nelle **singole unità immobiliari** e attestazione di collaudo ove previsto" + sotto-tipologie chkd_12_10..16 (stesse 7 tipologie del gruppo 1).

**Gruppo 3 — chkd_12_17** (rispondenza ante D.M. 37/2008): "dichiarazione di rispondenza, per gli impianti eseguiti **prima dell'entrata in vigore del D.M. 37/2008**" + sotto-tipologie chkd_12_18..23 (6 tipologie — manca "protezione antincendio" rispetto ai gruppi 1 e 2).

{: .warning }
> Nel modulo è presente anche `chkd_12_24` ("impianti di protezione antincendio" nel gruppo 3 — rispondenza ante D.M. 37/2008) ma il codice di validazione verifica solo fino a `chkd_12_23`. La checkbox `chkd_12_24` non viene mai conteggiata nel controllo "almeno una"; se si spunta solo `chkd_12_24` senza spuntarne nessuna altra, l'errore comparirà comunque.

---

## Consigli pratici — Richiesta Agibilità Piemonte

### Prima di validare ✅

- [ ] Per ogni checkbox titolo spuntata (PdC, DIA, SCIA, CILA + varianti): inserisci **numero** e **data** (GG/MM/AAAA)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona l'**oggetto dell'agibilità** (3_1..3_5); se 3_2/3_3/3_5: inserisci la specificazione
- [ ] Se `chkd_3` spuntata: spunta almeno **chkd_3_1** (collaudo statico)
- [ ] Se `chkd_4` spuntata: seleziona il **radio urbanizzazione primaria** (4_1/4_2)
- [ ] Se `chkd_5` spuntata: inserisci **numero pratica** e **data** del precedente certificato
- [ ] Se `chkd_6` spuntata: seleziona il **radio dichiarazione conformità** (6_1/6_2)
- [ ] Se `chkd_8` spuntata: seleziona il **radio prevenzione incendi** (8_1/8_2)
- [ ] Se `chkd_12` spuntata: spunta almeno una delle **23 checkbox** impianti (non usare solo chkd_12_24)

### Documentazione non validata ℹ️

I seguenti punti sono presenti nel modulo ma non vengono validati: chkd_2 (denuncia catastale), chkd_7 (APE), chkd_9 (fognario/scarico), chkd_10 (acustica), chkd_11 (risparmio energetico), chkd_12_24 (protezione antincendio nel gruppo rispondenza), `txtVariantiCorsoOpera`, privacy (solo testo).

### Differenze rispetto alla CAGI Piemonte ℹ️

La Richiesta di Agibilità usa "RICHIEDE" + "DICHIARA" invece di "TRASMETTE". La sezione sicurezza impianti ha 23 checkbox flat invece delle 3 "parent" della CAGI (ciascuna con 7 sotto-checkbox). Il punto 3 (sicurezza statica) ha un bug nel codice che ignora `chkd_3_2`.

### Bug noti ⚠️

**Sicurezza statica (chkd_3)**: il codice verifica `chkd_3_1 = False AND chkd_3_1 = False` invece di `chkd_3_1 = False AND chkd_3_2 = False`. Conseguenza pratica: spuntare `chkd_3_1` risolve sempre l'errore; `chkd_3_2` non viene mai verificata.

**Sicurezza impianti (chkd_12)**: `chkd_12_24` è presente nel modulo ma non inclusa nel controllo "almeno una" (il loop arriva solo a chkd_12_23).

### Errori frequenti 🔍

1. **Data titoli nel formato errato** → GG/MM/AAAA; le date dei titoli abilitativi vengono verificate nel formato a differenza della data del punto 5 (abitabilità precedente)
2. **chkd_3 senza chkd_3_1** → spuntare chkd_3 richiede necessariamente chkd_3_1; chkd_3_2 da sola non basta a causa del bug
3. **chkd_12 con solo chkd_12_24** → la checkbox 24 non è contata dal validatore; usare una delle 23 verificate
4. **Oggetto agibilità senza testo** → le opzioni 3_2, 3_3 e 3_5 richiedono specificazione obbligatoria

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Vedi anche [CAGI Piemonte](errori-comunicazione-agibilita-piemonte.html) — struttura analoga
3. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiAgibilita e DatiAgibilita.ascx
