---
title: Errori SCIA Alternativa al Permesso di Costruire - Regione Liguria
parent: Errori di validazione
nav_order: 57
description: Errori di validazione specifici per la SCIA Alternativa al Permesso di Costruire - Regione Liguria (art. 23 D.P.R. 380/2001, L.R. 16/2008, L.R. 20/2020)
keywords: [SCIA alternativa permesso costruire, SCIA alt PdC, SCIA Unica, SCIA Condizionata, Liguria, art. 23 DPR 380, L.R. 16/2008, L.R. 20/2020, lettera incarico progettista, qualificazione intervento, regolarità urbanistica, contributo costruzione, sicurezza lavoro]
IDRegione: 3
IDTipoPratica: 261
Fonte: Manuale
---

# Errori di validazione - SCIA Alternativa al Permesso di Costruire
## Regione Liguria

Guida completa agli errori specifici per la **Segnalazione Certificata di Inizio Attività Alternativa al Permesso di Costruire** ai sensi dell'art. 23 del D.P.R. 6 giugno 2001, n. 380, della L.R. 6 giugno 2008, n. 16 e della L.R. 27 luglio 2020, n. 20 — Regione Liguria.

{: .note }
> La SCIA alt PdC Liguria condivide con il [PdC Nazionale](errori-validazione-pdc-9915.html) la struttura della sezione "Regolarità urbanistica e precedenti edilizi" (identiche logiche di validazione con checkbox 1-13, sotto-checkbox 9 e stato attuale 6_1/6_2) ma ha alcune differenze importanti. La sezione **"Tecnici incaricati"** ha una particolarità ligure specifica: ai sensi della L.R. 20/2020 è obbligatoria la **data della lettera di incarico del progettista** (`txtDataIncaricoProg`), sempre verificata nel formato GG/MM/AAAA, indipendentemente dal radio tecnici selezionato. Se si sceglie h_1 ("altri tecnici già incaricati"), serve anche la **data della lettera di incarico degli altri tecnici** (`txtDataIncaricoAltri`). La qualificazione dell'intervento non ha l'opzione "nuova costruzione" (g_7 assente). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Presentazione SCIA Alternativa al PdC](#2-presentazione-scia-alternativa-al-pdc)
3. [Qualificazione dell'intervento](#3-qualificazione-dellintervento)
4. [Descrizione dell'intervento](#4-descrizione-dellintervento)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Opere su parti comuni o modifiche esterne](#6-opere-su-parti-comuni-o-modifiche-esterne)
7. [Regolarità urbanistica e precedenti edilizi](#7-regolarità-urbanistica-e-precedenti-edilizi)
8. [Calcolo del contributo di costruzione](#8-calcolo-del-contributo-di-costruzione)
9. [Tecnici incaricati (L.R. 20/2020)](#9-tecnici-incaricati-lr-202020)
10. [Impresa esecutrice dei lavori](#10-impresa-esecutrice-dei-lavori)
11. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#11-sicurezza-sul-lavoro-dlgs-812008)
12. [Tecnici e imprese nei soggetti coinvolti](#12-tecnici-e-imprese-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi"

{: .note }
> Il menu `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) è presente ma **non validato**. Non genera errori se lasciato sull'opzione vuota.

---

## 2. Presentazione SCIA Alternativa al PdC

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della denuncia di inizio attività'.

**Dove si trova**: Sezione "Presentazione della SCIA Alternativa al Permesso di Costruire / SCIA Unica / SCIA Condizionata" → 3 radio button

**Causa**: Nessuno dei 3 radio button `$PresSCIAaltPDC` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **b_1** — "**SCIA Alternativa al Permesso di Costruire**: Il titolare dichiara che i lavori avranno inizio non prima di 30 giorni dalla data di presentazione della segnalazione"
- ⚪ **b_2** — "**SCIA Alternativa al Permesso di Costruire più altre segnalazioni o comunicazioni (SCIA Unica)**: contestualmente alla SCIA le altre segnalazioni [...] i lavori avranno inizio non prima di 30 giorni"
- ⚪ **b_3** — "**SCIA Alternativa al Permesso di Costruire più domanda per il rilascio di atti di assenso (SCIA Condizionata)**: contestualmente alla SCIA la richiesta di acquisizione degli atti di assenso [...]"

---

## 3. Qualificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → radio button del gruppo `$TipoIntervento`

**Causa**: Il radio button della qualificazione non risulta selezionato.

**Soluzione**: Seleziona il radio button **c_1** — "interventi per i quali è possibile presentare la SCIA alternativa al permesso di costruire (individuati dall'art. 23 del d.P.R. n. 380/2001 ed elencati nella Sezione II-Edilizia della Tabella A del d.lgs. n. 222/2016 o altri interventi individuati dalla legislazione regionale)".

{: .note }
> Il radio button c_1 è l'**unica opzione disponibile** ed è preselezionato con `Checked="True"` nel modulo. In circostanze normali non dovrebbe mai generare questo errore. Se compare, potrebbe indicare un problema tecnico con il caricamento del modulo — ricaricare la pagina e verificare che c_1 risulti selezionato.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Interventi per i quali è possibile presentare la SCIA alternativa al permesso di costruire'

**Causa**: Il radio c_1 è selezionato ma non è stato specificato il sotto-tipo di intervento nel gruppo `$TipoIntSpec1`.

**Soluzione**: Seleziona **uno dei cinque radio button** del sotto-gruppo:
- ⚪ **c_1_1** — "**non comporta** mutamento di destinazione d'uso di una singola unità immobiliare o di un intero immobile"
- ⚪ **c_1_2** — "**comporta mutamento di destinazione d'uso di una singola U.I. all'interno della stessa categoria funzionale**"
- ⚪ **c_1_3** — "**comporta mutamento di destinazione d'uso di una singola U.I.** [...] in immobili nelle zone A), B) e C) del d.m. 1444/1968, **tra categorie funzionali di cui all'art. 23 ter c. 1, lett. a), a-bis), b) e c)**"
- ⚪ **c_1_5** — "**comporta mutamento di destinazione d'uso di una singola U.I. all'interno delle categorie funzionali ex art. 13 l.r. 16 del 2008**" *(opzione specifica Liguria)*
- ⚪ **c_1_4** — "**comporta mutamento di destinazione d'uso di un intero immobile all'interno della stessa categoria funzionale** nelle ipotesi di cui all'art. 23-ter, c. 3 e art. 13 della l.r. 16 del 2008"

{: .note }
> A differenza del PdC Nazionale che ha 4 sotto-opzioni, la SCIA alt PdC Liguria ha **5 sotto-opzioni** — la c_1_5 è specifica per la legislazione regionale ligure (mutamento d'uso entro categorie funzionali ex art. 13 L.R. 16/2008). L'opzione c_1_1 ("non comporta mutamento d'uso") è quella più comune per gli interventi edilizi ordinari.

---

## 4. Descrizione dell'intervento

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → campo multiriga `txtDescrIntervento` "Descrizione sintetica dell'intervento" (max 300 caratteri)

**Causa**: Il campo descrizione è vuoto. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice.

**Soluzione**: Inserisci la descrizione sintetica delle opere nel campo multiriga (max **300 caratteri**).

---

## 5. Localizzazione dell'intervento

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

{: .note }
> Il campo "Coordinate" (`txtCoordinate`) è presente ma non validato.

---

## 6. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Nessun radio button `$Opere` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **e_1** — "non riguardano parti comuni"
- ⚪ **e_2** — "riguardano le parti comuni di un fabbricato condominiale" (l'amministratore deve disporre della delibera assembleare)
- ⚪ **e_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ⚪ **e_4** — "riguardano parti di proprietà comune ma non necessitano di assenso (art. 1102 c.c.)"

---

## 7. Regolarità urbanistica e precedenti edilizi

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Dove si trova**: Sezione "Regolarità urbanistica e precedenti edilizi" → 5 radio button `$StatoAttualeImm`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei cinque radio button**:
- ⚪ **g_1** — "che l'immobile/U.I. è stato oggetto del/i seguente/i titolo/i o pratica/che edilizie" → spunta almeno una delle 13 checkbox con n. e data; poi spunta chk 6_1 o 6_2
- ⚪ **g_2** — "si tratta di immobile realizzato in un'epoca in cui non era obbligatorio un titolo abilitativo" → almeno una delle 2 checkbox; se 2_1: n. + data accatastamento
- ⚪ **g_3** — "non sono disponibili copia o estremi del titolo ma sussiste principio di prova documentale" → almeno una delle 2 checkbox; se 3_1: n. + data
- ⚪ **g_4** — "sono state irrogate le seguenti sanzioni pecuniarie (artt. 33, 34, 37, 38)" → almeno una delle 2 checkbox; se 4_2: importo + date pagamento e protocollo
- ⚪ **g_5** — "è stato oggetto della/e dichiarazione/i di tolleranza costruttiva (art. 34-bis o 34-ter, c. 4)" → almeno una delle 2 checkbox con n. e data ciascuna

{: .note }
> A differenza del [PdC Nazionale](errori-validazione-pdc-9915.html), la SCIA alt PdC Liguria **non ha l'opzione g_7** ("nuova costruzione su area libera"). La regolarità urbanistica deve quindi sempre riferirsi a interventi su immobili esistenti. Le checkbox 6_1/6_2 ("stato attuale immobile") sono comunque sempre obbligatorie.

La logica di validazione delle opzioni g_1..g_5 e delle relative sotto-selezioni è **identica** a quella del PdC Nazionale. Per i dettagli di ogni errore (numeri pratica, date, checkbox 9 sanatoria, checkbox 10-13 "altro", accatastamento, sanzioni pecuniarie, tolleranze) consulta la sezione corrispondente in [Errori PdC Nazionale](errori-validazione-pdc-9915.html#7-regolarità-urbanistica-e-precedenti-edilizi).

---

### ATTENZIONE! Indicare almeno uno stato attuale dell'immobile.

**Causa**: Nessuna delle 2 checkbox dello stato attuale (6_1/6_2) è spuntata. Questo controllo è sempre eseguito indipendentemente dall'opzione g scelta.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm6_1** — "pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"
- ☐ **chkStatoAttualeImm6_2** — "conforme alla documentazione [...] unitamente alla/e dichiarazione/i di tolleranza esecutive di cui alla relazione tecnica di asseverazione, quadro 'Dichiarazione di tolleranze'"

{: .warning }
> Le checkbox 6_1/6_2 sono **sempre obbligatorie** per qualsiasi opzione di regolarità urbanistica (g_1..g_5). Non dimenticarle dopo aver compilato le sezioni precedenti.

---

## 8. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Nessun radio button `$Intervento` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_1** — "è a titolo gratuito, ai sensi della seguente normativa ___" → inserisci la normativa nel campo `txtGratuitog1_2`
- ⚪ **g_2** — "è a titolo oneroso (l.r. 16/2008, art. 38)" → nessun campo strettamente obbligatorio dal validatore; compilare le checkbox di calcolo e pagamento

---

### ATTENZIONE ! Campo obbligatorio non inserito. (contributo gratuito)

**Causa**: Hai selezionato `rdbInterventog_1` (gratuito) ma `txtGratuitog1_2` è vuoto.

**Soluzione**: Inserisci la normativa di riferimento per la gratuità del contributo di costruzione (es. `art. 17 comma 3 lett. a) D.P.R. 380/2001`).

---

## 9. Tecnici incaricati (L.R. 20/2020)

Questa sezione ha una struttura specifica della Liguria, diversa dal PdC Nazionale, prevista dalla L.R. 27 luglio 2020, n. 20 che impone la documentazione della lettera di affidamento.

---

### ATTENZIONE ! Campo obbligatorio 'Data incarico progettista' non inserito.

**Dove si trova**: Sezione "Tecnici incaricati" → campo `txtDataIncaricoProg` nel testo "di aver incaricato, mediante lettera di affidamento sottoscritta in data ___ ed allegata alla presente istanza ai sensi della l.r. 27 luglio 2020, n. 20, in qualità di progettista"

**Causa**: Il campo della data della lettera di incarico del progettista è vuoto.

**Soluzione**: Inserisci la data in cui è stata sottoscritta la lettera di affidamento al progettista, nel formato **GG/MM/AAAA**.

{: .note }
> Questo campo è **sempre obbligatorio** per la SCIA alt PdC Liguria, indipendentemente dal radio `$Tecnici` selezionato. La L.R. 20/2020 richiede che la lettera di incarico al progettista sia allegata all'istanza e che la sua data sia indicata nel modulo.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data incarico progettista)

**Causa**: La data della lettera di incarico del progettista non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Causa**: Nessun radio button `$Tecnici` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **h_1** — "di aver incaricato, **mediante lettera di affidamento sottoscritta in data ___ ed allegata alla presente istanza** ai sensi della l.r. 27 luglio 2020, n. 20, in qualità di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'Soggetti coinvolti'" → inserisci la data della lettera di incarico degli altri tecnici e aggiungi almeno un tecnico
- ⚪ **h_2** — "che il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"

---

### ATTENZIONE ! Campo obbligatorio 'Data incarico' non inserito.

**Causa**: Hai selezionato `rdbTecnicih_1` ma il campo `txtDataIncaricoAltri` (data lettera incarico altri tecnici) è vuoto.

**Soluzione**: Inserisci la data della lettera di affidamento agli altri tecnici nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data incarico altri tecnici)

**Causa**: La data della lettera di incarico degli altri tecnici non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 10. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **i_1** — "che i lavori saranno eseguiti/sono stati eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'" → deve essere presente almeno un'impresa nei soggetti
- ⚪ **i_2** — "che l'impresa esecutrice/imprese esecutrici dei lavori sarà/saranno individuata/e prima dell'inizio dei lavori"
- ⚪ **i_3** — "che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori sono eseguiti in prima persona, senza alcun affidamento a ditte esterne"

{: .note }
> La SCIA alt PdC Liguria ha **3 opzioni impresa** (contro le 4 del PdC Nazionale — manca l'i_4 "lavori non eseguiti da impresa per pratiche in sanatoria", che non è applicabile alla SCIA alt PdC).

---

## 11. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessun radio button `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **l_1** — "non ricade nell'ambito di applicazione [...] (d.lgs. n. 81/2008)"
- ⚪ **l_2** — "ricade nell'ambito di applicazione [...] e pertanto" → seleziona documentazione imprese e, se applicabile, notifica
- ⚪ **l_3** — "ricade [...] ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'. / 'Notifica preliminare'. / 'Comunicazione/Estremi Notifica'.

Questi errori si attivano con la stessa logica a 4 livelli del PdC Nazionale: l_2 → `$ImpEs` → se l_2_2: `$Notifica` → se notifica_2_2_2: `$Allega`. Per i dettagli consulta la sezione corrispondente in [Errori PdC Nazionale](errori-validazione-pdc-9915.html#11-sicurezza-sul-lavoro-dlgs-812008).

---

## 12. Tecnici e imprese nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Hai selezionato `rdbTecnicih_1` ("altri tecnici già incaricati") ma nessun tecnico è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico.

{: .note }
> Il controllo tecnici nei soggetti **si attiva solo se h_1 è selezionato**. Se si sceglie h_2 ("tecnici individuati prima dell'inizio lavori"), non è richiesta la presenza di tecnici nei soggetti coinvolti al momento della presentazione.

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato `rdbImpresai_1` ma nessuna impresa è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice, oppure seleziona l'opzione i_2 o i_3.

---

## Consigli pratici — SCIA alt PdC Liguria

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona il **tipo di presentazione** (SCIA / SCIA Unica / SCIA Condizionata)
- [ ] Seleziona la **qualificazione c_1** e il **sotto-tipo** (c_1_1..c_1_5)
- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona le **opere su parti comuni** (e_1..e_4)
- [ ] Seleziona la **regolarità urbanistica** (g_1..g_5) e compila le sotto-selezioni; spunta sempre **chk 6_1 o 6_2**
- [ ] Seleziona il **contributo di costruzione** (gratuito con normativa / oneroso)
- [ ] Inserisci la **data incarico progettista** (sempre, GG/MM/AAAA — L.R. 20/2020)
- [ ] Seleziona il **radio tecnici** (h_1/h_2); se h_1: inserisci **data incarico altri tecnici** (GG/MM/AAAA) e aggiungi almeno un tecnico nei soggetti
- [ ] Seleziona il **radio impresa** (i_1/i_2/i_3); se i_1: aggiungi almeno un'impresa nei soggetti
- [ ] Seleziona la **sicurezza** (l_1/l_2/l_3); se l_2: compila i 4 livelli

### Differenze rispetto al PdC Nazionale ⚠️

Rispetto al PdC Nazionale, la SCIA alt PdC Liguria ha: sezione "Presentazione" obbligatoria (3 opzioni SCIA/SCIA Unica/Condizionata); qualificazione con 5 sotto-opzioni (inclusa c_1_5 specifica Liguria); assenza di g_7 (nuova costruzione); sezione tecnici con data lettera incarico progettista **sempre obbligatoria** (L.R. 20/2020); se h_1: data lettera incarico altri tecnici; 3 opzioni impresa (no i_4 sanatoria); assenza della sanatoria (checkbox `chkSanatoriax1_0`); assenza allacciamento fognatura; impresa verificata nei soggetti (come il PdC Nazionale per i_1).

### Errori frequenti 🔍

1. **Data incarico progettista mancante o formato errato** → è il primo errore della sezione tecnici; sempre richiesta ai sensi L.R. 20/2020; inserire la data della lettera di affidamento in GG/MM/AAAA
2. **h_1 selezionato senza data incarico altri tecnici** → dopo `txtDataIncaricoProg` (sempre obbligatoria), se si sceglie h_1 bisogna inserire anche `txtDataIncaricoAltri`
3. **Checkbox 6_1/6_2 dimenticate** → come nel PdC Nazionale, obbligatorie per qualsiasi opzione g
4. **Qualificazione c_1 senza sotto-tipo** — il radio c_1 è preselezionato ma il sotto-tipo `$TipoIntSpec1` non lo è; bisogna selezionare una delle 5 opzioni
5. **Contributo gratuito senza normativa** → come nel PdC Nazionale, `txtGratuitog1_2` obbligatorio se si sceglie gratuito

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Per errori della sezione Regolarità urbanistica, vedi [Errori PdC Nazionale](errori-validazione-pdc-9915.html#7-regolarità-urbanistica-e-precedenti-edilizi)
3. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiSCIAaltPDCLiguria e DatiSCIAaltPDCLiguria.ascx
