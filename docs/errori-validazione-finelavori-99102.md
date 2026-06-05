---
title: Errori Fine Lavori - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 51
description: Errori di validazione specifici per la Comunicazione di Fine Lavori Nazionale - Tutte le regioni
keywords: [fine lavori, comunicazione fine lavori, ultimazione lavori, nazionale, tutte le regioni, tipo ultimazione, titolo legittimante, prot.]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 1102 }  # Valle d'Aosta - Fine Lavori
  - { Reg: 6, Prat: 6102 } # Veneto - Fine Lavori
  - { Reg: 8, Prat: 8102 } # Emilia-Romagna - Fine Lavori
  - { Reg: 12, Prat: 12102 } # Lazio - Fine Lavori
  - { Reg: 13, Prat: 13102 } # Abruzzo - Fine Lavori
  - { Reg: 15, Prat: 15102 } # Campania - Fine Lavori
  - { Reg: 16, Prat: 16102 } # Basilicata - Fine Lavori
  - { Reg: 17, Prat: 17102 } # Puglia - Fine Lavori
  - { Reg: 18, Prat: 18102 } # Calabria - Fine Lavori
  - { Reg: 19, Prat: 19102 } # Sicilia - Fine Lavori
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Fine Lavori
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per la **Comunicazione di Fine Lavori** applicabile su tutto il territorio nazionale, relativa ai lavori eseguiti in base a permesso di costruire, SCIA o altro titolo edilizio.

{: .note }
> La Fine Lavori Nazionale è una delle pratiche più semplici del sistema. Ha pochissimi campi obbligatori: localizzazione standard, data di ultimazione lavori, modalità di ultimazione (completa o parziale), e i dati del titolo che ha legittimato l'intervento (tipo + prot./n. + data). A differenza di quasi tutte le altre pratiche, la **data di fine lavori** e la **data del protocollo** del titolo vengono verificate solo come "non vuoto" — il formato GG/MM/AAAA non è controllato. Non sono richiesti tecnici, imprese o coordinate. La privacy è solo un testo informativo statico. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Data ultimazione e tipo di ultimazione](#2-data-ultimazione-e-tipo-di-ultimazione)
3. [Titolo legittimante l'intervento](#3-titolo-legittimante-lintervento)

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
> Il campo "Coordinate" (`txtCoordinate`) è presente nel modulo come campo testo libero ma **non viene validato** — non genera errori se vuoto.

---

## 2. Data ultimazione e tipo di ultimazione

### ATTENZIONE ! Inserire la data di ultimazione lavori.

**Dove si trova**: Sezione "COMUNICA" → campo "che in data ___ i lavori sono stati ultimati" (`txtDataFineLavori`)

**Causa**: Il campo della data di fine lavori è vuoto.

**Soluzione**: Inserisci nel campo la data in cui i lavori sono stati ultimati.

{: .note }
> A differenza di quasi tutte le altre pratiche GeoTecSUE, la data di ultimazione lavori viene verificata solo come "non vuoto" — **il formato GG/MM/AAAA non viene controllato**. Un valore come `marzo 2024` o `2024` supera la validazione. È comunque buona prassi inserire la data nel formato standard GG/MM/AAAA per la correttezza documentale.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Ultimazione lavori'.

**Dove si trova**: Sezione "COMUNICA" → 2 radio button sotto la data di ultimazione

**Causa**: Non hai indicato se i lavori sono stati ultimati completamente o parzialmente.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbTipoUltimazionea_1** — "completamente"
- ⚪ **rdbTipoUltimazionea_2** — "in forma parziale come da planimetria allegata"

---

## 3. Titolo legittimante l'intervento

### ATTENZIONE ! Indicare il tipo di pratica.

**Dove si trova**: Sezione "COMUNICA" → campo testo `txtTipoPratica` sotto "che il titolo e/o comunicazione che ha legittimato l'intervento è il seguente:"

**Causa**: Il campo del tipo di pratica/titolo è vuoto.

**Soluzione**: Inserisci nel campo testo il tipo di titolo edilizio che ha legittimato l'intervento (es. `Permesso di Costruire`, `SCIA`, `SCIA alternativa al PdC`, `CILA`).

---

### ATTENZIONE ! Campo obbligatorio 'Prot. / N.' non inserito.

**Dove si trova**: Campo "prot. / n." (`txtNProt`) affiancato al tipo di pratica

**Causa**: Il campo del numero di protocollo o numero del titolo è vuoto.

**Soluzione**: Inserisci il numero di protocollo o il numero identificativo del titolo edilizio di riferimento (es. `123/2022`, `PdC n. 45`).

---

### ATTENZIONE ! Campo obbligatorio 'Data' non inserita.

**Dove si trova**: Campo "del" (`txtDataProt`) affiancato al prot./n.

**Causa**: Il campo della data del titolo è vuoto.

**Soluzione**: Inserisci la data del titolo edilizio nel campo "del".

{: .note }
> Anche la data del titolo legittimante viene verificata solo come "non vuoto" — **il formato GG/MM/AAAA non viene controllato**. Inserire il formato corretto è comunque raccomandato.

---

## Consigli pratici — Fine Lavori Nazionale

### Prima di validare ✅

- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data di ultimazione lavori**
- [ ] Seleziona il **tipo di ultimazione** (completa o parziale)
- [ ] Inserisci il **tipo di pratica** del titolo legittimante (es. `Permesso di Costruire`)
- [ ] Inserisci il **prot./n.** del titolo
- [ ] Inserisci la **data** del titolo

### Campi presenti ma non validati ℹ️

- **`txtCoordinate`** (campo testo "Coordinate"): presente ma non validato
- **`txtData` e `txtLuogo`** (data e luogo firma in calce): facoltativi, non validati
- **Privacy**: testo informativo statico, nessuna checkbox, nessun errore
- **Tecnici e imprese**: non richiesti per questa pratica

### Date non verificate nel formato ⚠️

Sia `txtDataFineLavori` che `txtDataProt` vengono controllate solo come "non vuoto". Questo è inusuale rispetto alla quasi totalità delle altre pratiche GeoTecSUE che verificano sempre il formato GG/MM/AAAA. Inserire il formato standard è comunque corretto e previene possibili problemi nelle fasi successive di protocollazione.

### Errori frequenti 🔍

1. **Campo tipo pratica lasciato vuoto** → è un campo testo libero (non un menu) e viene spesso ignorato; descrivere il tipo di titolo usato per l'intervento
2. **Data fine lavori vuota** → nonostante non verifichi il formato, il campo deve contenere qualcosa; inserire la data effettiva di ultimazione
3. **Nessun radio ultimazione selezionato** → i due radio button (completa / parziale) vengono validati dopo la data; verificarli entrambi

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
**Fonte**: Analisi codice ValidaDatiFineLavoriNazionale e DatiFineLavoriNaz.ascx
