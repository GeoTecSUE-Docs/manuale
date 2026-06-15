---
title: Errori Collaudo/DRE - Lombardia
parent: Errori di validazione
nav_order: 41
description: Errori di validazione specifici per il Collaudo Statico / Dichiarazione di Regolare Esecuzione (DRE) - Regione Lombardia
keywords: [collaudo statico, DRE, dichiarazione regolare esecuzione, Lombardia, coordinate UTM, WGS84, sisma bonus, privacy, pratica di riferimento]
IDRegione: 4
IDTipoPratica: 459
Fonte: Manuale
---

# Errori di validazione - Collaudo Statico / DRE
## Regione Lombardia

Guida completa agli errori specifici per la **Comunicazione di Collaudo Statico o Dichiarazione di Regolare Esecuzione (DRE)** nella Regione Lombardia.

{: .note }
> Questa pratica è **esclusiva della Lombardia** e presenta caratteristiche non presenti in nessun'altra pratica della piattaforma: la **selezione obbligatoria del tipo di documento** (collaudo statico o DRE), i campi **numero e data della pratica di riferimento**, le **coordinate geografiche UTM-WGS84 con range numerico validato**, la sezione **Sisma Bonus** con logica condizionale, e la **checkbox privacy obbligatoria** (a differenza della C.I.L. nazionale dove la privacy è solo informativa). Non sono presenti le sezioni Titolarità, Opere su parti comuni, date lavori o Sicurezza D.Lgs. 81/2008. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Tipo di presentazione — collaudo o DRE](#1-tipo-di-presentazione--collaudo-o-dre)
2. [Pratica di riferimento — numero e data](#2-pratica-di-riferimento--numero-e-data)
3. [Localizzazione dell'intervento](#3-localizzazione-dellintervento)
4. [Coordinate geografiche UTM](#4-coordinate-geografiche-utm)
5. [Sisma Bonus](#5-sisma-bonus)
6. [Privacy](#6-privacy)

---

## 1. Tipo di presentazione — collaudo o DRE

### ATTENZIONE ! Non è stata selezionata nessuna voce per il tipo di presentazione (collaudo o DRE).

**Dove si trova**: Sezione **"Di presentare"** in cima al modulo

**Causa**: Non hai selezionato quale documento stai presentando.

**Soluzione**: Seleziona **una delle due opzioni**:
- ⚪ **"certificato di collaudo statico"**
- ⚪ **"dichiarazione di regolare esecuzione (DRE)"**

{: .note }
> La scelta tra collaudo statico e DRE dipende dalla tipologia e complessità dei lavori strutturali eseguiti. Se non sei sicuro di quale documento presentare, contatta il professionista incaricato o l'ufficio SUE prima di procedere.

---

## 2. Pratica di riferimento — numero e data

### ATTENZIONE ! Inserire il numero pratica di riferimento.

**Dove si trova**: Sezione **"Di presentare"** → campo **"relativi alla pratica n."**

**Causa**: Non hai indicato il numero della pratica edilizia a cui si riferisce il collaudo o la DRE.

**Soluzione**: Inserisci il numero della pratica originaria nel campo **"relativi alla pratica n."** (max 20 caratteri). Si tratta del numero assegnato dal SUE alla pratica dei lavori strutturali oggetto del collaudo.

---

### ATTENZIONE ! Inserire la data della pratica di riferimento.

**Dove si trova**: Sezione **"Di presentare"** → campo **"del"** (data)

**Causa**: Non hai inserito la data della pratica di riferimento.

**Soluzione**: Inserisci la data della pratica nel campo **"del"** nel formato **GG/MM/AAAA** (es. `15/03/2024`). Puoi usare l'icona calendario o digitare direttamente.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data della pratica di riferimento è in un formato non riconosciuto dal sistema.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA**. Esempi corretti: `15/03/2024` ✅. Errati: `15-03-2024` ❌, `15/03/24` ❌.

---

## 3. Localizzazione dell'intervento

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

## 4. Coordinate geografiche UTM

Questa sezione è **esclusiva della Lombardia** e richiede le coordinate piane dell'intervento nel sistema **UTM - WGS 84 32N**, espresse in metri. Il sistema valida sia la presenza sia il range numerico di ciascuna coordinata.

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
3. Se non disponi delle coordinate, usa il pulsante **"Calcola Coordinate"** (se visibile) oppure consulta il geoportale regionale o un GIS per ricavarle dall'indirizzo dell'intervento

{: .note }
> Le coordinate UTM-WGS84 32N per la Lombardia hanno tipicamente coordinata X intorno a 450.000–570.000 e coordinata Y intorno a 4.950.000–5.200.000. Se il valore che ottieni è molto diverso, probabilmente stai usando un sistema di riferimento diverso (es. Gauss-Boaga o gradi decimali). Il campo accetta valori decimali con il punto come separatore (es. `514823.5`).

---

### ATTENZIONE ! Inserire coordinata Y della località di intervento.

**Dove si trova**: Sezione **"Localizzazione dell'intervento"** → campo **"Coord. asse Y"**

**Causa**: Il campo della coordinata Y è vuoto.

**Soluzione**: Inserisci la coordinata Y (nord) nel campo **"Coord. asse Y"**. Il valore deve essere un numero compreso tra **4.800.000 e 5.700.000** metri.

---

### ATTENZIONE ! La coordinata Y deve essere compresa tra 4800000 e 5700000.

**Causa**: Il valore inserito per la coordinata Y non è un numero valido oppure è fuori dal range accettato per il territorio lombardo nel sistema UTM-WGS84 32N.

**Soluzione**:
1. Verifica che il valore sia un **numero** (es. `5034512` oppure `5034512.3`) — nessun punto migliaia, nessun simbolo
2. Il valore deve essere **≥ 4.800.000** e **≤ 5.700.000**
3. Se non disponi delle coordinate, consulta il geoportale regionale o un GIS per ricavarle dall'indirizzo dell'intervento

{: .warning }
> **Errore frequente**: inserire le coordinate in gradi decimali (es. `45.4654` per la latitudine) invece che in metri UTM. Un valore come `45` o `9.18` è in gradi e causerà sempre questo errore perché è fuori range. Occorre convertire le coordinate nel sistema UTM-WGS84 32N prima di inserirle.

---

## 5. Sisma Bonus

### ATTENZIONE ! Selezionare almeno una voce relativa al 'Sisma Bonus'.

**Dove si trova**: Sezione **"Dichiarazioni"** → checkbox **"che la pratica è finalizzata a beneficiare delle detrazioni Sisma Bonus"** e sottovoci

**Causa**: Hai spuntato la checkbox principale del Sisma Bonus ma non hai selezionato nessuna delle due dichiarazioni obbligatorie che la seguono.

**Soluzione**: Se hai spuntato **"che la pratica è finalizzata a beneficiare delle detrazioni Sisma Bonus"**, devi obbligatoriamente selezionare almeno una delle due sottovoci che si attivano:
- ☑ **"la dichiarazione del direttore dei lavori... è già stata prodotta all'atto della comunicazione di fine lavori strutturali"** (art. 3, c. 4, DM 28/02/2017 n. 58)
- ☑ **"si allega alla presente dichiarazione del collaudatore statico... la conformità degli interventi eseguiti al progetto depositato"** (art. 3, c. 4, DM 28/02/2017 n. 58)

{: .note }
> Le due sottovoci del Sisma Bonus sono abilitate solo dopo aver spuntato la checkbox principale. Se non intendi beneficiare delle detrazioni Sisma Bonus, lascia la checkbox principale non spuntata: in questo caso le due dichiarazioni non sono richieste e la sezione non genera errori.

---

## 6. Privacy

### ATTENZIONE ! Non è stata spuntata la voce relativa a 'Rispetto normativa sulla privacy'.

**Dove si trova**: Sezione **"Rispetto della normativa sulla privacy"**

**Causa**: Non hai spuntato la checkbox di accettazione dell'informativa privacy.

**Soluzione**: Leggi l'informativa sulla privacy riportata in fondo al modulo (Art. 13 del D.Lgs. n. 196/2003), quindi spunta la checkbox:
- ☑ **"di aver letto l'informativa sul trattamento dei dati personali pubblicata sul portale istituzionale del Comune"**

{: .warning }
> **Differenza rispetto alla C.I.L. nazionale**: in questa pratica la checkbox privacy è **obbligatoria** per completare la validazione. Nella C.I.L. nazionale la sezione privacy è solo informativa e non genera errori di validazione. Non è possibile procedere con "Valida e Salva" senza aver spuntato questa voce.

---

## Consigli pratici Collaudo/DRE Lombardia

### Prima di validare ✅

- [ ] Seleziona il **tipo di documento** (collaudo statico o DRE)
- [ ] Compila la **descrizione dei lavori** nel campo "per i lavori di"
- [ ] Inserisci il **numero della pratica** di riferimento
- [ ] Inserisci la **data della pratica** di riferimento nel formato GG/MM/AAAA
- [ ] Seleziona l'**indirizzo** della località (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno) e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **coordinata X** (numero tra 430.000 e 700.000, sistema UTM-WGS84 32N)
- [ ] Inserisci la **coordinata Y** (numero tra 4.800.000 e 5.700.000, sistema UTM-WGS84 32N)
- [ ] Se richiesto, spunta il **Sisma Bonus** e seleziona almeno una delle due dichiarazioni subordinate
- [ ] Spunta la **checkbox privacy**
- [ ] **Salva** frequentemente

### Coordinate UTM-WGS84 32N: come ottenerle ⚠️

| Metodo | Come fare |
|---|---|
| Pulsante **"Calcola Coordinate"** | Se visibile nel modulo, clicca per importarle automaticamente dalla cartografia |
| **Geoportale Regione Lombardia** | Cerca l'indirizzo su [geoportale.regione.lombardia.it](https://geoportale.regione.lombardia.it) e leggi le coordinate UTM |
| **Google Maps + conversione** | Ottieni lat/lon da Google Maps, poi converti in UTM-WGS84 32N con un tool online |
| **GIS (QGIS, ArcGIS)** | Individua il punto e leggi le coordinate nel sistema EPSG:32632 |

### Errori frequenti Collaudo/DRE Lombardia 🔍

1. **Tipo di presentazione non selezionato** → è il primo controllo; blocca tutto il resto
2. **Data pratica formato errato** → usare sempre GG/MM/AAAA con barre, non trattini
3. **Coordinate in gradi decimali** → errore molto comune; i valori devono essere in metri UTM, non in gradi (es. `515000` non `9.18`)
4. **Coordinata fuori range** → verificare di usare il fuso 32N (EPSG:32632); il fuso 33N darebbe valori X troppo bassi
5. **Sisma Bonus spuntato senza sottovoce** → se si attiva la checkbox principale, almeno una delle due dichiarazioni subordinate è obbligatoria
6. **Privacy non spuntata** → a differenza di altre pratiche, qui è obbligatoria per validare

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
**Fonte**: Analisi codice `ValidaDatiCCLombardia` e `DatiCCLombardia.ascx`
