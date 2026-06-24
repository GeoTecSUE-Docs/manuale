---
title: Errori Richiesta Certificazione - Piemonte
parent: Errori di validazione
nav_order: 47
description: Errori di validazione specifici per la Richiesta di Certificazione edilizio-urbanistica (RC) - Regione Piemonte
keywords: [richiesta certificazione, RC, Piemonte, art. 3 DPR 380/2001, pertinenza, lusso, D.M. 02/08/1969, L. 122/89, tipologia intervento, certificato, riferimento pratica, multipratica]
IDRegione: 2         # Piemonte
IDTipoPratica: 14
Fonte: Manuale
---

# Errori di validazione - Richiesta di Certificazione (RC)
## Regione Piemonte

Guida completa agli errori specifici per la **Richiesta di Certificazione edilizio-urbanistica** ai sensi dell'art. 3, comma 1, del D.P.R. 380/2001 e s.m.i. — Regione Piemonte.

{: .note }
> La RC è una pratica strutturalmente insolita nella piattaforma: non ha sezioni di titolarità, opere su parti comuni, date lavori, impresa o tecnici — la sua logica è tutta incentrata sul **riferimento alla pratica edilizia** oggetto della certificazione e sul **tipo di certificato** richiesto. La sezione "Riferimenti pratica" ha **due modalità di rendering alternative**, determinate a runtime dal sistema in base al contesto: la modalità **C** (Comunicazione) mostra una singola riga precompilata e in sola lettura; la modalità **P** (Pratica) mostra tre righe editabili in parallelo e richiede che almeno una dropdown sia selezionata, validando poi numero e data per ciascuna riga selezionata. Il messaggio di errore per la data nel ramo C recita "data di realizzazione dell'opera" anziché "data della pratica" — disallineamento semantico nel codice. La privacy è solo informativa. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Riferimenti alla pratica edilizia](#1-riferimenti-alla-pratica-edilizia)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Tipologia di certificato richiesto](#3-tipologia-di-certificato-richiesto)

---

## 1. Riferimenti alla pratica edilizia

Questa sezione funziona in due modalità alternative, attivate automaticamente dal sistema. L'utente non sceglie la modalità: viene determinata dal contesto della pratica.

---

### Modalità C — Comunicazione (riga singola precompilata)

La modalità C (`divPraticaRif_C`) è attiva quando il modulo RC è collegato a una comunicazione esistente. I campi sono **precompilati e in sola lettura** (`Enabled="false"`); la validazione verifica solo che i valori siano presenti.

---

#### ATTENZIONE ! Inserire la descrizione della pratica. *(modalità C — campo testo)*

**Causa**: Il campo `txtTipoPratica` (testo libero, visibile solo in alcuni casi della modalità C) è vuoto.

**Soluzione**: Inserisci la descrizione del tipo di pratica nel campo apposito. In modalità C questo campo di solito è precompilato dal sistema; se risulta vuoto, verifica che la pratica di riferimento sia stata correttamente collegata prima di aprire questo modulo.

---

#### ATTENZIONE ! Selezionare la descrizione della pratica. *(modalità C — dropdown)*

**Causa**: Il menu a discesa `cmbTipoPratica` è a indice 0 (nessuna selezione).

**Soluzione**: Seleziona il tipo di pratica dal menu a discesa **"tipo pratica"**. In modalità C questo menu è di solito precompilato dal sistema; se risulta vuoto, verifica il collegamento con la pratica di origine.

---

#### ATTENZIONE ! Inserire il numero della pratica.

**Causa**: Il campo **"n."** (numero pratica) è vuoto.

**Soluzione**: Inserisci il numero della pratica edilizia di riferimento nel campo **"n."**.

---

#### ATTENZIONE ! Inserire la data di realizzazione dell'opera.

**Dove si trova**: Campo **"presentata in data"** nella riga della modalità C

**Causa**: Il campo data della pratica è vuoto.

**Soluzione**: Inserisci la data nel campo **"presentata in data"** nel formato **GG/MM/AAAA**.

{: .warning }
> **Disallineamento semantico nel codice**: il messaggio recita "Inserire la data di **realizzazione dell'opera**" ma il campo si chiama **"presentata in data"** e si riferisce alla data di presentazione/deposito della pratica edilizia, non alla data di realizzazione. Il campo da compilare è inequivocabilmente quello della data accanto al numero pratica. Segnalare al team di sviluppo per correzione del testo del messaggio.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(modalità C)*

**Causa**: La data inserita nel campo "presentata in data" della modalità C non è in formato valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `10/06/2023` ✅, `10-06-2023` ❌).

---

### Modalità P — Pratica (fino a tre righe editabili)

La modalità P (`divPraticaRif_P`) è attiva quando la RC viene presentata autonomamente, non collegata a una comunicazione preesistente. Sono disponibili **tre righe in parallelo** (`_P1`, `_P2`, `_P3`), ciascuna con dropdown tipo pratica, numero e data. Il sistema richiede che **almeno una riga** abbia la dropdown selezionata; per ogni riga selezionata vengono poi richiesti numero e data.

---

#### ATTENZIONE ! Selezionare la descrizione della pratica. *(modalità P)*

**Causa**: Tutte e tre le dropdown `cmbTipoPratica_P1`, `_P2`, `_P3` sono a indice 0 (nessuna selezione in nessuna riga).

**Soluzione**: Seleziona il tipo di pratica in **almeno una** delle tre righe disponibili dalla dropdown **"tipo pratica"**. Per le righe rimanenti, se non servono, lascia la dropdown a zero — verranno ignorate dalla validazione.

{: .note }
> La validazione della modalità P raccoglie prima quali righe hanno la dropdown selezionata (costruisce la stringa `idxSel` concatenando "1", "2", "3"), poi per ciascuna riga selezionata verifica numero e data. Le righe con dropdown a zero vengono completamente saltate: non è necessario compilare tutte e tre le righe, una sola è sufficiente.

---

#### ATTENZIONE ! Inserire il numero della pratica. *(modalità P)*

**Causa**: Hai selezionato il tipo di pratica in una riga (`_P1`, `_P2` o `_P3`) ma non hai compilato il campo **"n."** della stessa riga.

**Soluzione**: Inserisci il numero della pratica edilizia nel campo **"n."** della riga in cui hai selezionato il tipo pratica. La riga con dropdown selezionata e campo numero vuoto blocca la validazione.

---

#### ATTENZIONE ! Inserire la data della pratica. *(modalità P)*

**Causa**: Hai selezionato tipo e numero di pratica in una riga ma non hai compilato il campo **"presentata in data"**.

**Soluzione**: Inserisci la data nel campo **"presentata in data"** della riga corrispondente, nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(modalità P)*

**Causa**: La data inserita in una delle righe attive (`_P1`, `_P2` o `_P3`) non è in formato valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `10/06/2023` ✅, `10-06-2023` ❌).

---

## 2. Localizzazione dell'intervento

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
3. Salva la riga con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 3. Tipologia di certificato richiesto

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipologia di certificato'.

**Dove si trova**: Sezione **"CHIEDE"** → radio button del tipo di certificato

**Causa**: Non hai selezionato il tipo di certificazione richiesta.

**Soluzione**: Seleziona **uno dei tre tipi di certificato** disponibili:
- ⚪ **"la tipologia di intervento edilizio in cui ricade la pratica edilizia inviata con riferimento alle definizioni di cui all'art. 3 c. 1 del D.P.R. 380/2001 e s.m.i."** — certifica la categoria di intervento (manutenzione ordinaria, straordinaria, ristrutturazione, nuova costruzione, ecc.)
- ⚪ **"pertinenza ai sensi dell'art. 11 c. 2 legge 122/89 e s.m.i."** — certifica che l'opera è pertinenza di un immobile principale
- ⚪ **"caratteristiche di lusso di cui al D.M. 02/08/1969"** — certifica le caratteristiche di lusso dell'immobile ai fini fiscali

{: .note }
> La scelta del tipo di certificato determina la natura del provvedimento che l'ufficio SUE emetterà. Selezionare la voce coerente con la finalità della richiesta (es. per agevolazioni fiscali prima casa: "tipologia di intervento"; per detrazioni parcheggi pertinenziali: "pertinenza art. 11 L. 122/89"). In caso di dubbio, consultare l'ufficio SUE prima di presentare la domanda.

---

## Consigli pratici Richiesta Certificazione

### Prima di validare ✅

**Modalità C** (riga precompilata — pratica collegata):
- [ ] Verifica che la **descrizione tipo pratica** sia presente (precompilata dal sistema)
- [ ] Verifica che il **numero pratica** sia presente (precompilato)
- [ ] Verifica che la **data pratica** sia presente e in formato GG/MM/AAAA (precompilata)

**Modalità P** (righe editabili — pratica autonoma):
- [ ] Seleziona il **tipo pratica** in almeno una delle tre righe dalla dropdown
- [ ] Per ogni riga con dropdown selezionata: inserisci **numero** e **data** (GG/MM/AAAA)
- [ ] Le righe con dropdown a zero vengono ignorate: non è necessario compilarle

**Entrambe le modalità**:
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona la **tipologia di certificato** (uno dei tre radio button)
- [ ] **Salva** frequentemente

### Logica di validazione modalità P ⚠️

La validazione della modalità P è **selettiva**: non richiede che tutte e tre le righe siano compilate, ma che almeno una lo sia. L'algoritmo funziona così:

1. Controlla se almeno una delle tre dropdown `_P1`, `_P2`, `_P3` ha un'opzione selezionata
2. Costruisce la stringa `idxSel` con i numeri delle righe selezionate (es. `"13"` se selezionate P1 e P3)
3. Per ogni numero in `idxSel`, verifica che numero e data della riga corrispondente siano compilati e validi
4. Righe con dropdown a zero vengono saltate interamente

| Situazione | Risultato |
|---|---|
| Tutte e tre le dropdown a zero | Errore: "Selezionare la descrizione della pratica" |
| Solo P1 selezionata, P2 e P3 a zero | OK se P1 ha numero e data validi |
| P1 e P3 selezionate, P2 a zero | Verifica numero e data di P1 e P3; P2 ignorata |
| P2 selezionata senza numero | Errore: "Inserire il numero della pratica" |

### Differenze tra modalità C e modalità P

| | Modalità C | Modalità P |
|---|---|---|
| Attivazione | Automatica (pratica collegata) | Automatica (presentazione autonoma) |
| Righe pratica | 1 (precompilata, in sola lettura) | Fino a 3 (editabili) |
| Tipo pratica | Dropdown o testo libero (visibile/nascosto a runtime) | Sempre dropdown |
| Messaggio errore data | "Inserire la data di realizzazione dell'opera" ⚠️ | "Inserire la data della pratica" |
| Controllo formato data | ☑ Sì (`ControlloFormatoData`) | ☑ Sì (`ControlloFormatoData`) |

### Errori frequenti RC 🔍

1. **Modalità non riconosciuta** → se i campi appaiono disabilitati (grigi), si è in modalità C: i valori sono precompilati dal sistema; verificare che la pratica di riferimento sia correttamente collegata
2. **Tutte le dropdown P a zero** → in modalità P, almeno una riga deve avere il tipo pratica selezionato
3. **Riga selezionata senza numero o data** → in modalità P, ogni riga con dropdown selezionata richiede entrambi i campi
4. **Nessun radio button certificato** → la sezione "CHIEDE" è l'ultimo controllo ma spesso dimenticata perché visivamente separata dalla sezione pratica

### Bug documentato: testo messaggio data modalità C

```vb
' Messaggio attuale (semanticamente errato):
pValidaDati &= "ATTENZIONE ! Inserire la data di realizzazione dell'opera."

' Testo corretto atteso:
pValidaDati &= "ATTENZIONE ! Inserire la data della pratica."
```

Il campo si chiama "presentata in data" nell'ASCX e si riferisce alla data di deposito/presentazione della pratica edilizia, non alla data di realizzazione dell'opera. Il messaggio non impedisce il corretto funzionamento ma può disorientare l'utente.

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
**Fonte**: Analisi codice `ValidaDatiRC` e `DatiRC.ascx`
