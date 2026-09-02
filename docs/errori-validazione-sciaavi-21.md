---
title: Errori S.C.I.A. Vincolo Idrogeologico - Liguria
parent: Errori di validazione
nav_order: 48
description: Errori di validazione specifici per la Segnalazione Certificata di Inizio Attività per Vincolo Idrogeologico (SCIAVI) - Regione Liguria
keywords: [SCIA vincolo idrogeologico, SCIAVI, Liguria, L.R. 4/99, art. 35, Piano di Bacino, ambito idrogeologico, movimenti di terreno, variante, SCIA precedente, progettista, geologo, altron, titolarità]
IDRegione: 3         # Liguria
IDTipoPratica: 21
Fonte: Manuale
---

# Errori di validazione - S.C.I.A. per Vincolo Idrogeologico (SCIAVI)
## Regione Liguria

Guida completa agli errori specifici per la **Segnalazione Certificata di Inizio Attività per movimenti di terreno in area sottoposta a vincolo idrogeologico** ai sensi degli artt. 35 c. 2 e 3 della L.R. 4/99 — Regione Liguria.

{: .note }
> La SCIAVI è la variante SCIA dell'[AVI Liguria](errori-validazione-avi-41.html) e condivide con essa quasi tutta la struttura e la logica di validazione. La differenza principale è la presenza del campo **"Piano di Bacino e/o Ambito n."** (`txtNumAmbito`), che viene validato **per primo** prima ancora della descrizione dell'intervento. Tutti i bug dell'AVI Liguria sono presenti anche nella SCIAVI: il controllo del formato data SCIA legge `txtDataAUT` invece di `txtDataSCIA`, e il checkbox DIA (`chkInterventod2_3`) non viene validato. I due tecnici obbligatori (Progettista + Geologo) sono identici. La privacy è solo informativa. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Piano di Bacino e/o Ambito e descrizione dell'intervento](#1-piano-di-bacino-eo-ambito-e-descrizione-dellintervento)
2. [Titolarità dell'intervento](#2-titolarità-dellintervento)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Riferimenti a precedenti autorizzazioni / SCIA](#4-riferimenti-a-precedenti-autorizzazioni--scia)
5. [Tecnici incaricati — Progettista e Geologo](#5-tecnici-incaricati--progettista-e-geologo)

---

## 1. Piano di Bacino e/o Ambito e descrizione dell'intervento

### ATTENZIONE ! Inserire il numero relativo al Piano di Bacino e/o Ambito.

**Dove si trova**: Sezione **"Tipo di intervento"** in cima al modulo → campo di testo inline accanto alla dicitura "ricadente nel Piano di Bacino e/o nell'Ambito n."

**Causa**: Non hai inserito il numero del Piano di Bacino e/o Ambito in cui ricade l'area soggetta a vincolo idrogeologico.

**Soluzione**: Inserisci il numero del Piano di Bacino o dell'Ambito nel campo accanto alla dicitura **"Piano di Bacino e/o nell'Ambito n."**. Il numero è reperibile nel certificato di vincolo idrogeologico rilasciato dalla Regione o sul portale cartografico ligure (Geoportale Regione Liguria).

{: .note }
> Questo campo è **esclusivo della SCIAVI** rispetto all'AVI Liguria, dove non esiste. È il **primo controllo** eseguito dalla funzione di validazione: se vuoto, nessun altro errore viene mostrato.

---

### ATTENZIONE ! Inserire la Descrizione dell'intervento.

**Dove si trova**: Sezione **"Tipo di intervento"** → campo di testo **"connesso ai lavori di"**

**Causa**: Non hai inserito la descrizione dei lavori connessi ai movimenti di terreno in area soggetta a vincolo idrogeologico.

**Soluzione**: Inserisci una descrizione chiara e sintetica nel campo **"connesso ai lavori di"** (max **300 caratteri**). Esempi:
- `Scavo per fondazioni di nuovo fabbricato residenziale di mc 450 in area collinare.`
- `Sbancamento per realizzazione strada privata di accesso al lotto, lunghezza 80 m, pendenza 8%.`
- `Livellamento e sistemazione terreno per impianto frutteto, superficie 3000 mq.`

---

## 2. Titolarità dell'intervento

### ATTENZIONE ! Inserire la Titolarità dell'intervento.

**Dove si trova**: Sezione **"Titolarità dell'intervento"** → campo di testo **"(Specificare se altro)"**

**Causa**: Hai selezionato la voce **"altro"** nel menu a discesa della titolarità (`cmbTitoloSuImm`, valore interno `altron`) ma non hai compilato il campo di testo libero di specificazione.

**Soluzione**:
1. Verifica la voce selezionata nel menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"**
2. Se hai selezionato la voce con valore interno `altron`, il campo **"(Specificare se altro)"** è obbligatorio
3. Inserisci la specifica del titolo nel campo di testo che si attiva

{: .note }
> Il controllo è identico a quello dell'AVI Liguria: si attiva solo sul valore interno `altron`. Le voci standard del menu (proprietario, locatario, ecc.) non attivano questo campo.

---

## 3. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

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

## 4. Riferimenti a precedenti autorizzazioni / SCIA

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Riferimenti a precedenti autorizzazioni rilasciate / SCIA presentate'.

**Dove si trova**: Sezione **"Riferimenti a precedenti autorizzazioni rilasciate / SCIA presentate"**

**Causa**: Non hai selezionato nessuno dei due radio button che descrivono la natura della presente segnalazione.

**Soluzione**: Seleziona **uno dei due scenari**:
- ⚪ **Scenario d.1** — "una nuova attività o un nuovo intervento di modificazione/trasformazione del terreno in area sottoposta a vincolo idrogeologico" → nessun campo aggiuntivo
- ⚪ **Scenario d.2** — "un'attività o un intervento… in variante a precedente pratica presentata" → si attivano i checkbox con i riferimenti della pratica precedente

---

### Scenario d.2 — Variante a precedente pratica

Se selezioni lo Scenario d.2 si attivano tre checkbox. Spunta **almeno uno** corrispondente alla pratica precedente a cui la presente è in variante.

#### Checkbox d.2.1 — Autorizzazione rilasciata

#### ATTENZIONE ! Inserire la data. *(autorizzazione)*

**Causa**: Hai spuntato il checkbox **"autorizzazione rilasciata in data"** ma il campo data (`txtDataAUT`) è vuoto.

**Soluzione**: Inserisci la data dell'autorizzazione precedente nel campo accanto al checkbox nel formato **GG/MM/AAAA**.

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

**Causa**: Hai spuntato il checkbox **"Segnalazione Certificata di Inizio Attività presentata in data"** ma il campo data SCIA (`txtDataSCIA`) è vuoto.

**Soluzione**: Inserisci la data della SCIA precedente nel campo accanto al checkbox nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(SCIA)*

**Causa**: Il campo data della SCIA contiene un valore in formato non valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

{: .warning }
> **Bug noto nel codice — validazione SCIA (identico all'AVI Liguria)**: il controllo del formato data per `chkInterventod2_2` verifica `txtDataAUT` invece di `txtDataSCIA`. Se `txtDataAUT` è già in formato valido, il formato di `txtDataSCIA` non viene mai verificato, ma il focus va correttamente su `txtDataSCIA`. Inserire sempre GG/MM/AAAA in entrambi i campi.
>
> ```vb
> ' Codice attuale (errato):
> If clsModuloAsp.ControlloFormatoData(Trim(CType(...FindControl("txtDataAUT"), TextBox).Text)) = False Then
>
> ' Codice corretto atteso:
> If clsModuloAsp.ControlloFormatoData(Trim(CType(...FindControl("txtDataSCIA"), TextBox).Text)) = False Then
> ```

---

#### ATTENZIONE ! Inserire il numero. *(SCIA)*

**Causa**: Hai spuntato il checkbox SCIA e inserito la data, ma il campo **"pratica n."** della SCIA è vuoto.

**Soluzione**: Inserisci il numero della SCIA precedente nel campo **"pratica n."** accanto al campo data SCIA.

---

#### Checkbox d.2.3 — DIA presentata (non validato)

{: .warning }
> **Funzionalità non validata (identica all'AVI Liguria)**: il checkbox **"Denuncia di Inizio Attività presentata in data"** (`chkInterventod2_3`) con i relativi campi `txtDataDIA` e `txtNumDIA` è presente nell'ASCX ma **non viene validato** dalla funzione `ValidaDatiSCIAVI_Liguria`. I dati vengono salvati ma non verificati. Segnalare al team di sviluppo per allineamento.

---

## 5. Tecnici incaricati — Progettista e Geologo

Identico all'AVI Liguria: sono obbligatori **entrambi** i ruoli, verificati in sequenza.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Causa**: Nessun tecnico con ruolo **Progettista** (codice `PR`) nei soggetti coinvolti.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Progettista"**
4. Compila i dati e salva
5. Torna al modulo SCIAVI, clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Geologo.

**Causa**: Nessun tecnico con ruolo **Geologo** (codice `GE`) nei soggetti coinvolti. Appare solo dopo che il Progettista è già presente.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Geologo"**
4. Compila i dati del geologo e salva
5. Torna al modulo SCIAVI, clicca **"Salva"** e riprova **"Valida e Salva"**

{: .warning }
> I controlli Progettista e Geologo sono **sequenziali**: il Geologo viene verificato solo dopo che il Progettista è già corretto. Aggiungere entrambi nei Soggetti coinvolti prima di tentare la validazione finale.

---

## Consigli pratici SCIAVI Liguria

### Prima di validare ✅

- [ ] Inserisci il **numero del Piano di Bacino e/o Ambito** nel campo inline in cima al modulo
- [ ] Inserisci la **descrizione dell'intervento** (movimenti di terreno connessi ai lavori, max 300 caratteri)
- [ ] Seleziona la **titolarità** dal menu a discesa
- [ ] Se selezioni "altro" (`altron`): compila il campo **"(Specificare se altro)"**
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona il **tipo di segnalazione** (nuovo intervento o variante)
- [ ] **Se variante (d.2)**: spunta almeno uno tra i checkbox d.2.1 (autorizzazione) e/o d.2.2 (SCIA), inserendo data e numero per ciascuno spuntato
- [ ] Aggiungi il **Progettista** nei Soggetti coinvolti (ruolo `PR`)
- [ ] Aggiungi il **Geologo** nei Soggetti coinvolti (ruolo `GE`)
- [ ] **Salva** frequentemente

### Confronto SCIAVI vs AVI Liguria ⚠️

| Campo / Caratteristica | AVI Liguria (`HfTipoIstanza=4`) | SCIAVI Liguria (`HfTipoIstanza=21`) |
|---|---|---|
| Numero Piano di Bacino/Ambito | ✗ Non presente | ☑ Obbligatorio (primo controllo) |
| Descrizione intervento | ☑ Campo testo (primo controllo) | ☑ Campo testo (secondo controllo) |
| Tipo pratica | "istanza" (AVI) | "segnalazione" (SCIA) |
| Struttura variante (d.2) | Identica (3 checkbox) | Identica (3 checkbox) |
| Bug formato data SCIA | ☑ Presente | ☑ Presente (identico) |
| DIA non validata | ☑ Presente | ☑ Presente (identico) |
| Progettista (`PR`) obbligatorio | ☑ Sì | ☑ Sì |
| Geologo (`GE`) obbligatorio | ☑ Sì | ☑ Sì |
| Privacy | Solo informativa | Solo informativa |

### Errori frequenti SCIAVI Liguria 🔍

1. **Numero Ambito mancante** → è il primo controllo: se vuoto, nessun altro errore viene mostrato; compilarlo prima di tutto il resto
2. **Descrizione intervento vuota** → secondo controllo; immediatamente dopo il numero Ambito
3. **Titolarità "altro" senza specificazione** → solo la voce con valore interno `altron` attiva il campo di testo
4. **Variante senza checkbox spuntato** → selezionare il secondo radio button non è sufficiente: occorre spuntare almeno d.2.1 o d.2.2 con data e numero
5. **DIA non validata** → come nell'AVI, il checkbox d.2.3 non viene controllato
6. **Geologo mancante** → appare solo dopo aver corretto l'errore del Progettista; aggiungere entrambi prima di validare

### Bug documentati (identici all'AVI Liguria)

**Bug 1 — Validazione formato data SCIA**:

```vb
' Codice attuale (errato) — controlla txtDataAUT invece di txtDataSCIA:
If clsModuloAsp.ControlloFormatoData(
    Trim(CType(DatiSCIAVILiguria1.FindControl("txtDataAUT"), TextBox).Text)) = False Then

' Codice corretto atteso:
If clsModuloAsp.ControlloFormatoData(
    Trim(CType(DatiSCIAVILiguria1.FindControl("txtDataSCIA"), TextBox).Text)) = False Then
```

**Bug 2 — Checkbox DIA non validato**: il checkbox `chkInterventod2_3` con campi `txtDataDIA` e `txtNumDIA` è presente nell'ASCX ma assente dalla logica di validazione VB. Stesso bug presente in `DatiAVILiguria.ascx.vb`.

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
**Fonte**: Analisi codice `ValidaDatiSCIAVI_Liguria` e `DatiSCIAVILiguria.ascx`
