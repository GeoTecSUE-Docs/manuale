---
title: Errori Permesso di Costruire - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 56
description: Errori di validazione specifici per il Permesso di Costruire Nazionale - Tutte le regioni (artt. 10, 14, 36, 36-bis D.P.R. 380/2001)
keywords: [permesso di costruire, PdC, nazionale, tutte le regioni, art. 10 DPR 380, art. 14, art. 36, art. 36-bis, sanatoria, variazione essenziale, deroga, regolarità urbanistica, contributo costruzione, sicurezza lavoro, progettista, rilevatore]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 127 }  # Valle d'Aosta - Permesso di Costruire
  - { Reg: 6, Prat: 615 } # Veneto - Permesso di Costruire
  - { Reg: 8, Prat: 815 } # Emilia-Romagna - Permesso di Costruire
  - { Reg: 12, Prat: 1215 } # Lazio - Permesso di Costruire
  - { Reg: 13, Prat: 1315 } # Abruzzo - Permesso di Costruire
  - { Reg: 15, Prat: 1515 } # Campania - Permesso di Costruire
  - { Reg: 16, Prat: 1615 } # Basilicata - Permesso di Costruire
  - { Reg: 17, Prat: 1715 } # Puglia - Permesso di Costruire
  - { Reg: 18, Prat: 1815 } # Calabria - Permesso di Costruire
  - { Reg: 19, Prat: 1915 } # Sicilia - Permesso di Costruire
Fonte: Manuale
---

# Errori di validazione - Permesso di Costruire
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per il **Permesso di Costruire (PdC) Nazionale** — applicabile su tutto il territorio nazionale salvo versioni regionali specifiche. Il modulo è strutturato ai sensi degli artt. 10, 14, 36 e 36-bis del D.P.R. 6 giugno 2001, n. 380.

{: .note }
> Il PdC Nazionale è la pratica più articolata del sistema. La sezione **"Qualificazione dell'intervento"** ha 5 opzioni con logiche condizionali diverse. La sezione **"Sanatoria"** è una checkbox opzionale che, se spuntata, aggiunge un intero blocco condizionale con 2 opzioni (art. 36 e art. 36-bis) e impone il **Rilevatore (RI)** invece del Progettista (PR) come tecnico obbligatorio. La sezione **"Regolarità urbanistica"** (g) ha 7 opzioni con sotto-selezioni estremamente dettagliate — il blocco g_6 dello "stato attuale immobile" (checkbox 6_1/6_2) è sempre obbligatorio indipendentemente dal radio scelto. La sezione **Sicurezza** ha 4 livelli annidati. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Qualificazione dell'intervento](#1-qualificazione-dellintervento)
2. [Sanatoria (opzionale)](#2-sanatoria-opzionale)
3. [Titolarità dell'intervento](#3-titolarità-dellintervento)
4. [Localizzazione dell'intervento](#4-localizzazione-dellintervento)
5. [Opere su parti comuni o modifiche esterne](#5-opere-su-parti-comuni-o-modifiche-esterne)
6. [Descrizione sintetica dell'intervento](#6-descrizione-sintetica-dellintervento)
7. [Regolarità urbanistica e precedenti edilizi](#7-regolarità-urbanistica-e-precedenti-edilizi)
8. [Calcolo del contributo di costruzione](#8-calcolo-del-contributo-di-costruzione)
9. [Tecnici incaricati](#9-tecnici-incaricati)
10. [Impresa esecutrice dei lavori](#10-impresa-esecutrice-dei-lavori)
11. [Sicurezza sul lavoro (D.Lgs. 81/2008)](#11-sicurezza-sul-lavoro-dlgs-812008)
12. [Allacciamento fognatura](#12-allacciamento-fognatura)
13. [Tecnico obbligatorio nei soggetti coinvolti](#13-tecnico-obbligatorio-nei-soggetti-coinvolti)

---

## 1. Qualificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Dove si trova**: Sezione "Qualificazione dell'intervento" → 5 radio button principali

**Causa**: Nessuna opzione del gruppo `$TipoIntervento` è selezionata.

**Soluzione**: Seleziona **uno dei cinque radio button** e compila le eventuali sotto-selezioni:

- ⚪ **a_1** — "interventi di cui all'articolo 10 del d.P.R. n. 380/2001" → seleziona un sotto-radio `$TipoIntSpec1`
- ⚪ **a_2** — "interventi assoggettati a SCIA per i quali è facoltà richiedere il permesso (art. 22 comma 7) (specificare)" → compila il campo testo
- ⚪ **a_4** — "intervento realizzato, ai sensi dell'art. 36 comma 1, conforme alla disciplina vigente sia al momento della realizzazione sia alla presentazione" → nessun campo aggiuntivo
- ⚪ **a_5** — "intervento in deroga agli strumenti di pianificazione urbanistica (art. 14)" → spunta almeno una deroga e compila la specificazione
- ⚪ **a_6** — "variazione essenziale e/o sostanziale al/alla:" → spunta almeno una variazione e inserisci n. e data

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Interventi di cui all'articolo 10'.

**Causa**: Hai selezionato a_1 ("art. 10") ma non hai specificato la tipologia di intervento nel sotto-radio `$TipoIntSpec1`.

**Soluzione**: Seleziona **uno dei quattro radio button** del sotto-gruppo:
- ⚪ **a_1_1** — "non comporta mutamento di destinazione d'uso di una singola U.I. o di un intero immobile"
- ⚪ **a_1_2** — "comporta mutamento di destinazione d'uso di una singola U.I. all'interno della stessa categoria funzionale"
- ⚪ **a_1_3** — "comporta mutamento di destinazione d'uso di una singola U.I. [...] tra categorie funzionali di cui all'art. 23 ter c. 1, lett. a), a-bis), b) e c)"
- ⚪ **a_1_4** — "comporta mutamento di destinazione d'uso di un intero immobile all'interno della stessa categoria funzionale (art. 23-ter, c. 3)"

---

### ATTENZIONE ! Specificare gli interventi.

**Causa**: Hai selezionato a_2 (SCIA facoltativa) ma non hai compilato il campo testo `txtSpecifIntervento1`.

**Soluzione**: Descrivi nel campo multiriga la tipologia specifica degli interventi soggetti a SCIA per cui si richiede facoltativamente il permesso di costruire.

---

### Opzione a_5 — Deroga (art. 14 D.P.R. 380/2001)

#### ATTENZIONE ! Selezionare almeno una deroga.

**Causa**: Hai selezionato a_5 ma non hai spuntato nessuna delle 4 checkbox della deroga.

**Soluzione**: Spunta **almeno una** tra le 4 checkbox e compila il campo specificazione affiancato:
- ☐ **chkDerogaa_5_1** — "alla densità edilizia (specificare)" → campo `txtSpecifDeroga1`
- ☐ **chkDerogaa_5_2** — "all'altezza (specificare)" → campo `txtSpecifDeroga2`
- ☐ **chkDerogaa_5_3** — "alla distanza tra i fabbricati (specificare)" → campo `txtSpecifDeroga3`
- ☐ **chkDerogaa_5_4** — "alla destinazione d'uso (nei casi di cui al comma 1bis)" → campo `txtSpecifDeroga4`

---

#### ATTENZIONE ! Specificare la densità edilizia.

**Causa**: `chkDerogaa_5_1` è spuntata ma `txtSpecifDeroga1` è vuoto.

**Soluzione**: Inserisci la specificazione della densità edilizia da cui si chiede deroga.

---

#### ATTENZIONE ! Specificare l'altezza.

**Causa**: `chkDerogaa_5_2` è spuntata ma `txtSpecifDeroga2` è vuoto.

**Soluzione**: Inserisci la specificazione dell'altezza da cui si chiede deroga.

---

#### ATTENZIONE ! Specificare la distanza tra fabbricati.

**Causa**: `chkDerogaa_5_3` è spuntata ma `txtSpecifDeroga3` è vuoto.

**Soluzione**: Inserisci la specificazione della distanza tra fabbricati da cui si chiede deroga.

---

#### ATTENZIONE ! Specificare la destinazione d'uso.

**Causa**: `chkDerogaa_5_4` è spuntata ma `txtSpecifDeroga4` è vuoto.

**Soluzione**: Inserisci la specificazione della destinazione d'uso da cui si chiede deroga.

---

### Opzione a_6 — Variazione essenziale

#### ATTENZIONE ! Selezionare almeno una variazione.

**Causa**: Hai selezionato a_6 ("variazione essenziale") ma non hai spuntato nessuna delle 3 checkbox.

**Soluzione**: Spunta **almeno una** tra le 3 checkbox e inserisci n. pratica e data:
- ☐ **chkVariazionea_6_1** — "titolo unico" → n. (`txtNPraticaTitolo`) + data (`txtDataPraticaTitolo`, formato GG/MM/AAAA)
- ☐ **chkVariazionea_6_2** — "permesso di costruire" → n. (`txtNPraticaPermesso`) + data (`txtDataPraticaPermesso`, formato)
- ☐ **chkVariazionea_6_3** — "segnalazione certificata/denuncia di inizio attività alternativa al permesso di costruire" → n. (`txtNPraticaInizioAtt`) + data (`txtDataPraticaInizioAtt`, formato)

---

#### ATTENZIONE ! Inserire N° Pratica titolo unico.

**Causa**: `chkVariazionea_6_1` è spuntata ma manca il numero pratica `txtNPraticaTitolo`.

**Soluzione**: Inserisci il numero del titolo unico nel campo "n."

---

#### ATTENZIONE ! Inserire Data Pratica titolo unico. / Inserire la data nel formato gg/mm/aaaa.

**Causa**: Data assente o in formato errato per la variazione al titolo unico.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire N° Pratica del permesso di costruire. / Inserire Data Pratica del permesso di costruire.

**Causa**: `chkVariazionea_6_2` è spuntata ma mancano n. o data della variazione al PdC.

**Soluzione**: Compila n. e data (GG/MM/AAAA) del permesso di costruire originario.

---

#### ATTENZIONE ! Inserire N° Pratica della denuncia inizio attività. / Inserire Data Pratica della denuncia inizio attività.

**Causa**: `chkVariazionea_6_3` è spuntata ma mancano n. o data.

**Soluzione**: Compila n. e data (GG/MM/AAAA) della SCIA/DIA alternativa al PdC.

---

## 2. Sanatoria (opzionale)

La checkbox `chkSanatoriax1_0` è facoltativa. Se spuntata attiva la modalità sanatoria che richiede radio e campi aggiuntivi e cambia il tecnico obbligatorio da Progettista (PR) a **Rilevatore (RI)**.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per la tipologia di sanatoria.

**Causa**: `chkSanatoriax1_0` è spuntata ma nessuno dei 2 radio button `$TipoSanatoria` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **x1_1** — "sanatoria di intervento soggetto a permesso di costruire, realizzato in data ___ in assenza del permesso o in totale difformità [...] conforme alla disciplina vigente sia al momento della realizzazione sia alla presentazione (art. 36)" → inserisci data e spunta la checkbox di consapevolezza
- ⚪ **x1_2** — "sanatoria [...] in parziale difformità dal permesso o con variazioni essenziali (art. 36-bis)" → inserisci data, seleziona la conformità e spunta le 2 checkbox di consapevolezza

---

### Opzione x1_1 — Art. 36 (sanatoria ordinaria)

#### ATTENZIONE ! Specificare la data del permesso di costruire. (x1_1)

**Causa**: `rdbTipoSanatoriax1_1` è selezionato ma il campo `txtDatax1_1_1` è vuoto.

**Soluzione**: Inserisci la data di realizzazione dell'intervento nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (x1_1)

**Causa**: La data inserita per la sanatoria x1_1 non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Selezionare la presa visione per il rilascio del permesso. (x1_1 — chkTipoSanatoriax1_1_2)

**Causa**: Non hai spuntato la checkbox `chkTipoSanatoriax1_1_2` di consapevolezza sull'oblazione.

**Soluzione**: Spunta la checkbox "il rilascio del permesso di costruire in sanatoria è subordinato al pagamento, a titolo di oblazione, di un importo pari al doppio del contributo di costruzione [...] (art. 36, comma 2 d.P.R. 380/2001)".

---

### Opzione x1_2 — Art. 36-bis (sanatoria parziale difformità)

#### ATTENZIONE ! Specificare la data del permesso di costruire. (x1_2)

**Causa**: `rdbTipoSanatoriax1_2` è selezionato ma `txtDatax1_2_1` è vuoto.

**Soluzione**: Inserisci la data di realizzazione dell'intervento nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Non è stata selezionata nessuna voce per la conformità urbanistica.

**Causa**: Manca la selezione del radio `$Conforme` (conformità urbanistica).

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **x1_2_2** — "che risulta conforme alla disciplina urbanistica vigente al momento della presentazione della richiesta e ai requisiti prescritti dalla disciplina edilizia vigente al momento della realizzazione" → spunta le 2 checkbox obbligatorie
- ⚪ **x1_2_3** — "che risulta conforme alla disciplina urbanistica vigente sia al momento della realizzazione sia al momento della presentazione della richiesta" → spunta le 2 checkbox obbligatorie

---

#### ATTENZIONE ! Selezionare la presa visione per il rilascio del permesso. (x1_2_2 o x1_2_3 — prima checkbox)

**Causa**: Non hai spuntato `chkRilasciox1_2_2_1` (opzione x1_2_2) o `chkRilasciox1_2_3_1` (opzione x1_2_3) — la checkbox sull'oblazione.

**Soluzione**: Spunta la checkbox relativa al pagamento dell'oblazione (doppio del contributo di costruzione, incrementato del 20% per parziale difformità — art. 36-bis, comma 5, lettera a).

---

#### ATTENZIONE ! Selezionare la presa visione per il rilascio del permesso. (x1_2_2 o x1_2_3 — seconda checkbox)

**Causa**: Non hai spuntato `chkSportellox1_2_2_2` (opzione x1_2_2) o `chkSportellox1_2_3_2` (opzione x1_2_3) — la checkbox sullo Sportello Unico.

**Soluzione**: Spunta la checkbox "lo Sportello Unico può subordinare il rilascio [...] alla realizzazione di interventi strutturali necessari alla sicurezza e/o alla rimozione di opere che non possono essere sanate (art. 36-bis comma 2)".

{: .note }
> Per l'opzione x1_2_2 e x1_2_3 entrambe le checkbox di consapevolezza sono obbligatorie. Il messaggio d'errore è lo stesso ("Selezionare la presa visione per il rilascio del permesso") sia per la prima che per la seconda checkbox — il validatore le controlla in sequenza e si ferma alla prima mancante.

---

## 3. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Nessuno dei 2 radio button `$Titolarita` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **b_1** — "avere titolarità esclusiva all'esecuzione dell'intervento"
- ⚪ **b_2** — "non avere titolarità esclusiva all'esecuzione dell'intervento, ma di disporre comunque della dichiarazione di assenso dei terzi"

{: .note }
> Il menu `cmbTitoloSuImm` (proprietario, usufruttuario, ecc.) è presente ma **non validato** — non genera errori. A differenza della ROPD Liguria, il PdC Nazionale non verifica la presenza di titolari aggiuntivi anche se si sceglie b_2.

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

{: .note }
> Il campo "Coordinate" (`txtCoordinate`) è presente ma non validato.

---

## 5. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Nessun radio button del gruppo `$Opere` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **d_1** — "non riguardano parti comuni"
- ⚪ **d_2** — "riguardano le parti comuni di un fabbricato condominiale" (richiede delibera assembleare)
- ⚪ **d_3** — "riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"
- ⚪ **d_4** — "riguardano parti comuni ma non necessitano di assenso (art. 1102 c.c.)"

---

## 6. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Sezione "Descrizione sintetica dell'intervento" → campo multiriga `txtDescrIntervento` (max 300 caratteri)

**Causa**: Il campo è vuoto.

**Soluzione**: Inserisci la descrizione delle opere nel campo multiriga (max **300 caratteri**).

---

## 7. Regolarità urbanistica e precedenti edilizi

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Dove si trova**: Sezione "Regolarità urbanistica e precedenti edilizi" → 7 radio button `$StatoAttualeImm`

**Causa**: Nessuno dei 7 radio button è selezionato.

**Soluzione**: Seleziona **uno dei sette radio button**:
- ⚪ **g_7** — "le opere riguardano un intervento di nuova costruzione su area libera" → nessun campo aggiuntivo (poi spunta chk 6_1 o 6_2)
- ⚪ **g_1** — "l'immobile/U.I. è stato oggetto dei seguenti titoli o pratiche edilizie" → spunta almeno una delle 13 checkbox con n. e data
- ⚪ **g_2** — "immobile realizzato in epoca senza obbligo di titolo e pertanto allega" → almeno una delle 2 checkbox; se 2_1: n.+data accatastamento
- ⚪ **g_3** — "non sono disponibili copia o estremi del titolo ma sussiste principio di prova documentale" → almeno una delle 2 checkbox; se 3_1: n.+data
- ⚪ **g_4** — "irrogate le seguenti sanzioni pecuniarie (artt. 33, 34, 37, 38)" → almeno una delle 2 checkbox; se 4_2: importo + date pagamento e protocollo
- ⚪ **g_5** — "oggetto della/e dichiarazione/i di tolleranza costruttiva (art. 34-bis o 34-ter, c. 4)" → almeno una delle 2 checkbox con n. e data ciascuna

---

### Opzione g_1 — Titoli edilizi precedenti

#### ATTENZIONE! Indicare almeno una tipologia di pratica. (g_1)

**Causa**: Hai selezionato g_1 ma nessuna delle 13 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** delle 13 checkbox corrispondenti al/ai titolo/i edilizio/i precedente/i:

Le prime 8 (con n. e data ciascuna): titolo unico (SUAP), permesso di costruire/licenza/concessione, autorizzazione edilizia, comunicazione edilizia (art. 26 L. 47/1985), DIA, DIA/SCIA alternativa al PdC, SCIA, comunicazione edilizia libera.

La checkbox **9** ("titolo edilizio in sanatoria") apre 4 sotto-checkbox (condono edilizio, PdC in sanatoria artt. 36/36-bis, SCIA in sanatoria art. 36-bis, SCIA in sanatoria per variante ante L. 10/1977) — ciascuna richiede n. e data.

Le checkbox **10, 11, 12, 13** ("altro") richiedono: tipo pratica (campo testo) + n. + data.

---

#### ATTENZIONE! Specificare numero della pratica. (g_1, checkbox 1-8)

**Causa**: Una delle checkbox 1-8 è spuntata ma manca il numero pratica affiancato.

**Soluzione**: Inserisci il numero nel campo "n." della checkbox corrispondente.

---

#### ATTENZIONE! Specificare data della pratica. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa. (g_1, checkbox 1-8)

**Causa**: Manca la data o il formato non è corretto per una delle checkbox 1-8.

**Soluzione**: Inserisci la data nel campo "del" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE! Indicare almeno una tipologia di pratica come 'titolo edilizio in sanatoria con il pagamento della relativa oblazione'. (checkbox 9)

**Causa**: La checkbox 9 ("titolo edilizio in sanatoria") è spuntata ma nessuna delle 4 sotto-checkbox è selezionata.

**Soluzione**: Spunta **almeno una** delle 4 sotto-checkbox e inserisci n. e data:
- ☐ **9_1** — "condono edilizio"
- ☐ **9_2** — "permesso di costruire in sanatoria di cui agli artt. 36 o 36-bis"
- ☐ **9_3** — "SCIA in sanatoria di cui all'art. 36-bis"
- ☐ **9_4** — "SCIA in sanatoria per variante in corso d'opera costituente parziale difformità dal titolo rilasciato prima della L. 10/1977"

---

#### ATTENZIONE! Specificare tipologia della pratica. (checkbox 10-13 "altro")

**Causa**: Una delle checkbox "altro" (10, 11, 12 o 13) è spuntata ma il campo testo del tipo di pratica è vuoto.

**Soluzione**: Inserisci la descrizione del tipo di pratica nel campo testo affiancato alla checkbox.

---

### Opzione g_2 — Immobile ante obbligo titolo

#### ATTENZIONE! Indicare almeno un tipo di allegato. (g_2)

**Causa**: Hai selezionato g_2 ma nessuna delle 2 checkbox è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm2_1** — "copia accatastamento di primo impianto o si forniscono i relativi estremi" → inserisci n. e data (formato GG/MM/AAAA)
- ☐ **chkStatoAttualeImm2_2** — "altri documenti probanti (riprese fotografiche, estratti cartografici, documenti di archivio...)" → nessun campo aggiuntivo

---

#### ATTENZIONE! Specificare numero della copia accatastamento. / Specificare data della copia accatastamento. (g_2, chk 2_1)

**Soluzione**: Compila n. e data (GG/MM/AAAA) nel campo accatastamento di primo impianto.

---

### Opzione g_3 — Principio di prova documentale

#### ATTENZIONE! Indicare almeno un tipo di allegato. (g_3)

**Causa**: Nessuna delle 2 checkbox di g_3 è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm3_1** — "copia accatastamento di primo impianto o si forniscono i relativi estremi" → inserisci n. e data
- ☐ **chkStatoAttualeImm3_2** — "altri documenti probanti (art. 9-bis, comma 1-bis)" → nessun campo aggiuntivo

---

#### ATTENZIONE! Specificare numero della copia accatastamento. / Specificare data della copia accatastamento. (g_3)

**Soluzione**: Compila n. e data (GG/MM/AAAA) per l'accatastamento g_3.

---

### Opzione g_4 — Sanzioni pecuniarie

#### ATTENZIONE! Indicare almeno una sanzione pecuniaria. (g_4)

**Causa**: Nessuna delle 2 checkbox di g_4 è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm4_1** — "si allega la relativa ricevuta" → nessun campo aggiuntivo
- ☐ **chkStatoAttualeImm4_2** — "si forniscono gli estremi del pagamento" → inserisci importo, data pagamento, n. protocollo, data protocollo

---

#### ATTENZIONE! Specificare importo della sanzione pecuniaria.

**Causa**: `chkStatoAttualeImm4_2` è spuntata ma `txtImporto4_2_1` è vuoto.

**Soluzione**: Inserisci l'importo della sanzione pecuniaria nel campo "€".

---

#### ATTENZIONE! Specificare data del pagamento della sanzione pecuniaria. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Soluzione**: Inserisci la data di irrogazione della sanzione nel formato **GG/MM/AAAA** (`txtDataImporto4_2_2`).

---

#### ATTENZIONE! Specificare numero di protocollo della sanzione pecuniaria.

**Soluzione**: Inserisci il numero di protocollo (`txtNProt4_2_3`).

---

#### ATTENZIONE! Specificare data di protocollo della sanzione pecuniaria. / ATTENZIONE! Inserire la data nel formato gg/mm/aaaa.

**Soluzione**: Inserisci la data di protocollo nel formato **GG/MM/AAAA** (`txtDataProt4_2_4`).

---

### Opzione g_5 — Tolleranze costruttive (art. 34-bis)

#### ATTENZIONE! Indicare almeno una dichiarazione di tolleranza costruttiva. (g_5)

**Causa**: Nessuna delle 2 checkbox di g_5 è spuntata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm5_1** — "dichiarazione delle tolleranze presentata nella modulistica relativa alla pratica edilizia prot." → n. + data
- ☐ **chkStatoAttualeImm5_2** — "dichiarazione allegata agli atti aventi per oggetto trasferimento o costituzione di diritti reali (art. 34-bis, c. 3)" → n. atto + data

---

#### ATTENZIONE! Specificare numero di protocollo della pratica edilizia. / Specificare data di protocollo della pratica edilizia. (g_5, chk 5_1)

**Soluzione**: Compila n. e data (GG/MM/AAAA) della pratica edilizia nella tolleranza 5_1.

---

#### ATTENZIONE! Specificare numero dell'atto di registrazione. / Specificare data dell'atto di registrazione. (g_5, chk 5_2)

**Soluzione**: Compila n. e data (GG/MM/AAAA) dell'atto di registrazione nella tolleranza 5_2.

---

### Stato attuale immobile — sempre obbligatorio (checkbox 6_1/6_2)

#### ATTENZIONE! Indicare almeno uno stato attuale dell'immobile.

**Dove si trova**: Sotto il radio group `$StatoAttualeImm`, in fondo alla sezione → "dichiara che lo stato attuale dell'immobile/U.I. risulta:" → 2 checkbox

**Causa**: Nessuna delle 2 checkbox dello stato attuale è spuntata. Questo controllo viene eseguito **sempre**, indipendentemente dall'opzione di regolarità urbanistica scelta.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **chkStatoAttualeImm6_1** — "pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"
- ☐ **chkStatoAttualeImm6_2** — "conforme alla documentazione [...] unitamente alla/e sanatoria/e di cui al quadro 'Sanatoria' e alla/e dichiarazione/i di tolleranza esecutive"

{: .warning }
> Le checkbox 6_1/6_2 sono sempre obbligatorie, anche scegliendo g_7 ("nuova costruzione su area libera"). Non dimenticarle anche nel caso più semplice — il validatore le controlla come ultimo passaggio del blocco regolarità urbanistica per qualsiasi opzione radio.

---

## 8. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Nessun radio button del gruppo `$Intervento` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_1** — "è a titolo gratuito, ai sensi della seguente normativa ___" → compila il campo testo `txtGratuitog1_2`
- ⚪ **g_2** — "è a titolo oneroso ai sensi dell'art. 38 l.r. 16/2008" → nessun campo strettamente obbligatorio dal validatore, ma le checkbox di calcolo e pagamento sono raccomandate

---

### ATTENZIONE ! Campo obbligatorio non inserito. (contributo gratuito)

**Causa**: Hai selezionato `rdbInterventog_1` (gratuito) ma `txtGratuitog1_2` è vuoto.

**Soluzione**: Inserisci nel campo testo la normativa ai sensi della quale l'intervento è a titolo gratuito (es. `art. 17 comma 3 lett. a) D.P.R. 380/2001`, `art. 9 comma 1 L. 10/1977`).

---

## 9. Tecnici incaricati

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Causa**: Nessun radio button del gruppo `$Tecnici` è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **h_1** — "di aver incaricato, in qualità di progettista delle opere strutturali, di direttori dei lavori, e di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'Soggetti coinvolti'"
- ⚪ **h_2** — "che il progettista delle opere strutturali, il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"

---

## 10. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Nessun radio button del gruppo `$Impresa` è selezionato.

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **i_1** — "i lavori saranno eseguiti/sono stati eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'" → deve essere presente almeno un'impresa nei soggetti
- ⚪ **i_2** — "l'impresa esecutrice sarà individuata prima dell'inizio dei lavori"
- ⚪ **i_3** — "i lavori sono eseguiti in economia a cura diretta della committenza"
- ⚪ **i_4** — "lavori non eseguiti da impresa (per pratiche in sanatoria)"

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato `rdbImpresai_1` ("lavori eseguiti da impresa") ma nessuna impresa è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → aggiungi almeno un'impresa esecutrice, oppure seleziona un'altra opzione (i_2, i_3 o i_4).

---

## 11. Sicurezza sul lavoro (D.Lgs. 81/2008)

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Nessun radio button del gruppo `$AmbitoRicade` è selezionato.

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **l_1** — "non ricade nell'ambito di applicazione delle norme [...] (d.lgs. n. 81/2008)" → nessun campo aggiuntivo
- ⚪ **l_2** — "ricade nell'ambito di applicazione [...] e pertanto" → seleziona documentazione imprese e, se applicabile, notifica
- ⚪ **l_3** — "ricade nell'ambito ma si riserva di presentare le dichiarazioni prima dell'inizio lavori" → nessun campo aggiuntivo

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato l_2 ma non hai indicato la tipologia di documentazione delle imprese.

**Soluzione**: Seleziona **uno dei due radio button** `$ImpEs`:
- ⚪ **l_2_1** — "entità presunta del cantiere è inferiore a 200 uomini-giorno e i lavori non comportano i rischi particolari dell'Allegato XI" → nessun campo aggiuntivo
- ⚪ **l_2_2** — "entità presunta del cantiere è pari o superiore a 200 uomini-giorno o i lavori comportano i rischi particolari dell'Allegato XI" → seleziona il radio notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato l_2_2 ma non hai indicato la situazione della notifica preliminare.

**Soluzione**: Seleziona **uno dei due radio button** `$Notifica`:
- ⚪ **notifica_2_2_1** — "l'intervento non è soggetto all'invio della notifica" → nessun campo aggiuntivo
- ⚪ **notifica_2_2_2** — "l'intervento è soggetto all'invio della notifica" → seleziona il radio `$Allega`

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione/Estremi Notifica'.

**Causa**: Hai selezionato notifica_2_2_2 ma non hai indicato modalità di trasmissione della notifica.

**Soluzione**: Seleziona **uno dei due radio button** `$Allega`:
- ⚪ **l_2_2_2_1** — "invierà la notifica prima dell'inizio dei lavori"
- ⚪ **l_2_2_2_2** — "allega la notifica, il cui contenuto sarà riprodotto su apposita tabella esposta in cantiere"

---

## 12. Allacciamento fognatura

### ATTENZIONE ! Campo obbligatorio non inserito. (fognatura)

**Dove si trova**: Sezione "Allacciamento fognatura" → campo `txtAutFognatura`

**Causa**: La sezione allacciamento fognatura è compilata con `rdbAllaccFognaturaq_4` (richiede autorizzazione) selezionato, ma il campo `txtAutFognatura` è vuoto.

**Soluzione**: Inserisci gli estremi dell'autorizzazione all'allacciamento fognario nel campo `txtAutFognatura`.

{: .note }
> Questa sezione è opzionale e il validatore la controlla solo se il radio group `$AllaccFognatura` è stato compilato. Se la sezione non è pertinente, lasciarla non compilata non genera errori.

---

## 13. Tecnico obbligatorio nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Causa**: **Modalità ordinaria** (sanatoria non spuntata) — nessun tecnico con ruolo **PR** (Progettista) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **PR – Progettista**.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Rilevatore.

**Causa**: **Modalità sanatoria** (`chkSanatoriax1_0` spuntata) — nessun tecnico con ruolo **RI** (Rilevatore) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **RI – Rilevatore**.

{: .note }
> Il ruolo richiesto cambia in base alla modalità della pratica: **PR (Progettista)** per il PdC ordinario; **RI (Rilevatore)** per il PdC in sanatoria. Il validatore determina la modalità dalla checkbox `chkSanatoriax1_0` — se spuntata imposta `sanatoria = True` e richiede RI invece di PR. Se si spunta la sanatoria per sbaglio e poi si rimuove il rilevatore, il sistema continuerà a richiedere RI.

---

## Consigli pratici — PdC Nazionale

### Prima di validare ✅

- [ ] Seleziona la **qualificazione** (a_1..a_6) e compila le sotto-selezioni richieste
- [ ] Se sanatoria: spunta `chkSanatoriax1_0`, seleziona x1_1 o x1_2 con data e checkbox obbligatorie
- [ ] Seleziona la **titolarità** (b_1/b_2)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona le **opere su parti comuni** (d_1..d_4)
- [ ] Inserisci la **descrizione** delle opere (max 300 caratteri)
- [ ] Seleziona la **regolarità urbanistica** (g_1..g_7) e compila le sotto-selezioni; spunta sempre **chk 6_1 o 6_2** (stato attuale immobile)
- [ ] Seleziona il **contributo di costruzione** (gratuito con normativa / oneroso)
- [ ] Seleziona le dichiarazioni **tecnici** (h_1/h_2) e **impresa** (i_1..i_4)
- [ ] Seleziona la **sicurezza** (l_1/l_2/l_3); se l_2: documenta imprese e notifica
- [ ] Aggiungi il tecnico obbligatorio: **PR** (ordinario) o **RI** (sanatoria)

### Campi presenti ma non validati ℹ️

- **`cmbTitoloSuImm`** (proprietario/usufruttuario): non validato
- **`txtCoordinate`**: non validato
- **`txtNote`**: facoltativo
- **`txtData` e `txtLuogo`** (data e luogo firma): facoltativi
- **Privacy**: solo testo informativo statico

### Ordine di validazione ⚠️

Qualificazione → Sanatoria → Titolarità → Localizzazione → Opere comuni → Descrizione → Regolarità urbanistica → Contributo → Tecnici (sezione h) → Impresa → Sicurezza → Fognatura → Tecnico soggetti coinvolti (PR o RI) → Imprese soggetti coinvolti (se i_1)

### Errori frequenti 🔍

1. **Checkbox 6_1/6_2 dimenticate** → lo stato attuale dell'immobile è obbligatorio per qualsiasi opzione di regolarità urbanistica, inclusa la nuova costruzione (g_7); spuntarne almeno una prima di validare
2. **Sanatoria attivata per sbaglio** → se `chkSanatoriax1_0` viene spuntata, il sistema richiede RI invece di PR; deselezionarla se non si tratta di sanatoria
3. **Checkbox 9_x senza sotto-checkbox** → la checkbox 9 ("titolo in sanatoria") attiva 4 sotto-checkbox; spuntare la 9 senza selezionare almeno una sotto-checkbox genera "Indicare almeno una tipologia"
4. **Checkbox 10-13 "altro" senza tipo pratica** → le 4 voci "altro" richiedono il testo della tipologia oltre a n. e data
5. **Contributo gratuito senza normativa** → `txtGratuitog1_2` è obbligatorio se si sceglie "gratuito"; inserire la norma di riferimento

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
**Fonte**: Analisi codice ValidaDatiPdCNazionale e DatiPdCNaz.ascx
