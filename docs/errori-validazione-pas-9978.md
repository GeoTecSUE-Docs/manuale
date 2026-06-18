---
title: Errori Procedura Abilitativa Semplificata (P.A.S.) - Tutte le regioni
parent: Errori di validazione
nav_order: 70
description: Errori di validazione per la Procedura Abilitativa Semplificata (PAS) per impianti da fonti rinnovabili - Tutte le regioni (D.Lgs. 190/2024, D.Lgs. 387/2003, art. 12)
keywords: [PAS, procedura abilitativa semplificata, fonti rinnovabili, impianti fotovoltaici, D.Lgs. 190/2024, D.Lgs. 387/2003, Allegato B, nuova costruzione, impianti esistenti, completamento, variante, regolarità urbanistica, data luogo]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 2, Prat: 78 }  # Piemonte - P.A.S.
  - { Reg: 1, Prat: 178 }  # Valle d'Aosta - P.A.S.
  - { Reg: 3, Prat: 378 } # Liguria - P.A.S.
  - { Reg: 4, Prat: 478 } # Lombardia - P.A.S.
  - { Reg: 6, Prat: 678 } # Veneto - P.A.S.
  - { Reg: 8, Prat: 878 } # Emilia-Romagna - P.A.S.
  - { Reg: 12, Prat: 1278 } # Lazio - P.A.S.
  - { Reg: 13, Prat: 1378 } # Abruzzo - P.A.S.
  - { Reg: 15, Prat: 1578 } # Campania - P.A.S.
  - { Reg: 16, Prat: 1678 } # Basilicata - P.A.S.
  - { Reg: 17, Prat: 1778 } # Puglia - P.A.S.
  - { Reg: 18, Prat: 1878 } # Calabria - P.A.S.
  - { Reg: 19, Prat: 1978 } # Sicilia - P.A.S.
Fonte: Manuale
---

# Errori di validazione - Procedura Abilitativa Semplificata (P.A.S.)
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per la **Procedura Abilitativa Semplificata (PAS)** per la costruzione, esercizio e modifica di impianti da fonti rinnovabili — Tutte le regioni, ai sensi dell'art. 12 del D.Lgs. 29 dicembre 2003, n. 387 e del D.Lgs. 8 novembre 2024, n. 190 (artt. 1 e 8, Allegato B).

{: .note }
> La PAS è una pratica specifica per impianti di produzione di energia da fonti rinnovabili e ha una struttura originale rispetto alle pratiche edilizie ordinarie. Presenta caratteristiche uniche nel sistema: la sezione "Qualificazione dell'intervento" è basata sul D.Lgs. 190/2024 Allegato B (la versione precedente con 8 tipologie è commentata nel codice), la sezione "Regolarità urbanistica" ha 3 opzioni con fino a 17 checkbox e verifica rigorosa di numero, data e formato per le checkbox 1-14, e la sezione finale richiede obbligatoriamente **data e luogo** con verifica del formato — unica pratica del sistema con entrambi i campi data/luogo obbligatori. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Presentazione della PAS](#2-presentazione-della-pas)
3. [Qualificazione dell'intervento — Territorio](#3-qualificazione-dellintervento--territorio)
4. [Qualificazione dell'intervento — Tipo di intervento](#4-qualificazione-dellintervento--tipo-di-intervento)
5. [Descrizione dell'intervento](#5-descrizione-dellintervento)
6. [Localizzazione dell'intervento](#6-localizzazione-dellintervento)
7. [Opere su parti comuni o modifiche esterne](#7-opere-su-parti-comuni-o-modifiche-esterne)
8. [Regolarità urbanistica e precedenti edilizi](#8-regolarità-urbanistica-e-precedenti-edilizi)
9. [Comunicazioni contestuali (sezione 3)](#9-comunicazioni-contestuali-sezione-3)
10. [Atti di assenso da acquisire (sezione 4)](#10-atti-di-assenso-da-acquisire-sezione-4)
11. [Tecnici incaricati](#11-tecnici-incaricati)
12. [Impresa esecutrice dei lavori](#12-impresa-esecutrice-dei-lavori)
13. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#13-sicurezza-sul-lavoro-dlgs-812008)
14. [Data e Luogo](#14-data-e-luogo)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Inserire la Titolarità dell'intervento.

**Causa**: Il menu `cmbTitoloSuImm` ha il valore "altron" selezionato ma il campo `txtSpecifTitolarita1` "Specificare se altro" è vuoto.

**Soluzione**: Inserisci la specificazione della titolarità nel campo "Specificare se altro".

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

---

## 2. Presentazione della PAS

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della PAS/PAS Unica/PAS Condizionata'.

**Dove si trova**: Sezione "Presentazione della PAS/PAS Unica/PAS Condizionata" → 3 radio button `$Presentazione`

**Causa**: Nessuno dei 3 radio button è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **v_1** — "**PAS in assenza di atti di assenso presupposti**, altre segnalazioni o comunicazioni" → termine inizio attività sospeso 30 giorni (art. 8 c. 6 D.Lgs. 190/2024)
- ⚪ **v_2** — "**PAS completa di tutti gli atti di assenso presupposti**" → il titolare ha già acquisito tutte le dichiarazioni/segnalazioni; termine sospeso 30 giorni (art. 8 c. 6 D.Lgs. 190/2024)
- ⚪ **v_3** — "**PAS più domanda per il rilascio di atti di assenso (PAS Condizionata)**" → seleziona almeno una delle 3 checkbox

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'PAS più domanda per il rilascio di atti di assenso'.

**Causa**: Hai selezionato v_3 (PAS Condizionata) ma nessuna delle 3 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 3 opzioni:
- ☐ **chkAcqAttAss** — "L'acquisizione degli atti di assenso di competenza comunale" (termine 45 giorni, art. 8 c. 7 D.Lgs. 190/2024)
- ☐ **chkAcqDiversi** — "L'acquisizione degli atti di assenso di competenza di altre amministrazioni" (termine 60 giorni, art. 8 c. 8 lett. c D.Lgs. 190/2024)
- ☐ **chkAttProc** — "L'attivazione del procedimento per espropriazione (DPR 327/2001)" (termine sospeso fino a conclusione procedimento)

---

## 3. Qualificazione dell'intervento — Territorio

### ATTENZIONE ! Non è stata selezionata nessuna voce per il territorio di 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → 2 radio button `$Territorio`

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **t_1** — "del solo comune"
- ⚪ **t_2** — "di più comuni" (il Comune procedente è quello con la maggior porzione di impianto)

---

## 4. Qualificazione dell'intervento — Tipo di intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → 4 radio button `$TipoIntervento`

**Causa**: Nessuno dei 4 radio button è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button** ai sensi del D.Lgs. 190/2024 Allegato B:
- ⚪ **e_1** — "interventi di nuova costruzione indicati alla Sezione I - Allegato B del D.Lgs. 190/2024 di cui all'art. 1 comma ___" → inserisci la lettera del comma nel campo `txtNCComma`
- ⚪ **e_2** — "interventi su impianti esistenti indicati alla Sezione II - Allegato B del D.Lgs. 190/2024 di cui all'art. 1 comma ___" → inserisci la lettera del comma nel campo `txtIEComma`
- ⚪ **e_3** — "interventi di completamento di intervento non ultimato autorizzato con PAS n. ___ del ___" → inserisci numero e data del titolo precedente
- ⚪ **e_4** — "variante in corso d'opera il cui intervento risulta autorizzato con PAS n. ___ del ___" → inserisci numero e data del titolo precedente

{: .note }
> La sezione "Qualificazione dell'intervento" nella PAS è stata aggiornata con il D.Lgs. 190/2024. La versione precedente con 8 tipologie specifiche (impianti fotovoltaici, flottanti, agrivoltaici, ecc.) è commentata nel codice ma non più attiva nel modulo. La versione attiva richiede di specificare la lettera del comma dell'Allegato B del D.Lgs. 190/2024.

---

### ATTENZIONE ! Inserire il numero del comma. (e_1 — nuova costruzione)

**Causa**: Hai selezionato e_1 ma `txtNCComma` è vuoto.

**Soluzione**: Inserisci la lettera del comma dell'art. 1 della Sezione I dell'Allegato B del D.Lgs. 190/2024 applicabile alla tipologia di intervento di nuova costruzione.

---

### ATTENZIONE ! Inserire il numero del comma. (e_2 — impianti esistenti)

**Causa**: Hai selezionato e_2 ma `txtIEComma` è vuoto.

**Soluzione**: Inserisci la lettera del comma dell'art. 1 della Sezione II dell'Allegato B del D.Lgs. 190/2024 applicabile alla tipologia di intervento su impianto esistente.

---

### ATTENZIONE ! Inserire il numero del titolo precedente. (e_3 — completamento)

**Causa**: Hai selezionato e_3 ma `txtCINumero` è vuoto.

**Soluzione**: Inserisci il numero della PAS originaria con cui era stato autorizzato l'intervento non ultimato.

---

### ATTENZIONE ! Inserire la data del titolo precedente. (e_3 — completamento)

**Causa**: Il campo `txtCIData` è vuoto.

**Soluzione**: Inserisci la data della PAS originaria nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (e_3)

**Causa**: La data del completamento non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire il numero del titolo precedente. (e_4 — variante)

**Causa**: Hai selezionato e_4 ma `txtVCNumero` è vuoto.

**Soluzione**: Inserisci il numero della PAS originaria a cui si riferisce la variante in corso d'opera.

---

### ATTENZIONE ! Inserire la data del titolo precedente. (e_4 — variante)

**Causa**: Il campo `txtVCData` è vuoto.

**Soluzione**: Inserisci la data della PAS originaria nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (e_4)

**Causa**: La data della variante non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 5. Descrizione dell'intervento

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → campo multiriga `txtDescrIntervento` "Descrizione sintetica dell'intervento" (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione sintetica dell'impianto (max **300 caratteri**).

{: .note }
> Nell'ordine di validazione, la descrizione viene verificata **dopo** la qualificazione (territorio + tipo intervento) e **prima** della localizzazione — ordine insolito rispetto alla maggior parte delle pratiche del sistema.

---

## 6. Localizzazione dell'intervento

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

## 7. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per le opere su parti comuni.

**Causa**: Nessuno dei 4 radio button `$OpereComuni` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **d_1** — "non riguardano parti comuni"
- ⚪ **d_2** — "riguardano le parti comuni di un fabbricato condominiale" (richiede delibera assembleare)
- ⚪ **d_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ⚪ **d_4** — "riguardano parti comuni ma non necessitano di assenso (art. 1102 c.c.)"

---

## 8. Regolarità urbanistica e precedenti edilizi

La sezione "Regolarità urbanistica" della PAS è tra le più complesse del sistema. Ha 3 opzioni principali (f_1/f_2/f_3) con sotto-selezioni estese — fino a 16 checkbox (f_2) o 17 checkbox (f_3) di titoli edilizi, ciascuna con numero e data da verificare nel formato.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Causa**: Nessun radio button `$StatoAttualeImm` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **f_1** — "che le opere riguardano un intervento di nuova costruzione su area libera" → nessun campo aggiuntivo
- ⚪ **f_2** — "pienamente conforme alla documentazione dello stato di fatto legittimato dal seguente titolo/pratica edilizia" → spunta almeno una delle 16 checkbox con n. e data
- ⚪ **f_3** — "in difformità rispetto alla documentazione [...] tali opere sono state realizzate in data ___" → inserisci la data delle difformità e spunta almeno una delle 17 checkbox

---

### Opzione f_2 — Pienamente conforme (16 checkbox)

#### ATTENZIONE ! Indicare almeno una tipologia di pratica. (f_2)

**Causa**: Hai selezionato f_2 ma nessuna delle 16 checkbox (chkStatoAttualeImm2_1..16) è spuntata.

**Soluzione**: Spunta **almeno una** delle 16 checkbox del titolo/pratica edilizia che legittima lo stato attuale. Le prime 14 hanno numero e data obbligatori con verifica formato; le ultime 2 hanno logiche speciali:

Checkbox 1-14 (con numero e data obbligatori): titolo unico (SUAP); permesso di costruire/licenza edil./concessione edilizia; autorizzazione edilizia; comunicazione edilizia (art. 26 L. 47/1985); condono edilizio; denuncia di inizio attività; DIA/SCIA alternativa al permesso di costruire; segnalazione certificata di inizio attività; dichiarazione di inizio lavori asseverata (DILA); procedura abilitativa semplificata (PAS); autorizzazione ex art. 12 D.Lgs. 387/2003; comunicazione ex art. 11 c. 3 D.Lgs. 115/2008; comunicazione edilizia libera; **altro** (chkStatoAttualeImm2_14 → richiede anche `txtAltro2_14` descrizione tipologia).

Checkbox 15 — **informazioni catastali di primo impianto**: non richiede numero e data.

Checkbox 16 — **altri documenti probanti**: richiede almeno una sotto-checkbox (chkDocProbanti2_1..4).

---

#### ATTENZIONE ! Inserire il numero della pratica. (f_2, checkbox 1-14)

**Causa**: Una checkbox chkStatoAttualeImm2_N (1≤N≤14) è spuntata ma `txtNProt2_N` è vuoto.

**Soluzione**: Inserisci il numero del titolo/pratica per la riga corrispondente.

---

#### ATTENZIONE ! Inserire la data della pratica. (f_2, checkbox 1-14)

**Causa**: Il campo data (`txtDataProt2_N`) è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (f_2)

**Causa**: La data non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la tipologia della pratica. (f_2, checkbox 14 — altro)

**Causa**: `chkStatoAttualeImm2_14` ("altro") è spuntata ma `txtAltro2_14` è vuoto.

**Soluzione**: Inserisci la descrizione del tipo di titolo nel campo testuale della checkbox "altro" prima dei campi numero e data.

---

#### ATTENZIONE ! Indicare almeno una tipologia di documento probante. (f_2, checkbox 16)

**Causa**: `chkStatoAttualeImm2_16` ("altri documenti probanti") è spuntata ma nessuna delle 4 sotto-checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 4 sotto-opzioni: riprese fotografiche; estratti cartografici; documenti d'archivio; altro atto pubblico o privato di cui sia dimostrata la provenienza.

---

### Opzione f_3 — In difformità (17 checkbox)

#### ATTENZIONE ! Inserire la data della pratica. (f_3 — data difformità)

**Dove si trova**: Campo `txtDataDiff3_18` — la data in cui sono state realizzate le opere in difformità, nella riga del radio f_3

**Causa**: Hai selezionato f_3 ma il campo data delle difformità è vuoto. Questo è il **primo** controllo di f_3 — verificato prima dell'obbligo di checkbox.

**Soluzione**: Inserisci la data di realizzazione delle difformità nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (f_3 — data difformità)

**Causa**: La data delle difformità non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Indicare almeno una tipologia di pratica. (f_3)

**Causa**: La data difformità è inserita ma nessuna delle 17 checkbox (chkStatoAttualeImm3_1..17) è spuntata.

**Soluzione**: Spunta **almeno una** delle 17 checkbox. Le prime 14 hanno numero e data obbligatori (stesse tipologie di f_2); la 15 = informazioni catastali; la 16 = altri documenti probanti (con sotto-checkbox); la 17 = "le difformità non costituiscono violazioni edilizie in quanto rientrano nelle tolleranze esecutive (art. 34-bis, comma 4 art. 34-ter D.P.R. 380/2001)".

{: .note }
> Il loop di validazione dei titoli edilizi per f_3 scorre le checkbox da 1 a 14, verificando numero + data con formato. Le checkbox 15, 16 e 17 non richiedono numero e data. La checkbox 16 richiede almeno uno dei 4 documenti probanti (chkDocProbanti3_1..4). La checkbox 17 (tolleranze esecutive) non ha campi aggiuntivi.

---

## 9. Comunicazioni contestuali (sezione 3)

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito. (sezione 3)

**Dove si trova**: Sezione "Altre comunicazioni, segnalazioni, asseverazioni etc." → 5 righe (chkPres3_1..5)

**Causa**: Una delle 5 checkbox è spuntata ma `txtTipologiaAtto3_N` è vuoto.

**Soluzione**: Inserisci la tipologia della comunicazione/segnalazione nel campo "Comunicazioni, segnalazioni, etc." della riga corrispondente.

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito. (sezione 3)

**Causa**: `chkPres3_N` è spuntata e il tipo è compilato, ma `txtAutComp3_N` è vuoto.

**Soluzione**: Inserisci l'autorità competente nel campo corrispondente.

---

## 10. Atti di assenso da acquisire (sezione 4)

### ATTENZIONE ! Campo obbligatorio 'Tipologia di atto' non inserito. (sezione 4)

**Dove si trova**: Sezione "Atti di assenso da acquisire" → 5 righe (chkPres4_1..5)

**Causa**: Una delle 5 checkbox è spuntata ma `txtPres4_N` ("Tipologia di atto") è vuoto.

**Soluzione**: Inserisci la tipologia dell'atto di assenso da acquisire.

---

### ATTENZIONE ! Campo obbligatorio 'Autorità competente' non inserito. (sezione 4)

**Causa**: `chkPres4_N` è spuntata e la tipologia è compilata, ma `txtAutComp4_N` ("Autorità competente al rilascio") è vuoto.

**Soluzione**: Inserisci l'autorità competente al rilascio dell'atto.

---

## 11. Tecnici incaricati

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Causa**: Nessuno dei 2 radio button `$Tecnici` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **h_1** — "di aver incaricato, in qualità di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'SOGGETTI COINVOLTI'"
- ⚪ **h_2** — "che il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"

---

## 12. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **i_1** — "che i lavori sono eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'SOGGETTI COINVOLTI'"
- ⚪ **i_2** — "che l'impresa esecutrice dei lavori sarà individuata prima dell'inizio dei lavori"
- ⚪ **i_3** — "che la presente PAS è di modifica alla PAS n. ___ del ___" → inserisci numero e data della PAS originaria

---

### ATTENZIONE ! Inserire il numero della Pratica. (i_3 — modifica PAS)

**Causa**: Hai selezionato i_3 ma `txtNProtImp` è vuoto.

**Soluzione**: Inserisci il numero della PAS originaria che si intende modificare.

---

### ATTENZIONE ! Inserire la data della Pratica. (i_3 — modifica PAS)

**Causa**: Il campo `txtDataProtImp` è vuoto.

**Soluzione**: Inserisci la data della PAS originaria nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data PAS modifica)

**Causa**: La data della PAS originaria non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 13. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessuno dei 4 radio button `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **l_1** — "non ricade nell'ambito di applicazione [...] (d.lgs. n. 81/2008)"
- ⚪ **l_2** — "ricade [...] e pertanto" → seleziona documentazione imprese e notifica
- ⚪ **l_3** — "ricade [...] ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"
- ⚪ **l_4** — "ricade [...] ma la presente pratica è in variante e non sono previste modifiche" *(opzione specifica PAS — assente nelle altre pratiche)*

{: .note }
> La PAS ha **4 livelli** di radio per la sicurezza invece dei 3 tipici di SCIA/PdC, con l'aggiunta dell'opzione l_4 per le varianti senza modifiche alle dichiarazioni di sicurezza già prodotte.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato l_2 ma nessuno dei 2 radio button `$ImpEs` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **l_2_1** — "entità presunta del cantiere inferiore a 200 uomini-giorno e lavori senza rischi particolari (Allegato XI)"
- ⚪ **l_2_2** — "entità presunta del cantiere pari o superiore a 200 uomini-giorno o con rischi particolari"

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato l_2 (con qualsiasi ImpEs) ma nessuno dei 2 radio button `$Notifica` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **l_2_2_1** — "l'intervento non è soggetto all'invio della notifica"
- ⚪ **l_2_2_2** — "l'intervento è soggetto all'invio della notifica e" → la checkbox `chkAllegal1_1_4_1` (allega notifica) è presente nel modulo ma **non validata**

{: .note }
> A differenza di SCIA/PdC, nella PAS la notifica è richiesta per **qualsiasi** scelta di ImpEs (l_2_1 o l_2_2), non solo per l_2_2. Il validatore verifica `$Notifica` dopo aver verificato `$ImpEs`, indipendentemente dal radio ImpEs scelto.

---

## 14. Data e Luogo

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Sezione finale del modulo (sotto il blocco "Attenzione: qualora dai controlli...") → campo `txtData`

**Causa**: Il campo data è vuoto.

**Soluzione**: Inserisci la data di presentazione nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data finale)

**Causa**: La data finale non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Campo `txtLuogo` accanto al campo data

**Causa**: Il campo "luogo" è vuoto.

**Soluzione**: Inserisci il Comune o luogo dove viene firmata la dichiarazione.

{: .warning }
> La PAS è l'**unica pratica del sistema** in cui sia `txtData` (con verifica formato) sia `txtLuogo` sono obbligatori nel modulo principale. In quasi tutte le altre pratiche questi campi sono presenti ma non validati. Non dimenticarli — sono gli ultimi due controlli prima della validazione finale.

---

## Consigli pratici — PAS Nazionale

### Prima di validare ✅

- [ ] Se titolarità "altro": inserisci **specificazione** nel campo testo
- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona la **presentazione PAS** (v_1/v_2/v_3); se v_3: almeno una delle 3 checkbox (chkAcqAttAss/chkAcqDiversi/chkAttProc)
- [ ] Seleziona il **territorio** (t_1/t_2)
- [ ] Seleziona il **tipo di intervento** (e_1..e_4) con i campi richiesti (lettera comma o n.+data PAS precedente in GG/MM/AAAA)
- [ ] Inserisci la **descrizione** dell'impianto (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**; aggiungi **mappale** e **destinazione d'uso**
- [ ] Seleziona le **opere su parti comuni** (d_1..d_4)
- [ ] Seleziona lo **stato attuale** (f_1/f_2/f_3); se f_2: almeno una checkbox 1-16 con n.+data GG/MM/AAAA; se f_3: data difformità GG/MM/AAAA + almeno una checkbox 1-17
- [ ] Se sezione 3 spuntata: inserisci **tipologia** e **autorità competente** per ogni riga
- [ ] Se sezione 4 spuntata: inserisci **tipologia atto** e **autorità competente al rilascio** per ogni riga
- [ ] Seleziona il **radio tecnici** (h_1/h_2)
- [ ] Seleziona il **radio impresa** (i_1/i_2/i_3); se i_3: n. e data PAS originaria in GG/MM/AAAA
- [ ] Seleziona la **sicurezza** (l_1..l_4); se l_2: ImpEs + Notifica
- [ ] Inserisci **data** (GG/MM/AAAA) e **luogo**

### Ordine di validazione ⚠️

Titolarità → Presentazione PAS → Territorio → Tipo intervento → Descrizione → Localizzazione → Opere comuni → Regolarità urbanistica → Sezione 3 → Sezione 4 → Tecnici → Impresa → Sicurezza → Data → Luogo

### Campi e sezioni non validati ℹ️

La sezione "Misure per la prevenzione delle cadute dall'alto" è completamente commentata nel codice e non appare nel modulo. `chkAllegal1_1_4_1` (allega notifica) non validata. `txtNote` facoltativo. Privacy solo testo informativo.

### Errori frequenti 🔍

1. **Data e Luogo dimenticati** → ultimi controlli della validazione; appaiono solo se tutto il resto è corretto; inserirli prima di validare
2. **Data difformità f_3 vuota** → primo controllo di f_3, prima ancora delle checkbox; la data deve essere in GG/MM/AAAA
3. **Checkbox 14 "altro" senza tipologia** → richiede 3 campi: tipo (`txtAltro2_14` o `txtAltro3_14`), numero e data
4. **Checkbox 16 senza documenti probanti** → obbligatoria almeno una delle 4 sotto-checkbox (riprese fotografiche/estratti cartografici/documenti archivio/altro)
5. **Notifica sicurezza** → nella PAS viene verificata per qualsiasi scelta ImpEs; non solo per l_2_2

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
**Fonte**: Analisi codice ValidaDatiPAS e DatiPAS.ascx
