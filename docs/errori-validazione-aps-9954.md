---
title: Errori Autorizzazione Paesaggistica Semplificata - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 68
description: Errori di validazione per l'Autorizzazione Paesaggistica Semplificata (APS) Nazionale - Tutte le regioni (D.P.R. 13 febbraio 2017, n. 31, art. 146 D.Lgs. 42/2004)
keywords: [autorizzazione paesaggistica semplificata, APS, nazionale, tutte le regioni, DPR 31/2017, Allegato B, art. 136, art. 142, art. 134, D.Lgs. 42/2004, scheda semplificata Allegato D, vincolo paesaggistico, legge regionale]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 154 }  # Valle d'Aosta - Autorizzazione Paesaggistica Semplificata
  - { Reg: 6, Prat: 654 } # Veneto - Autorizzazione Paesaggistica Semplificata
  - { Reg: 8, Prat: 854 } # Emilia-Romagna - Autorizzazione Paesaggistica Semplificata
  - { Reg: 12, Prat: 1254 } # Lazio - Autorizzazione Paesaggistica Semplificata
  - { Reg: 13, Prat: 1354 } # Abruzzo - Autorizzazione Paesaggistica Semplificata
  - { Reg: 15, Prat: 1554 } # Campania - Autorizzazione Paesaggistica Semplificata
  - { Reg: 16, Prat: 1654 } # Basilicata - Autorizzazione Paesaggistica Semplificata
  - { Reg: 17, Prat: 1754 } # Puglia - Autorizzazione Paesaggistica Semplificata
  - { Reg: 18, Prat: 1854 } # Calabria - Autorizzazione Paesaggistica Semplificata
  - { Reg: 19, Prat: 1954 } # Sicilia - Autorizzazione Paesaggistica Semplificata
Fonte: Manuale
---

# Errori di validazione - Autorizzazione Paesaggistica Semplificata (A.P.S.)
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per l'**Autorizzazione Paesaggistica Semplificata (APS) Nazionale** ai sensi dell'art. 3 del D.M. n. 31 del 13 febbraio 2017 (D.P.R. 31/2017) e dell'art. 146 del D.Lgs. 22 gennaio 2004, n. 42 (Codice dei beni culturali e del paesaggio).

{: .note }
> L'APS Nazionale ha una struttura diversa rispetto alle versioni regionali ([Piemonte](errori-aps-piemonte.html), [Lombardia](errori-aps-lombardia.html), [Liguria](errori-aps-liguria.html)). Non ha radio Titolarità, radio Contributo, Impresa o Sicurezza. La sezione "Titolarità" è presente solo come menu non validato. La particolarità principale è la sezione **"Opere"** — con articolo e legge regionale — che è **sempre obbligatoria** (non condizionale), a differenza delle versioni regionali. La sezione **Vincolo** richiede almeno una delle 3 checkbox, ma solo se si sceglie `chkVincolo1` (art. 136) si attivano ulteriori campi obbligatori (lettera e estremi del provvedimento). L'intera scheda del professionista redattore è presente ma non validata. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Descrizione sintetica dell'intervento](#2-descrizione-sintetica-dellintervento)
3. [Riconducibilità](#3-riconducibilità)
4. [Documentazione tecnica allegata](#4-documentazione-tecnica-allegata)
5. [Vincolo paesaggistico — Normativa di riferimento](#5-vincolo-paesaggistico--normativa-di-riferimento)
6. [Opere — Legge regionale di competenza](#6-opere--legge-regionale-di-competenza)
7. [Variante o rinnovo](#7-variante-o-rinnovo)

---

## 1. Localizzazione dell'intervento

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
> Il menu `cmbTitoloSuImm` nella sezione "Titolarità dell'intervento" è presente ma **non validato**. L'APS Nazionale è una delle poche pratiche senza radio `$Titolarita` — la titolarità è gestita solo tramite menu.

---

## 2. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "CHIEDE — Descrizione sintetica dell'intervento" → campo multiriga `txtDescrIntervento` (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione sintetica delle opere di lieve entità per cui si richiede l'autorizzazione paesaggistica (max **300 caratteri**).

---

## 3. Riconducibilità

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Riconducibilità'.

**Dove si trova**: Sezione "Descrizione sintetica" → 2 radio button `$Riconducibilita`

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **c_1** — "riconducibile alla voce ___ dell'Allegato B D.P.R. 13 febbraio 2017, n. 31" → inserisci la lettera/voce nel campo `txtVoceAllegatoB`
- ⚪ **c_2** — "riconducibile all'art. 7, c. 1 e 3, del D.P.R. 31/2017"

{: .note }
> Il D.P.R. 31/2017 distingue due percorsi: l'intervento può ricadere nell'Allegato B (elenco specifico di categorie di interventi di lieve entità) oppure nell'art. 7 c. 1 e 3 (interventi su immobili non soggetti a specifiche limitazioni o con caratteristiche particolari). La scelta dipende dalla tipologia dell'opera e dalla natura del vincolo paesaggistico.

---

### ATTENZIONE ! Specificare lettera Allegato B.

**Causa**: Hai selezionato `rdbRiconducibilitac_1` ma il campo `txtVoceAllegatoB` è vuoto.

**Soluzione**: Inserisci la lettera o il numero identificativo della voce dell'**Allegato B** del D.P.R. 31/2017 a cui l'intervento è riconducibile (es. `A.1`, `B.3`, ecc.).

---

## 4. Documentazione tecnica allegata

### ATTENZIONE ! Selezionare almeno una tipologia di documentazione tecnica.

**Dove si trova**: Sezione "Descrizione sintetica" → 2 checkbox dopo "così come indicato nella documentazione tecnica allegata composta da:"

**Causa**: Nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkDocTecne_1_4** — "scheda semplificata di cui all'Allegato D (non barrare nei casi previsti dall'art. 7, c.3)"
- ☐ **chkDocTecne_1_5** — "elaborati di progetto"

{: .note }
> Per gli interventi di cui all'art. 7 c. 1 (riconducibilità c_2) non è necessaria la scheda semplificata — si usa solo `chkDocTecne_1_5`. Per gli interventi dell'Allegato B (c_1) si usa in genere `chkDocTecne_1_4`. Entrambe possono essere spuntate contemporaneamente se necessario.

---

## 5. Vincolo paesaggistico — Normativa di riferimento

### ATTENZIONE ! Nessuna voce relativa a normativa di riferimento è stata indicata.

**Dove si trova**: Sezione "DICHIARAZIONI" → 3 checkbox per la normativa di tutela paesaggistica

**Causa**: Nessuna delle 3 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 3 normative di riferimento:
- ☐ **chkVincolo1** — "dell'art. 136, c. 1, lett. ___) del d.lgs. n. 42/2004" → inserisci la lettera e gli estremi del provvedimento
- ☐ **chkVincolo2** — "dell'art. 142, c. 1, lett. ___) del d.lgs. n. 42/2004" → il campo lettera (`txtVincolo2`) è presente ma **non validato**
- ☐ **chkVincolo3** — "dell'art. 134, c. 1, lett. c) del d.lgs. n. 42/2004" → nessun campo aggiuntivo

{: .note }
> L'art. 136 del D.Lgs. 42/2004 riguarda i beni paesaggistici dichiarati di notevole interesse pubblico con provvedimento amministrativo (d.m. o d.g.r.); l'art. 142 riguarda le aree tutelate per legge (laghi, fiumi, boschi, coste, ecc.); l'art. 134 lett. c) riguarda i beni tutelati dai piani paesaggistici. La scelta dipende dal tipo di vincolo che grava sull'immobile.

---

### ATTENZIONE ! Inserire la lettera relativa all'articolo 136.

**Causa**: `chkVincolo1` è spuntata ma `txtVincolo1` (campo lettera) è vuoto.

**Soluzione**: Inserisci la lettera della fattispecie dell'art. 136 c. 1 del D.Lgs. 42/2004 applicabile al vincolo (le fattispecie sono: a = bellezze naturali; b = ville/giardini; c = complessi di cose immobili; d = bellezze panoramiche).

---

### ATTENZIONE ! Inserire estremi del provvedimento - d.m./d.g.r.

**Causa**: `chkVincolo1` è spuntata e la lettera è compilata, ma `txtEstremiProvvedimento` è vuoto.

**Soluzione**: Inserisci gli estremi del provvedimento che ha dichiarato il bene di notevole interesse pubblico (es. "d.m. 15/04/1960" o "d.g.r. n. 123 del 01/01/2000") nel campo placeholder "(citare estremi del provvedimento - d.m./d.g.r.)".

{: .note }
> A differenza di `chkVincolo1`, la checkbox `chkVincolo2` (art. 142) ha un campo lettera affiancato (`txtVincolo2`) che **non viene validato** dal codice — può essere lasciato vuoto anche se la checkbox è spuntata.

---

## 6. Opere — Legge regionale di competenza

La sezione "Opere" è **sempre obbligatoria** in questa versione Nazionale, indipendentemente da qualsiasi altra selezione. Questa è la principale differenza rispetto alle versioni regionali dell'APS (Piemonte, Lombardia, Liguria) dove la sezione Opere non esiste o è strutturata diversamente.

---

### ATTENZIONE ! Inserire l'articolo della Legge regionale relativa alle Opere.

**Dove si trova**: Sezione "Opere" → campo `txtOpereArt` "che le opere previste sono attribuite alla competenza di codesta Amministrazione ai sensi dell'art. ___"

**Causa**: Il campo dell'articolo è vuoto.

**Soluzione**: Inserisci il numero dell'articolo della legge regionale che attribuisce la competenza per le opere paesaggistiche di questo tipo all'amministrazione ricevente (es. `3` per D.M. 31/2017 o l'articolo della legge regionale specifica). Se in dubbio, consultare l'ufficio competente.

---

### ATTENZIONE ! Inserire la Legge regionale di riferimento.

**Dove si trova**: Campo `txtLeggeReg` "della legge regionale ___"

**Causa**: Il campo della legge regionale è vuoto.

**Soluzione**: Inserisci il riferimento normativo completo della legge regionale (es. "L.R. 15 aprile 1975, n. 33" oppure il D.M. o D.P.R. di riferimento qualora non esista specifica legge regionale).

{: .note }
> La sezione "Opere" è specifica della versione Nazionale e non ha equivalenti diretti nelle versioni regionali del sistema. La legge regionale da indicare dipende dalla Regione in cui si trova l'immobile e dalla normativa paesaggistica regionale vigente. Per interventi in cui non esiste una specifica legge regionale, indicare il decreto ministeriale o provvedimento statale applicabile.

---

## 7. Variante o rinnovo

La sezione "In caso di intervento di variante o di rinnovo" si attiva solo se si spunta `chkInterventoVariante`. Se non spuntata, nessun campo è richiesto.

---

### ATTENZIONE ! Inserire l'Ente che ha rilasciato l'autorizzazione.

**Causa**: `chkInterventoVariante` è spuntata ma `txtEnteRilascio` è vuoto.

**Soluzione**: Inserisci il nome dell'ente che ha rilasciato la precedente autorizzazione paesaggistica (es. "Comune di XXX", "Soprintendenza ABAP di XXX").

---

### ATTENZIONE ! Inserire il numero dell'autorizzazione rilasciata.

**Causa**: Il campo `txtAutPaes` è vuoto.

**Soluzione**: Inserisci il numero della precedente autorizzazione paesaggistica.

---

### ATTENZIONE ! Inserire la data di rilascio dell'autorizzazione.

**Causa**: Il campo `txtDataAutPaes` è vuoto.

**Soluzione**: Inserisci la data di rilascio nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data autorizzazione)

**Causa**: La data dell'autorizzazione non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `20/03/2022`).

---

## Consigli pratici — APS Nazionale

### Prima di validare ✅

- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **descrizione** dell'intervento (max 300 caratteri)
- [ ] Seleziona la **riconducibilità** (c_1 Allegato B o c_2 art. 7); se c_1: inserisci la **voce dell'Allegato B**
- [ ] Spunta almeno una delle 2 **tipologie di documentazione** (scheda Allegato D e/o elaborati di progetto)
- [ ] Spunta almeno una delle 3 **checkbox vincolo** (art. 136/142/134); se chkVincolo1: inserisci **lettera** e **estremi del provvedimento**
- [ ] Inserisci l'**articolo** della legge regionale competente per le opere
- [ ] Inserisci la **legge regionale** di riferimento
- [ ] Se è una variante/rinnovo: spunta `chkInterventoVariante` e inserisci **ente**, **numero** e **data** (GG/MM/AAAA) dell'autorizzazione precedente

### Campi presenti ma non validati ℹ️

`cmbTitoloSuImm` (titolarità menu), `txtVincolo2` (lettera art. 142), tutta la scheda professionista redattore (`txtRedattore`, `txtComuneSede`, `txtViaSede`, `txtCivicoSede`, `txtTelFaxSede`, `txtEMailSede`, `txtNIscrOrdine`, `txtProvOrdColl`), privacy solo testo informativo.

### Differenze rispetto alle versioni regionali ⚠️

Rispetto alle versioni [APS Piemonte](errori-aps-piemonte.html), [APS Lombardia](errori-aps-lombardia.html) e [APS Liguria](errori-aps-liguria.html): nessun radio `$Titolarita`; sezione "Opere" sempre obbligatoria con articolo + legge regionale; solo 2 checkbox documentazione tecnica invece di 4 checkbox vincolo regionali; chkVincolo1 richiede lettera + estremi provvedimento; la scheda del professionista redattore è presente ma non validata; nessuna coordinata UTM (a differenza della versione Lombardia).

### Errori frequenti 🔍

1. **Riconducibilità c_1 senza voce Allegato B** → il campo `txtVoceAllegatoB` si abilita solo dopo aver selezionato il radio c_1; verificare che il radio sia selezionato e inserire la voce
2. **Nessuna tipologia documentazione spuntata** → obbligatoria almeno una delle 2 checkbox; verificare dopo aver compilato la riconducibilità
3. **chkVincolo1 senza lettera o estremi** → entrambi i campi sono obbligatori se l'art. 136 è selezionato; `txtVincolo2` invece non è validato
4. **Sezione Opere vuota** → a differenza delle versioni regionali, articolo e legge regionale sono sempre obbligatori nella versione Nazionale
5. **Variante spuntata senza dati** → tutti e 3 i campi (ente, numero, data) sono obbligatori e la data deve essere in formato GG/MM/AAAA

---

## Non trovi l'errore? 🆘

1. **Cerca in questa guida** con Ctrl+F (copia/incolla il messaggio esatto)
2. Vedi versioni regionali: [APS Piemonte](errori-aps-piemonte.html) — [APS Lombardia](errori-aps-lombardia.html) — [APS Liguria](errori-aps-liguria.html)
3. Verifica [Errori Comuni](errori-validazione.html#errori-comuni)
4. Contatta [Assistenza](assistenza-tecnica.html)

---

## Prossimi passi

- [Errori comuni](errori-validazione.html#errori-comuni) - Errori validi per tutte le pratiche
- [Troubleshooting](troubleshooting.html) - Problemi tecnici
- [Assistenza tecnica](assistenza-tecnica.html) - Contatti supporto

---

**Ultima revisione**: Aprile 2026
**Fonte**: Analisi codice ValidaDatiAPSNaz e DatiAPSNaz.ascx
