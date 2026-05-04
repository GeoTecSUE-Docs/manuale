---
title: Errori Segnalazione Certificata di Agibilità - Regione Lombardia
parent: Errori di validazione
nav_order: 32
description: Errori di validazione specifici per la Segnalazione Certificata di Agibilità (SCA) - Regione Lombardia (art. 24 D.P.R. 380/2001, L.R. 12/2005)
keywords: [segnalazione certificata agibilità, SCA, agibilità, Lombardia, coordinate UTM, titolo edilizio, fine lavori contestuale, SCIA agibilità, direttore lavori, sezione B]
IDRegione: 4
IDTipoPratica: 412
Fonte: Manuale
---

# Errori di validazione - Segnalazione Certificata di Agibilità (SCA)
## Regione Lombardia

Guida completa agli errori specifici per la **Segnalazione Certificata di Agibilità** ai sensi dell'art. 24 del D.P.R. 6 giugno 2001, n. 380 e della L.R. Lombardia 11 marzo 2005, n. 12, relativa alla **Regione Lombardia**.

{: .note }
> La SCA Lombardia è una delle pratiche più articolate della piattaforma. Include obbligatoriamente le **coordinate UTM WGS 84 32N** (stessa logica del Fine Lavori Lombardia), la dichiarazione del **titolo edilizio** che ha legittimato l'intervento (in due varianti alternative: titolo esterno a GeoTecSUE con 6 campi, oppure titolo presente su GeoTecSUE con selezione da menu), la sezione **comunicazione di fine lavori** (già presentata, contestuale o collaudo allegato), la scelta della **tipologia di agibilità** (SCIA o SCIA Unica, totale o parziale), e tre **checkbox documenti** tutte obbligatorie (Sezione B, Quadro Riepilogativo, Privacy). Nei soggetti coinvolti è richiesto almeno un tecnico con ruolo **TA** (Professionista incaricato Agibilità) o **DR** (Direttore Lavori). Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento e coordinate UTM](#1-localizzazione-dellintervento-e-coordinate-utm)
2. [Titolo edilizio di riferimento](#2-titolo-edilizio-di-riferimento)
3. [Comunicazione di fine lavori](#3-comunicazione-di-fine-lavori)
4. [Presentazione agibilità — SCIA o SCIA Unica](#4-presentazione-agibilità--scia-o-scia-unica)
5. [Documenti allegati e privacy — tre checkbox obbligatorie](#5-documenti-allegati-e-privacy--tre-checkbox-obbligatorie)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

---

## 1. Localizzazione dell'intervento e coordinate UTM

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

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `20121`).

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

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Dove si trova**: Campo **"Coord. asse X"** nella sezione Coordinate dell'intervento (UTM – WGS 84 32N)

**Causa**: Il campo coordinata X è vuoto.

**Soluzione**: Inserisci la coordinata X nel campo corrispondente. Deve essere compresa tra **430.000 e 700.000** (es. `514500`). Usa il punto come separatore decimale, non la virgola.

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: La coordinata X inserita è fuori dal range valido oppure contiene caratteri non numerici o usa la virgola come separatore decimale.

**Soluzione**: Verifica che la coordinata X sia un numero compreso tra **430.000 e 700.000**. Usa il punto (es. `514500.5` ✅ — `514500,5` ❌).

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Causa**: Il campo coordinata Y è vuoto.

**Soluzione**: Inserisci la coordinata Y: un numero compreso tra **4.800.000 e 5.700.000** (es. `5034200`).

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: La coordinata Y è fuori dal range valido oppure in formato errato.

**Soluzione**: Verifica che la coordinata Y sia compresa tra **4.800.000 e 5.700.000**. Usa il punto come separatore decimale.

---

## 2. Titolo edilizio di riferimento

Questa sezione permette di indicare il titolo edilizio che ha legittimato l'intervento in due modi alternativi, tramite due checkbox distinte. **Almeno una** deve essere spuntata.

---

### ATTENZIONE ! Non è stata selezionata la comunicazione che legittima l'intervento.

**Causa**: Non hai spuntato nessuna delle due checkbox che identificano il titolo edilizio di riferimento.

**Soluzione**: Spunta **una** delle due opzioni disponibili:
- ☐ **Titolo esterno a GeoTecSUE** (`chkComunicazFLa_0`) → "che il titolo e/o la comunicazione... (selezionare questa voce se il titolo non è presente su GeoTecSUE)" → compila i 6 campi manuali
- ☐ **Titolo su GeoTecSUE** (`chkComunicazFLa_3`) → "che il titolo... (selezionare questa voce se il titolo è presente su GeoTecSUE)" → seleziona dal menu a discesa il tipo e il riferimento

---

### Titolo esterno a GeoTecSUE — 6 campi obbligatori

Se hai spuntato la prima checkbox (titolo non presente su GeoTecSUE), devi compilare tutti e 6 i campi seguenti.

#### ATTENZIONE ! Inserire il tipo di procedimento.

**Causa**: Campo "Tipo procedimento" vuoto.

**Soluzione**: Inserisci il tipo di pratica edilizia (es. `CILA`, `SCIA`, `Permesso di Costruire`).

---

#### ATTENZIONE ! Inserire ufficio SUAP/SUE. (titolo esterno)

**Causa**: Campo "SUAP/SUE" vuoto.

**Soluzione**: Inserisci la sigla o il nome dell'ufficio ricevente (es. `SUE`, `SUAP`).

---

#### ATTENZIONE ! Comune non indicato. (titolo esterno)

**Causa**: Campo "del Comune di" vuoto.

**Soluzione**: Inserisci il nome del Comune che ha ricevuto il titolo edilizio (es. `Milano`, `Bergamo`).

---

#### ATTENZIONE ! Inserire il numero di pratica. (titolo esterno)

**Causa**: Campo "Pratica edilizia" vuoto.

**Soluzione**: Inserisci il numero o la denominazione della pratica edilizia (es. `CILA-2023-42`, `SCIA 2024/15`).

---

#### ATTENZIONE ! Inserire il prot. / n. di pratica. (titolo esterno)

**Causa**: Campo "prot. / n." vuoto.

**Soluzione**: Inserisci il numero di protocollo del titolo edilizio (es. `PROT-2023-45678`).

---

#### ATTENZIONE ! Campo obbligatorio 'Data protocollo' non inserito.

**Causa**: Campo data del titolo edilizio vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA** (es. `15/06/2023`).

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data titolo esterno)

**Causa**: La data del titolo edilizio è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

### Titolo su GeoTecSUE — selezione da menu

Se hai spuntato la seconda checkbox (titolo presente su GeoTecSUE), devi selezionare il tipo di titolo e poi la pratica specifica dai menu a discesa.

#### ATTENZIONE ! Selezionare il titolo abitativo edilizio.

**Causa**: Il primo menu a discesa del titolo su GeoTecSUE è rimasto sulla voce iniziale (nessuna selezione).

**Soluzione**: Seleziona il tipo di titolo edilizio dal primo menu (es. CILA, SCIA, Permesso di Costruire). La selezione abilita il secondo menu.

---

#### ATTENZIONE ! Selezionare il riferimento della pratica.

**Causa**: Hai selezionato il tipo di titolo ma non hai selezionato la pratica specifica dal secondo menu.

**Soluzione**: Seleziona la pratica di riferimento dal secondo menu a discesa, che si popola automaticamente dopo la selezione del tipo.

---

## 3. Comunicazione di fine lavori

Questa sezione richiede che almeno una delle tre checkbox sia spuntata. Le opzioni non si escludono: è possibile spuntarne più di una se la situazione lo richiede.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione di fine dei lavori'.

**Causa**: Nessuna delle tre checkbox sulla comunicazione di fine lavori è stata spuntata.

**Soluzione**: Spunta **almeno una** tra le tre opzioni:
- ☐ **FL già presentata** (`chkComunicazFLa_1`) → "che la comunicazione di fine lavori è stata già presentata al SUE/SUAP" → compila SUAP/SUE, Comune, prot./n. e data
- ☐ **FL contestuale** (`chkComunicazFLa_2`) → "che la presente segnalazione vale come comunicazione di fine lavori e a tal fine attesta che gli stessi sono stati ultimati in data ___" → inserisci data e seleziona tipo ultimazione
- ☐ **Collaudo allegato** (`chkAllegaCertCollaudo`) → "allega certificato di collaudo finale/parziale ai sensi dell'art. 23 c. 7 DPR 380/01" → solo per SCIA Alternativa al Permesso di Costruire

---

### Fine lavori già presentata (chkComunicazFLa_1) — 4 campi

Se hai spuntato la checkbox "FL già presentata", devi compilare i 4 campi seguenti.

#### ATTENZIONE ! Inserire ufficio SUAP/SUE. (FL già presentata)

**Causa**: Campo "SUAP/SUE" della fine lavori già presentata vuoto.

**Soluzione**: Inserisci la sigla dell'ufficio ricevente la comunicazione di fine lavori (es. `SUE`, `SUAP`).

---

#### ATTENZIONE ! Comune non indicato. (FL già presentata)

**Causa**: Campo "del Comune di" vuoto.

**Soluzione**: Inserisci il Comune dove è stata presentata la comunicazione di fine lavori.

---

#### ATTENZIONE ! Inserire il prot. / n. di pratica. (FL già presentata)

**Causa**: Campo prot./n. della comunicazione di fine lavori già presentata vuoto.

**Soluzione**: Inserisci il numero di protocollo della comunicazione di fine lavori.

---

#### ATTENZIONE ! Campo obbligatorio 'Data pratica' non inserito.

**Causa**: Campo data della comunicazione di fine lavori già presentata vuoto.

**Soluzione**: Inserisci la data della comunicazione di fine lavori nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data FL già presentata)

**Causa**: La data della comunicazione di fine lavori già presentata è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

### Fine lavori contestuale (chkComunicazFLa_2) — data + tipo ultimazione

Se hai spuntato la checkbox "FL contestuale", devi compilare la data e selezionare il tipo di ultimazione.

#### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Causa**: Campo data di ultimazione dei lavori vuoto.

**Soluzione**: Inserisci la data in cui i lavori sono stati ultimati nel formato **GG/MM/AAAA** (es. `20/04/2026`).

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori contestuale)

**Causa**: La data di fine lavori è in formato errato.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo ultimazione lavori'.

**Dove si trova**: Due radio button sotto la data di fine lavori: "completamente" e "in forma parziale come da planimetria allegata"

**Causa**: Hai inserito la data di fine lavori ma non hai dichiarato se i lavori sono stati ultimati completamente o parzialmente.

**Soluzione**: Seleziona **una** delle due opzioni:
- ⚪ **"completamente"**
- ⚪ **"in forma parziale come da planimetria allegata"** → allega la planimetria

---

## 4. Presentazione agibilità — SCIA o SCIA Unica

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione agibilità'.

**Dove si trova**: Sezione **"PRESENTA"** → 6 radio button divisi in due gruppi (SCIA e SCIA Unica)

**Causa**: Non hai indicato per quale tipo di agibilità si presenta la segnalazione.

**Soluzione**: Seleziona **una delle sei opzioni**:

**SCIA per:**
- ⚪ **"l'agibilità relativa all'immobile oggetto dell'intervento edilizio"** (agibilità totale)
- ⚪ **"l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione"** (art. 24, c. 4, lett. a))
- ⚪ **"l'agibilità parziale relativa a singole unità immobiliari"** (art. 24, c. 4, lett. b))

**SCIA Unica per:**
- ⚪ **"l'agibilità relativa all'immobile oggetto dell'intervento edilizio"** (con altre segnalazioni allegate)
- ⚪ **"l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione"**
- ⚪ **"l'agibilità parziale relativa a singole unità immobiliari"**

{: .note }
> SCIA e SCIA Unica differiscono per la presenza o meno di ulteriori segnalazioni allegate. Con la **SCIA Unica** si allegano contestualmente le altre comunicazioni/attestazioni/asseverazioni indicate nel quadro riepilogativo.

---

## 5. Documenti allegati e privacy — tre checkbox obbligatorie

Tutte e tre le checkbox seguenti sono sempre obbligatorie. Il sistema le verifica in sequenza: prima `chkSezB`, poi `chkSezCD`, poi `chkPrivacy`.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'SEZIONE B Attestazione del direttore dei lavori o del professionista abilitato'.

**Dove si trova**: Sezione **"ED ALLEGA"** → prima checkbox

**Causa**: Non hai dichiarato di allegare la Sezione B del modulo (attestazione del direttore dei lavori o professionista abilitato).

**Soluzione**: Spunta la checkbox ☑ **"SEZIONE B 'Attestazione del direttore dei lavori o del professionista abilitato', sottoscritta dal direttore dei lavori o tecnico abilitato"**.

{: .note }
> La Sezione B è un documento separato che deve essere fisicamente allegato alla SCA. Spuntare la checkbox dichiara che tale documento è stato predisposto e allegato. Non è possibile presentare la SCA senza la Sezione B.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'SEZIONE Quadro Riepilogativo della documentazione allegata'.

**Dove si trova**: Sezione **"ED ALLEGA"** → seconda checkbox

**Causa**: Non hai dichiarato di allegare le comunicazioni o segnalazioni del Quadro Riepilogativo.

**Soluzione**: Spunta la checkbox ☑ **"le comunicazioni o segnalazioni di cui alla sezione 'Quadro Riepilogativo della documentazione allegata' debitamente firmato dal direttore dei lavori o tecnico abilitato"**.

---

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione **"INFORMATIVA SUL TRATTAMENTO DEI DATI PERSONALI"** → checkbox in fondo all'informativa

**Causa**: Non hai dichiarato di aver letto l'informativa sul trattamento dei dati personali.

**Soluzione**: Spunta la checkbox ☑ **"Il/la sottoscritto/a dichiara di aver letto l'informativa sul trattamento dei dati personali pubblicata sul sito istituzionale del SUAP/SUE"**.

{: .note }
> La SCA Lombardia usa l'informativa privacy GDPR (Reg. UE 2016/679) con checkbox dedicata, a differenza di molte altre pratiche dove la privacy è solo testo informativo senza checkbox. La checkbox si trova in fondo all'informativa, quasi in fondo all'intero modulo.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Professionista incaricato per Agibilità o come Direttore Lavori.

**Dove si trova**: Sezione **"Soggetti coinvolti"** → Tecnici

**Causa**: Non hai aggiunto nessun tecnico con ruolo **TA** (Professionista incaricato Agibilità) o **DR** (Direttore Lavori).

**Soluzione**:
1. Vai alla sezione **"Soggetti coinvolti"** → **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Compila i dati del tecnico e seleziona il ruolo **"TA – Professionista incaricato Agibilità"** oppure **"DR – Direttore Lavori"**
4. Clicca l'**icona ✅** per salvare
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La SCA Lombardia è una delle poche pratiche della piattaforma che accetta due ruoli alternativi nel controllo tecnico: il **Professionista incaricato Agibilità (TA)** — figura specifica per l'agibilità — oppure il **Direttore Lavori (DR)**. È sufficiente che almeno uno dei due ruoli sia presente; non è necessario averli entrambi.

---

## Consigli pratici SCA Lombardia

### Prima di validare ✅

- [ ] Seleziona l'**indirizzo** della località
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci le **coordinate UTM** (X: 430.000–700.000; Y: 4.800.000–5.700.000), separatore decimale con punto
- [ ] Spunta la **checkbox del titolo edilizio** (esterno a GeoTecSUE o su GeoTecSUE) e compila tutti i campi richiesti
- [ ] Spunta **almeno una** delle tre checkbox di **fine lavori** (FL già presentata / FL contestuale / Collaudo allegato)
- [ ] Se FL già presentata: compila SUAP/SUE, Comune, prot./n. e data
- [ ] Se FL contestuale: inserisci data e seleziona tipo ultimazione
- [ ] Seleziona la **tipologia di agibilità** (uno dei 6 radio button SCIA/SCIA Unica)
- [ ] Spunta ☑ **Sezione B** (attestazione direttore lavori/professionista)
- [ ] Spunta ☑ **Quadro Riepilogativo** (comunicazioni firmate)
- [ ] Spunta ☑ **Privacy** (informativa GDPR in fondo al modulo)
- [ ] Aggiungi un tecnico con ruolo **TA** o **DR** nei soggetti coinvolti
- [ ] **Salva** frequentemente

### Struttura unica della SCA Lombardia ⚠️

La SCA Lombardia ha tre caratteristiche non presenti in altre pratiche. Il **doppio binario per il titolo edilizio**: il titolo può essere indicato manualmente (6 campi) se non è su GeoTecSUE, oppure selezionato da menu se è su GeoTecSUE — le due opzioni sono checkbox alternative. Le **tre checkbox fine lavori compatibili**: a differenza di tutti i moduli con radio button, le tre opzioni di fine lavori (già presentata, contestuale, collaudo) sono checkbox non esclusive e almeno una deve essere spuntata. Le **tre checkbox documenti tutte obbligatorie**: Sezione B, Quadro Riepilogativo e Privacy devono essere spuntate tutte e tre prima di poter validare.

### Errori frequenti SCA Lombardia 🔍

1. **Coordinate UTM mancanti o fuori range** → come per il Fine Lavori Lombardia; usare il punto come separatore decimale
2. **Nessuna checkbox titolo edilizio spuntata** → la sezione "DICHIARA" ha le due checkbox visivamente simili; è necessario spuntarne almeno una
3. **Nessuna checkbox fine lavori spuntata** → le tre opzioni si trovano dopo i blocchi del titolo edilizio; facile da dimenticare
4. **Tipo ultimazione non selezionato** → se si spunta la FL contestuale (chkc2), appare la data e poi i radio button completamente/parzialmente; la data senza il radio non è sufficiente
5. **Sezione B o Quadro Riepilogativo non spuntati** → checkbox nella sezione "ED ALLEGA" quasi in fondo al modulo
6. **Privacy non spuntata** → l'informativa privacy è molto lunga; la checkbox è alla fine del testo, facile da non raggiungere con lo scroll
7. **Tecnico mancante** → la SCA richiede un tecnico con ruolo TA o DR, non il Progettista (PR) usato nelle pratiche edilizie ordinarie

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
**Fonte**: Analisi codice ValidaDatiSCALombardia e DatiSCALombardia.ascx
