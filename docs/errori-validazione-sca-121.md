---
title: Errori Segnalazione Certificata di Agibilità - Regione Liguria
parent: Errori di validazione
nav_order: 47
description: Errori di validazione specifici per la Segnalazione Certificata di Agibilità - Regione Liguria (art. 24 D.P.R. 380/2001)
keywords: [segnalazione certificata agibilità, SCA, agibilità, Liguria, art. 24 DPR 380/2001, titolo edilizio, fine lavori, tecnico agibilità, TA, direttore lavori, SCIA agibilità]
IDRegione: 3
IDTipoPratica: 121
Fonte: Manuale
---

# Errori di validazione - Segnalazione Certificata di Agibilità
## Regione Liguria

Guida completa agli errori specifici per la **Segnalazione Certificata di Agibilità (SCA)** ai sensi dell'art. 24 del D.P.R. 380/2001 — Regione Liguria. La pratica permette di presentare sia la SCIA per agibilità totale o parziale sia la SCIA Unica (con altre segnalazioni allegate).

{: .note }
> La SCA Liguria ha alcune caratteristiche distintive. La sezione del **titolo edilizio** ha un doppio binario: titolo esterno a GeoTecSUE (menu + n. + data) oppure titolo già presente su GeoTecSUE (menu tipo + menu riferimento pratica); almeno uno dei due deve essere compilato. Il sistema valida solo il primo gruppo (titolo esterno) per n. e data; il secondo richiede solo la selezione del riferimento pratica. La **comunicazione di fine lavori** è condizionale: genera errori solo se la checkbox è spuntata. Per i tecnici, è richiesto obbligatoriamente almeno uno con ruolo **TA (Tecnico Agibilità) o DR (Direttore Lavori)**. Non sono richieste coordinate geografiche. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Titolo edilizio di riferimento](#2-titolo-edilizio-di-riferimento)
3. [Comunicazione di fine lavori](#3-comunicazione-di-fine-lavori)
4. [Presentazione agibilità](#4-presentazione-agibilità)
5. [Privacy](#5-privacy)
6. [Tecnici nei soggetti coinvolti](#6-tecnici-nei-soggetti-coinvolti)

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
> A differenza di molte pratiche lombarde, la SCA Liguria **non richiede le coordinate geografiche**. Il campo `txtCoordinate` (campo testo libero "Coordinate") è presente nel modulo ma non viene validato: non genera errori se vuoto.

---

## 2. Titolo edilizio di riferimento

La sezione del titolo edilizio ha una struttura a **doppio binario** che gestisce due casi distinti: il titolo che ha legittimato l'intervento può essere esterno a GeoTecSUE (immesso manualmente) oppure già presente come pratica in GeoTecSUE. Il validatore richiede che **almeno uno dei due** sia compilato.

---

### ATTENZIONE ! Selezionare il titolo abitativo edilizio.

**Dove si trova**: Sezione dichiarazioni → prima riga del titolo → menu a discesa `cmbTitoliAbitEdilizi` (titolo esterno) **e** menu `cmbTitoliAbitEdilizi1` (titolo su GeoTecSUE) — entrambi sull'opzione vuota iniziale

**Causa**: Entrambi i menu del titolo edilizio sono rimasti sull'opzione vuota: né il titolo esterno né quello interno a GeoTecSUE sono stati selezionati.

**Soluzione**: Compila **almeno uno** dei due percorsi:

**Percorso 1 — Titolo esterno (non presente su GeoTecSUE):**
Seleziona il tipo di titolo dal primo menu (`cmbTitoliAbitEdilizi`), poi compila il numero e la data nel formato GG/MM/AAAA.

**Percorso 2 — Titolo su GeoTecSUE:**
Seleziona il tipo dal menu `cmbTitoliAbitEdilizi1`, poi seleziona la pratica specifica dal menu `cmbTitoloRif1` che si attiva.

{: .note }
> I due percorsi non sono mutuamente esclusivi: è possibile compilarli entrambi. La validazione richiede però che almeno uno sia compilato. Se si usa il percorso GeoTecSUE, la pratica viene collegata direttamente e i campi n./data vengono popolati automaticamente dal sistema.

---

### ATTENZIONE ! Selezionare il riferimento della pratica.

**Causa**: Hai selezionato un tipo di titolo nel menu `cmbTitoliAbitEdilizi1` (percorso GeoTecSUE) ma non hai selezionato la pratica specifica dal menu `cmbTitoloRif1` che si è abilitato.

**Soluzione**: Seleziona la pratica corrispondente dal menu a discesa `cmbTitoloRif1` ("selezionare il riferimento della pratica"). Il menu mostra le pratiche del tipo selezionato presenti nel sistema GeoTecSUE per questo ente.

---

### ATTENZIONE ! Inserire il numero.

**Causa**: Hai selezionato un tipo di titolo nel primo menu (`cmbTitoliAbitEdilizi`, percorso esterno) ma non hai compilato il campo "prot. / n."

**Soluzione**: Inserisci il numero di protocollo o il numero del titolo edilizio nel campo "prot. / n." accanto al menu.

---

### ATTENZIONE ! Inserire la data.

**Causa**: Hai selezionato un tipo di titolo nel percorso esterno e il campo data è vuoto.

**Soluzione**: Inserisci la data del titolo edilizio nel campo "del" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (titolo edilizio)

**Causa**: La data inserita per il titolo edilizio esterno non rispetta il formato richiesto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/03/2022`).

{: .note }
> Il modulo prevede anche slot aggiuntivi per "altri titoli su GeoTecSUE" (fino a 5 righe aggiuntive con menu cmbTitoliAbitEdilizi2..5 e relativi riferimenti e campi n./data). Questi campi aggiuntivi **non vengono validati** dal codice VB: non generano errori se vuoti o parzialmente compilati. Sono opzionali e servono a collegare più pratiche collegate allo stesso immobile.

---

## 3. Comunicazione di fine lavori

### ATTENZIONE ! Inserire il prot. / n. di pratica.

**Dove si trova**: Sezione dichiarazioni → checkbox `chkComunicazFLa_1` "che la comunicazione di fine lavori è stata già presentata prot. / n. ___ del ___"

**Causa**: Hai spuntato la checkbox della comunicazione di fine lavori ma non hai inserito il numero di protocollo/pratica nel campo affiancato.

**Soluzione**: Inserisci il numero di protocollo o pratica della comunicazione di fine lavori già presentata nel campo "prot. / n."

---

### ATTENZIONE ! Campo obbligatorio 'Data pratica' non inserito.

**Causa**: Hai spuntato la checkbox e inserito il numero, ma il campo data è vuoto.

**Soluzione**: Inserisci la data della comunicazione di fine lavori nel campo "del" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (fine lavori)

**Causa**: La data inserita per la comunicazione di fine lavori non rispetta il formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

{: .note }
> La checkbox `chkComunicazFLa_1` è **opzionale** — se non viene spuntata, nessun campo della sezione viene validato. Si spunta solo se la comunicazione di fine lavori è stata già presentata. Se i lavori non sono ancora terminati o la fine lavori non è stata presentata, si lascia la checkbox non spuntata.

---

## 4. Presentazione agibilità

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Presentazione agibilità'.

**Dove si trova**: Sezione "PRESENTA" → 6 radio button divisi in due gruppi (SCIA e SCIA Unica)

**Causa**: Non hai indicato il tipo di agibilità richiesta.

**Soluzione**: Seleziona **uno dei sei radio button**:

**SCIA per:**
- ⚪ **rdbPresenta1** — "l'agibilità relativa all'immobile oggetto dell'intervento edilizio" (agibilità totale)
- ⚪ **rdbPresenta2** — "l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione (art. 24, comma 4, lett. a) del d.P.R. n. 380/2001)"
- ⚪ **rdbPresenta3** — "l'agibilità parziale relativa a singole unità immobiliari (art. 24, comma 4, lett. b) del d.P.R. n. 380/2001)"

**SCIA Unica per:**
- ⚪ **rdbPresenta4** — "l'agibilità relativa all'immobile oggetto dell'intervento edilizio" (agibilità totale con allegati)
- ⚪ **rdbPresenta5** — "l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione (art. 24, comma 4, lett. a)..."
- ⚪ **rdbPresenta6** — "l'agibilità parziale relativa a singole unità immobiliari (art. 24, comma 4, lett. b)..."

{: .note }
> La distinzione tra SCIA e SCIA Unica riguarda la presenza di ulteriori segnalazioni allegate (Sezione C/D dei soggetti coinvolti e Quadro Riepilogativo). Se si sceglie SCIA Unica (rdbPresenta4..6), il sistema si aspetta che vengano allegate le altre comunicazioni necessarie indicate nel quadro riepilogativo.

---

## 5. Privacy

### ATTENZIONE ! Selezionare la presa visione dell'informativa sul trattamento dei dati personali.

**Dove si trova**: Sezione "Informativa sulla privacy" → checkbox `chkPrivacy` in fondo alla pagina, incorporata nel testo dell'informativa

**Causa**: Non hai spuntato la dichiarazione di aver letto l'informativa sul trattamento dei dati personali.

**Soluzione**: Scorri fino alla sezione "Informativa sulla privacy (Art. 13 del d.lgs. n. 196/2003)" e spunta la checkbox `chkPrivacy` — "Il/la sottoscritto/a dichiara di aver letto l'informativa sul trattamento dei dati personali pubblicata sul sito istituzionale del SUAP/SUE".

{: .note }
> Il messaggio di errore della SCA Liguria è diverso da quello delle altre pratiche ("Selezionare la presa visione..." invece del consueto "Non è stata spuntata la voce relativa a..."). L'informativa citata fa riferimento al **Reg. UE n. 2016/679 del 27 aprile 2016** (GDPR), più aggiornata rispetto ad altre pratiche che citano ancora il D.Lgs. 196/2003.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Professionista incaricato per Agibilità o come Direttore Lavori.

**Causa**: Nessun tecnico con ruolo **TA** (Professionista Incaricato Agibilità) o **DR** (Direttore Lavori) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico con uno dei due ruoli:
- **TA — Professionista Incaricato Agibilità**: il tecnico abilitato che attesta la conformità dell'immobile ai requisiti di agibilità
- **DR — Direttore Lavori**: il direttore dei lavori delle opere architettoniche

{: .note }
> Il controllo TA/DR è specifico della SCA Liguria — è sufficiente uno dei due ruoli. Non è richiesto che siano due soggetti distinti: lo stesso tecnico può avere entrambi i ruoli, ma in quel caso deve comparire due volte nei soggetti (una con ruolo TA e una con ruolo DR) oppure il sistema potrebbe già associare entrambi i ruoli allo stesso soggetto. Verificare con l'interfaccia dei soggetti coinvolti come è stato configurato nell'ente.

---

## Consigli pratici — SCA Liguria

### Prima di validare ✅

- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Compila il **titolo edilizio**: percorso esterno (menu + n. + data GG/MM/AAAA) **oppure** percorso GeoTecSUE (menu tipo + menu riferimento pratica), o entrambi
- [ ] Se la **fine lavori è già stata presentata**: spunta la checkbox e compila n. protocollo + data (GG/MM/AAAA)
- [ ] Seleziona uno dei 6 **radio button agibilità** (SCIA o SCIA Unica, totale o parziale)
- [ ] Spunta **chkPrivacy**
- [ ] Aggiungi nei soggetti almeno un tecnico con ruolo **TA** o **DR**

### Campi presenti ma non validati ℹ️

- **`txtCoordinate`** (campo testo libero "Coordinate"): presente ma non validato — nessun errore se vuoto
- **Titoli aggiuntivi GeoTecSUE** (cmbTitoliAbitEdilizi2..5 con relativi riferimenti, n. e data): fino a 5 titoli aggiuntivi collegabili; nessuno è validato
- **`txtNTitEdilizio1`, `txtDataTitEdilizio1`** (n. e data del percorso GeoTecSUE): compilati automaticamente dal sistema, non validati direttamente
- **`chkSezB`** (Sezione B — Attestazione direttore lavori): checkbox informativa non validata
- **`chkSezCD`** (Sezione C/D — comunicazioni soggetti coinvolti): checkbox informativa non validata
- **`txtData` e `txtLuogo`** (data e luogo firma): campi facoltativi non validati

### Doppio binario titolo edilizio — schema rapido ⚠️

Il validatore controlla: se `cmbTitoliAbitEdilizi.SelectedIndex = 0` **AND** `cmbTitoliAbitEdilizi1.SelectedIndex = 0` → errore "Selezionare il titolo abitativo edilizio". Se il primo menu è selezionato (`> 0`): verifica n. e data (obbligatori, data con formato). Se il secondo menu è selezionato (`> 0`): verifica `cmbTitoloRif1` (riferimento pratica) obbligatorio. I due percorsi sono indipendenti e cumulabili.

### Errori frequenti 🔍

1. **Entrambi i menu titolo su opzione vuota** → bisogna usare almeno un percorso; spesso si confonde tra i due e si lascia tutto vuoto
2. **Percorso GeoTecSUE selezionato senza riferimento pratica** → dopo aver selezionato il tipo titolo nel secondo menu, aspettare che si carichi il menu `cmbTitoloRif1` e selezionare la pratica
3. **Fine lavori spuntata ma campi vuoti** → se si spunta `chkComunicazFLa_1`, n. e data diventano obbligatori; se la fine lavori non è ancora presentata, non spuntare la checkbox
4. **Nessun tecnico TA o DR** → a differenza di altre pratiche che accettano qualsiasi tecnico, la SCA Liguria richiede specificamente TA o DR; verificare il ruolo assegnato al tecnico nei soggetti coinvolti
5. **Privacy non spuntata** → la checkbox `chkPrivacy` è incorporata all'interno del lungo testo dell'informativa GDPR; può essere facile non vederla; si trova alla fine del testo dell'informativa

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
**Fonte**: Analisi codice ValidaDatiSCALiguria e DatiSCALiguria.ascx
