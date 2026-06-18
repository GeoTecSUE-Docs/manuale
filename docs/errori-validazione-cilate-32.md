---
title: Errori C.I.L.A. Tolleranze Esecutive - Piemonte
parent: Errori di validazione
nav_order: 44
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori Asseverata per Tolleranze Esecutive (CILATE) - Regione Piemonte
keywords: [CILATE, tolleranze esecutive, tolleranze costruttive, art. 34-bis DPR 380/2001, L.R. 19/1999, DGR 2-4519/2022, Piemonte, regolarità urbanistica, precedenti edilizi, rilevatore, progettista asseverante, stato attuale immobile, condono edilizio, sanatoria]
IDRegione: 2         # Piemonte
IDTipoPratica: 53
Fonte: Manuale
---

# Errori di validazione - C.I.L.A. Tolleranze Esecutive (CILATE)
## Regione Piemonte

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori Asseverata per Tolleranze Esecutive** ai sensi dell'art. 6-bis commi 1, 2 e 3 della L.R. n. 19 del 08/07/1999, della D.G.R. n. 2-4519 del 14/01/2022 e dell'art. 34-bis del D.P.R. n. 380/2001 — Regione Piemonte.

{: .note }
> La CILATE è la pratica strutturalmente più complessa della piattaforma. La sezione **"Regolarità urbanistica e precedenti edilizi"** presenta 5 scenari alternativi (radio button) ciascuno con logica condizionale propria: checkbox, sottocheckbox e campi numero/data obbligatori solo se il checkbox padre è spuntato. Nessun'altra pratica raggiunge questo livello di annidamento. Altre caratteristiche esclusive: la **data e il luogo** di sottoscrizione sono **entrambi obbligatori** (con validazione formato data); i dati del **Progettista asseverante** (cognome/nome, ordine/collegio, sede, numero iscrizione) sono una sezione separata dalla parte dichiarativa; il **Rilevatore** deve essere obbligatoriamente presente tra i tecnici nei Soggetti coinvolti (ruolo `RI`). Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Regolarità urbanistica e precedenti edilizi](#2-regolarità-urbanistica-e-precedenti-edilizi)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Data e luogo di sottoscrizione](#4-data-e-luogo-di-sottoscrizione)
5. [Dichiarazioni del progettista asseverante](#5-dichiarazioni-del-progettista-asseverante)
6. [Dichiarazione tolleranze](#6-dichiarazione-tolleranze)
7. [Tecnici incaricati — Rilevatore](#7-tecnici-incaricati--rilevatore)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità Intervento'.

**Causa**: Non hai compilato il menu a discesa iniziale né selezionato il radio button sulla titolarità.

**Soluzione**: Compila il menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"** e seleziona una delle due opzioni:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva... ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"**

---

## 2. Regolarità urbanistica e precedenti edilizi

Questa sezione è la più articolata dell'intera pratica. Contiene **5 scenari alternativi** selezionabili con radio button, ognuno con propri checkbox e campi obbligatori. La logica è: scegli **uno** scenario con il radio button, poi compila le sottovoci previste da quello scenario.

{: .note }
> La validazione controlla prima che sia selezionato almeno un radio button (errore generale), poi, a seconda dello scenario scelto, verifica le sottovoci. In fondo alla sezione, indipendentemente dallo scenario, è sempre obbligatorio dichiarare **lo stato attuale dell'immobile** (sezione 6 — checkbox `chkStatoAttualeImm6_1` o `chkStatoAttualeImm6_2`).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Causa**: Non hai selezionato nessuno dei 5 scenari disponibili.

**Soluzione**: Seleziona **uno dei cinque scenari**:
- ⚪ **Scenario 1** — "l'immobile/U.I. è stato oggetto del/i seguente/i titolo/i o pratica/che edilizie"
- ⚪ **Scenario 2** — "si tratta di immobile realizzato in un'epoca in cui non era obbligatorio un titolo abilitativo"
- ⚪ **Scenario 3** — "non sono disponibili la copia o gli estremi del titolo abilitativo, ma sussiste un principio di prova documentale"
- ⚪ **Scenario 4** — "sono state irrogate le seguenti sanzioni pecuniarie... interamente versate"
- ⚪ **Scenario 5** — "l'immobile/U.I. è stato oggetto della/e seguente/i dichiarazione/i di tolleranza/e costruttiva/e"

---

### Scenario 1 — Titoli o pratiche edilizie

#### ATTENZIONE! Indicare almeno una tipologia di pratica.

**Causa**: Hai selezionato lo Scenario 1 ma non hai spuntato nessuno dei 13 checkbox delle tipologie di pratiche edilizie.

**Soluzione**: Spunta almeno uno dei titoli o pratiche disponibili, tra cui:
- ☑ titolo unico (SUAP)
- ☑ permesso di costruire / licenza edil. / concessione edilizia
- ☑ autorizzazione edilizia
- ☑ comunicazione edilizia (art. 26 l. n. 47/1985)
- ☑ denuncia di inizio attività
- ☑ DIA/SCIA alternativa al permesso di costruire
- ☑ segnalazione certificata di inizio attività
- ☑ comunicazione edilizia libera
- ☑ titolo edilizio in sanatoria con il pagamento della relativa oblazione (checkbox 9, con sottoscelte)
- ☑ altro (checkbox 10–13, con campo descrizione libera)

---

#### ATTENZIONE! Specificare numero della pratica.

**Causa**: Hai spuntato uno dei checkbox 1–8 ma non hai compilato il campo **"n."** (numero) della pratica corrispondente.

**Soluzione**: Inserisci il numero della pratica edilizia nel campo **"n."** accanto al checkbox spuntato. Ogni checkbox spuntato richiede sia il numero sia la data.

---

#### ATTENZIONE! Specificare data della pratica. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Hai spuntato uno dei checkbox 1–8 ma il campo **"del"** (data) è vuoto oppure contiene una data in formato non valido.

**Soluzione**: Inserisci la data nel campo **"del"** accanto al numero, nel formato **GG/MM/AAAA** (es. `15/03/2010`). Puoi usare l'icona calendario.

---

#### Checkbox 9 — Titolo edilizio in sanatoria (sottoscelte obbligatorie)

#### ATTENZIONE! Indicare almeno una tipologia di pratica come 'titolo edilizio in sanatoria con il pagamento della relativa oblazione'.

**Causa**: Hai spuntato il checkbox **"titolo edilizio in sanatoria"** (checkbox 9) ma non hai spuntato nessuna delle 4 sottoscelte.

**Soluzione**: Spunta almeno una delle quattro sottoscelte che compaiono rientrate:
- ☑ **condono edilizio** (n. + data)
- ☑ **permesso di costruire in sanatoria** di cui agli artt. 36 o 36-bis (n. + data)
- ☑ **SCIA in sanatoria** di cui all'art. 36-bis (n. + data)
- ☑ **SCIA in sanatoria per variante in corso d'opera** realizzata costituente parziale difformità dal titolo rilasciato prima della L. 10/1977 (n. + data)

Per ciascuna sottoscelta spuntata sono richiesti numero e data con le stesse regole dei checkbox principali.

---

#### Checkbox 10–13 — "Altro" (campo descrizione obbligatorio)

#### ATTENZIONE! Specificare tipologia della pratica.

**Causa**: Hai spuntato uno dei checkbox **"altro"** (10, 11, 12 o 13) ma non hai compilato il campo di testo libero che descrive la tipologia.

**Soluzione**: Compila il campo di testo libero accanto al checkbox "altro" con la descrizione della tipologia di pratica, quindi inserisci anche numero e data nei campi corrispondenti.

{: .note }
> I checkbox "altro" (10–13) richiedono tre campi: **descrizione tipologia** + **numero** + **data**. I checkbox 1–8 richiedono solo numero e data. Il checkbox 9 richiede la selezione di almeno una sottoscelta, ciascuna con numero e data.

---

### Scenario 2 — Immobile realizzato senza obbligo di titolo

#### ATTENZIONE! Indicare almeno un tipo di allegato.

**Causa**: Hai selezionato lo Scenario 2 ("immobile realizzato in un'epoca in cui non era obbligatorio un titolo abilitativo") ma non hai spuntato nessuno dei due allegati previsti.

**Soluzione**: Spunta **almeno uno** dei due allegati:
- ☑ **"copia accatastamento di primo impianto o si forniscono i relativi estremi"** → richiede numero e data
- ☑ **"altri documenti probanti (riprese fotografiche, estratti cartografici, documenti di archivio, ecc.)"** → nessun campo aggiuntivo

---

#### ATTENZIONE! Specificare numero della copia accatastamento. / ATTENZIONE! Specificare data della copia accatastamento.

**Causa**: Hai spuntato il checkbox "copia accatastamento di primo impianto" nello Scenario 2 ma non hai compilato numero e/o data.

**Soluzione**: Inserisci il numero e la data dell'accatastamento di primo impianto nei campi **"n."** e **"del"** accanto al checkbox.

---

### Scenario 3 — Principio di prova documentale

#### ATTENZIONE! Indicare almeno un tipo di allegato.

**Causa**: Hai selezionato lo Scenario 3 ("non sono disponibili la copia o gli estremi del titolo, ma sussiste un principio di prova documentale") ma non hai spuntato nessuno dei due allegati.

**Soluzione**: Spunta **almeno uno** dei due allegati (stessi dell'Scenario 2):
- ☑ **"copia accatastamento di primo impianto o si forniscono i relativi estremi"** → richiede numero e data
- ☑ **"altri documenti probanti"** → nessun campo aggiuntivo

---

#### ATTENZIONE! Specificare numero della copia accatastamento. / ATTENZIONE! Specificare data della copia accatastamento.

**Causa**: Hai spuntato il checkbox "copia accatastamento" nello Scenario 3 ma non hai compilato numero e/o data.

**Soluzione**: Inserisci numero e data nei campi **"n."** e **"del"** accanto al checkbox.

---

### Scenario 4 — Sanzioni pecuniarie irrogate e versate

#### ATTENZIONE! Indicare almeno una sanzione pecuniaria.

**Causa**: Hai selezionato lo Scenario 4 ("sono state irrogate sanzioni pecuniarie, interamente versate") ma non hai spuntato nessuno dei due checkbox.

**Soluzione**: Spunta **almeno uno** dei due:
- ☑ **"si allega la relativa ricevuta"** → nessun campo aggiuntivo
- ☑ **"si forniscono gli estremi del pagamento"** → richiede importo, data irrogazione, numero protocollo e data protocollo

---

#### ATTENZIONE! Specificare importo della sanzione pecuniaria.

**Causa**: Hai spuntato "si forniscono gli estremi del pagamento" ma non hai inserito l'importo in euro.

**Soluzione**: Inserisci l'importo in euro nel campo **"€"** accanto al checkbox.

---

#### ATTENZIONE! Specificare data del pagamento della sanzione pecuniaria. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Il campo della data di irrogazione della sanzione è vuoto o in formato errato.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** nel campo **"irrogata in data"**.

---

#### ATTENZIONE! Specificare numero di protocollo della sanzione pecuniaria.

**Causa**: Il campo **"Prot. n."** del provvedimento di irrogazione è vuoto.

**Soluzione**: Inserisci il numero di protocollo del provvedimento di irrogazione della sanzione.

---

#### ATTENZIONE! Specificare data di protocollo della sanzione pecuniaria. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Il campo **"del"** accanto al numero di protocollo è vuoto o in formato errato.

**Soluzione**: Inserisci la data di protocollo nel formato **GG/MM/AAAA**.

---

### Scenario 5 — Dichiarazioni di tolleranza costruttiva precedenti

#### ATTENZIONE! Indicare almeno una dichiarazione di tolleranza costruttiva.

**Causa**: Hai selezionato lo Scenario 5 ("l'immobile è stato oggetto di dichiarazioni di tolleranza costruttiva di cui all'art. 34-bis o 34-ter, comma 4") ma non hai spuntato nessuno dei due checkbox.

**Soluzione**: Spunta **almeno uno** dei due:
- ☑ **"dichiarazione delle tolleranze... nella modulistica relativa alla pratica edilizia prot."** → richiede numero protocollo e data
- ☑ **"dichiarazione delle tolleranze... allegata agli atti di trasferimento... atto di registrazione"** → richiede numero e data dell'atto

---

#### ATTENZIONE! Specificare numero di protocollo della pratica edilizia. / ATTENZIONE! Specificare data di protocollo della pratica edilizia.

**Causa**: Hai spuntato il primo checkbox dello Scenario 5 ma non hai compilato numero e/o data del protocollo.

**Soluzione**: Inserisci il numero e la data di protocollo della pratica edilizia originaria nei campi **"n."** e **"del"**.

---

#### ATTENZIONE! Specificare numero dell'atto di registrazione. / ATTENZIONE! Specificare data dell'atto di registrazione.

**Causa**: Hai spuntato il secondo checkbox dello Scenario 5 ma non hai compilato numero e/o data dell'atto di registrazione.

**Soluzione**: Inserisci il numero e la data dell'atto di registrazione nei campi **"n."** e **"del"**.

---

### Stato attuale dell'immobile — obbligatorio per tutti gli scenari

#### ATTENZIONE! Indicare almeno uno stato attuale dell'immobile.

**Dove si trova**: In fondo alla sezione "Regolarità urbanistica", sotto tutti i 5 scenari → **"dichiara che lo stato attuale dell'immobile/U.I. risulta:"**

**Causa**: Indipendentemente dallo scenario scelto, non hai dichiarato lo stato attuale dell'immobile. Questo blocco è sempre obbligatorio.

**Soluzione**: Spunta **almeno uno** dei due:
- ☑ **"pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"**
- ☑ **"conforme alla documentazione... unitamente alla/e sanatoria/e... e alla/e dichiarazione/i di tolleranza esecutive..."**

{: .warning }
> Questo controllo è **separato dalla scelta dello scenario** ed è posizionato in fondo alla sezione: è facile dimenticarlo dopo aver compilato il corpo principale. Scorrere sempre fino in fondo alla sezione "Regolarità urbanistica" per verificare che almeno uno dei due checkbox di stato attuale sia spuntato.

---

## 3. Localizzazione dell'intervento

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
3. Salva con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Data e luogo di sottoscrizione

### ATTENZIONE ! Inserire la data. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Dove si trova**: Riquadro **"Attenzione"** in fondo alla parte dichiarativa → campo **"data"**

**Causa**: Il campo data di sottoscrizione è vuoto oppure contiene una data in formato non valido.

**Soluzione**: Inserisci la data di sottoscrizione della comunicazione nel formato **GG/MM/AAAA**. A differenza di altre pratiche, questa data è **validata nel formato** (controllo `ControlloFormatoData`).

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Riquadro **"Attenzione"** → campo **"luogo"**

**Causa**: Il campo luogo di sottoscrizione è vuoto.

**Soluzione**: Inserisci il Comune o la località in cui viene sottoscritta la comunicazione.

{: .note }
> Nella CILATE sia **data** sia **luogo** sono obbligatori e validati. In molte altre pratiche della piattaforma questi campi non sono controllati dalla funzione di validazione. Ricordati di compilarli entrambi prima di cliccare "Valida e Salva".

---

## 5. Dichiarazioni del progettista asseverante

Questa sezione è separata dalla parte dichiarativa del titolare e contiene i dati identificativi del progettista che assevera la comunicazione.

---

### ATTENZIONE ! Inserire il Cognome e Nome del Progettista.

**Dove si trova**: Sezione **"DICHIARAZIONI DEL PROGETTISTA"** → campo **"Cognome e Nome"**

**Causa**: Il campo cognome e nome del progettista asseverante è vuoto.

**Soluzione**: Inserisci cognome e nome del progettista nel campo **"Cognome e Nome"**.

{: .note }
> Nella CILATE il progettista asseverante ha una sezione dati dedicata separata dai soggetti coinvolti. Il campo raccoglie cognome e nome in un unico campo di testo. I dati anagrafici completi (timbro, ecc.) sono richiesti nell'allegato **"Soggetti coinvolti"**.

---

### ATTENZIONE ! Inserire il Collegio del Progettista.

**Dove si trova**: Sezione **"DICHIARAZIONI DEL PROGETTISTA"** → campo **"Iscritto all'ordine/collegio"**

**Causa**: Non hai indicato l'ordine o collegio professionale di appartenenza del progettista.

**Soluzione**: Inserisci il nome dell'ordine o collegio nel campo **"Iscritto all'ordine/collegio"** (es. `Ordine degli Architetti`, `Collegio dei Geometri`).

---

### ATTENZIONE ! Inserire la sede del Collegio del Progettista.

**Dove si trova**: Sezione **"DICHIARAZIONI DEL PROGETTISTA"** → campo **"di"** (sede)

**Causa**: Non hai indicato la sede dell'ordine o collegio professionale.

**Soluzione**: Inserisci la sede (provincia o città) nel campo **"di"** accanto al nome del collegio (es. `Torino`, `Cuneo`).

---

### ATTENZIONE ! Inserire il numero del Collegio del Progettista.

**Dove si trova**: Sezione **"DICHIARAZIONI DEL PROGETTISTA"** → campo **"al numero"**

**Causa**: Non hai inserito il numero di iscrizione all'ordine o collegio professionale.

**Soluzione**: Inserisci il numero di iscrizione nel campo **"al numero"**.

---

## 6. Dichiarazione tolleranze

### ATTENZIONE ! Dichiarare almeno una tollerenza.

**Dove si trova**: Sezione **"DICHIARA"** del progettista → checkbox delle tolleranze esecutive

**Causa**: Il progettista non ha dichiarato a quali norme si riferiscono le tolleranze esecutive oggetto della comunicazione.

**Soluzione**: Spunta **almeno uno** dei tre riferimenti normativi:
- ☑ **"ai commi 1, 2 e 3 della Legge regionale n. 19 del 08 Luglio 1999"**
- ☑ **"alla D.G.R. n. 2-4519 del 14 Gennaio 2022"**
- ☑ **"all'art. 34-bis del D.P.R. n. 380 del 6 Giugno 2001"**

{: .note }
> È possibile spuntare più di uno dei tre riferimenti normativi se le tolleranze ricadono contemporaneamente in più ambiti. Il messaggio recita "tollerenza" (con un refuso nel codice sorgente) invece di "tolleranza": il messaggio nell'interfaccia potrebbe apparire con questa grafia.

---

## 7. Tecnici incaricati — Rilevatore

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Rilevatore.

**Dove si trova**: Sezione **"Tecnici incaricati"** del modulo + scheda **"Soggetti coinvolti"** → tecnici

**Causa**: Non hai aggiunto nessun tecnico con ruolo **"Rilevatore"** (codice `RI`) tra i soggetti coinvolti. La CILATE richiede obbligatoriamente la presenza di almeno un rilevatore incaricato.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Rilevatore"**
4. Compila i dati del tecnico e salva
5. Torna al modulo CILATE, clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> Il controllo sul Rilevatore è l'**ultimo** eseguito dalla funzione di validazione: tutti gli altri errori devono essere corretti prima che questo venga verificato. Se non compare questo errore ma la validazione non passa, controlla le sezioni precedenti. Se compare, significa che tutti gli altri controlli sono stati superati.

---

## Consigli pratici CILATE

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (menu a discesa + radio button)
- [ ] Seleziona uno dei **5 scenari** di regolarità urbanistica
- [ ] **Scenario 1**: spunta almeno un titolo edilizio (1–13) con numero e data per ciascuno spuntato; se spunti il checkbox 9 (sanatoria), scegli almeno una delle 4 sottoscelte con numero e data; se spunti i checkbox 10–13 (altro), compila anche la descrizione
- [ ] **Scenario 2 o 3**: spunta almeno un allegato; se spunti "copia accatastamento", inserisci numero e data
- [ ] **Scenario 4**: spunta almeno una voce; se spunti "si forniscono gli estremi", compila importo, data irrogazione, numero e data protocollo
- [ ] **Scenario 5**: spunta almeno una dichiarazione; inserisci numero e data per ciascuna spuntata
- [ ] **Tutti gli scenari**: spunta almeno uno dei due checkbox di **stato attuale immobile** in fondo alla sezione
- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data** di sottoscrizione (GG/MM/AAAA) nel riquadro "Attenzione"
- [ ] Inserisci il **luogo** di sottoscrizione
- [ ] Compila i dati del **progettista asseverante**: cognome/nome, ordine/collegio, sede, numero iscrizione
- [ ] Spunta almeno **una tolleranza** (L.R. 19/1999, DGR 2-4519/2022 o art. 34-bis DPR 380/2001)
- [ ] Aggiungi il **Rilevatore** nei Soggetti coinvolti (ruolo `RI`)
- [ ] **Salva** frequentemente

### Mappa della sezione "Regolarità urbanistica" ⚠️

| Scenario | Condizione | Cosa serve |
|---|---|---|
| 1 | Titoli edilizi esistenti | ≥ 1 checkbox tra 1–13 spuntato; n. + data per ciascuno; se checkbox 9 → ≥ 1 sottoscelta con n. + data; se checkbox 10–13 → anche descrizione |
| 2 | Immobile ante-obbligo titolo | ≥ 1 allegato; se "copia accatastamento" → n. + data |
| 3 | Prova documentale parziale | ≥ 1 allegato; se "copia accatastamento" → n. + data |
| 4 | Sanzioni pecuniarie pagate | ≥ 1 voce; se "si forniscono estremi" → importo + data irrogazione + n. prot. + data prot. |
| 5 | Tolleranze precedenti | ≥ 1 checkbox; per ciascuno → n. + data |
| Tutti | Stato attuale immobile | ≥ 1 checkbox tra `6_1` e `6_2` |

### Errori frequenti CILATE 🔍

1. **Stato attuale immobile non spuntato** → è in fondo alla sezione Regolarità, dopo tutti i 5 scenari; spesso dimenticato
2. **Checkbox 9 (sanatoria) spuntato senza sottoscelta** → il checkbox padre non basta: occorre spuntare almeno una delle 4 sottoscelte con n. e data
3. **Checkbox 10–13 ("altro") senza descrizione** → questi richiedono tre campi (descrizione + n. + data); la sola spunta non è sufficiente
4. **Data e luogo mancanti** → questi campi sono in fondo al modulo titolare, prima della sezione "Dichiarazioni del progettista"; facili da saltare
5. **Rilevatore mancante** → deve essere aggiunto nei Soggetti coinvolti con ruolo specifico `RI`, non basta aggiungere un tecnico generico
6. **Nessuna tolleranza dichiarata** → i tre checkbox delle tolleranze (sezione "DICHIARA" del progettista) sono obbligatori e separati dal resto

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
**Fonte**: Analisi codice `ValidaDatiCILATE` e `DatiCILATE.ascx`
