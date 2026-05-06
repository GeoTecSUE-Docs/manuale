---
title: Errori SCIA - Tutte le regioni
parent: Errori di validazione
nav_order: 34
description: Errori di validazione specifici per la Segnalazione Certificata di Inizio Attività (SCIA) nazionale - art. 22 e 23 D.P.R. 380/2001, D.Lgs. 222/2016
keywords: [SCIA, segnalazione certificata inizio attività, art. 22 DPR 380/2001, qualificazione intervento, sanatoria art. 36-bis, regolarità urbanistica, stato legittimo, contributo costruzione, Progettista, Direttore Lavori, Rilevatore]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 123 }  # Valle d'Aosta - SCIA
  - { Reg: 6, Prat: 623 } # Veneto - SCIA
  - { Reg: 8, Prat: 823 } # Emilia-Romagna - SCIA
  - { Reg: 12, Prat: 1223 } # Lazio - SCIA
  - { Reg: 13, Prat: 1323 } # Abruzzo - SCIA
  - { Reg: 15, Prat: 1523 } # Campania - SCIA
  - { Reg: 16, Prat: 1623 } # Basilicata - SCIA
  - { Reg: 17, Prat: 1723 } # Puglia - SCIA
  - { Reg: 18, Prat: 1823 } # Calabria - SCIA
  - { Reg: 19, Prat: 1923 } # Sicilia - SCIA
Fonte: Manuale
---

# Errori di validazione - SCIA (Segnalazione Certificata di Inizio Attività)
## Tutte le regioni

Guida completa agli errori specifici per la **Segnalazione Certificata di Inizio Attività** ai sensi degli artt. 22 e 23 del D.P.R. 6 giugno 2001, n. 380, e del D.Lgs. 25 novembre 2016, n. 222.

{: .note }
> La SCIA nazionale è la pratica più articolata della piattaforma. Presenta una struttura a più livelli: la **qualificazione** ha 8 opzioni ciascuna con sotto-opzioni specifiche; la **sanatoria** (facoltativa) ha 4 tipologie con complesse logiche di pagamento; la **regolarità urbanistica** ha 5 macro-opzioni con numerose sotto-checkbox ciascuna con campi n. e data. I tecnici richiesti cambiano a seconda che la pratica sia in sanatoria (solo Rilevatore) o ordinaria (Progettista + Direttore Lavori, salvo proroga). Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Presentazione della SCIA / SCIA Unica / SCIA Condizionata](#2-presentazione-della-scia--scia-unica--scia-condizionata)
3. [Qualificazione dell'intervento](#3-qualificazione-dellintervento)
4. [Sanatoria e regolarizzazioni — sezione facoltativa](#4-sanatoria-e-regolarizzazioni--sezione-facoltativa)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Opere su parti comuni o modifiche esterne](#6-opere-su-parti-comuni-o-modifiche-esterne)
7. [Regolarità urbanistica e precedenti edilizi](#7-regolarità-urbanistica-e-precedenti-edilizi)
8. [Calcolo del contributo di costruzione](#8-calcolo-del-contributo-di-costruzione)
9. [Tecnici incaricati e impresa esecutrice](#9-tecnici-incaricati-e-impresa-esecutrice)
10. [Sicurezza sul lavoro — D.Lgs. 81/2008](#10-sicurezza-sul-lavoro--dlgs-812008)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Titolarità dell'Intervento'.

**Causa**: Non hai compilato il menu a discesa né selezionato il radio button sulla titolarità.

**Soluzione**: Compila il menu **"di avere titolo alla presentazione di questa pratica edilizia in quanto"** e seleziona una delle due opzioni:
- ⚪ **"avere titolarità esclusiva all'esecuzione dell'intervento"**
- ⚪ **"non avere titolarità esclusiva... ma di disporre comunque della dichiarazione di assenso dei terzi"**

---

## 2. Presentazione della SCIA / SCIA Unica / SCIA Condizionata

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione della segnalazione certificata di inizio attività'.

**Causa**: Non hai dichiarato quale tipo di SCIA stai presentando.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **b.1 — SCIA** → inserisci la data di inizio lavori
- ⚪ **b.2 — SCIA Unica** (con altre segnalazioni contestuali alla realizzazione dell'intervento) → inserisci la data di inizio lavori
- ⚪ **b.3 — SCIA Condizionata** (con richiesta di atti di assenso) → nessuna data richiesta; i lavori inizieranno dopo comunicazione degli assensi

---

### ATTENZIONE ! Inserire la data di inizio lavori. (presentazione b.1 o b.2)

**Dove si trova**: Campo data accanto al testo "Il titolare dichiara che i lavori avranno inizio in data" nella riga b.1 o b.2

**Causa**: Hai selezionato SCIA o SCIA Unica ma non hai inserito la data prevista di inizio lavori.

**Soluzione**: Inserisci la data di inizio lavori nel formato **GG/MM/AAAA** (es. `15/06/2026`).

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data inizio lavori)

**Causa**: La data di inizio lavori è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `15/06/2026` ✅ — `15-06-2026` ❌).

---

## 3. Qualificazione dell'intervento

La qualificazione indica la tipologia di intervento edilizio. Ogni opzione principale (c.1-c.8) ha sotto-opzioni obbligatorie. Il sistema valida prima la scelta principale e poi le sotto-opzioni.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione dell'Intervento'.

**Causa**: Non hai indicato la tipologia di intervento.

**Soluzione**: Seleziona **una delle otto qualificazioni**:
- ⚪ **c.1** — Manutenzione straordinaria (pesante) sulle parti strutturali o prospetti → seleziona poi una delle 4 sotto-opzioni mutamento d'uso
- ⚪ **c.2** — Restauro e risanamento conservativo (pesante) sulle parti strutturali → seleziona poi una delle 4 sotto-opzioni
- ⚪ **c.3** — Ristrutturazione edilizia (leggera, escluso art. 10 c. 1 lett. c) → seleziona poi una delle 4 sotto-opzioni
- ⚪ **c.4** — Variante in corso d'opera a permesso di costruire → inserisci n. e data del PdC
- ⚪ **c.5** — Variante in corso d'opera a SCIA (variazione essenziale) → inserisci n. e data della SCIA
- ⚪ **c.6** — Variante in corso d'opera a SCIA (variazione essenziale ex art. 32) → inserisci n. e data della SCIA
- ⚪ **c.7** — Mutamento destinazione d'uso (singola UI) → seleziona poi una delle 4 sotto-opzioni
- ⚪ **c.8** — Mutamento destinazione d'uso intero immobile (art. 23-ter c. 3) → seleziona poi una delle 2 sotto-opzioni

---

### Qualificazioni c.1, c.2, c.3 — sotto-opzioni mutamento d'uso

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Intervento di manutenzione straordinaria' (oppure restauro / ristrutturazione)

**Dove si trova**: 4 radio button sotto c.1 (o c.2 / c.3), con il testo "a tal fine si specifica che l'intervento"

**Causa**: Hai selezionato c.1, c.2 o c.3 ma non hai specificato l'impatto sul mutamento di destinazione d'uso.

**Soluzione**: Seleziona **una delle quattro sotto-opzioni**:
- ⚪ **non comporta** mutamento di destinazione d'uso
- ⚪ **comporta mutamento** all'interno della stessa categoria funzionale (singola UI)
- ⚪ **comporta mutamento tra categorie funzionali** (singola UI in zone A/B/C, art. 23-ter c. 1 lett. a/a-bis/b/c)
- ⚪ **comporta mutamento** di intero immobile all'interno della stessa categoria (art. 23-ter c. 3)

---

### Qualificazioni c.4, c.5, c.6 — varianti con n. e data

#### ATTENZIONE ! Specificare il numero di riferimento.

**Causa**: Hai selezionato c.4, c.5 o c.6 (variante in corso d'opera) ma non hai inserito il numero del titolo edilizio originario a cui la variante si riferisce.

**Soluzione**: Inserisci il numero nel campo **"n."** accanto alla qualificazione (es. `PdC 123/2023`, `SCIA-2024-42`).

---

#### ATTENZIONE ! Specificare la data di riferimento.

**Causa**: Numero inserito ma data mancante.

**Soluzione**: Inserisci la data del titolo originario nel campo **"del"** nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (variante c.4/c.5/c.6)

**Causa**: La data del titolo di riferimento è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

### Qualificazioni c.7, c.8 — mutamento destinazione d'uso

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Mutamento di destinazione d'uso' (c.7 o c.8)

**Dove si trova**: Sotto-opzioni di c.7 (4 radio) o c.8 (2 radio)

**Causa**: Hai selezionato c.7 o c.8 ma non hai specificato la tipologia di mutamento.

**Soluzione per c.7**: Seleziona una delle 4 sotto-opzioni (senza opere/stessa categoria, senza opere/tra categorie, con opere/stessa categoria, con opere/tra categorie).

**Soluzione per c.8**: Seleziona una delle 2 sotto-opzioni (con opere riconducibili all'art. 6-bis, oppure senza opere o con opere art. 6).

---

### ATTENZIONE ! Inserire la descrizione dell'intervento.

**Dove si trova**: Campo di testo **"Descrizione sintetica dell'intervento"** nella sezione Qualificazione, dopo tutte le sotto-opzioni

**Causa**: Non hai inserito la descrizione delle opere.

**Soluzione**: Inserisci una descrizione sintetica delle opere (max **300 caratteri**).

---

## 4. Sanatoria e regolarizzazioni — sezione facoltativa

La sezione sanatoria è attivata dalla checkbox **"che la presente segnalazione riguarda"**. È facoltativa: se non spuntata, non viene validata. Se spuntata, richiede la selezione di una delle 4 tipologie, ciascuna con proprie sotto-condizioni.

{: .note }
> Quando la sanatoria è attiva, la logica dei tecnici cambia: anziché Progettista + Direttore Lavori, il sistema verifica la presenza del **Rilevatore (RI)** nei soggetti coinvolti.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per la tipologia di sanatoria.

**Causa**: Hai spuntato la checkbox sanatoria ma non hai indicato quale tipologia.

**Soluzione**: Seleziona **una delle quattro tipologie**:
- ⚪ **x.1** — Intervento soggetto a SCIA in corso di esecuzione con pagamento di sanzione (art. 37, c. 5, D.P.R. 380/2001)
- ⚪ **x.2** — Sanatoria di intervento soggetto a SCIA realizzato in assenza/difformità, conforme sia al momento della realizzazione sia al momento della segnalazione (art. 36-bis)
- ⚪ **x.3** — Sanatoria di intervento soggetto a SCIA realizzato in assenza/difformità, conforme alla disciplina urbanistica vigente al momento della segnalazione (art. 36-bis, prima parte)
- ⚪ **x.4** — Regolarizzazione di variante in corso d'opera costituente parziale difformità da titolo rilasciato prima della L. 47/1977 (art. 34-ter D.P.R. 380/2001)

---

### Sanatoria x.1 — In corso di esecuzione

#### ATTENZIONE ! Indicare almeno una tipologia di presentazione del pagamento.

**Causa**: Hai selezionato x.1 ma non hai indicato come viene attestato il pagamento della sanzione di € 516,00.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"si forniscono gli estremi del pagamento di € 516,00 del ___"** → inserisci la data del pagamento (con verifica formato)
- ☐ **"si allega la ricevuta del pagamento di € 516,00"**

---

#### ATTENZIONE ! Specificare la data del pagamento. (x.1)

**Causa**: Hai spuntato "si forniscono gli estremi del pagamento" ma non hai inserito la data.

**Soluzione**: Inserisci la data del pagamento nel formato **GG/MM/AAAA**.

---

### Sanatoria x.2 — Conforme sia al momento della realizzazione sia al momento della segnalazione

#### ATTENZIONE ! Specificare la data della SCIA. (x.2)

**Causa**: Hai selezionato x.2 ma non hai inserito la data di realizzazione dell'intervento.

**Soluzione**: Inserisci la data di realizzazione nel campo a fianco di "sanatoria di intervento... realizzato in data" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Indicare almeno una tipologia di presentazione del pagamento. (x.2)

**Causa**: Hai compilato la data ma non hai indicato come viene attestato il pagamento dell'oblazione.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"si forniscono gli estremi del pagamento di € ___"** → inserisci importo e data (con verifica formato)
- ☐ **"si allega la ricevuta del pagamento di € ___"** → inserisci l'importo

---

#### ATTENZIONE ! Specificare l'importo del pagamento. / Specificare la data del pagamento. (x.2)

**Causa**: Hai spuntato una delle checkbox di pagamento ma non hai compilato tutti i campi.

**Soluzione**: Inserisci l'importo in € e la data nel formato **GG/MM/AAAA**.

---

### Sanatoria x.3 — Conforme alla disciplina urbanistica vigente al momento della segnalazione

La logica di x.3 è identica a x.2 (data di realizzazione + almeno una checkbox pagamento + importo/data). I messaggi di errore sono gli stessi. Vedi le soluzioni della sanatoria x.2 e applicale alla sezione x.3.

---

### Sanatoria x.4 — Regolarizzazione variante in corso d'opera (art. 34-ter)

#### ATTENZIONE ! Indicare almeno una tipologia del titolo variato.

**Causa**: Hai selezionato x.4 ma non hai indicato né gli estremi del titolo né altri documenti probanti.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"si indicano gli estremi del titolo edilizio variato n. ___ del ___"** → inserisci numero e data con verifica formato
- ☐ **"si allega altra documentazione..."** (principio di prova, art. 9-bis c. 1-bis)

---

#### ATTENZIONE ! Specificare il numero del titolo edilizio. / Specificare la data del titolo edilizio. (x.4)

**Causa**: Hai spuntato "si indicano gli estremi" ma non hai compilato tutti i campi.

**Soluzione**: Inserisci numero e data del titolo edilizio variato nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Specificare l'importo del pagamento. / Specificare la data del pagamento. (x.4 — pagamento oblazione)

**Causa**: Hai spuntato la checkbox di versamento oblazione ma non hai compilato tutti i campi.

**Soluzione**: Inserisci l'importo in € e la data nel formato **GG/MM/AAAA**.

---

## 5. Localizzazione dell'intervento

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma indirizzo non inserito.

**Soluzione**: Compila il campo di testo accanto a "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona dal menu a discesa, oppure spunta ☑ "Toponimo mancante" e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: CAP mancante.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10121`).

{: .warning }
> **CRITICO**: CAP errato blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Numero civico mancante.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito.

**Soluzione**: Aggiungi almeno un fabbricato o terreno dalla sezione mappali, compila i dati e salva con l'icona ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 6. Opere su parti comuni o modifiche esterne

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Opere su parti comuni o modifiche esterne'.

**Causa**: Non hai dichiarato se i lavori riguardano parti comuni.

**Soluzione**: Seleziona **una delle quattro opzioni**:
- ⚪ **"non riguardano parti comuni"**
- ⚪ **"riguardano le parti comuni di un fabbricato condominiale"** ¹
- ⚪ **"riguardano parti comuni di un fabbricato con più proprietà, non costituito in condominio"**
- ⚪ **"riguardano parti di proprietà comune ma non necessitano di assenso"** (art. 1102 c.c.)

---

## 7. Regolarità urbanistica e precedenti edilizi

Questa sezione è la più complessa dell'intero modulo. Richiede la selezione di una delle 5 macro-opzioni (g.1–g.5), più le sotto-checkbox della sezione 6 ("stato attuale dell'immobile"). Il codice valida in sequenza la macro-opzione, poi le sotto-condizioni di ciascuna.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Regolarità urbanistica e precedenti edilizi'.

**Causa**: Non hai indicato la situazione dell'immobile rispetto ai titoli edilizi pregressi.

**Soluzione**: Seleziona **una delle cinque opzioni**:
- ⚪ **g.1** — L'immobile è stato oggetto di titoli/pratiche edilizie → spunta almeno una delle 13 checkbox e compila n. e data
- ⚪ **g.2** — Immobile realizzato in epoca in cui non era obbligatorio titolo abilitativo → spunta almeno una delle 2 checkbox
- ⚪ **g.3** — Non disponibili copia/estremi del titolo ma esiste principio di prova → spunta almeno una delle 2 checkbox
- ⚪ **g.4** — Sanzioni pecuniarie irrogate e versate (artt. 33, 34, 37, 38) → spunta almeno una delle 2 checkbox
- ⚪ **g.5** — Dichiarazioni di tolleranza costruttiva (art. 34-bis o 34-ter c. 4) → spunta almeno una delle 2 checkbox

---

### Opzione g.1 — Titoli e pratiche edilizie

#### ATTENZIONE! Indicare almeno una tipologia di pratica.

**Causa**: Hai selezionato g.1 ma non hai spuntato nessuna delle 13 checkbox dei titoli edilizi.

**Soluzione**: Spunta **almeno una** tra le 13 tipologie di titolo/pratica:
- ☐ Titolo unico (SUAP)
- ☐ Permesso di costruire / licenza / concessione edilizia
- ☐ Autorizzazione edilizia
- ☐ Comunicazione edilizia (art. 26 L. 47/1985)
- ☐ Denuncia di inizio attività
- ☐ DIA/SCIA alternativa al permesso di costruire
- ☐ Segnalazione certificata di inizio attività
- ☐ Comunicazione edilizia libera
- ☐ Titolo in sanatoria con oblazione (condono, PdC in sanatoria, SCIA in sanatoria, variante L. 10/1977)
- ☐ "Altro" (4 righe, ciascuna con tipo + n. + data)

---

#### ATTENZIONE! Specificare numero della pratica. / Specificare data della pratica. (g.1, checkbox 1–8)

**Causa**: Hai spuntato una delle prime 8 checkbox ma non hai compilato n. e/o data.

**Soluzione**: Per ogni checkbox spuntata compila il campo **"n."** e il campo **"del"** nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE! Indicare almeno una tipologia di pratica come 'titolo edilizio in sanatoria con il pagamento della relativa oblazione'. (g.1, checkbox 9)

**Causa**: Hai spuntato la checkbox 9 "titolo edilizio in sanatoria" ma non hai spuntato nessuna delle 4 sotto-opzioni (condono, PdC in sanatoria, SCIA in sanatoria, SCIA variante L. 10/1977).

**Soluzione**: Spunta almeno una delle 4 sotto-tipologie e compila n. e data corrispondenti.

---

#### ATTENZIONE! Specificare tipologia della pratica. / Specificare numero della pratica. / Specificare data della pratica. (g.1, checkbox 10–13 "altro")

**Causa**: Hai spuntato una delle 4 checkbox "altro" ma non hai compilato tutti i campi (tipo + n. + data).

**Soluzione**: Per ogni "altro" spuntato: inserisci la tipologia nel campo di testo, il numero nel campo "n." e la data nel campo "del" in formato GG/MM/AAAA.

---

### Opzione g.2 — Immobile ante-titolo obbligatorio

#### ATTENZIONE! Indicare almeno un tipo di allegato. (g.2)

**Causa**: Hai selezionato g.2 ma non hai spuntato nessuna checkbox.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"copia accatastamento di primo impianto o si forniscono i relativi estremi"** → compila n. e data
- ☐ **"altri documenti probanti (riprese fotografiche, estratti cartografici, ecc.)"**

---

#### ATTENZIONE! Specificare numero della copia accatastamento. / Specificare data della copia accatastamento.

**Causa**: Hai spuntato la checkbox accatastamento ma non hai compilato n. e/o data.

**Soluzione**: Compila il campo **"n."** e il campo **"del"** con la data in formato GG/MM/AAAA.

---

### Opzione g.3 — Principio di prova

Stessa struttura di g.2 (2 checkbox, prima con n. e data). I messaggi di errore sono identici con riferimento alla "copia accatastamento". Vedi le soluzioni di g.2.

---

### Opzione g.4 — Sanzioni pecuniarie versate

#### ATTENZIONE! Indicare almeno una sanzione pecuniaria. (g.4)

**Causa**: Hai selezionato g.4 ma non hai spuntato nessuna checkbox.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"si allega la relativa ricevuta"**
- ☐ **"si forniscono gli estremi del pagamento di € ___ irrogata in data ___, Prot. n. ___, del ___"** → 4 campi obbligatori

---

#### ATTENZIONE! Specificare importo / data del pagamento / numero di protocollo / data di protocollo della sanzione pecuniaria.

**Causa**: Hai spuntato la checkbox "si forniscono gli estremi" ma non hai compilato tutti i 4 campi.

**Soluzione**: Compila importo, data del pagamento, numero di protocollo e data di protocollo — tutti obbligatori. Le date devono essere in formato GG/MM/AAAA.

---

### Opzione g.5 — Dichiarazioni di tolleranza costruttiva

#### ATTENZIONE! Indicare almeno una dichiarazione di tolleranza costruttiva.

**Causa**: Hai selezionato g.5 ma non hai spuntato nessuna checkbox.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"dichiarazione delle tolleranze... presentata nella modulistica relativa alla pratica edilizia prot."** → compila n. e data
- ☐ **"dichiarazione delle tolleranze... allegata agli atti aventi per oggetto trasferimento... atto di registrazione"** → compila n. e data

---

#### ATTENZIONE! Specificare numero di protocollo / data di protocollo della pratica edilizia. / Specificare numero / data dell'atto di registrazione.

**Causa**: Hai spuntato la checkbox ma non hai compilato n. e/o data.

**Soluzione**: Compila il campo **"n."** e il campo **"del"** nel formato GG/MM/AAAA.

---

### Stato attuale dell'immobile — sezione obbligatoria sempre

#### ATTENZIONE! Indicare almeno uno stato attuale dell'immobile.

**Dove si trova**: In fondo alla sezione Regolarità urbanistica → "dichiara che lo stato attuale dell'immobile/U.I. risulta:" → 2 checkbox

**Causa**: Non hai dichiarato se lo stato attuale dell'immobile è conforme alla documentazione indicata sopra. Questa sezione è obbligatoria indipendentemente dalla macro-opzione g.1–g.5 selezionata.

**Soluzione**: Spunta **almeno una** tra:
- ☐ **"pienamente conforme alla documentazione dello stato legittimo o di fatto legittimato sopra indicato"**
- ☐ **"conforme alla documentazione... unitamente alla/e sanatoria/e"** (quando la pratica include anche sanatoria contestuale)

---

## 8. Calcolo del contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Calcolo del contributo di costruzione'.

**Causa**: Non hai dichiarato se l'intervento è gratuito o oneroso.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"è a titolo gratuito, ai sensi della seguente normativa"** → inserisci la norma nel campo di testo
- ⚪ **"è a titolo oneroso"** → seleziona le sotto-checkbox appropriate (calcolo, prospetto, versamento)

---

### ATTENZIONE ! Inserire la normativa. (contributo gratuito)

**Causa**: Hai selezionato "a titolo gratuito" ma non hai inserito la normativa di riferimento.

**Soluzione**: Inserisci nel campo di testo la normativa che esenta dall'obbligo di contributo (es. `art. 17 c. 3 lett. a) DPR 380/2001 — opere di manutenzione straordinaria`, `art. 9 c. 1 lett. d) LR X/XXXX`).

---

## 9. Tecnici incaricati e impresa esecutrice

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Causa**: Non hai dichiarato la situazione relativa al direttore dei lavori.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"di aver incaricato, in qualità di direttori dei lavori e di altri tecnici, i soggetti indicati alla sezione 2 dell'allegato 'Soggetti coinvolti'"**
- ⚪ **"che il/i direttore/i dei lavori e gli altri tecnici incaricati saranno individuati prima dell'inizio dei lavori"** ← questa opzione consente di rimandare il DR

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai dichiarato la situazione relativa all'impresa esecutrice.

**Soluzione**: Seleziona **una delle quattro opzioni**:
- ⚪ **"i lavori sono eseguiti / sono stati eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'Soggetti coinvolti'"** → l'impresa diventa obbligatoria nei soggetti
- ⚪ **"l'impresa esecutrice sarà individuata prima dell'inizio dei lavori"**
- ⚪ **"opere di modesta entità... lavori eseguiti in prima persona"**
- ⚪ **"lavori non eseguiti da impresa (per pratiche in sanatoria)"**

---

### ATTENZIONE ! Non è stata selezionata nessuna Impresa esecutrice dei lavori.

**Causa**: Hai selezionato "lavori da impresa" ma non hai aggiunto nessuna impresa nei soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Imprese"** → Aggiungi l'impresa.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Causa**: Nessun tecnico con ruolo **PR (Progettista)** nei soggetti coinvolti (pratica ordinaria, non sanatoria).

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **PR**.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Direttore Lavori.

**Causa**: Nessun tecnico con ruolo **DR (Direttore Lavori)** e non hai selezionato l'opzione "il DR sarà individuato prima dell'inizio dei lavori".

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **DR**, oppure nella sezione "Tecnici incaricati" seleziona l'opzione che rimanda l'indicazione del DR.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Rilevatore.

**Causa**: Hai attivato la sezione sanatoria ma non hai aggiunto nessun tecnico con ruolo **RI (Rilevatore)**.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **RI – Rilevatore**.

{: .note }
> Quando la sezione sanatoria è attiva (checkbox `chkSanatoriax1_0` spuntata), il sistema richiede il **Rilevatore** invece di Progettista + Direttore Lavori. Se la sanatoria non è attiva, servono Progettista (PR) e Direttore Lavori (DR), a meno che non venga selezionata l'opzione "il DR sarà individuato prima dell'inizio".

---

## 10. Sicurezza sul lavoro — D.Lgs. 81/2008

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Applicazione delle norme in materia di salute e sicurezza sul luogo di lavoro (d.lgs. n. 81/2008)'.

**Causa**: Non hai dichiarato se i lavori rientrano nell'ambito di applicazione del D.Lgs. 81/2008.

**Soluzione**: Seleziona **una delle tre opzioni**:
- ⚪ **"non ricade nell'ambito di applicazione"** → nessun altro adempimento
- ⚪ **"ricade nell'ambito di applicazione"** → seleziona poi le dichiarazioni sulle imprese e sulla notifica
- ⚪ **"ricade ma si riserva di presentare le dichiarazioni prima dell'inizio lavori"** (dati impresa non ancora disponibili)

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai dichiarato che i lavori ricadono nel D.Lgs. 81/2008 ma non hai specificato la documentazione delle imprese.

**Soluzione**: Seleziona **una delle due opzioni** relative alla documentazione:
- ⚪ Cantiere **< 200 uomini-giorno** e senza rischi allegato XI → si dichiara verifica di CCIAA, DURC, autocertificazione contratto
- ⚪ Cantiere **≥ 200 uomini-giorno** o con rischi allegato XI → si dichiara verifica documentazione art. 90 c. 9 D.Lgs. 81/2008

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato la seconda opzione (cantiere ≥ 200 UG) ma non hai dichiarato la situazione relativa alla notifica preliminare.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"l'intervento non è soggetto all'invio della notifica"**
- ⚪ **"l'intervento è soggetto all'invio della notifica"** → spunta la checkbox "allega" la notifica

---

## Consigli pratici SCIA Nazionale

### Prima di validare ✅

- [ ] Compila il menu a discesa **titolarità** + seleziona radio button
- [ ] Seleziona la **tipologia di presentazione** (b.1/b.2/b.3) e inserisci la data se b.1 o b.2
- [ ] Seleziona la **qualificazione** (c.1–c.8) + la relativa sotto-opzione
- [ ] Per c.4/c.5/c.6: inserisci **n. e data** del titolo di riferimento
- [ ] Inserisci la **descrizione sintetica** dell'intervento
- [ ] Se sanatoria: spunta checkbox + seleziona tipologia (x.1–x.4) + compila i campi richiesti
- [ ] Seleziona l'**indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona le **opere su parti comuni** (e.1–e.4)
- [ ] Seleziona la **regolarità urbanistica** (g.1–g.5) + compila tutte le sotto-checkbox
- [ ] Spunta almeno una checkbox della sezione **"stato attuale dell'immobile"**
- [ ] Seleziona il **contributo** (gratuito con norma / oneroso)
- [ ] Seleziona la voce **tecnici incaricati**
- [ ] Seleziona la voce **impresa esecutrice**
- [ ] Aggiungi nei soggetti coinvolti: **PR** (Progettista) + **DR** (Direttore Lavori), oppure **RI** (Rilevatore) se sanatoria
- [ ] Seleziona la voce **sicurezza D.Lgs. 81/2008** e compila le sotto-dichiarazioni se necessario
- [ ] **Salva** frequentemente

### Errori frequenti SCIA Nazionale 🔍

1. **Sotto-opzione qualificazione non selezionata** → c.1/c.2/c.3 richiedono obbligatoriamente una delle 4 sotto-opzioni sul mutamento d'uso; c.7/c.8 richiedono rispettivamente 4 o 2 sotto-opzioni
2. **Stato attuale immobile non spuntato** → le due checkbox "stato attuale" in fondo alla sezione Regolarità urbanistica sono obbligatorie sempre, indipendentemente dalla g.1–g.5 selezionata
3. **Sanatoria attiva = logica tecnici diversa** → con sanatoria serve il Rilevatore (RI), non Progettista + DR
4. **Contributo gratuito senza norma** → il campo di testo accanto a "a titolo gratuito" è obbligatorio; non basta selezionare il radio button
5. **g.1 con checkbox spuntate ma n./data mancanti** → ogni checkbox delle prime 8 richiede n. e data; omettere anche solo uno dei due genera errore
6. **"Stato attuale" sezione 6 dimenticata** → visivamente separata dalle sezioni g.1–g.5, spesso non trovata

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
**Fonte**: Analisi codice ValidaDatiSCIANazionale e DatiSCIANaz.ascx
