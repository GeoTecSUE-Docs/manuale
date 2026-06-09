---
title: Errori SCIA Alternativa al Permesso di Costruire - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 61
description: Errori di validazione specifici per la SCIA Alternativa al Permesso di Costruire Nazionale - Tutte le regioni (art. 23 D.P.R. 380/2001, d.lgs. 222/2016)
keywords: [SCIA alternativa permesso costruire, SCIA alt PdC, nazionale, tutte le regioni, art. 23 DPR 380, SCIA Unica, SCIA Condizionata, qualificazione intervento, regolarità urbanistica, contributo costruzione, sicurezza lavoro, progettista, tecnici]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 126 }  # Valle d'Aosta - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 6, Prat: 626 } # Veneto - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 8, Prat: 826 } # Emilia-Romagna - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 12, Prat: 1226 } # Lazio - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 13, Prat: 1326 } # Abruzzo - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 15, Prat: 1526 } # Campania - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 16, Prat: 1626 } # Basilicata - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 17, Prat: 1726 } # Puglia - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 18, Prat: 1826 } # Calabria - S.C.I.A. Alternativa al P.d.C.
  - { Reg: 19, Prat: 1926 } # Sicilia - S.C.I.A. Alternativa al P.d.C.
Fonte: Manuale
---

# Errori di validazione - SCIA Alternativa al Permesso di Costruire
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per la **Segnalazione Certificata di Inizio Attività Alternativa al Permesso di Costruire (SCIA alt PdC) Nazionale** ai sensi dell'art. 23 del D.P.R. 6 giugno 2001, n. 380 e della Sezione II-Edilizia della Tabella A del D.Lgs. 25 novembre 2016, n. 222.

{: .note }
> La SCIA alt PdC Nazionale è strutturalmente molto simile alla [SCIA alt PdC Liguria](errori-scia-alt-pdc-liguria.html) con due differenze principali: la qualificazione ha **4 sotto-opzioni** invece di 5 (manca la c_1_5 specifica della L.R. 16/2008 ligure) e la sezione tecnici **non richiede la data della lettera di incarico** (assenza della L.R. 20/2020). La sezione regolarità urbanistica (g_1..g_5, con checkbox 6_1/6_2 sempre obbligatorie) e la sezione sicurezza (4 livelli completi) sono identiche alla versione Liguria. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

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
9. [Tecnici incaricati](#9-tecnici-incaricati)
10. [Impresa esecutrice dei lavori](#10-impresa-esecutrice-dei-lavori)
11. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#11-sicurezza-sul-lavoro-dlgs-812008)
12. [Tecnici e imprese nei soggetti coinvolti](#12-tecnici-e-imprese-nei-soggetti-coinvolti)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **a_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi titolari di altri diritti reali o obbligatori"

{: .note }
> Il menu `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) è presente ma **non validato**.

---

## 2. Presentazione SCIA Alternativa al PdC

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della denuncia di inizio attività'.

**Dove si trova**: Sezione "Presentazione della SCIA Alternativa al Permesso di Costruire / SCIA Unica / SCIA Condizionata" → 3 radio button `$PresSCIAaltPDC`

**Causa**: Nessuno dei 3 radio button è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **b_1** — "**SCIA Alternativa al Permesso di Costruire**: Il titolare dichiara che i lavori avranno inizio non prima di 30 giorni dalla data di presentazione della segnalazione"
- ⚪ **b_2** — "**SCIA Unica**: contestualmente alla SCIA le altre segnalazioni o comunicazioni [...] i lavori avranno inizio non prima di 30 giorni"
- ⚪ **b_3** — "**SCIA Condizionata** da atti di assenso: [...] l'intervento può essere iniziato dopo la comunicazione da parte del Comune dell'avvenuto rilascio degli atti di assenso"

---

## 3. Qualificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → radio `$TipoIntervento`

**Causa**: Il radio c_1 non risulta selezionato.

**Soluzione**: Seleziona il radio button **c_1** — "interventi per i quali è possibile presentare la SCIA alternativa al permesso di costruire (individuati dall'art. 23 del d.P.R. n. 380/2001 ed elencati nella Sezione II-Edilizia della Tabella A del d.lgs. n. 222/2016 o altri interventi individuati dalla legislazione regionale)".

{: .note }
> Il radio c_1 è preselezionato con `Checked="True"` nel modulo. Se compare questo errore, potrebbe indicare un problema tecnico con il caricamento del modulo — ricaricare la pagina.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Interventi per i quali è possibile presentare la SCIA alternativa al permesso di costruire'

**Causa**: Il radio c_1 è selezionato ma non è stato specificato il sotto-tipo `$TipoIntSpec1`.

**Soluzione**: Seleziona **uno dei quattro radio button** del sotto-gruppo:
- ⚪ **c_1_1** — "**non comporta** mutamento di destinazione d'uso di una singola U.I. o di un intero immobile"
- ⚪ **c_1_2** — "**comporta mutamento di destinazione d'uso di una singola U.I. all'interno della stessa categoria funzionale**"
- ⚪ **c_1_3** — "**comporta mutamento di destinazione d'uso di una singola U.I.** [...] in immobili nelle zone A), B) e C) del d.m. 1444/1968, **tra categorie funzionali di cui all'art. 23 ter c. 1, lett. a), a-bis), b) e c)**"
- ⚪ **c_1_4** — "**comporta mutamento di destinazione d'uso di un intero immobile all'interno della stessa categoria funzionale** nelle ipotesi di cui all'art. 23-ter, comma 3"

{: .note }
> La versione Nazionale ha **4 sotto-opzioni** invece delle 5 della SCIA alt PdC Liguria — manca la c_1_5 specifica per la legislazione regionale ligure (art. 13 L.R. 16/2008).

---

## 4. Descrizione dell'intervento

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → campo multiriga `txtDescrIntervento` "Descrizione sintetica dell'intervento" (max 300 caratteri)

**Causa**: Il campo è vuoto. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice.

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
- ⚪ **e_2** — "riguardano le parti comuni di un fabbricato condominiale" (richiede delibera assembleare)
- ⚪ **e_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ⚪ **e_4** — "riguardano parti comuni ma non necessitano di assenso (art. 1102 c.c.)"

---

## 7. Regolarità urbanistica e precedenti edilizi

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Dove si trova**: Sezione "Regolarità urbanistica e precedenti edilizi" → 5 radio button `$StatoAttualeImm`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei cinque radio button**:
- ⚪ **g_1** — "che l'immobile/U.I. è stato oggetto del/i seguente/i titolo/i o pratica/che edilizie" → spunta almeno una delle 13 checkbox con n. e data; poi spunta chk 6_1 o 6_2
- ⚪ **g_2** — "si tratta di immobile realizzato in un'epoca in cui non era obbligatorio un titolo abilitativo" → almeno una delle 2 checkbox; se 2_1: n. + data
- ⚪ **g_3** — "non sono disponibili copia o estremi del titolo ma sussiste principio di prova documentale" → almeno una delle 2 checkbox; se 3_1: n. + data
- ⚪ **g_4** — "sono state irrogate le seguenti sanzioni pecuniarie (artt. 33, 34, 37, 38)" → almeno una delle 2 checkbox; se 4_2: importo + date pagamento e protocollo
- ⚪ **g_5** — "è stato oggetto della/e dichiarazione/i di tolleranza costruttiva (art. 34-bis o 34-ter, c. 4)" → almeno una delle 2 checkbox con n. e data ciascuna

{: .note }
> Come la SCIA alt PdC Liguria, la versione Nazionale **non ha l'opzione g_7** ("nuova costruzione su area libera") presente nel PdC Nazionale. La sezione si applica sempre a interventi su immobili esistenti. La logica di validazione delle sotto-selezioni è identica a quella del PdC Nazionale e della SCIA alt PdC Liguria. Per i dettagli di ogni singolo errore (checkbox 1-13, sotto-checkbox 9, checkbox 10-13 "altro", accatastamento, sanzioni, tolleranze) vedi [Errori PdC Nazionale — sezione 7](errori-pdc-nazionale.html#7-regolarità-urbanistica-e-precedenti-edilizi).

---

### ATTENZIONE! Indicare almeno uno stato attuale dell'immobile.

**Causa**: Nessuna delle 2 checkbox 6_1/6_2 è spuntata. Sempre obbligatorie indipendentemente dall'opzione g scelta.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm6_1** — "pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"
- ☐ **chkStatoAttualeImm6_2** — "conforme alla documentazione [...] unitamente alla/e dichiarazione/i di tolleranza esecutive di cui alla relazione tecnica di asseverazione, quadro 'Dichiarazione di tolleranze'"

{: .warning }
> Le checkbox 6_1/6_2 sono **sempre obbligatorie** per qualsiasi opzione g_1..g_5. Non dimenticarle dopo aver compilato le sezioni precedenti.

---

## 8. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Nessun radio button `$Intervento` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_1** — "è a titolo gratuito, ai sensi della seguente normativa ___" → inserisci la normativa nel campo `txtGratuitog1_2`
- ⚪ **g_2** — "è a titolo oneroso e pertanto" → nessun campo strettamente obbligatorio dal validatore

---

### ATTENZIONE ! Campo obbligatorio non inserito. (contributo gratuito)

**Causa**: Hai selezionato `rdbInterventog_1` (gratuito) ma `txtGratuitog1_2` è vuoto.

**Soluzione**: Inserisci nel campo testo la normativa di riferimento (es. `art. 17 comma 3 lett. a) D.P.R. 380/2001`).

---

## 9. Tecnici incaricati

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Dove si trova**: Sezione "Tecnici incaricati" → 2 radio button `$Tecnici`

**Causa**: Nessun radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **h_1** — "di aver incaricato, in qualità di direttori dei lavori, e di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'SOGGETTI COINVOLTI'" → deve essere presente almeno un tecnico nei soggetti coinvolti
- ⚪ **h_2** — "che il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"

{: .note }
> A differenza della [SCIA alt PdC Liguria](errori-scia-alt-pdc-liguria.html#9-tecnici-incaricati-lr-202020), la versione Nazionale **non richiede la data della lettera di incarico** del progettista né degli altri tecnici — la L.R. 27 luglio 2020, n. 20 si applica solo alla Liguria. Il modulo prevede il progettista come presupposto fisso ("di aver incaricato, in qualità di progettista/i, il tecnico/i indicato/i alla sezione 2") senza campo data associato.

---

## 10. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **i_1** — "che i lavori saranno eseguiti/sono stati eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'" → deve essere presente almeno un'impresa
- ⚪ **i_2** — "che l'impresa esecutrice dei lavori sarà individuata prima dell'inizio dei lavori"
- ⚪ **i_3** — "che, in quanto opere di modesta entità [...] i lavori sono eseguiti in prima persona, senza alcun affidamento a ditte esterne"

---

## 11. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessun radio button `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **l_1** — "non ricade nell'ambito di applicazione [...] (d.lgs. n. 81/2008)"
- ⚪ **l_2** — "ricade [...] e pertanto" → compila i livelli annidati
- ⚪ **l_3** — "ricade [...] ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato l_2 ma nessuno dei 2 radio button `$ImpEs` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **l_2_1** — "entità presunta del cantiere inferiore a 200 uomini-giorno e lavori senza rischi particolari (Allegato XI)"
- ⚪ **l_2_2** — "entità presunta del cantiere pari o superiore a 200 uomini-giorno o lavori con rischi particolari" → seleziona il radio notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato l_2_2 ma nessuno dei 2 radio button `$Notifica` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **l_2_2_1** — "l'intervento non è soggetto all'invio della notifica"
- ⚪ **l_2_2_2** — "l'intervento è soggetto all'invio della notifica" → seleziona il radio `$Allega`

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione/Estremi Notifica'.

**Causa**: Hai selezionato l_2_2_2 ma nessuno dei 2 radio button `$Allega` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **l_2_2_2_1** — "allega alla presente segnalazione la notifica, il cui contenuto sarà riprodotto su apposita tabella esposta in cantiere"
- ⚪ **l_2_2_2_2** — "invierà la notifica prima dell'inizio dei lavori"

{: .note }
> La SCIA alt PdC Nazionale ha il **4° livello sicurezza** (`$Allega`) a differenza della [CIL Liguria](errori-cil-liguria.html) che si ferma al 3° livello. La struttura è identica a quella della [SCIA alt PdC Liguria](errori-scia-alt-pdc-liguria.html).

---

## 12. Tecnici e imprese nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Hai selezionato `rdbTecnicih_1` ma nessun tecnico è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico con qualsiasi ruolo.

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato `rdbImpresai_1` ma nessuna impresa è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice, oppure seleziona i_2 o i_3.

---

## Consigli pratici — SCIA alt PdC Nazionale

### Prima di validare ✅

- [ ] Seleziona la **titolarità** (a_1/a_2)
- [ ] Seleziona il **tipo di presentazione** (SCIA / SCIA Unica / SCIA Condizionata)
- [ ] Seleziona la **qualificazione c_1** e il **sotto-tipo** (c_1_1..c_1_4)
- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona le **opere su parti comuni** (e_1..e_4)
- [ ] Seleziona la **regolarità urbanistica** (g_1..g_5) con sotto-selezioni; spunta **chk 6_1 o 6_2**
- [ ] Seleziona il **contributo di costruzione** (gratuito con normativa / oneroso)
- [ ] Seleziona il **radio tecnici** (h_1/h_2); se h_1: aggiungi almeno un tecnico nei soggetti
- [ ] Seleziona il **radio impresa** (i_1/i_2/i_3); se i_1: aggiungi almeno un'impresa
- [ ] Seleziona la **sicurezza** (l_1/l_2/l_3); se l_2: compila i 4 livelli

### Differenze rispetto alle versioni regionali ⚠️

Rispetto alla **SCIA alt PdC Liguria**: senza data lettera incarico progettista (assenza L.R. 20/2020); 4 sotto-opzioni qualificazione (no c_1_5).

Rispetto al **PdC Nazionale**: senza sezione Sanatoria; senza g_7 (nuova costruzione); 3 opzioni impresa (no i_4 sanatoria); sezione tecnici con radio h_1/h_2 (senza date incarico); nessuna verifica ruolo specifico (PR/RI) nei soggetti — basta la presenza di almeno un tecnico se h_1.

### Campi presenti ma non validati ℹ️

`cmbTitoloSuImm`, `txtCoordinate`, `txtNote`, `txtData`, `txtLuogo`, privacy — tutti facoltativi.

### Errori frequenti 🔍

1. **Checkbox 6_1/6_2 dimenticate** → obbligatorie per qualsiasi opzione g_1..g_5; verificarle sempre prima di validare
2. **Qualificazione c_1 senza sotto-tipo** → il radio c_1 è preselezionato ma il sotto-tipo non lo è; selezionare c_1_1..c_1_4
3. **Contributo gratuito senza normativa** → `txtGratuitog1_2` obbligatorio se si sceglie gratuito
4. **Checkbox g_1 senza sottoselezioni** → per le checkbox 1-8 servono n. e data; la checkbox 9 richiede almeno una sotto-checkbox con n. e data; le checkbox 10-13 richiedono tipo + n. + data

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Per errori della sezione Regolarità urbanistica, vedi [Errori PdC Nazionale](errori-pdc-nazionale.html#7-regolarità-urbanistica-e-precedenti-edilizi)
3. Vedi anche [SCIA alt PdC Liguria](errori-scia-alt-pdc-liguria.html) per confronto
4. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
5. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiSCIAaltPDCNazionale e DatiSCIAaltPDCNaz.ascx
