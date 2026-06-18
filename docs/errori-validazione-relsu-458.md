---
title: Errori Relazione a Strutture Ultimate - Lombardia
parent: Errori di validazione
nav_order: 45
description: Errori di validazione specifici per la Trasmissione di Relazione a Strutture Ultimate (RelSU) - Regione Lombardia
keywords: [relazione strutture ultimate, RelSU, Lombardia, art. 93 DPR 380/2001, conglomerato cementizio, struttura metallica, data ultimazione lavori, collaudatore, coordinate UTM, WGS84, privacy, denuncia strutturale]
IDRegione: 4         # Lombardia
IDTipoPratica: 458
Fonte: Manuale
---

# Errori di validazione - Relazione a Strutture Ultimate (RelSU)
## Regione Lombardia

Guida completa agli errori specifici per la **Trasmissione di Relazione a Strutture Ultimate** per opere in conglomerato cementizio armato normale, precompresso o a struttura metallica, ai sensi dell'art. 93 del D.P.R. 06/06/2001 n. 380 — Regione Lombardia.

{: .note }
> Questa pratica è strutturalmente simile al **Collaudo/DRE Lombardia** (`DatiCCLombardia`) ma con alcune differenze chiave: al posto della selezione collaudo/DRE è presente il riferimento alla **denuncia ai sensi dell'art. 93 D.P.R. 380/2001** (numero + data), e in più è richiesta la **data di ultimazione lavori** (campo `txtDataFineLavori`) e la **checkbox di avvenuta comunicazione al collaudatore**. Le **coordinate UTM-WGS84 32N** sono obbligatorie con gli stessi range del Collaudo/DRE. La **checkbox privacy è obbligatoria**. Non sono presenti sezioni di titolarità, opere su parti comuni, date inizio lavori o sicurezza D.Lgs. 81/2008. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Denuncia di riferimento — numero e data](#1-denuncia-di-riferimento--numero-e-data)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Coordinate geografiche UTM](#3-coordinate-geografiche-utm)
4. [Data di ultimazione lavori](#4-data-di-ultimazione-lavori)
5. [Dichiarazione — comunicazione al collaudatore](#5-dichiarazione--comunicazione-al-collaudatore)
6. [Privacy](#6-privacy)

---

## 1. Denuncia di riferimento — numero e data

### ATTENZIONE ! Inserire il numero pratica di riferimento.

**Dove si trova**: Sezione **"Relativamente a"** in cima al modulo → campo numero accanto a "Denuncia ai sensi dell'art. 93 D.P.R. 06/06/2001 n. 380 n."

**Causa**: Non hai indicato il numero della denuncia strutturale a cui si riferisce la relazione a strutture ultimate.

**Soluzione**: Inserisci il numero della denuncia nel campo accanto a **"Denuncia ai sensi dell'art. 93 D.P.R. 380/2001 n."** (max 20 caratteri). Si tratta del numero assegnato all'atto della presentazione della denuncia delle opere strutturali.

---

### ATTENZIONE ! Inserire la data della pratica di riferimento.

**Dove si trova**: Sezione **"Relativamente a"** → campo **"del"** accanto al numero

**Causa**: Non hai inserito la data della denuncia strutturale di riferimento.

**Soluzione**: Inserisci la data nel campo **"del"** nel formato **GG/MM/AAAA** (es. `10/04/2023`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data della denuncia di riferimento è in un formato non riconosciuto dal sistema.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `10/04/2023` ✅. Errati: `10-04-2023` ❌, `10/04/23` ❌.

---

## 2. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa **"Indirizzo (Via, Viale, Piazza, ecc.)"**, oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente nel campo di testo.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `20121`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non è stato inserito nessun mappale catastale né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila i campi Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva la riga con l'icona ✅ (tasto verde con spunta)

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata nella ListBox.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Per selezionare più voci tieni premuto CTRL mentre clicchi.

---

## 3. Coordinate geografiche UTM

Questa sezione è **esclusiva delle pratiche lombarde** e richiede le coordinate piane dell'intervento nel sistema **UTM - WGS 84 32N**, espresse in metri. Il sistema valida sia la presenza sia il range numerico di ciascuna coordinata.

---

### ATTENZIONE ! Inserire coordinata X della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo **"Coord. asse X"**

**Causa**: Il campo della coordinata X è vuoto.

**Soluzione**: Inserisci la coordinata X (est) nel campo **"Coord. asse X"**. Il valore deve essere un numero compreso tra **430.000 e 700.000** metri.

---

### ATTENZIONE ! La coordinata X deve essere compresa tra 430000 e 700000.

**Causa**: Il valore inserito per la coordinata X non è un numero valido oppure è fuori dal range accettato per il territorio lombardo nel sistema UTM-WGS84 32N.

**Soluzione**:
1. Verifica che il valore sia un **numero** (es. `514823` oppure `514823.45`) — nessun punto migliaia, nessun simbolo
2. Il valore deve essere **≥ 430.000** e **≤ 700.000**
3. Se non disponi delle coordinate, usa il pulsante **"Calcola Coordinate"** (se visibile) oppure consulta il geoportale regionale o un GIS

{: .note }
> Le coordinate UTM-WGS84 32N per la Lombardia hanno tipicamente coordinata X intorno a 450.000–570.000 e coordinata Y intorno a 4.950.000–5.200.000. Se il valore è molto diverso, probabilmente stai usando un sistema di riferimento diverso (es. Gauss-Boaga o gradi decimali). Il campo accetta valori decimali con il punto come separatore (es. `514823.5`).

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo **"Coord. asse Y"**

**Causa**: Il campo della coordinata Y è vuoto.

**Soluzione**: Inserisci la coordinata Y (nord) nel campo **"Coord. asse Y"**. Il valore deve essere un numero compreso tra **4.800.000 e 5.700.000** metri.

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Il valore inserito per la coordinata Y non è un numero valido oppure è fuori dal range accettato.

**Soluzione**:
1. Verifica che il valore sia un **numero** (es. `5034512` oppure `5034512.3`) — nessun punto migliaia, nessun simbolo
2. Il valore deve essere **≥ 4.800.000** e **≤ 5.700.000**
3. Se non disponi delle coordinate, consulta il geoportale regionale o un GIS

{: .warning }
> **Errore frequente**: inserire le coordinate in gradi decimali (es. `45.46` per la latitudine) invece che in metri UTM. Un valore come `45` o `9.18` è in gradi e causerà sempre questo errore perché fuori range. Occorre convertire nel sistema UTM-WGS84 32N prima di inserire.

---

## 4. Data di ultimazione lavori

### ATTENZIONE ! Inserire la data di ultimazione lavori.

**Dove si trova**: Sezione **"Deposita"** → campo data accanto a "ultimate in data"

**Causa**: Non hai inserito la data in cui le strutture sono state ultimate.

**Soluzione**: Inserisci la data di ultimazione lavori nel campo **"ultimate in data"** nel formato **GG/MM/AAAA** (es. `20/05/2024`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(ultimazione lavori)*

**Causa**: La data di ultimazione lavori è in un formato non riconosciuto dal sistema.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `20/05/2024` ✅. Errati: `20-05-2024` ❌, `20/05/24` ❌.

{: .warning }
> **Bug noto nel codice**: la validazione del formato della data di ultimazione lavori (`txtDataFineLavori`) controlla erroneamente il contenuto del campo `txtDataPratica` (data della denuncia di riferimento) invece di `txtDataFineLavori`. In pratica, se la data della denuncia è già in formato corretto, il controllo formato sulla data di ultimazione non si attiva mai — anche se quest'ultima fosse in formato errato. Il campo viene comunque controllato per la presenza (campo vuoto = errore). Segnalare al team di sviluppo per correzione.

---

## 5. Dichiarazione — comunicazione al collaudatore

### ATTENZIONE ! Selezionare la voce relativa alla comunicazione di avvenuto termine dei lavori al collaudatore nominato per le opere.

**Dove si trova**: Sezione **"Dichiarazioni"** → checkbox **"che è stata data comunicazione di avvenuto termine dei lavori al collaudatore nominato per le opere"**

**Causa**: Non hai spuntato la dichiarazione obbligatoria di avvenuta comunicazione al collaudatore.

**Soluzione**: Leggi la dichiarazione e, se corrispondente al vero, spunta la checkbox:
- ☑ **"che è stata data comunicazione di avvenuto termine dei lavori al collaudatore nominato per le opere"**

{: .note }
> Questa dichiarazione attesta che il collaudatore delle opere strutturali è stato regolarmente informato del completamento dei lavori, come previsto dalla normativa sulle opere in cemento armato e strutture metalliche. Non è possibile depositare la relazione a strutture ultimate senza aver prima dato questa comunicazione al collaudatore.

---

## 6. Privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione **"Rispetto della normativa sulla privacy"**

**Causa**: Non hai spuntato la checkbox di accettazione dell'informativa privacy.

**Soluzione**: Leggi l'informativa sulla privacy riportata in fondo al modulo (Art. 13 del D.Lgs. n. 196/2003), quindi spunta la checkbox:
- ☑ **"di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune"**

{: .warning }
> Come per il Collaudo/DRE Lombardia, la checkbox privacy è **obbligatoria** per completare la validazione. Non è possibile procedere con "Valida e Salva" senza averla spuntata.

---

## Consigli pratici Relazione a Strutture Ultimate

### Prima di validare ✅

- [ ] Inserisci il **numero della denuncia** ex art. 93 D.P.R. 380/2001
- [ ] Inserisci la **data della denuncia** di riferimento nel formato GG/MM/AAAA
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **coordinata X** (numero tra 430.000 e 700.000, sistema UTM-WGS84 32N)
- [ ] Inserisci la **coordinata Y** (numero tra 4.800.000 e 5.700.000, sistema UTM-WGS84 32N)
- [ ] Inserisci la **data di ultimazione lavori** nel formato GG/MM/AAAA
- [ ] Spunta la checkbox **"comunicazione al collaudatore"**
- [ ] Spunta la **checkbox privacy**
- [ ] **Salva** frequentemente

### Confronto con Collaudo/DRE Lombardia ⚠️

| Campo | Collaudo/DRE (`DatiCCLombardia`) | RelSU (`DatiRelSULombardia`) |
|---|---|---|
| Riferimento pratica | Numero pratica generica | Numero **denuncia art. 93** D.P.R. 380/2001 |
| Tipo documento | Radio button (collaudo / DRE) | Non presente |
| Descrizione lavori | Campo testo libero | Non presente |
| Data ultimazione lavori | Non presente | ☑ Campo obbligatorio |
| Comunicazione collaudatore | Non presente | ☑ Checkbox obbligatoria |
| Sisma Bonus | ☑ Checkbox condizionale | Non presente |
| Coordinate UTM | ☑ Obbligatorie | ☑ Obbligatorie (stesso range) |
| Privacy | ☑ Obbligatoria | ☑ Obbligatoria |

### Errori frequenti RelSU Lombardia 🔍

1. **Numero denuncia mancante** → è il primo controllo; senza di esso nulla viene validato
2. **Coordinate in gradi decimali** → i valori devono essere in metri UTM-WGS84 32N, non in gradi (es. `515000` non `9.18`)
3. **Data ultimazione lavori vuota** → il campo è nella sezione "Deposita", visivamente separata dalla sezione "Relativamente a"; facile da saltare
4. **Checkbox collaudatore non spuntata** → obbligatoria; la relazione non può essere depositata senza aver comunicato il termine lavori al collaudatore
5. **Privacy non spuntata** → come per tutte le pratiche lombarde, è obbligatoria e posizionata in fondo al modulo

### Bug documentato: validazione data ultimazione lavori ⚠️

Il controllo del formato della data di ultimazione (`txtDataFineLavori`) nel codice VB verifica erroneamente il campo `txtDataPratica`:

```vb
' Codice attuale (errato):
If clsModuloAsp.ControlloFormatoData(CType(...FindControl("txtDataPratica"), TextBox).Text) = False Then

' Codice corretto atteso:
If clsModuloAsp.ControlloFormatoData(CType(...FindControl("txtDataFineLavori"), TextBox).Text) = False Then
```

**Conseguenza pratica**: se la data della denuncia (`txtDataPratica`) è in formato valido, il sistema non valida il formato di `txtDataFineLavori` — anche se quest'ultima contenesse una data in formato errato. Il campo viene comunque verificato per la presenza (vuoto = errore). Inserire sempre le date in formato GG/MM/AAAA per evitare problemi.

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
**Fonte**: Analisi codice `ValidaDatiRelSULombardia` e `DatiRelSULombardia.ascx`
