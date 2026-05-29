---
title: Errori SCIA Alternativa al Permesso di Costruire - Regione Lombardia
parent: Errori di validazione
nav_order: 45
description: Errori di validazione specifici per la SCIA Alternativa al Permesso di Costruire - Regione Lombardia (art. 23 D.P.R. 380/2001, L.R. 12/2005)
keywords: [SCIA alternativa PdC, SCIA alternativa permesso di costruire, Lombardia, art. 23 DPR 380, qualificazione intervento, regolarità urbanistica, opere comuni, coordinate UTM, contributo di costruzione, Ge.CA, D.Lgs. 81/2008, sicurezza]
IDRegione: 4
IDTipoPratica: 426
Fonte: Manuale
---

# Errori di validazione - SCIA Alternativa al Permesso di Costruire
## Regione Lombardia

Guida completa agli errori specifici per la **SCIA Alternativa al Permesso di Costruire** ai sensi dell'art. 23 del D.P.R. 380/2001 — Regione Lombardia. Comprende le varianti SCIA Unica (con altre segnalazioni) e SCIA Condizionata (con istanze per atti di assenso).

{: .note }
> La SCIA alt. PdC Lombardia è una delle pratiche più complesse del sistema. Ha 11 sezioni da compilare, di cui la più articolata è la **Regolarità urbanistica** con 6 opzioni principali e una struttura di checkbox a 3 livelli (13 titoli ordinari + 4 sanatorie + 4 "altro" con 3 campi ciascuna). La sezione **sicurezza** ha 3 opzioni invece delle usuali 2, con la terza ("riserva presentazione dichiarazioni") che non richiede sotto-selezioni. Le ultime 3 checkbox (**conoscenza efficacia**, **diritti terzi**, **privacy**) sono tutte obbligatorie e il sistema le verifica in sequenza. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Presentazione della segnalazione](#2-presentazione-della-segnalazione)
3. [Qualificazione dell'intervento](#3-qualificazione-dellintervento)
4. [Localizzazione dell'intervento](#4-localizzazione-dellintervento)
5. [Opere su parti comuni o modifiche esterne](#5-opere-su-parti-comuni-o-modifiche-esterne)
6. [Regolarità urbanistica e precedenti edilizi](#6-regolarità-urbanistica-e-precedenti-edilizi)
7. [Calcolo del contributo di costruzione](#7-calcolo-del-contributo-di-costruzione)
8. [Tecnici incaricati](#8-tecnici-incaricati)
9. [Impresa esecutrice dei lavori](#9-impresa-esecutrice-dei-lavori)
10. [Sicurezza sul lavoro — D.Lgs. 81/2008](#10-sicurezza-sul-lavoro--dlgs-812008)
11. [Dichiarazioni finali obbligatorie](#11-dichiarazioni-finali-obbligatorie)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Dove si trova**: Sezione "Titolarità dell'intervento" → 2 radio button sotto "dell'immobile interessato dall'intervento e di"

**Causa**: Non hai indicato se hai titolarità esclusiva o non esclusiva sull'immobile.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu a discesa `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) e il campo "Specificare se altro" sono presenti nel modulo ma **non vengono validati** dal codice VB — non generano errori se vuoti o sul valore "altron". Il sistema valida solo il radio button della titolarità esclusiva/non esclusiva.

---

## 2. Presentazione della segnalazione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della denuncia di inizio attività'.

**Dove si trova**: Sezione "Presentazione della segnalazione" → 3 radio button

**Causa**: Non hai indicato la modalità di presentazione della SCIA.

**Soluzione**: Seleziona **uno dei tre radio button** in base al tipo di comunicazione scelto in testa al modulo:
- ⚪ **b_1** — "SCIA Alternativa al Permesso di Costruire: i lavori avranno inizio non prima di 30 giorni dalla data di presentazione"
- ⚪ **b_2** — "SCIA Alternativa al Permesso di Costruire più altre segnalazioni o comunicazioni (SCIA Unica)..."
- ⚪ **b_3** — "SCIA Alternativa al Permesso di Costruire più domanda per il rilascio di atti di assenso (SCIA Condizionata)..."

{: .note }
> I tre radio button della presentazione corrispondono ai tre "Tipi di Comunicazione" in cima al modulo (SCIA semplice / SCIA Unica / SCIA Condizionata). Il tipo di comunicazione in testa al modulo **non è validato** dal codice — è solo un elemento informativo. Il radio button della presentazione invece è obbligatorio. Assicurati che i due siano coerenti.

---

## 3. Qualificazione dell'intervento

### ATTENZIONE ! Non è stato selezionato l'intervento i cui lavori avranno inizio.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → radio button "interventi i cui lavori avranno inizio"

**Causa**: Non hai spuntato il radio button principale della qualificazione.

**Soluzione**: Seleziona il radio button "interventi i cui lavori avranno inizio" (il solo disponibile), poi seleziona anche la data o la modalità di inizio.

---

### ATTENZIONE ! Inidicare la data di inizio lavori o se la comunicazione avverrà successivamente.

**Causa**: Hai selezionato il radio principale ma non hai indicato quando avranno inizio i lavori.

**Soluzione**: Seleziona **uno dei due sotto-radio**:
- ⚪ **a_1_1** — "in data ___" → inserisci la data di inizio lavori
- ⚪ **a_1_2** — "dopo la comunicazione, da parte dello sportello unico, dell'avvenuta acquisizione degli atti di assenso presupposti"

{: .note }
> Il messaggio contiene un refuso ("Inidicare" invece di "Indicare") — è il testo esatto del codice sorgente.

---

### ATTENZIONE ! Specificare la data di inizio lavori.

**Causa**: Hai selezionato a_1_1 ("in data") ma il campo data è vuoto.

**Soluzione**: Inserisci la data prevista di inizio lavori nel campo accanto al radio button.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data inserita non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/09/2025`).

---

### ATTENZIONE ! Indicare almeno una tipologia di intervento.

**Causa**: La checkbox principale `chkQualInt2` — "interventi per i quali è possibile presentare la SCIA alternativa al permesso di costruire (individuati dall'articolo 23, del d.P.R. n. 380/2001 o altri interventi individuati dalla legislazione regionale)" — non è spuntata.

**Soluzione**: Spunta la checkbox `chkQualInt2` e poi seleziona almeno una delle 4 sotto-checkbox relative al mutamento di destinazione d'uso.

---

### ATTENZIONE ! Indicare il mutamento di destinazione d'uso.

**Causa**: Hai spuntato la checkbox principale `chkQualInt2` ma non hai specificato la situazione relativa al mutamento di destinazione d'uso.

**Soluzione**: Spunta **almeno una** delle 4 sotto-checkbox:
- ☐ **chkQualInt2_1** — "**non comporta** mutamento di destinazione d'uso di una singola unità immobiliare o di un intero immobile"
- ☐ **chkQualInt2_2** — "**comporta mutamento** di destinazione d'uso di una singola unità immobiliare all'interno della stessa categoria funzionale"
- ☐ **chkQualInt2_3** — "**comporta mutamento** di destinazione d'uso di una singola unità immobiliare, ubicata in zone A), B) e C) del d.m. n. 1444/1968, tra categorie funzionali di cui all'art. 23 ter c.1, lett. a), a-bis), b) e c)"
- ☐ **chkQualInt2_4** — "**comporta mutamento** di destinazione d'uso di un intero immobile all'interno della stessa categoria funzionale ai sensi dell'art. 23-ter, comma 3"

{: .note }
> Le 4 sotto-checkbox non sono mutuamente esclusive: è possibile spuntarne più di una se l'intervento riguarda tipologie diverse. La prima (chkQualInt2_1 — non comporta mutamento) è tipicamente selezionata per interventi di ristrutturazione senza cambio d'uso. Le altre tre riguardano scenari di mutamento disciplinati dall'art. 23-ter del D.P.R. 380/2001.

---

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Causa**: Il campo `txtDescrIntervento` è vuoto. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice sorgente.

**Soluzione**: Inserisci la descrizione sintetica nel campo multiriga (max **300 caratteri**).

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

**Soluzione**: Aggiungi almeno un fabbricato o terreno e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista.

---

### Coordinate UTM WGS84 32N

#### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Soluzione**: Inserisci la coordinata X (tra **430.000 e 700.000**).

---

#### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: Valore fuori intervallo o non numerico.

**Soluzione**: Inserisci un numero compreso tra **430.000** e **700.000** in formato UTM WGS84 32N (es. `514523`). Valori negativi, gradi decimali (es. `9.1`) o testo generano questo errore.

---

#### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Soluzione**: Inserisci la coordinata Y (tra **4.800.000 e 5.700.000**).

---

#### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Valore fuori intervallo o non numerico.

**Soluzione**: Inserisci un numero compreso tra **4.800.000** e **5.700.000** (es. `5034512`). Vedi nota sulle coordinate nell'[AP Lombardia](errori-ap-lombardia.html#coordinate-utm-wgs84-32n).

---

## 5. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Dove si trova**: Sezione "Opere su parti comuni o modifiche esterne" → 2 radio button

**Causa**: Non hai indicato se le opere riguardano parti comuni, oppure hai selezionato "riguardano" senza specificare il tipo.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **d_1** — "non riguardano opere comuni" → nessun campo aggiuntivo
- ⚪ **d_2** — "riguardano" → spunta almeno una delle 3 sotto-checkbox

Se hai selezionato d_2, spunta **almeno una** tra:
- ☐ **chkOpereb_2** — "le parti comuni di un fabbricato condominiale"
- ☐ **chkOpereb_3** — "parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ☐ **chkOpereb_4** — "parti dell'edificio di proprietà comune ma non necessitano di assenso dei comproprietari perché, secondo l'art. 1102 c.c., apportano... modificazioni necessarie per il miglior godimento delle parti comuni"

{: .note }
> Le 3 sotto-checkbox si attivano solo dopo aver selezionato il radio "riguardano" (d_2). Fino a quel momento sono disabilitate (`Enabled="False"`). Se nessuna delle 3 è spuntata dopo aver selezionato d_2, il validatore genera lo stesso messaggio "Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'."

---

## 6. Regolarità urbanistica e precedenti edilizi

Questa è la sezione più articolata della pratica. Il validatore richiede prima la selezione di uno dei 6 radio button principali (`$RegUrb`), poi verifica le checkbox e i campi in base all'opzione scelta.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Causa**: Non hai selezionato nessuno dei 6 radio button principali.

**Soluzione**: Seleziona **uno dei sei radio button** che descrive lo stato dell'immobile:
- ⚪ **g_1** — "le opere riguardano un intervento di nuova costruzione su area libera"
- ⚪ **g_2** — "l'immobile/U.I. è stato oggetto del/i seguente/i titolo/i o pratica/che edilizie" → seleziona i titoli precedenti
- ⚪ **g_3** — "si tratta di immobile realizzato in un'epoca in cui non era obbligatorio un titolo abilitativo" → allega documentazione storica
- ⚪ **g_4** — "non sono disponibili la copia o gli estremi del titolo abilitativo, ma sussiste un principio di prova documentale" → allega prova
- ⚪ **g_5** — "sono state irrogate le seguenti sanzioni pecuniarie... interamente versate"
- ⚪ **g_6** — "l'immobile/U.I. è stato oggetto della/e seguente/i dichiarazione/i di tolleranza/e costruttiva/e di cui all'art. 34-bis o 34-ter, comma 4 del D.P.R. 380/2001 e/o all'art. 6-bis, comma 2 e 3 della L.R. 19/1999"

---

### Opzione g_2 — Titoli edilizi precedenti (checkbox 1-13)

#### ATTENZIONE! Non è stata selezionata nessun titolo o pratica edilizia.

**Causa**: Hai selezionato g_2 ma non hai spuntato nessuna delle 13 checkbox dei titoli edilizi.

**Soluzione**: Spunta **almeno una** delle checkbox tra: titolo unico (SUAP), permesso di costruire/licenza/concessione, autorizzazione edilizia, comunicazione edilizia (art. 26 L. 47/1985), denuncia di inizio attività, DIA/SCIA alternativa al PdC, segnalazione certificata di inizio attività, comunicazione edilizia libera, titolo in sanatoria, oppure una delle 4 checkbox "altro".

---

#### ATTENZIONE ! Inserire il numero del titolo o pratica edilizia.

**Causa**: Hai spuntato una delle checkbox 1–8 (titoli con denominazione specifica) ma non hai compilato il campo "n." relativo.

**Soluzione**: Inserisci il numero del titolo nel campo "n." accanto alla checkbox spuntata.

---

#### ATTENZIONE ! Inserire la data del titolo o pratica edilizia.

**Causa**: Hai compilato il numero ma non la data del titolo, oppure la data non è nel formato corretto.

**Soluzione**: Inserisci la data nel campo "del" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data inserita per il titolo edilizio non rispetta il formato richiesto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### Checkbox g_2 — Sanatoria (chkRegUrb2_9)

Se spunti la checkbox "titolo edilizio in sanatoria con il pagamento della relativa oblazione ed in particolare", si apre un secondo livello con 4 sotto-checkbox di sanatoria.

#### ATTENZIONE! Non è stata selezionata nessun titolo edilizio in sanatoria.

**Causa**: Hai spuntato la checkbox "sanatoria" (chkRegUrb2_9) ma non hai spuntato nessuna delle 4 sotto-opzioni.

**Soluzione**: Spunta **almeno una** tra:
- ☐ condono edilizio
- ☐ permesso di costruire in sanatoria di cui agli artt. 36 o 36-bis
- ☐ SCIA in sanatoria di cui all'art. 36-bis
- ☐ SCIA in sanatoria per variante in corso d'opera realizzata costituente parziale difformità dal titolo rilasciato prima della L. 10/1977

Ogni sotto-checkbox spuntata richiede numero e data nel formato GG/MM/AAAA (stessi messaggi di errore delle checkbox 1-8).

---

### Checkbox g_2 — "Altro" (chkRegUrb2_10..13)

Le checkbox 10-13 sono denominate "altro" e hanno un campo aggiuntivo rispetto alle prime 8: richiedono descrizione + numero + data (3 campi invece di 2).

#### ATTENZIONE ! Inserire la descrizione del titolo o pratica edilizia.

**Causa**: Hai spuntato una checkbox "altro" (10-13) ma non hai compilato il campo descrizione (il primo campo, testo libero).

**Soluzione**: Inserisci la descrizione del tipo di titolo nel campo testo libero accanto alla checkbox "altro".

I campi n. e data vengono validati con gli stessi messaggi delle checkbox precedenti.

---

### Opzione g_3 — Immobile ante-obbligo titolo

#### ATTENZIONE! Non è stata selezionato nessun tipo di allegato. (g_3)

**Causa**: Hai selezionato g_3 ("immobile realizzato in epoca senza obbligo di titolo") ma non hai spuntato nessuno dei 2 allegati.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkRegUrb3_1** — "copia accatastamento di primo impianto o si forniscono i relativi estremi" → inserisci n. e data (GG/MM/AAAA)
- ☐ **chkRegUrb3_2** — "altri documenti probanti (riprese fotografiche, estratti cartografici, documenti di archivio, ecc.) a norma dell'art. 9-bis, comma 1-bis, quarto e quinto periodo, d.P.R. n. 380 del 2001" → nessun campo aggiuntivo

Se spunti chkRegUrb3_1: inserisci il numero e la data nel formato GG/MM/AAAA.

---

### Opzione g_4 — Principio di prova documentale

#### ATTENZIONE! Non è stata selezionato nessun tipo di allegato. (g_4)

**Causa**: Hai selezionato g_4 ("non disponibili copia o estremi titolo ma principio di prova") ma non hai spuntato nessun allegato.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkRegUrb4_1** — "copia accatastamento di primo impianto o si forniscono i relativi estremi" → inserisci n. e data (GG/MM/AAAA)
- ☐ **chkRegUrb4_2** — "altri documenti probanti" → nessun campo aggiuntivo

---

### Opzione g_5 — Sanzioni pecuniarie versate

#### ATTENZIONE! Non è stata selezionato nessun tipo di sanzioni pecuniarie.

**Causa**: Hai selezionato g_5 ("sanzioni pecuniarie interamente versate") ma non hai spuntato nessuna delle 2 opzioni.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkRegUrb5_1** — "si allega la relativa ricevuta" → nessun campo aggiuntivo
- ☐ **chkRegUrb5_2** — "si forniscono gli estremi del pagamento di €..." → compila tutti i 4 campi:

Se spunti chkRegUrb5_2, sono obbligatori:

**ATTENZIONE ! Inserire l'ammontare del pagamento.** → inserisci l'importo in euro nel primo campo.

**ATTENZIONE ! Inserire la data di irroga della sanzione.** → inserisci la data nel formato **GG/MM/AAAA**.

**ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.** (data irroga) → correggi il formato.

**ATTENZIONE ! Inserire il numero del protocollo.** → inserisci il n. del protocollo della sanzione.

**ATTENZIONE ! Inserire la data del protocollo.** → inserisci la data nel formato **GG/MM/AAAA**.

**ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.** (data protocollo) → correggi il formato.

---

### Opzione g_6 — Dichiarazioni di tolleranza

#### ATTENZIONE! Non è stata selezionato nessun tipo di tolleranza.

**Causa**: Hai selezionato g_6 ("dichiarazioni di tolleranza costruttiva art. 34-bis o 34-ter / art. 6-bis L.R. 19/1999") ma non hai spuntato nessuna delle 2 opzioni.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkRegUrb6_1** — "dichiarazione delle tolleranze di cui all'art. 34-bis o 34-ter, comma 4, presentata nella modulistica relativa alla pratica edilizia prot." → inserisci n. e data (GG/MM/AAAA)
- ☐ **chkRegUrb6_2** — "dichiarazione delle tolleranze di cui all'art. 34-bis o 34-ter, comma 4, allegata agli atti aventi per oggetto trasferimento o costituzione... atto di registrazione" → inserisci n. e data (GG/MM/AAAA)

Se spunti chkRegUrb6_1: **ATTENZIONE ! Inserire il numero di protocollo della pratica edilizia** e **ATTENZIONE ! Inserire la data del protocollo della pratica edilizia**.

Se spunti chkRegUrb6_2: **ATTENZIONE ! Inserire il numero dell'atto di registrazione** e **ATTENZIONE ! Inserire la data dell'atto di registrazione**.

---

### Stato attuale dell'immobile (chkRegUrb7) — obbligatoria per tutte le opzioni g_1..g_6

Dopo aver compilato la sezione regolarità urbanistica con uno dei 6 radio button, il sistema verifica sempre la checkbox dello stato attuale, indipendentemente dall'opzione scelta.

#### ATTENZIONE! Dichiarare lo stato attuale dell'immobile.

**Causa**: La checkbox `chkRegUrb7` — "dichiara che lo stato attuale dell'immobile/U.I risulta:" — non è spuntata.

**Soluzione**: Spunta la checkbox `chkRegUrb7`. Dopo averla spuntata, seleziona **almeno una** delle 2 sotto-checkbox.

---

#### ATTENZIONE! Selezionare lo stato attuale dell'immobile.

**Causa**: Hai spuntato `chkRegUrb7` ma non hai selezionato nessuna delle 2 sotto-opzioni.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkRegUrb7_1** — "pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"
- ☐ **chkRegUrb7_2** — "conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicata, unitamente alla/e sanatoria/e di cui al quadro relativo alla Sanatoria e alla/e dichiarazione/i di tolleranza esecutive di cui alla relazione tecnica di asseverazione"

{: .note }
> La checkbox `chkRegUrb7` con le sue sotto-opzioni è separata dal radio group principale `$RegUrb` e viene verificata sempre, indipendentemente da quale opzione g_1..g_6 sia selezionata. È un doppio livello di dichiarazione sullo stato attuale: prima il radio group dichiara la storia del titolo abilitativo, poi `chkRegUrb7` dichiara la conformità attuale dell'immobile a quella storia.

---

## 7. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Non hai indicato se il contributo è dovuto.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_1** — "è a titolo gratuito, ai sensi della seguente normativa" → inserisci la normativa
- ⚪ **g_2** — "è a titolo oneroso e pertanto allega il prospetto di calcolo preventivo del contributo di costruzione e/o monetizzazione..." → seleziona le modalità di versamento

---

### ATTENZIONE !  Inserire la normativa.

**Causa**: Hai selezionato "gratuito" (g_1) ma non hai compilato il campo della normativa di riferimento accanto al radio button. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice sorgente.

**Soluzione**: Inserisci la normativa che giustifica la gratuità del contributo (es. `art. 17 c.3 lett. a) DPR 380/2001`, `art. 23 c.7 LR 12/2005`).

---

### ATTENZIONE ! Indicare almeno una voce per 'Versamento del contributo dovuto'.

**Causa**: Hai selezionato "oneroso" (g_2) ma non hai spuntato nessuna delle 3 checkbox relative alle modalità di versamento.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkInterventog3_1** — "si effettuerà il pagamento del contributo di costruzione e/o monetizzazione... entro 30 giorni dalla data di presentazione della segnalazione..."
- ☐ **chkInterventog3_2** — "si chiede la rateizzazione del contributo di costruzione e/o monetizzazione..."
- ☐ **chkInterventog3_3** — "si impegna a corrispondere il costo di costruzione in corso di esecuzione delle opere..."

{: .note }
> La quarta checkbox `chkInterventog4_1` ("chiede di eseguire direttamente... le opere di urbanizzazione... a scomputo") è visibile ma **non validata** dal codice (è commentata nel validatore). La checkbox è opzionale e non genera errori. Le 3 checkbox validate possono essere selezionate anche in combinazione tra loro.

---

## 8. Tecnici incaricati

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Causa**: Non hai indicato la situazione dei direttori dei lavori.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **h_1** — "di aver incaricato, in qualità di direttori dei lavori, e di altri tecnici, i soggetti indicati alla sezione Tecnici incaricati dei 'SOGGETTI COINVOLTI'" → almeno un tecnico deve essere presente nei soggetti
- ⚪ **h_2** — "che il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori" → nessuna verifica sui soggetti

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Hai selezionato h_1 (tecnici già incaricati) ma la sezione soggetti coinvolti non ha nessun tecnico.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico. Non è richiesto un ruolo specifico.

---

## 9. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai indicato la situazione dell'impresa esecutrice.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **i_1** — "i lavori sono/saranno eseguiti dalla/e impresa/e indicata/e alla sezione Imprese Esecutrici dei 'SOGGETTI COINVOLTI'" → almeno un'impresa deve essere presente
- ⚪ **i_2** — "l'impresa esecutrice/imprese esecutrici dei lavori sarà/saranno individuata/e prima dell'inizio dei lavori"
- ⚪ **i_3** — "che, trattandosi di opere in sanatoria, non è nota l'impresa/e esecutrice/i dei lavori"

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato i_1 (impresa già individuata) ma non hai inserito nessuna impresa nella sezione soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice.

---

## 10. Sicurezza sul lavoro — D.Lgs. 81/2008

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Non hai selezionato nessuno dei 3 radio button.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **l_1** — "non ricade nell'ambito di applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)"
- ⚪ **l_2** — "ricade nell'ambito di applicazione delle norme... e pertanto" → seleziona documentazione imprese e notifica
- ⚪ **l_3** — "ricade... ma si riserva di presentare le dichiarazioni... prima dell'inizio lavori, poiché i dati dell'impresa esecutrice saranno forniti prima dell'inizio lavori" → nessuna sotto-selezione richiesta

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato l_2 ma non hai specificato la situazione della documentazione delle imprese.

**Soluzione**: Seleziona **uno dei due sotto-radio**:
- ⚪ **l_2_1** — "dichiara che l'entità presunta del cantiere è inferiore a 200 uomini-giorno ed i lavori non comportano i rischi particolari di cui all'allegato XI..." (verifica documentazione semplificata)
- ⚪ **l_2_2** — "dichiara che l'entità presunta del cantiere è pari o superiore a 200 uomini-giorno o i lavori comportano i rischi particolari..." → seleziona notifica preliminare

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato l_2_2 (≥ 200 UG o rischi particolari) ma non hai indicato se la notifica è dovuta.

**Soluzione**: Seleziona **uno dei due radio**:
- ⚪ "dichiara che l'intervento non è soggetto all'invio della notifica"
- ⚪ "dichiara che l'intervento è soggetto all'invio della notifica" → seleziona modalità

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione/Estremi Notifica'.

**Causa**: Hai indicato che la notifica è dovuta ma non hai selezionato la modalità.

**Soluzione**: Seleziona **uno dei due radio** (diversi dall'Inizio Lavori Nazionale — nessun campo data richiesto):
- ⚪ **l_2_2_2_1** — "la notifica è stata inserita nel sistema informativo **Ge.CA** (http://www.previmpresa.servizirl.it/cantieri/) e il relativo contenuto sarà esposto in cantiere per tutta la durata dei lavori, in luogo visibile dall'esterno"
- ⚪ **l_2_2_2_2** — "**invierà** la notifica prima dell'inizio dei lavori"

{: .note }
> A differenza della stessa sezione nell'Inizio Lavori Nazionale, qui la modalità notifica non richiede data e protocollo — i due radio button sono terminali e non aprono campi aggiuntivi. Il riferimento specifico a **Ge.CA** (sistema informativo regionale lombardo) è caratteristico della Lombardia.

---

## 11. Dichiarazioni finali obbligatorie

Le ultime tre sezioni contengono checkbox che devono essere **tutte e tre** obbligatoriamente spuntate. Il sistema le verifica nell'ordine: conoscenza → diritti terzi → privacy.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Conoscenza efficacia procedura edilizia'.

**Dove si trova**: Sezione "Rispetto degli obblighi in materia di salute e sicurezza" → checkbox `chkConoscenza`

**Causa**: Non hai spuntato la dichiarazione che recita "di essere a conoscenza che l'efficacia della presente procedura edilizia è sospesa qualora sia assente il piano di sicurezza e coordinamento di cui all'articolo 100 del d.lgs. n. 81/2008..."

**Soluzione**: Spunta la checkbox `chkConoscenza`.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Consapevolezza diritti di terzi'.

**Dove si trova**: Sezione "Diritti di terzi" → checkbox `chkDirittiTerzi`

**Causa**: Non hai spuntato la dichiarazione "di essere consapevole che quanto dichiarato non comporta limitazione dei diritti dei terzi".

**Soluzione**: Spunta la checkbox `chkDirittiTerzi`.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione "Rispetto della normativa sulla privacy" → checkbox `chkPrivacy`

**Causa**: Non hai spuntato la dichiarazione "di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune".

**Soluzione**: Spunta la checkbox `chkPrivacy`.

---

## Consigli pratici — SCIA alt. PdC Lombardia

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (esclusiva o non esclusiva)
- [ ] Seleziona la **modalità di presentazione** (SCIA semplice / Unica / Condizionata) coerente con il tipo comunicazione in cima
- [ ] Seleziona il radio "interventi i cui lavori avranno inizio" + sotto-radio (data o post-assenso); se data: compilare in GG/MM/AAAA
- [ ] Spunta `chkQualInt2` + almeno una delle 4 sotto-checkbox mutamento d'uso
- [ ] Inserisci la **descrizione** (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci **coordinata X** (430.000–700.000) e **Y** (4.800.000–5.700.000) UTM WGS84 32N
- [ ] Seleziona le **opere comuni** (non riguardano / riguardano con tipo)
- [ ] Seleziona la **regolarità urbanistica** (g_1..g_6) e compila le checkbox e campi relativi
- [ ] Spunta **chkRegUrb7** e seleziona almeno una delle 2 sotto-opzioni stato attuale
- [ ] Seleziona il **contributo** (gratuito con normativa / oneroso con modalità versamento)
- [ ] Seleziona i **tecnici** (già incaricati o da individuare)
- [ ] Seleziona l'**impresa** (già individuata / da individuare / sanatoria)
- [ ] Seleziona la voce **sicurezza** (l_1 / l_2 con sotto-selezioni / l_3)
- [ ] Spunta **chkConoscenza**, **chkDirittiTerzi**, **chkPrivacy**

### La sezione Regolarità urbanistica — schema rapido ⚠️

La sezione g_2 è la più complessa: il loop controlla le checkbox 1-8 (2 campi: n. + data), poi la checkbox 9-sanatoria che apre altre 4 sotto-checkbox (stessi 2 campi), poi le checkbox 10-13-altro (3 campi: descrizione + n. + data). Dopo qualsiasi opzione g_1..g_6, il validatore controlla sempre anche `chkRegUrb7` con le sue 2 sotto-opzioni — non dimenticarla.

### Errori frequenti 🔍

1. **`chkRegUrb7` dimenticata** → questa checkbox è separata dal radio group principale e compare in fondo alla sezione; è facile non vederla dopo la lunga compilazione dei titoli edilizi
2. **Coordinate fuori intervallo** → valori in gradi decimali (es. `45.46` per la latitudine) generano l'errore dell'intervallo; le coordinate UTM per la Lombardia hanno X ~500.000 e Y ~5.000.000
3. **Descrizione qualificazione mancante** → il campo `txtDescrIntervento` è in fondo alla sezione Qualificazione, dopo le 4 checkbox del mutamento d'uso; può essere dimenticato
4. **chkInterventog3 nessuna spuntata con contributo oneroso** → le 3 checkbox del versamento si abilitano solo dopo aver selezionato il radio "oneroso"; se ci si dimentica di spuntarle il validatore blocca con "Indicare almeno una voce"
5. **Tecnici o imprese mancanti nei soggetti** → i controlli su tecnici (se h_1) e imprese (se i_1) avvengono alla fine della validazione; verificare prima di iniziare la procedura

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
**Fonte**: Analisi codice ValidaDatiSCIAaltPDCLombardia e DatiSCIAaltPDCLombardia.ascx
