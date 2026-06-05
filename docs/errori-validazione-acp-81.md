---
title: Errori Accertamento Compatibilità Paesaggistica - Regione Liguria
parent: Errori di validazione
nav_order: 54
description: Errori di validazione specifici per l'Accertamento di Compatibilità Paesaggistica - Regione Liguria (art. 167 D.Lgs. 42/2004, art. 32 L. 47/1985, art. 36-bis D.P.R. 380/2001)
keywords: [accertamento compatibilità paesaggistica, ACP, sanatoria paesaggistica, Liguria, art. 167 D.Lgs. 42/2004, art. 181, art. 32 L. 47/1985, art. 36-bis DPR 380, condono paesaggistico, natura vincolo, art. 136, art. 142, titoli abitativi]
IDRegione: 3
IDTipoPratica: 81
Fonte: Manuale
---

# Errori di validazione - Accertamento di Compatibilità Paesaggistica
## Regione Liguria

Guida completa agli errori specifici per l'**Accertamento di Compatibilità Paesaggistica (ACP)** ai sensi dell'art. 167 del D.Lgs. 22 gennaio 2004, n. 42, dell'art. 32 della L. 28 febbraio 1985, n. 47 e dell'art. 36-bis del D.P.R. 6 giugno 2001, n. 380 — Regione Liguria.

{: .note }
> L'ACP Liguria è una pratica di accertamento postuma per opere realizzate in assenza o difformità dall'autorizzazione paesaggistica. Le caratteristiche principali sono: la **descrizione** viene validata prima di tutto; la **qualificazione** ha 3 percorsi normativi con sotto-selezioni diverse; la sezione **"Natura del vincolo"** ha 4 opzioni con campi condizionali distinti; la sezione **"Titoli abitativi"** ha 14 checkbox con almeno una obbligatoria e un loop di verifica campi; la sezione **"Diritti di terzi"** ha un comportamento particolare: il campo `txtAltro10_2_4` viene verificato come obbligatorio per qualsiasi sotto-opzione di assenso (non solo per "altro") — si veda la nota alla sezione 9. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Descrizione sintetica dell'intervento](#1-descrizione-sintetica-dellintervento)
2. [Qualificazione dell'intervento](#2-qualificazione-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Natura del vincolo](#4-natura-del-vincolo)
5. [Titoli abitativi](#5-titoli-abitativi)
6. [Epoca intervento](#6-epoca-intervento)
7. [Opere su parti comuni o modifiche esterne](#7-opere-su-parti-comuni-o-modifiche-esterne)
8. [Diritti di terzi](#8-diritti-di-terzi)
9. [Tecnici nei soggetti coinvolti](#9-tecnici-nei-soggetti-coinvolti)

---

## 1. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Prima sezione del modulo → campo multiriga `txtDescrACP` sotto "per l'avvenuta esecuzione dei seguenti lavori" (max 300 caratteri)

**Causa**: Il campo è vuoto. La descrizione viene validata **prima** di qualsiasi altra sezione.

**Soluzione**: Inserisci la descrizione sintetica delle opere eseguite nel campo multiriga (max **300 caratteri**).

---

## 2. Qualificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → 3 radio button principali sotto "CHIEDE l'accertamento della compatibilità paesaggistica"

**Causa**: Nessuna delle 3 opzioni è selezionata.

**Soluzione**: Seleziona **una delle tre opzioni** e compila le sotto-selezioni richieste:

- ⚪ **2_1** — "ai sensi dell'art. 167 comma 5 dell'art. 181 comma 1 quater D.Lgs. 22/01/2004 n. 42 (indicare il caso previsto dall'art. 167 comma 4)" → seleziona obbligatoriamente uno dei 5 radio button `$QualificazioneLav`
- ⚪ **2_2** — "ai sensi dell'art. 32 della L. 28/02/1985 n. 47 (indicare il riferimento normativo del Condono)" → seleziona obbligatoriamente uno dei 3 radio button `$QualificazioneArt`
- ⚪ **2_3** — "ai sensi del comma 4 dell'art. 36-bis del D.P.R. 6/06/2001 n. 380" → spunta almeno una delle 2 checkbox

---

### Opzione 2_1 — Art. 167/181 D.Lgs. 42/2004

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dei lavori'.

**Causa**: Hai selezionato la base normativa 2_1 ma non hai specificato la fattispecie dei lavori.

**Soluzione**: Seleziona **uno dei cinque radio button** del sotto-gruppo `$QualificazioneLav`:
- ⚪ "lavori, realizzati in assenza dall'autorizzazione paesaggistica, che non abbiano determinato creazione di superfici utili o volumi ovvero aumento di quelli legittimamente realizzati"
- ⚪ "lavori, realizzati in difformità dall'autorizzazione paesaggistica, che non abbiano determinato creazione di superfici utili o volumi ovvero aumento di quelli legittimamente realizzati"
- ⚪ "impiego di materiali in difformità dall'autorizzazione paesaggistica"
- ⚪ "lavori comunque configurabili quali interventi di manutenzione ordinaria ai sensi dell'art. 3 comma 1 lett. a del D.P.R. 6/06/2001 n. 380"
- ⚪ "lavori comunque configurabili quali interventi di manutenzione straordinaria ai sensi dell'art. 3 comma 1 lett. b del D.P.R. 6/06/2001 n. 380 ai sensi dell'art. 32 della L. 28/02/1985"

---

### Opzione 2_2 — Art. 32 L. 47/1985 (condono)

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Articoli'.

**Causa**: Hai selezionato la base normativa 2_2 ma non hai indicato a quale legge di condono si riferisce.

**Soluzione**: Seleziona **uno dei tre radio button** del sotto-gruppo `$QualificazioneArt`:
- ⚪ "L. 28/02/1985 n. 47"
- ⚪ "art. 39 L. 23/12/1994 n. 724"
- ⚪ "art. 32 L. 24/11/2003 n. 326"

---

### Opzione 2_3 — Art. 36-bis D.P.R. 380/2001

#### ATTENZIONE ! Non è stata selezionata nessuna voce per l'Accertamento di Conformità.

**Causa**: Hai selezionato la base normativa 2_3 ma non hai spuntato nessuna delle 2 checkbox.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkAumentoVolume** — "lavori che hanno determinato la creazione di superfici utili o volumi ovvero l'aumento di quelli legittimamente realizzati"
- ☐ **chkVincoloSucc** — "vincolo paesaggistico apposto in data successiva alla realizzazione dell'intervento"

Le due checkbox non sono mutuamente esclusive.

---

## 3. Localizzazione dell'intervento

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
> La sezione **Titolarità Intervento** contiene il menu `cmbTitoloSuImm` e i campi `txtNumAtto`, `txtDataAtto`, `txtNumRegistraz` — tutti presenti nel modulo ma **non validati** dal codice VB. Non generano errori se vuoti.

---

## 4. Natura del vincolo

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Natura del Vincolo'.

**Dove si trova**: Sezione "Natura del vincolo" → 4 radio button sotto "che gli immobili sopra individuati sono soggetti al vincolo di cui"

**Causa**: Nessuno dei 4 radio button del gruppo `$NaturaVincolo` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button** e compila gli eventuali campi aggiuntivi:
- ⚪ **5_1** — "all'art. 136 lett. ___ del D.Lgs. 22/01/2004 n. 42 'Immobili ed aree di notevole interesse pubblico'" → inserisci la lettera
- ⚪ **5_2** — "all'art. 142 lett. ___ del D.Lgs. 22/01/2004 n. 42 'Aree tutelate per legge'" → inserisci la lettera
- ⚪ **5_3** — "vincolo apposto con" → inserisci denominazione, G.U. e data
- ⚪ **5_4** — "altro" → inserisci la descrizione

---

### ATTENZIONE ! Specificare la lettera di riferimento per l'art. 136.

**Causa**: Hai selezionato 5_1 (art. 136) ma il campo lettera `txtLett5_1` è vuoto.

**Soluzione**: Inserisci la lettera del comma (es. `a`, `b`, `c`, `d`) nel piccolo campo testo affiancato ad "art. 136 lett. ___"

---

### ATTENZIONE ! Specificare la lettera di riferimento per l'art. 142.

**Causa**: Hai selezionato 5_2 (art. 142) ma il campo lettera `txtLett5_2` è vuoto.

**Soluzione**: Inserisci la lettera del comma corrispondente alla categoria di bene tutelato (es. `a` per fascia costiera, `b` per laghi, `c` per fiumi, ecc.) nel campo affiancato ad "art. 142 lett. ___"

---

### Opzione 5_3 — Vincolo apposto con atto

#### ATTENZIONE ! Specificare la denominazione del vincolo.

**Causa**: Hai selezionato 5_3 ma il campo `txtDenominazione` è vuoto.

**Soluzione**: Inserisci la denominazione del provvedimento con cui è stato apposto il vincolo.

---

#### ATTENZIONE ! Specificare il G.U. del vincolo.

**Causa**: Il campo `txtGU` (Gazzetta Ufficiale) è vuoto.

**Soluzione**: Inserisci il riferimento alla Gazzetta Ufficiale in cui è stato pubblicato il provvedimento (es. `G.U. n. 123 del 15/06/1985`).

---

#### ATTENZIONE ! Specificare la data del vincolo.

**Causa**: Il campo `txtData` (data del vincolo) è vuoto.

**Soluzione**: Inserisci la data del provvedimento.

{: .note }
> La data del vincolo apposto (opzione 5_3) viene verificata solo come "non vuoto" — **il formato GG/MM/AAAA non viene controllato**. Inserire il formato corretto è comunque buona prassi.

---

### ATTENZIONE ! Specificare la descrizione per 'Altro'. (natura vincolo)

**Causa**: Hai selezionato 5_4 ("altro") ma il campo `txtAltro5_4_1` è vuoto.

**Soluzione**: Inserisci la descrizione del tipo di vincolo non ricompreso nelle categorie precedenti nel campo testo affiancato.

---

## 5. Titoli abitativi

### ATTENZIONE ! Indicare almeno una tipologia di pratica.

**Dove si trova**: Sezione "Titoli Abitativi" → 14 checkbox sotto "che l'immobile in accertamento è stato oggetto dei seguenti titoli abilitativi"

**Causa**: Nessuna delle 14 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 14 checkbox che corrisponde al titolo con cui le opere erano state autorizzate (o avrebbero dovuto esserlo):

- ☐ **1** — PDC Permesso Di Costruire (art. 10 D.P.R. 06/06/2001 n. 380)
- ☐ **2** — DIA Denuncia Inizio Attività (art. 22 comma 3 D.P.R. 06/06/2001 n. 380)
- ☐ **3** — SCIA Segnalazione Certificata Inizio Attività (art. 22 commi 1 e 2 D.P.R. 06/06/2001 n. 380)
- ☐ **4** — CIL Comunicazione Inizio Lavori (art. 6 comma 1 D.P.R. 06/06/2001 n. 380)
- ☐ **5** — CIL Comunicazione Inizio Lavori (art. 6 comma 2 D.P.R. 06/06/2001 n. 380)
- ☐ **6** — Concessione edilizia
- ☐ **7** — Autorizzazione edilizia
- ☐ **8** — Licenza edilizia
- ☐ **9** — PDC Permesso Di Costruire (art. 36 D.P.R. 06/06/2001 n. 380)
- ☐ **10** — SCIA Segnalazione Certificata Inizio Attività (art. 37 D.P.R. 06/06/2001 n. 380)
- ☐ **11** — CIL Comunicazione Inizio Lavori (art. 6 comma 7 D.P.R. 06/06/2001 n. 380)
- ☐ **12** — Titolo unico (SUAP) (art. 7 D.P.R. 07/09/2010 n. 160)
- ☐ **13** — Comunicazione edilizia (art. 26 L. 28/02/1985 n. 47)
- ☐ **14** — Altro (con campo testo libero)

---

### ATTENZIONE ! Campo obbligatorio non inserito.

**Causa**: Hai spuntato una o più checkbox dei titoli abitativi ma un campo obbligatorio affiancato è rimasto vuoto.

**Soluzione**: Per ogni checkbox spuntata, verifica che i campi affiancati obbligatori siano compilati.

{: .note }
> Il validatore scorre tutti i TextBox figli del panel `pnlStatoAttualeImm` e verifica quelli con `CssClass = "CampoObbligatorio"`. Nell'implementazione attuale del modulo, i campi "Pratica n." (`txtNProt1_x`) e "del" (`txtDataProt1_x`) non hanno la classe `CampoObbligatorio` nel markup statico — vengono resi obbligatori dinamicamente via AJAX quando la checkbox corrispondente viene spuntata. Il messaggio "Campo obbligatorio non inserito" appare quindi per i campi che il sistema ha contrassegnato come obbligatori in seguito alla selezione delle checkbox.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data titolo abitativo)

**Causa**: Uno dei campi data dei titoli abitativi (`txtDataProt1_x`) contiene un valore ma non nel formato corretto.

**Soluzione**: Correggi la data nel formato **GG/MM/AAAA**.

{: .note }
> Tutti i campi data dei titoli abitativi (`txtDataProt1_1` .. `txtDataProt1_14`) vengono verificati nel formato se compilati, indipendentemente dall'obbligatorietà. Se lasciati vuoti non generano questo errore, ma possono generare "Campo obbligatorio non inserito" se il sistema li ha resi obbligatori tramite AJAX.

---

## 6. Epoca intervento

### ATTENZIONE ! Specificare la data di riferimento.

**Dove si trova**: Sezione "Epoca intervento" → campo `txtDataIntervento` sotto "Data realizzazione opere soggette all'accertamento di compatibilità paesaggistica"

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la data in cui le opere sono state realizzate nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data realizzazione opere)

**Causa**: La data inserita non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 7. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Dove si trova**: Sezione "Opere su parti comuni o modifiche esterne" → 4 radio button sotto "che le opere previste"

**Causa**: Nessuno dei 4 radio button del gruppo `$Opere` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **e_1** — "non riguardano parti comuni"
- ⚪ **e_2** — "riguardano le parti comuni di un fabbricato condominiale"
- ⚪ **e_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio, e dichiara che l'intervento è stato approvato dai comproprietari..."
- ⚪ **e_4** — "riguardano parti dell'edificio di proprietà comune ma non necessitano di assenso perché, secondo l'art. 1102 c.c., ..."

---

## 8. Diritti di terzi

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Diritti di Terzi'.

**Dove si trova**: Sezione "Diritti di terzi" → 2 radio button principali

**Causa**: Nessuno dei 2 radio button del gruppo `$Diritti` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **10_1** — "che l'intervento è conforme alle norme del Codice Civile e non lede alcun diritto di terzi" → nessun campo aggiuntivo
- ⚪ **10_2** — "che è stato ottenuto l'assenso del terzo contro interessato che si allega" → seleziona il tipo di assenso e compila il campo descrizione

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Assenso Diritti di Terzi'.

**Causa**: Hai selezionato 10_2 ("assenso del terzo") ma non hai indicato il tipo di assenso.

**Soluzione**: Seleziona **uno dei tre radio button** del sotto-gruppo `$DirittiAssenso`:
- ⚪ **10_2_1** — "assenso da parte del terzo per edificazione a confine o a distanza inferiore a quella prevista dalle normative di PRGC"
- ⚪ **10_2_2** — "assenso per nuove vedute o modifica di quelle esistenti"
- ⚪ **10_2_3** — "altro"

---

### ATTENZIONE ! Specificare la descrizione per 'Altro'. (diritti di terzi)

**Causa**: Hai selezionato 10_2 e hai scelto un tipo di assenso, ma il campo `txtAltro10_2_4` (descrizione) è vuoto.

**Soluzione**: Inserisci la descrizione nel campo testo `txtAltro10_2_4`.

{: .warning }
> **Comportamento inatteso**: il validatore verifica `txtAltro10_2_4` come obbligatorio per **qualsiasi** sotto-opzione di assenso (10_2_1, 10_2_2 e 10_2_3), non solo per "altro" (10_2_3). Questo sembra un bug nel codice: la condizione `If CType(DatiACPLiguria1.FindControl("rdbDiritti10_2"), RadioButton).Checked` viene ripetuta senza distinguere quale radio `$DirittiAssenso` è selezionato. In pratica, se scegli l'assenso 10_2_1 o 10_2_2 e lasci vuoto `txtAltro10_2_4`, il sistema genererà comunque questo errore. Per evitarlo, **inserisci sempre una descrizione nel campo** quando selezioni qualsiasi opzione del gruppo DirittiAssenso.

---

## 9. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico.

**Causa**: Nessun tecnico è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico. Il modulo indica "tecnico rilevatore delle opere architettoniche" — non è richiesto un ruolo specifico.

{: .note }
> Il controllo del tecnico Progettista (PR) era presente nel codice originale ma è stato **completamente commentato** in una versione precedente. La validazione attuale richiede solo la presenza di almeno un tecnico di qualsiasi ruolo. Il controllo del Direttore Lavori era stato anch'esso previsto ma rimosso.

---

## Consigli pratici — ACP Liguria

### Prima di validare ✅

- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Seleziona la **qualificazione**: 2_1 (art. 167) con sotto-radio `$QualificazioneLav`, 2_2 (condono) con sotto-radio `$QualificazioneArt`, o 2_3 (art. 36-bis) con almeno una checkbox
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona la **natura del vincolo** (5_1..5_4) e compila i campi condizionali: lettera per art. 136/142; denominazione+G.U.+data per vincolo apposto; testo per altro
- [ ] Spunta almeno una delle 14 **checkbox titoli abitativi** e compila i campi resi obbligatori
- [ ] Inserisci la **data realizzazione opere** (GG/MM/AAAA)
- [ ] Seleziona uno dei 4 radio **opere su parti comuni** (e_1..e_4)
- [ ] Seleziona i **diritti di terzi** (10_1 o 10_2); se 10_2: seleziona assenso e **compila sempre** `txtAltro10_2_4`
- [ ] Aggiungi almeno un **tecnico** nei soggetti coinvolti

### Campi presenti ma non validati ℹ️

- **Titolarità**: `cmbTitoloSuImm` (menu), `txtNumAtto`, `txtDataAtto`, `txtNumRegistraz` — non validati
- **Privacy**: testo informativo statico, nessuna checkbox
- **Date titoli abitativi `txtNProt1_x`**: non vengono verificati come obbligatori nel markup statico (solo se resi obbligatori dinamicamente via AJAX)

### Comportamento inatteso — campo "Altro" in diritti di terzi ⚠️

Il campo `txtAltro10_2_4` viene richiesto per **qualsiasi** selezione del gruppo `$DirittiAssenso`, non solo per l'opzione "altro" (10_2_3). Questo è un comportamento non previsto nel design del modulo. Per evitare l'errore "Specificare la descrizione per 'Altro'", inserire sempre una descrizione in quel campo quando si seleziona qualsiasi opzione di assenso (10_2_1, 10_2_2 o 10_2_3).

### Errori frequenti 🔍

1. **Qualificazione senza sotto-selezione** → dopo aver scelto 2_1 o 2_2, bisogna anche selezionare la fattispecie specifica nel sotto-pannello che si apre; il sotto-pannello è visivamente annidato sotto il radio principale
2. **Nessuna checkbox titoli abitativi** → la sezione "Titoli Abitativi" è lunga con 14 voci; verificarla prima di validare
3. **Data realizzazione opere senza formato** → `txtDataIntervento` è l'unica data della sezione "Epoca intervento"; deve essere in GG/MM/AAAA
4. **Campo descrizione diritti terzi sempre obbligatorio** → per il comportamento sopra descritto, compilare sempre `txtAltro10_2_4` quando si sceglie qualsiasi opzione di assenso (non solo "altro")
5. **Natura vincolo 5_1 o 5_2 senza lettera** → i piccoli campi lettera (`txtLett5_1`, `txtLett5_2`) affiancati ai radio button sono obbligatori; è facile non vederli

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
**Fonte**: Analisi codice ValidaDatiACPLiguria e DatiACPLiguria.ascx
