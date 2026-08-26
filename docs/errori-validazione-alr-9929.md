---
title: Errori Attività Libera Fonti Rinnovabili - Tutte le regioni
parent: Errori di validazione
nav_order: 35
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori per Attività Libera per la Produzione di Energia da Fonti Rinnovabili (ALR) - Tutte le regioni
keywords: [attività libera fonti rinnovabili, ALR, D.Lgs. 190/2024, energia rinnovabile, nuova costruzione, impianti esistenti, variante in corso d'opera, comunicazione inizio lavori, data inizio lavori futura, impresa esecutrice, altri atti di assenso]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9928
IDTarget:
  - { Reg: 2, Prat: 28 }   # Piemonte - ALR
  - { Reg: 1, Prat: 128 }   # Valle d'Aosta - ALR
  - { Reg: 3, Prat: 328 }   # Liguria - ALR
  - { Reg: 4, Prat: 428 }   # Lombardia - ALR
  - { Reg: 6, Prat: 628 }   # Veneto - ALR
  - { Reg: 8, Prat: 828 }   # Emilia-Romagna - ALR
  - { Reg: 12, Prat: 1228 }  # Lazio - ALR
  - { Reg: 13, Prat: 1328 }  # Abruzzo - ALR
  - { Reg: 15, Prat: 1528 }  # Campania - ALR
  - { Reg: 16, Prat: 1628 }  # Basilicata - ALR
  - { Reg: 17, Prat: 1728 }  # Puglia - ALR
  - { Reg: 18, Prat: 1828 }  # Calabria - ALR
  - { Reg: 19, Prat: 1928 }  # Sicilia - ALR
Fonte: Manuale
---

# Errori di validazione - Attività Libera per la Produzione di Energia da Fonti Rinnovabili (A.L.R.)
## Tutte le regioni

Guida completa agli errori specifici per la **Comunicazione di Attività Libera per la Produzione di Energia da Fonti Rinnovabili** ai sensi dell'art. 7 del D.Lgs. 25 novembre 2024, n. 190 (Allegato A).

{: .note }
> L'ALR è stata **completamente rivista** con il recepimento del decreto 15 Luglio 2016 n. 223 del Ministero dell'Ambiente e della Sicurezza Energetica. 

---

## Indice sezioni

1. [Classificazione dell'intervento — impianto ibrido o singolo](#1-classificazione-dellintervento--impianto-ibrido-o-singolo)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Area agricola e SAU](#3-area-agricola-e-sau)
4. [Area idonea — art. 11-bis D.Lgs. 190/2024](#4-area-idonea--art-11-bis-dlgs-1902024)
5. [Zone di accelerazione — art. 12 D.Lgs. 190/2024](#5-zone-di-accelerazione--art-12-dlgs-1902024)
6. [Titolo edilizio](#6-titolo-edilizio)
7. [Data e luogo](#7-data-e-luogo)

---

## 1. Classificazione dell'intervento — impianto ibrido o singolo

### ATTENZIONE ! Non è stata selezionata nessuna voce per la classificazione dell'intervento.

**Dove si trova**: Sezione **"COMUNICA"** → i due radio button principali in cima al modulo

**Causa**: Non hai selezionato se l'intervento è un impianto ibrido oppure un intervento singolo.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"un intervento classificato come impianto ibrido"** ai sensi dell'art. 4, c. 1 del D.Lgs. 190/2024, composto da più interventi di cui all'Allegato A → si attivano fino a 5 righe di sotto-interventi (vedi sotto)
- ⚪ **intervento singolo** di cui all'Allegato A del D.Lgs. 190/2024 → si attivano i tre campi sezione, lettera e descrizione (vedi sotto)

---

### Impianto ibrido (fino a 5 sotto-interventi)

Se selezioni **impianto ibrido**, devi spuntare **almeno uno** dei 5 checkbox disponibili. Per ogni checkbox spuntato diventano obbligatori tre campi: **Sezione**, **Lettera** e **Descrizione**.

---

#### ATTENZIONE ! Selezionare almeno un intervento di cui all'Allegato A.

**Causa**: Hai selezionato **impianto ibrido** ma non hai spuntato nessuno dei 5 checkbox sotto-intervento.

**Soluzione**: Spunta **almeno uno** dei 5 checkbox delle righe di sotto-intervento, poi compila i tre campi della riga:
- **Sezione** — sezione dell'Allegato A del D.Lgs. 190/2024 (es. `I`, `II`)
- **Lettera** — lettera del comma (es. `a`, `b`, `c`)
- **Descrizione** — descrizione sintetica dell'intervento (es. `Impianto fotovoltaico su tetto 6 kWp`)

---

#### ATTENZIONE ! Indicare la sezione.

**Causa**: Hai spuntato il checkbox ma il campo **"Sezione"** della riga corrispondente è vuoto.

**Soluzione**: Inserisci la sezione dell'Allegato A nel campo **"Sezione"** della riga spuntata (es. `I` per Sezione I — nuove costruzioni, `II` per Sezione II — impianti esistenti).

---

#### ATTENZIONE ! Indicare la lettera.

**Causa**: Hai spuntato il checkbox e compilato la sezione, ma il campo **"Lettera"** è vuoto.

**Soluzione**: Inserisci la lettera nel campo **"Lettera"** (es. `a`, `b`, `c`). Consulta l'Allegato A del D.Lgs. 190/2024 per individuare la lettera corrispondente alla tipologia dell'impianto.

---

#### ATTENZIONE ! Indicare la descrizione.

**Causa**: Hai spuntato il checkbox, compilato sezione e lettera, ma il campo **"Descrizione"** è vuoto.

**Soluzione**: Inserisci una descrizione sintetica dell'intervento nel campo **"Descrizione"** della riga corrispondente (es. `Impianto fotovoltaico su falda tetto 6 kWp`, `Sistema di accumulo 10 kWh`).

{: .note }
> La validazione verifica i checkbox nell'ordine 1 → 5. Per ogni checkbox spuntato controlla prima Sezione, poi Lettera, poi Descrizione, poi passa al checkbox successivo. I checkbox non spuntati vengono saltati interamente. Per un impianto ibrido con 2 tipologie, è sufficiente spuntare 2 dei 5 checkbox e compilare i rispettivi 6 campi (3 per ciascuno).

---

### Intervento singolo Allegato A

Se selezioni **intervento singolo**, diventano obbligatori tre campi nella riga che si attiva.

---

#### ATTENZIONE ! Indicare la sezione. *(intervento singolo)*

**Causa**: Hai selezionato **intervento singolo** ma il campo **"Sezione"** è vuoto.

**Soluzione**: Inserisci la sezione dell'Allegato A nel campo **"Sezione"** (es. `I`, `II`).

---

#### ATTENZIONE ! Indicare la lettera. *(intervento singolo)*

**Causa**: Hai compilato la sezione ma il campo **"Lettera"** è vuoto.

**Soluzione**: Inserisci la lettera nel campo **"Lettera"** (es. `a`, `b`, `c`).

---

#### ATTENZIONE ! Indicare la descrizione. *(intervento singolo)*

**Causa**: Hai compilato sezione e lettera ma il campo **"Descrizione"** è vuoto.

**Soluzione**: Inserisci una descrizione sintetica dell'intervento nel campo **"Descrizione"** (es. `Impianto fotovoltaico integrato in copertura 20 kWp`).

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
3. Salva con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 3. Area agricola e SAU

### ATTENZIONE ! Indicare se la tipologia/classificazione dell'area/superficie oggetto di intervento corrisponde ad un'area agricola (si/no).

**Dove si trova**: Sezione dichiarazioni → radio button relativo all'Area Agricola

**Causa**: Non hai dichiarato se l'area oggetto dell'intervento è classificata come area agricola.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — l'area è agricola → si attiva il campo SAU obbligatorio (vedi sotto)
- ⚪ **no** — l'area non è agricola

---

### ATTENZIONE ! Indicare la Superficie Agricola Utilizzata (SAU).

**Causa**: Hai selezionato "sì" (area agricola) ma non hai compilato il campo **SAU**.

**Soluzione**: Inserisci la superficie agricola utilizzata in ettari nel campo che si attiva (es. `2.5`, `10`, `0.8`). La SAU è la superficie effettivamente utilizzata per la produzione agricola, al netto di boschi, incolti e fabbricati.

{: .note }
> Il campo SAU si attiva **solo se si seleziona "sì"** al radio button area agricola. Se si seleziona "no", il campo non compare e non è richiesto. La dichiarazione sull'area agricola è rilevante ai fini dell'applicazione dell'art. 20-bis del D.Lgs. 199/2021 e delle norme regionali sugli impianti agrivoltaici.

---

## 4. Area idonea — art. 11-bis D.Lgs. 190/2024

### ATTENZIONE ! Indicare se l'intervento ricade in area idonea ai sensi dell'art. 11 bis del D.Lgs 190/2024 ai sensi della normativa vigente (si/no).

**Dove si trova**: Sezione dichiarazioni → radio button Area Idonea

**Causa**: Non hai dichiarato se il sito dell'intervento ricade in un'area idonea ai sensi dell'art. 11-bis del D.Lgs. 190/2024.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — l'intervento ricade in area idonea
- ⚪ **no** — l'intervento non ricade in area idonea

{: .note }
> Le "aree idonee" ai sensi dell'art. 11-bis del D.Lgs. 190/2024 sono definite dai Piani Nazionali e Regionali per la transizione energetica (PNIEC, PITESAI, piani regionali). La classificazione è verificabile sul portale cartografico del MASE o sui geoportali regionali. La dichiarazione non attiva campi aggiuntivi: è sufficiente la selezione sì/no.

---

## 5. Zone di accelerazione — art. 12 D.Lgs. 190/2024

### ATTENZIONE ! Indicare se l'intervento ricade in zone di accelerazione ai sensi dell'art. 12 del D.Lgs 190/2024 (si/no).

**Dove si trova**: Sezione dichiarazioni → radio button Zone Accelerazione

**Causa**: Non hai dichiarato se il sito dell'intervento ricade in una zona di accelerazione ai sensi dell'art. 12 del D.Lgs. 190/2024.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — l'intervento ricade in zona di accelerazione
- ⚪ **no** — l'intervento non ricade in zona di accelerazione

{: .note }
> Le "zone di accelerazione" ai sensi dell'art. 12 del D.Lgs. 190/2024 sono aree prioritarie per l'installazione di impianti rinnovabili, identificate da piani regionali e nazionali. Come per l'area idonea, la dichiarazione non attiva campi aggiuntivi.

---

## 6. Titolo edilizio

### ATTENZIONE ! Indicare se l'intervento necessita di titolo edilizio (si/no).

**Dove si trova**: Sezione **"Titolo edilizio"** → radio button Titolo Edilizio

**Causa**: Non hai dichiarato se l'intervento necessita di un titolo edilizio.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — l'intervento necessita di titolo edilizio → si attivano il campo Comune e la selezione del tipo di titolo (vedi sotto)
- ⚪ **no** — l'intervento non necessita di titolo edilizio

---

### ATTENZIONE ! Indicare il Comune da cui si è ottenuto il titolo edilizio.

**Causa**: Hai selezionato "sì" (necessita titolo edilizio) ma non hai inserito il Comune che ha rilasciato il titolo.

**Soluzione**: Inserisci il nome del Comune nel campo **"Comune"** che si attiva accanto al radio button.

---

### ATTENZIONE ! Indicare almeno un titolo edilizio.

**Causa**: Hai selezionato "sì" e inserito il Comune, ma non hai selezionato il tipo di titolo edilizio.

**Soluzione**: Seleziona **uno dei quattro tipi** di titolo edilizio tra i radio button che si attivano:
- ⚪ **CIL** → inserisci data e numero
- ⚪ **CILA** → inserisci data e numero
- ⚪ **SCIA alternativa al PdC** → inserisci data e numero
- ⚪ **PdC** (Permesso di Costruire) → inserisci data e numero

Per il tipo selezionato diventano obbligatori **data** (formato GG/MM/AAAA) e **numero** del titolo.

---

### CIL — Comunicazione di Inizio Lavori

#### ATTENZIONE ! Indicare la data della CIL. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Hai selezionato CIL ma il campo data è vuoto o in formato non valido.

**Soluzione**: Inserisci la data della CIL nel formato **GG/MM/AAAA**.

#### ATTENZIONE ! Indicare il numero della CIL.

**Causa**: Hai inserito la data della CIL ma il campo numero è vuoto.

**Soluzione**: Inserisci il numero della CIL nel campo **"numero"**.

---

### CILA — Comunicazione di Inizio Lavori Asseverata

#### ATTENZIONE ! Indicare la data della CILA. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Hai selezionato CILA ma il campo data è vuoto o in formato non valido.

**Soluzione**: Inserisci la data della CILA nel formato **GG/MM/AAAA**.

#### ATTENZIONE ! Indicare il numero della CILA.

**Causa**: Hai inserito la data ma il campo numero è vuoto.

**Soluzione**: Inserisci il numero della CILA nel campo **"numero"**.

---

### SCIA alternativa al PdC

#### ATTENZIONE ! Indicare la data della SCIA Alternativa al PdC. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Hai selezionato SCIA alternativa al PdC ma il campo data è vuoto o in formato non valido.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

#### ATTENZIONE ! Indicare il numero della SCIA Alternativa al PdC.

**Causa**: Il campo numero è vuoto.

**Soluzione**: Inserisci il numero della SCIA alternativa al PdC.

---

### PdC — Permesso di Costruire

#### ATTENZIONE ! Indicare la data del PdC. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: Hai selezionato PdC ma il campo data è vuoto o in formato non valido.

**Soluzione**: Inserisci la data del PdC nel formato **GG/MM/AAAA**.

#### ATTENZIONE ! Indicare il numero del PdC.

**Causa**: Il campo numero è vuoto.

**Soluzione**: Inserisci il numero del Permesso di Costruire.

---

## 7. Data e luogo

### ATTENZIONE ! Inserire la data. / ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Dove si trova**: Riquadro in fondo al modulo → campo Data

**Causa**: Il campo data di sottoscrizione è vuoto oppure in formato non valido.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**. Puoi usare l'icona calendario.

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Campo Luogo accanto alla data

**Causa**: Il campo luogo di sottoscrizione è vuoto.

**Soluzione**: Inserisci il Comune in cui viene sottoscritta la comunicazione.

{: .note }
> Come nella PAS, nell'ALR sia **data** (con verifica formato) sia **luogo** sono obbligatori e validati. Sono gli ultimi due controlli della funzione — verificarli prima di cliccare "Valida e Salva".

---

## Consigli pratici ALR

### Prima di validare ✅

- [ ] Seleziona la **classificazione intervento** (impianto ibrido c2_1 o singolo c2_2)
- [ ] **Se impianto ibrido (c2_1)**: spunta **almeno un checkbox** (1–5) e per ciascuno inserisci **Sezione**, **Lettera**, **Descrizione**
- [ ] **Se intervento singolo (c2_2)**: inserisci **Sezione**, **Lettera**, **Descrizione**
- [ ] Seleziona l'**indirizzo** (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Dichiara se l'area è **agricola** (sì/no)
- [ ] **Se area agricola = sì**: inserisci la **SAU** in ettari
- [ ] Dichiara se ricade in **area idonea** art. 11-bis (sì/no)
- [ ] Dichiara se ricade in **zone di accelerazione** art. 12 (sì/no)
- [ ] Dichiara se necessita di **titolo edilizio** (sì/no)
- [ ] **Se titolo edilizio = sì**: inserisci il **Comune** + seleziona il **tipo titolo** (CIL/CILA/SCIA alt./PdC) + inserisci **data** (GG/MM/AAAA) e **numero**
- [ ] Inserisci la **data** di sottoscrizione (GG/MM/AAAA)
- [ ] Inserisci il **luogo** di sottoscrizione
- [ ] **Salva** frequentemente

### Errori frequenti ALR 🔍

1. **Nessun checkbox impianto ibrido spuntato** → selezionare c2_1 non è sufficiente: occorre spuntare almeno uno dei 5 checkbox e compilare i 3 campi
2. **Checkbox 5 con focus errato** → se il 5° sotto-intervento ha Sezione o Lettera vuote, il cursore va al campo del 4° sotto-intervento; compilare manualmente il 5°
3. **Area agricola sì senza SAU** → il campo SAU si attiva solo selezionando "sì"; non dimenticarlo
4. **Tre dichiarazioni sì/no consecutive** → area agricola, area idonea e zone accelerazione sono tre radio button separati tutti obbligatori; verificarli tutti e tre
5. **Titolo edilizio sì senza tipo** → inserire il Comune non è sufficiente: occorre selezionare anche il tipo (CIL/CILA/SCIA alt./PdC) e compilare data e numero
6. **Bug formato data CILA** → il controllo formato legge il campo sbagliato; inserire sempre GG/MM/AAAA

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

**Ultima revisione**: Agosto 2026
**Fonte**: Analisi codice `ValidaDatiALR` e `DatiALR.ascx`
