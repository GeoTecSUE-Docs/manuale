---
title: Errori Autorizzazione Vincolo Idrogeologico - Liguria
parent: Errori di validazione
nav_order: 46
description: Errori di validazione specifici per la domanda di Autorizzazione in area soggetta a Vincolo Idrogeologico (AVI) - Regione Liguria
keywords: [vincolo idrogeologico, AVI, Liguria, L.R. 4/99, art. 35, art. 36, movimenti di terreno, variante, autorizzazione precedente, SCIA, DIA, progettista, geologo, altron, titolarità]
IDRegione: 4
IDTipoPratica: 41
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Vincolo Idrogeologico (AVI)
## Regione Liguria

Guida completa agli errori specifici per la domanda di **Autorizzazione ad eseguire movimenti di terreno in area sottoposta a vincolo idrogeologico** ai sensi degli artt. 35 e 36 della L.R. 4/99 — Regione Liguria.

{: .note }
> L'AVI Liguria ha caratteristiche esclusive rispetto alle altre pratiche della piattaforma. La **descrizione dell'intervento** è il primo campo validato (prima ancora della titolarità). La **titolarità** ha un controllo condizionale basato sul valore `altron` del menu a discesa: solo se selezionata la voce "altro" diventa obbligatorio il campo di testo libero. La sezione **"Riferimenti a precedenti autorizzazioni"** ha due radio button alternativi: se si sceglie la variante (secondo radio), si attivano tre checkbox — ciascuna con data e numero — ma solo i checkbox 1 (autorizzazione) e 2 (SCIA) vengono validati; il checkbox 3 (DIA) è presente nell'ASCX ma **non è validato nel codice**. Sono obbligatoriamente richiesti **due tecnici con ruoli distinti**: un **Progettista** (ruolo `PR`) e un **Geologo** (ruolo `GE`). La privacy è solo informativa, senza checkbox obbligatoria. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Descrizione dell'intervento](#1-descrizione-dellintervento)
2. [Titolarità dell'intervento](#2-titolarità-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Riferimenti a precedenti autorizzazioni / SCIA](#4-riferimenti-a-precedenti-autorizzazioni--scia)
5. [Tecnici incaricati — Progettista e Geologo](#5-tecnici-incaricati--progettista-e-geologo)

---

## 1. Descrizione dell'intervento

### ATTENZIONE ! Inserire la Descrizione dell'intervento.

**Dove si trova**: Sezione **"Tipo di intervento"** in cima al modulo → campo di testo sotto la dicitura "ai sensi degli artt. 35 e 36 della L.R. 4/99 … l'autorizzazione ad eseguire movimenti di terreno in area sottoposta a vincolo idrogeologico connessi ai lavori di"

**Causa**: Non hai inserito la descrizione dei lavori che motivano la richiesta di autorizzazione al vincolo idrogeologico.

**Soluzione**: Inserisci una descrizione chiara e sintetica dei movimenti di terreno e dei lavori connessi nel campo di testo (max **300 caratteri**). Esempi:
- `Scavo per fondazioni di nuovo fabbricato residenziale di mc 450 in area collinare.`
- `Sbancamento per realizzazione strada privata di accesso al lotto, lunghezza 80 m, pendenza 8%.`
- `Livellamento e sistemazione terreno per impianto frutteto, superficie 3000 mq.`

{: .note }
> A differenza di tutte le altre pratiche della piattaforma, nell'AVI Liguria la **descrizione dell'intervento è il primo campo validato**, prima ancora della titolarità e della localizzazione. Se questo campo è vuoto, nessun altro controllo viene eseguito.

---

## 2. Titolarità dell'intervento

### ATTENZIONE ! Inserire la Titolarità dell'intervento.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo di testo **"(Specificare se altro)"**

**Causa**: Hai selezionato la voce **"altro"** nel menu a discesa della titolarità (`cmbTitoloSuImm`) ma non hai compilato il campo di testo libero di specificazione.

**Soluzione**:
1. Verifica la voce selezionata nel menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"**
2. Se hai selezionato una voce generica come **"altro"** o simile (valore interno `altron`), il campo **"(Specificare se altro)"** diventa obbligatorio
3. Inserisci la specifica del tuo titolo nel campo di testo che si attiva

{: .note }
> Il controllo viene attivato solo se il valore selezionato nel menu a discesa è esattamente `altron` (il valore interno della voce "altro"). Per tutte le altre voci standard del menu (proprietario, locatario, ecc.) questo campo non è richiesto e la validazione passa direttamente alla sezione successiva.

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `16100`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 4. Riferimenti a precedenti autorizzazioni / SCIA

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Riferimenti a precedenti autorizzazioni rilasciate / SCIA presentate'.

**Dove si trova**: Sezione **"Riferimenti a precedenti autorizzazioni rilasciate / SCIA presentate"**

**Causa**: Non hai selezionato nessuno dei due radio button che descrivono la natura della presente istanza.

**Soluzione**: Seleziona **uno dei due scenari**:
- ⚪ **Scenario d.1** — "una nuova attività o un nuovo intervento di modificazione/trasformazione del terreno in area sottoposta a vincolo idrogeologico" → nessun campo aggiuntivo
- ⚪ **Scenario d.2** — "un'attività o un intervento… in variante a precedente pratica presentata" → si attivano i checkbox con i riferimenti della pratica precedente (vedi sotto)

---

### Scenario d.2 — Variante a precedente pratica

Se selezioni lo Scenario d.2 si attivano tre checkbox, ciascuna con campi data e numero propri. Spunta **almeno uno** dei checkbox corrispondente alla pratica precedente a cui la presente è in variante.

#### Checkbox d.2.1 — Autorizzazione rilasciata

#### ATTENZIONE ! Inserire la data.

**Causa**: Hai spuntato il checkbox **"autorizzazione rilasciata in data"** ma il campo data è vuoto.

**Soluzione**: Inserisci la data dell'autorizzazione precedente nel campo accanto al checkbox nel formato **GG/MM/AAAA**. Puoi usare l'icona calendario.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(autorizzazione)*

**Causa**: Il campo data dell'autorizzazione contiene un valore in formato non valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `10/06/2022` ✅, `10-06-2022` ❌).

---

#### ATTENZIONE ! Inserire il numero. *(autorizzazione)*

**Causa**: Hai spuntato il checkbox autorizzazione e inserito la data, ma il campo **"pratica n."** è vuoto.

**Soluzione**: Inserisci il numero della pratica dell'autorizzazione precedente nel campo **"pratica n."**.

---

#### Checkbox d.2.2 — SCIA presentata

#### ATTENZIONE ! Inserire la data. *(SCIA)*

**Causa**: Hai spuntato il checkbox **"Segnalazione Certificata di Inizio Attività presentata in data"** ma il campo data SCIA è vuoto.

**Soluzione**: Inserisci la data della SCIA precedente nel campo accanto al checkbox nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(SCIA)*

**Causa**: Il campo data della SCIA contiene un valore in formato non valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

{: .warning }
> **Bug noto nel codice — validazione SCIA**: il controllo del formato data per la SCIA (`chkInterventod2_2`) verifica erroneamente il contenuto di `txtDataAUT` (il campo data dell'autorizzazione) invece di `txtDataSCIA`. In pratica, il formato di `txtDataSCIA` **non viene mai controllato** se `txtDataAUT` è già in formato corretto — il focus va comunque su `txtDataSCIA`. Inserire sempre le date in formato GG/MM/AAAA per entrambi i campi. Segnalare al team di sviluppo per correzione.
>
> **Snippet codice attuale (errato)**:
> ```vb
> ' Verifica il formato di txtDataAUT invece di txtDataSCIA:
> If clsModuloAsp.ControlloFormatoData(Trim(CType(...FindControl("txtDataAUT"), TextBox).Text)) = False Then
> ```
> **Codice corretto atteso**:
> ```vb
> If clsModuloAsp.ControlloFormatoData(Trim(CType(...FindControl("txtDataSCIA"), TextBox).Text)) = False Then
> ```

---

#### ATTENZIONE ! Inserire il numero. *(SCIA)*

**Causa**: Hai spuntato il checkbox SCIA e inserito la data, ma il campo **"pratica n."** della SCIA è vuoto.

**Soluzione**: Inserisci il numero della SCIA precedente nel campo **"pratica n."** accanto al campo data SCIA.

---

#### Checkbox d.2.3 — DIA presentata (non validato)

{: .warning }
> **Funzionalità non validata**: il checkbox **"Denuncia di Inizio Attività presentata in data"** (`chkInterventod2_3`) con i relativi campi `txtDataDIA` e `txtNumDIA` è presente nell'ASCX ma **non viene validato** dalla funzione `ValidaDatiAVI_Liguria`. Se spunti solo questo checkbox (senza spuntare i checkbox d.2.1 o d.2.2), la validazione non richiederà data né numero per la DIA. I dati inseriti vengono comunque salvati ma non verificati. Segnalare al team di sviluppo per allineamento.

---

## 5. Tecnici incaricati — Progettista e Geologo

Questa pratica è **l'unica nella piattaforma** che richiede obbligatoriamente **due tecnici con ruoli distinti**: un Progettista e un Geologo. I due controlli sono sequenziali: prima viene verificata la presenza del Progettista, poi quella del Geologo.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Dove si trova**: Sezione **"Tecnici incaricati"** del modulo + scheda **"Soggetti coinvolti"** → tecnici

**Causa**: Non hai aggiunto nessun tecnico con ruolo **Progettista** (codice `PR`) tra i soggetti coinvolti.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Progettista"**
4. Compila i dati del tecnico e salva
5. Torna al modulo AVI, clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Geologo.

**Dove si trova**: Sezione **"Tecnici incaricati"** + scheda **"Soggetti coinvolti"** → tecnici

**Causa**: Non hai aggiunto nessun tecnico con ruolo **Geologo** (codice `GE`) tra i soggetti coinvolti. Questo errore appare solo **dopo** che il Progettista è stato correttamente aggiunto.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Geologo"**
4. Compila i dati del tecnico geologo e salva
5. Torna al modulo AVI, clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> I due controlli sono **sequenziali**: se manca il Progettista, l'errore sul Geologo non viene mostrato. Solo dopo aver aggiunto il Progettista e riprovato a validare comparirà eventualmente l'errore sul Geologo. È necessario aggiungere **entrambe** le figure prima di poter completare la validazione. Verificare di averle entrambe nei Soggetti coinvolti prima di cliccare "Valida e Salva".

---

## Consigli pratici AVI Liguria

### Prima di validare ✅

- [ ] Inserisci la **descrizione dell'intervento** (movimenti di terreno, max 300 caratteri)
- [ ] Seleziona la **titolarità** dal menu a discesa
- [ ] Se selezioni "altro" (`altron`): compila il campo **"(Specificare se altro)"**
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **tipo di istanza** (nuovo intervento o variante)
- [ ] **Se variante (d.2)**: spunta almeno uno tra i checkbox d.2.1 (autorizzazione) e/o d.2.2 (SCIA), inserendo data e numero per ciascuno spuntato
- [ ] Aggiungi il **Progettista** nei Soggetti coinvolti (ruolo `PR`)
- [ ] Aggiungi il **Geologo** nei Soggetti coinvolti (ruolo `GE`)
- [ ] **Salva** frequentemente

### Confronto requisiti tecnici con altre pratiche ⚠️

| Pratica | Tecnici obbligatori | Ruoli |
|---|---|---|
| AVI Liguria | 2 (obbligatori distinti) | Progettista (`PR`) + Geologo (`GE`) |
| CILATE Piemonte | 1 | Rilevatore (`RI`) |
| ACP Tutte le regioni | ≥ 1 (qualsiasi) | — |
| Lavori AC Piemonte | ≥ 1 (qualsiasi) | — |

### Errori frequenti AVI Liguria 🔍

1. **Descrizione intervento vuota** → è il primo controllo; blocca tutto il resto prima ancora della titolarità
2. **Titolarità "altro" senza specificazione** → solo la voce con valore interno `altron` attiva il campo di testo; le voci standard non lo richiedono
3. **Variante senza checkbox spuntato** → selezionare il secondo radio button non è sufficiente: occorre spuntare almeno uno dei checkbox d.2.1 o d.2.2 con data e numero
4. **DIA non validata** → il checkbox d.2.3 (DIA) non è validato nel codice: i dati vengono salvati ma non verificati; usare preferibilmente d.2.1 o d.2.2 per pratiche valide
5. **Geologo mancante** → errore mostrato solo dopo aver corretto quello del Progettista; aggiungere entrambi prima di validare
6. **Bug formato data SCIA** → il controllo formato verifica `txtDataAUT` invece di `txtDataSCIA`; inserire sempre GG/MM/AAAA in entrambi i campi per evitare problemi

### Bug documentati

**Bug 1 — Validazione formato data SCIA**:

```vb
' Codice attuale (errato) — controlla txtDataAUT invece di txtDataSCIA:
If clsModuloAsp.ControlloFormatoData(
    Trim(CType(DatiAVILiguria1.FindControl("txtDataAUT"), TextBox).Text)) = False Then

' Codice corretto atteso:
If clsModuloAsp.ControlloFormatoData(
    Trim(CType(DatiAVILiguria1.FindControl("txtDataSCIA"), TextBox).Text)) = False Then
```

**Bug 2 — Checkbox DIA non validato**: il checkbox `chkInterventod2_3` con campi `txtDataDIA` e `txtNumDIA` è presente nell'ASCX ma assente dalla logica di validazione VB. Nessun errore viene generato se la DIA è spuntata senza data o numero.

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
**Fonte**: Analisi codice `ValidaDatiAVI_Liguria` e `DatiAVILiguria.ascx`
