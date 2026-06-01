---
title: Errori Denuncia Sismica - Regione Liguria
parent: Errori di validazione
nav_order: 53
description: Errori di validazione specifici per la Denuncia Sismica (Denuncia delle Opere Strutturali) - Regione Liguria (artt. 65, 93, 94 D.P.R. 380/2001)
keywords: [denuncia sismica, denuncia opere strutturali, Liguria, art. 65 DPR 380, art. 93, art. 94, cemento armato, zona sismica, collaudatore, strumento urbanistico esecutivo, vincolo idrogeologico, dichiarazione conformità]
IDRegione: 3
IDTipoPratica: 217
Fonte: Manuale
---

# Errori di validazione - Denuncia Sismica (Opere Strutturali)
## Regione Liguria

Guida completa agli errori specifici per la **Denuncia delle Opere Strutturali** (Denuncia Sismica) ai sensi degli artt. 65, 93 e 94 del D.P.R. 6 giugno 2001, n. 380 — Regione Liguria.

{: .note }
> La Denuncia Sismica Liguria è una delle pratiche più complesse del sistema. Le caratteristiche principali sono: 4 schede professionisti in loop obbligatorio (Progettista architettonico, Direttore lavori architettonici, Progettista strutture, Direttore lavori strutturali) con 3 campi base ciascuna; 1 Costruttore; il Collaudatore (scheda 5) è obbligatorio solo se si seleziona l'Autorizzazione sismica preventiva. Le sezioni Strumento Urbanistico Esecutivo e Vincolo Idrogeologico hanno campi condizionali attivati a runtime via CssClass. La data della denuncia lavori precedenti viene verificata **solo nel formato** se compilata (non è obbligatoria). La sezione finale "Dichiarazione di conformità" richiede 4 campi obbligatori. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Tipo di denuncia](#1-tipo-di-denuncia)
2. [Informazioni tecnico-amministrative — Inizio lavori e Procedura](#2-informazioni-tecnico-amministrative--inizio-lavori-e-procedura)
3. [Descrizione sintetica dell'intervento](#3-descrizione-sintetica-dellintervento)
4. [Localizzazione dell'intervento](#4-localizzazione-dellintervento)
5. [Professionisti (schede 1–4 in loop)](#5-professionisti-schede-14-in-loop)
6. [Costruttore](#6-costruttore)
7. [Collaudatore delle opere](#7-collaudatore-delle-opere)
8. [Referente per i rapporti con la pubblica amministrazione](#8-referente-per-i-rapporti-con-la-pubblica-amministrazione)
9. [Strumento urbanistico esecutivo](#9-strumento-urbanistico-esecutivo)
10. [Vincolo idrogeologico](#10-vincolo-idrogeologico)
11. [Data denuncia lavori precedenti](#11-data-denuncia-lavori-precedenti)
12. [Data, firma dichiarante e firma Costruttore](#12-data-firma-dichiarante-e-firma-costruttore)
13. [Dichiarazione di conformità](#13-dichiarazione-di-conformità)

---

## 1. Tipo di denuncia

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo di Denuncia'.

**Dove si trova**: Sezione "Tipo di denuncia" → 3 radio button

**Causa**: Nessuna delle 3 opzioni è selezionata.

**Soluzione**: Seleziona **uno dei tre radio button** in base alla tipologia dell'opera:
- ⚪ **"CA"** — Denuncia di opera in conglomerato cementizio armato, normale e precompresso o in struttura metallica (art. 65 D.P.R. 380/2001)
- ⚪ **"ZS"** — Denuncia di opera in zona sismica (art. 93 D.P.R. 380/2001) con struttura diversa dal cemento armato e dalla struttura metallica
- ⚪ **"CA+ZS"** — Denuncia di opera in zona sismica (art. 93) con struttura in cemento armato o metallica (art. 65)

---

## 2. Informazioni tecnico-amministrative — Inizio lavori e Procedura

### ATTENZIONE ! Non è stata selezionata nessuna voce per la 'Tempistica di presentazione rispetto all'inizio dei lavori strutturali'.

**Dove si trova**: Sezione "Informazioni di carattere tecnico-amministrativo" → 2 radio button "regolare" / "tardiva"

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **b1_1 — "regolare"** inizio dei lavori previsto il ___ → inserisci la data prevista
- ⚪ **b1_2 — "tardiva"** inizio dei lavori avvenuto il ___ → inserisci la data effettiva

---

### ATTENZIONE !  Inserire la data di inizio lavori. (regolare)

**Causa**: Hai selezionato b1_1 ("regolare") ma il campo data `txtInizioLavoriReg` è vuoto. Il messaggio ha due spazi dopo il punto esclamativo — è il testo esatto del codice.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (inizio lavori regolare)

**Causa**: La data di inizio lavori (regolare) non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE !  Inserire la data di inizio lavori. (tardiva)

**Causa**: Hai selezionato b1_2 ("tardiva") ma il campo data `txtInizioLavoriTar` è vuoto.

**Soluzione**: Inserisci la data in cui i lavori strutturali sono effettivamente iniziati nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (inizio lavori tardiva)

**Causa**: La data di inizio lavori (tardiva) non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Selezionare almeno una Procedura tra Denuncia/Deposito e Autorizzazione.

**Dove si trova**: Sezione "Procedura" → 2 checkbox

**Causa**: Nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkDenuncia** — "Denuncia/Deposito" (art. 65 e art. 93, D.P.R. 380/2001)
- ☐ **chkAutorizz** — "Autorizzazione sismica preventiva" (art. 94, D.P.R. 380/2001) → richiede i dati del Collaudatore

Le due checkbox non sono mutuamente esclusive.

{: .note }
> Se spunti `chkAutorizz` (Autorizzazione sismica preventiva), il validatore verificherà immediatamente cognome, nome e CF del Collaudatore delle opere (scheda Prof5) prima di continuare con il resto della pratica. Assicurati di compilare anche la scheda Collaudatore se selezioni questa opzione.

---

## 3. Descrizione sintetica dell'intervento

### ATTENZIONE !  Inserire la descrizione dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga `txtDescrIntervento` (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione delle opere strutturali nel campo multiriga (max **300 caratteri**).

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

## 5. Professionisti (schede 1–4 in loop)

Il validatore controlla in sequenza le schede dei 4 professionisti obbligatori tramite un loop `For i = 0 To 3` che verifica `txtCognomeProf1..4`, `txtNomeProf1..4`, `txtCodFiscaleProf1..4`. I messaggi sono identici per tutte e 4 le schede.

Le 4 schede corrispondono a:
- **Scheda 1** (`txtCognomeProf1` / `txtNomeProf1` / `txtCodFiscaleProf1`) — **Progettista delle opere architettoniche**
- **Scheda 2** (`txtCognomeProf2` / `txtNomeProf2` / `txtCodFiscaleProf2`) — **Direttore dei lavori architettonici**
- **Scheda 3** (`txtCognomeProf3` / `txtNomeProf3` / `txtCodFiscaleProf3`) — **Progettista delle strutture**
- **Scheda 4** (`txtCognomeProf4` / `txtNomeProf4` / `txtCodFiscaleProf4`) — **Direttore dei lavori strutturali**

---

### ATTENZIONE ! Inserire il cognome del professionista.

**Causa**: Il campo cognome della scheda professionista in corso di verifica è vuoto.

**Soluzione**: Inserisci il cognome nella scheda corrispondente. Poiché il messaggio è identico per tutte e 4 le schede, identifica quale scheda è incompleta scorrendo il modulo dall'alto verso il basso (il loop parte dalla scheda 1).

---

### ATTENZIONE ! Inserire il nome del professionista.

**Causa**: Il campo nome della scheda corrente è vuoto.

**Soluzione**: Inserisci il nome nel campo corrispondente.

---

### ATTENZIONE ! Inserire il codice fiscale del professionista.

**Causa**: Il campo CF della scheda corrente è vuoto.

**Soluzione**: Inserisci il codice fiscale (16 caratteri) nel campo corrispondente.

{: .note }
> I campi **"con residenza di lavoro in"** (città), **via**, **n.** e **tel. n** di ogni scheda professionista hanno la classe `CampoObbligatorio` nel modulo ma **non vengono validati** dal loop nel codice VB — solo cognome, nome e CF sono verificati. Compilarli è comunque opportuno per la completezza del documento.

---

## 6. Costruttore

Dopo le 4 schede professionisti, il validatore verifica i 3 campi base del Costruttore (`txtCognomeImpr1`, `txtNomeImpr1`, `txtCodFiscaleImpr1`).

---

### ATTENZIONE ! Inserire il cognome del Costruttore.

**Dove si trova**: Sezione "Costruttore" → campo `txtCognomeImpr1`

**Causa**: Il campo cognome del Costruttore è vuoto.

**Soluzione**: Inserisci il cognome (o ragione sociale) del Costruttore.

---

### ATTENZIONE ! Inserire il nome del Costruttore.

**Soluzione**: Inserisci il nome nel campo `txtNomeImpr1`.

---

### ATTENZIONE ! Inserire il codice fiscale del Costruttore.

**Soluzione**: Inserisci il codice fiscale (o partita IVA/CF dell'impresa) nel campo `txtCodFiscaleImpr1`.

---

## 7. Collaudatore delle opere

La scheda del Collaudatore (Prof5) è **condizionale**: viene verificata solo se `chkAutorizz` (Autorizzazione sismica preventiva) è spuntata. Il validatore verifica cognome, nome e CF **due volte** nel codice — una prima della localizzazione (con messaggi generici) e una dopo il Costruttore (con messaggi specifici "Collaudatore"). In entrambi i casi gli errori sono identici e si riferiscono alla stessa scheda.

---

### ATTENZIONE ! Inserire il cognome del Collaudatore delle opere.

**Dove si trova**: Sezione "Collaudatore delle opere" → campo `txtCognomeProf5`

**Causa**: Hai spuntato `chkAutorizz` ma il campo cognome del Collaudatore è vuoto.

**Soluzione**: Inserisci il cognome del Collaudatore delle opere nel campo `txtCognomeProf5`.

---

### ATTENZIONE ! Inserire il nome del Collaudatore delle opere.

**Soluzione**: Inserisci il nome nel campo `txtNomeProf5`.

---

### ATTENZIONE ! Inserire il codice fiscale del Collaudatore delle opere.

**Soluzione**: Inserisci il codice fiscale nel campo `txtCodFiscaleProf5`.

{: .note }
> I campi città, via, n. e tel. della scheda Collaudatore **non hanno** la classe `CampoObbligatorio` nel modulo e non vengono validati. Il Collaudatore delle opere ai sensi dell'art. 94 D.P.R. 380/2001 è il soggetto designato dal committente per il collaudo statico delle strutture soggette ad autorizzazione sismica preventiva.

---

## 8. Referente per i rapporti con la pubblica amministrazione

### ATTENZIONE !  Referente per i rapporti con pubblica amministrazione non indicato.

**Dove si trova**: Campo `cmbReferentePA` — menu a discesa "designando tra di essi il ___ quale referente, per i rapporti con la pubblica amministrazione"

**Causa**: Il menu è rimasto sull'opzione vuota iniziale.

**Soluzione**: Seleziona **uno dei due valori** dal menu:
- **Progettista delle opere architettoniche** (POA)
- **Progettista delle strutture** (PDS)

Il referente PA è il professionista designato per i rapporti con la pubblica amministrazione tra quelli indicati nella denuncia.

---

## 9. Strumento urbanistico esecutivo

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Strumento Urbanistico Esecutivo'.

**Dove si trova**: Punto a) → 2 radio button "è" / "non è" soggetta a strumento urbanistico esecutivo

**Causa**: Nessuno dei 2 radio button del gruppo `$StrUrbEse` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbStrUrbEsea_1 — "è"** → compila i campi del tipo di strumento, numero delibera e data delibera
- ⚪ **rdbStrUrbEsea_2 — "non è"** → nessun campo aggiuntivo richiesto

---

### ATTENZIONE ! Inserire descrizione Strumento Urbanistico Esecutivo.

**Causa**: Hai selezionato "è" (soggetta a strumento urbanistico esecutivo) ma non hai specificato il tipo di strumento nel campo testo (`txtStrUrbEse`).

**Soluzione**: Inserisci la descrizione del tipo di strumento urbanistico esecutivo (es. `Piano Particolareggiato`, `Piano di Lottizzazione`, `Piano per l'Edilizia Economica e Popolare`).

---

### ATTENZIONE !  Inserire il numero della deliberazione comunale.

**Causa**: Manca il numero della delibera comunale di approvazione dello strumento urbanistico nel campo `txtNStrUrbEse`.

**Soluzione**: Inserisci il numero della deliberazione nel campo "n."

---

### ATTENZIONE ! Inserire la data della deliberazione comunale.

**Causa**: Il campo data della delibera `txtDataStrUrbEse` è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (delibera strumento urbanistico)

**Causa**: La data della delibera non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

{: .note }
> La visibilità e l'obbligatorietà dei campi dello strumento urbanistico (`txtStrUrbEse`, `txtNStrUrbEse`, `txtDataStrUrbEse`) vengono gestite a runtime modificando la classe CSS del campo. Il validatore VB verifica la presenza di "CampoObbligatorio" nella classe CSS del campo anziché controllare direttamente lo stato del radio button. Se si seleziona "è", il sistema aggiunge la classe al campo; se si seleziona "non è", la rimuove. Questo comportamento è condizionale via JavaScript/AJAX.

---

## 10. Vincolo idrogeologico

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Vincolo Idrogeologico'.

**Dove si trova**: Punto b) → 2 radio button "è" / "non è" sottoposta a vincolo idrogeologico

**Causa**: Nessuno dei 2 radio button del gruppo `$VincoloIdrogeologico` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbVincoloIdrogeologicob_1 — "è"** → compila ente rilasciante, n. prot. e data protocollo
- ⚪ **rdbVincoloIdrogeologicob_2 — "non è"** → nessun campo aggiuntivo

---

### ATTENZIONE ! Inserire descrizione dell'Ente rilasciante Autorizzazione.

**Causa**: Hai selezionato "è" (vincolo idrogeologico) ma non hai indicato l'ente che ha rilasciato l'autorizzazione nel campo `txtRilascianteAut`.

**Soluzione**: Inserisci il nome dell'ente che ha rilasciato l'autorizzazione idrogeologica (es. `Città Metropolitana di Genova`, `Regione Liguria - Settore Tutela Ambiente`).

---

### ATTENZIONE !  Inserire il numero di protocollo dell'Autorizzazione.

**Causa**: Manca il numero di protocollo dell'autorizzazione idrogeologica nel campo `txtNAut`.

**Soluzione**: Inserisci il numero di protocollo nel campo "Prot n."

---

### ATTENZIONE ! Inserire la data di protocollo dell'Autorizzazione.

**Causa**: Il campo data `txtDataAut` è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (protocollo autorizzazione vincolo)

**Causa**: La data del protocollo dell'autorizzazione non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 11. Data denuncia lavori precedenti

Il punto c) riguarda la denuncia di lavori già realizzati sul fabbricato. I campi `txtDenunciaLavori` (ente), `txtNDenunciaLavori` (n. prot.) e `txtDataDenunciaLavori` (data) **non hanno** la classe `CampoObbligatorio` nel modulo e non vengono validati come obbligatori. Tuttavia la **data** (`txtDataDenunciaLavori`) viene verificata nel formato se compilata.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (denuncia lavori precedenti)

**Causa**: Hai compilato il campo data della denuncia dei lavori precedenti (`txtDataDenunciaLavori`) ma il formato non è corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**, oppure svuota il campo se non applicabile (il campo è opzionale — se vuoto, il validatore non genera errori).

{: .note }
> Il punto c) è l'unica parte della pratica in cui la data viene verificata **solo nel formato** se compilata, senza un controllo di obbligatorietà. Se il fabbricato non è stato oggetto di precedenti denunce strutturali, lasciare vuoti i campi del punto c).

---

## 12. Data, firma dichiarante e firma Costruttore

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Campo `txtDataDich1` — "data" in calce alla dichiarazione del titolare

**Causa**: Il campo data della dichiarazione è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data dichiarazione)

**Causa**: La data della dichiarazione non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE !  Inserire la firma del dichiarante.

**Dove si trova**: Campo `txtFirmaDich1` — "firma" affiancato alla data della dichiarazione

**Causa**: Il campo firma del dichiarante è vuoto.

**Soluzione**: Inserisci il nominativo del dichiarante nel campo "firma".

---

### ATTENZIONE !  Inserire la firma del Costruttore.

**Dove si trova**: Campo `txtFirmaCostruttore` — in fondo alla sezione "Firma del Costruttore per opere disciplinate dal D.P.R. n. 380 del 6/06/2001 art. 65"

**Causa**: Il campo firma del Costruttore è vuoto.

**Soluzione**: Inserisci il nominativo del Costruttore nel campo "firma".

---

## 13. Dichiarazione di conformità

La sezione "Dichiarazione di conformità" richiede 4 campi obbligatori: nominativo del sottoscritto, tipo progettista, titolo abilitativo (radio) e firma.

---

### ATTENZIONE !  Inserire il nominativo del sottoscritto.

**Dove si trova**: Sezione "Dichiarazione di conformità" → campo `txtSottoscritto` nel testo "Il sottoscritto ___ in qualità di progettista..."

**Causa**: Il campo del nominativo del sottoscritto è vuoto.

**Soluzione**: Inserisci il nominativo del progettista che sottoscrive la dichiarazione di conformità.

---

### ATTENZIONE !  Tipo di progettista non indicato.

**Dove si trova**: Menu `cmbTipoProgettista` nella sezione dichiarazione di conformità

**Causa**: Il menu è rimasto sull'opzione vuota iniziale.

**Soluzione**: Seleziona **uno dei due valori** dal menu:
- **Progettista delle opere architettoniche** (POA)
- **Progettista delle strutture** (PDS)

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolo Abitativo'.

**Dove si trova**: 2 radio button "allegato" / "rilasciato" in fondo alla dichiarazione di conformità

**Causa**: Nessuno dei 2 radio button del gruppo `$TitoloAbitativo` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbTitoloAbitativo1** — "allegato" (il titolo abilitativo è allegato alla denuncia)
- ⚪ **rdbTitoloAbitativo2** — "rilasciato" (il titolo abilitativo è già stato rilasciato)

---

### ATTENZIONE !  Inserire nominativo firma del sottoscrittore.

**Dove si trova**: Campo `txtFirmaProgettista` — "firma" in calce alla dichiarazione di conformità

**Causa**: Il campo firma del progettista/sottoscrittore è vuoto.

**Soluzione**: Inserisci il nominativo del progettista nel campo "firma" della dichiarazione di conformità.

---

## Consigli pratici — Denuncia Sismica Liguria

### Prima di validare ✅

- [ ] Seleziona il **tipo di denuncia** (CA / ZS / CA+ZS)
- [ ] Seleziona la **tempistica** (regolare o tardiva) e inserisci la **data** (GG/MM/AAAA)
- [ ] Spunta almeno una **procedura** (Denuncia/Deposito e/o Autorizzazione); se Autorizzazione: compila scheda Collaudatore (cognome/nome/CF)
- [ ] Inserisci la **descrizione** dell'intervento (max 300 caratteri)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Compila le **schede 1–4 professionisti** (cognome + nome + CF per ciascuna)
- [ ] Compila la scheda **Costruttore** (cognome + nome + CF)
- [ ] Seleziona il **referente PA** (POA o PDS)
- [ ] Seleziona **strumento urbanistico** ("è" o "non è"); se "è": tipo + n. delibera + data (GG/MM/AAAA)
- [ ] Seleziona **vincolo idrogeologico** ("è" o "non è"); se "è": ente + n. prot. + data (GG/MM/AAAA)
- [ ] Se punto c) compilato: data **denuncia lavori precedenti** in GG/MM/AAAA
- [ ] Inserisci la **data dichiarazione** (GG/MM/AAAA) e la **firma dichiarante**
- [ ] Inserisci la **firma del Costruttore**
- [ ] Compila la **Dichiarazione di conformità**: nominativo sottoscritto + tipo progettista + titolo abitativo + firma progettista

### Campi presenti ma non validati ℹ️

- **Città/via/n./tel.** di ogni scheda professionista (1-4): campi presenti ma non verificati dal loop
- **Città/via/n./tel.** del Costruttore: stessa situazione
- **Città/via/n./tel.** del Collaudatore (Prof5): nessun campo è obbligatorio eccetto cognome/nome/CF
- **`txtProcedura`**: campo multiriga "specificare fattispecie e riferimenti normativi regionali" — non validato
- **`txtDenunciaLavori` e `txtNDenunciaLavori`** (punto c): non obbligatori

### Doppia verifica del Collaudatore ⚠️

Il validatore controlla i campi del Collaudatore (Prof5) **due volte**: la prima immediatamente dopo la selezione di `chkAutorizz` (con messaggi generici "professionista"), la seconda dopo il Costruttore (con messaggi specifici "Collaudatore"). Il comportamento è identico — entrambe le verifiche riguardano gli stessi campi `txtCognomeProf5`, `txtNomeProf5`, `txtCodFiscaleProf5`.

### Errori frequenti 🔍

1. **Mancata compilazione di una delle 4 schede professionisti** → il loop si ferma alla prima scheda incompleta; poiché il messaggio è identico per tutte e 4, bisogna identificare visivamente quale scheda è incompleta
2. **chkAutorizz spuntata senza dati Collaudatore** → l'errore sulla scheda Prof5 appare prima ancora di arrivare alla localizzazione
3. **Strumento urbanistico: radio "è" senza compilare i campi** → i campi si abilitano via AJAX; verificare che siano effettivamente compilati dopo aver selezionato "è"
4. **Data denuncia lavori precedenti in formato errato** → se si compila la data del punto c) in un formato diverso da GG/MM/AAAA, il validatore si blocca; lasciare vuoto il campo se non applicabile
5. **Dichiarazione di conformità parzialmente compilata** → i 4 campi finali (sottoscritto + tipo progettista + titolo abitativo + firma) sono alla fine del modulo e possono essere dimenticati

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
**Fonte**: Analisi codice ValidaDatiDSLiguria e DatiDSLiguria.ascx
