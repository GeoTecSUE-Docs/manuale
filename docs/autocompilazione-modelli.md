---
title: Autocompilazione modelli
nav_order: 20
parent: Gestione anagrafiche e strumenti
description: Come generare automaticamente modelli precompilati (procure, deleghe, dichiarazioni) usando l'anagrafica o i dati delle pratiche
keywords: [autocompilazione, modelli, procura, delega, dichiarazioni, PDF, precompilazione, template, documenti]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Autocompilazione modelli

Questa sezione spiega come generare automaticamente **documenti precompilati** (procure, deleghe, dichiarazioni) usando i dati della tua [anagrafica](gestione-anagrafiche.html) o delle pratiche in compilazione.

## Cos'è l'autocompilazione modelli

L'**autocompilazione modelli** è una funzionalità che genera documenti amministrativi standard con i dati già compilati, evitandoti di scrivere manualmente ogni volta gli stessi documenti.

### Vantaggi

✅ **Risparmio di tempo**: Genera documenti in pochi secondi invece di compilarli manualmente  
✅ **Riduzione errori**: Dati prelevati automaticamente da fonti affidabili (anagrafica o pratica)  
✅ **Formattazione corretta**: Template standard conformi alle normative  
✅ **Modificabilità**: Puoi personalizzare i dati prima di generare il PDF finale  
✅ **Riutilizzabilità**: Genera lo stesso tipo di documento quante volte vuoi  

### Modelli disponibili

I modelli variano in base all'Ente, ma tipicamente includono:

- **Modello di delega alla presentazione della pratica**
- **Soggetti coinvolti**

{: .note }
> L'elenco dei modelli disponibili dipende dalla configurazione dell'Ente. Alcuni Enti potrebbero avere modelli aggiuntivi specifici.

---

## Accedere all'autocompilazione

### Procedura

1. Dal **menu principale**, clicca su **"Le mie istanze"**
2. Nel sottomenu, seleziona **"Autocompilazione modelli"**
3. Si apre la pagina di selezione del modello

---

## Generare un modello

La procedura completa si articola in 4 passaggi.

## Passo 1: Selezionare il modello

Nella pagina di autocompilazione, vedi l'elenco dei **modelli disponibili**.

**Procedura**:
1. Apri il menu a discesa **"Seleziona il modello"**
2. Scegli il modello che ti serve (es. "Modello di delega alla presentazione della pratica")
3. Clicca **"Conferma"** o prosegui al passo successivo

**Descrizione modello**: Quando selezioni un modello, appare una breve descrizione che spiega:
- A cosa serve il documento
- Quali dati sono necessari
- Come verrà utilizzato

---

## Passo 2: Scegliere la fonte dei dati

Dopo aver selezionato il modello, devi indicare da dove prelevare i dati per compilarlo.

Hai **due opzioni**:

### Opzione A: Da Anagrafica

**Quando usarla**: Vuoi generare un documento generico non collegato a una pratica specifica.

**Procedura**:
1. Seleziona **"Da Anagrafica"**
2. Apri il menu a discesa **"Seleziona richiedente"**
3. Scegli il soggetto dall'[anagrafica richiedenti](gestione-anagrafiche.html#1-anagrafica-richiedenti)
4. Clicca **"Carica dati"**

**Dati prelevati**:
- Dati anagrafici completi del richiedente
- Residenza
- Codice fiscale
- Contatti

**Esempio d'uso**:
Vuoi generare una **procura generica** per il Sig. Rossi che ti autorizza a presentare pratiche per suo conto, ma non hai ancora una pratica specifica aperta.

### Opzione B: Da Pratica in compilazione

**Quando usarla**: Vuoi generare un documento specifico collegato a una pratica che stai compilando.

**Procedura**:
1. Seleziona **"Da Pratica"**
2. Apri il menu a discesa **"Seleziona pratica"**
3. Vedi l'elenco delle tue pratiche **in compilazione**
4. Scegli la pratica di interesse
5. Clicca **"Carica dati"**

**Dati prelevati**:
- Dati del titolare della pratica
- Dati della ditta/società (se presente)
- Tipo di pratica

{: .note }
> Se selezioni "Da Pratica", il menu mostra solo le pratiche in stato **"In Compilazione"**. Le pratiche già inviate non appaiono.

---

## Passo 3: Verificare e modificare i dati

Dopo aver caricato i dati (da anagrafica o da pratica), il sistema mostra un **form precompilato**.

### Form precompilato

Il form contiene:
- **Dati fissi** 
- **Campi modificabili** prelevati dalla fonte (anagrafica/pratica) che puoi personalizzare
- **Campi aggiuntivi** specifici del modello da compilare

### Modificare i dati

**Perché modificare**:
- Correggere dati non aggiornati
- Aggiungere informazioni specifiche
- Personalizzare il documento per il caso specifico

**Procedura**:
1. Scorri il form
2. Modifica i campi necessari
3. Compila i campi vuoti richiesti
4. Clicca **"Salva i dati"**

{: .warning }
> Le modifiche che fai nel form dell'autocompilazione **non** aggiornano l'anagrafica o la pratica originale. Valgono solo per il documento che stai generando.

### Validazione

Quando clicchi **"Salva i dati"**, il sistema non effettua alcun tipo di verifica e appare il pulsante **arancione "Genera PDF"**

---

## Passo 4: Generare il PDF

Dopo aver salvato i dati con successo, puoi generare il documento finale.

### Procedura

1. Clicca il pulsante **arancione "Genera PDF"**
2. Il sistema crea il documento
3. Il PDF viene **scaricato automaticamente** sul tuo computer (o visualizzato nel browser)

### Cosa contiene il PDF

Il PDF generato include:
- **Tutti i dati** inseriti nel form
- **Formattazione standard** conforme alle normative
- **Campi firma** predisposti (se applicabile)
- **Logo e intestazione** dell'Ente (se previsto dal template)

---

## Usare il documento generato

### Firma olografa

Se il documento richiede la **firma del delegante** (es. procura, delega):

**Procedura**:
1. **Stampa** il PDF generato
2. Fallo **firmare** al titolare/richiedente
3. **Scannerizza** il documento firmato
4. Carica il PDF firmato come allegato alla pratica

{: .note }
> La firma olografa (firma a penna) è valida per documenti come deleghe e procure dove il soggetto che appone firma non è detto che sia in possesso di una *firma digitale*.

### Firma digitale

Per alcuni modelli potrebbe essere richiesta la **firma digitale**.

**Procedura**:
1. Salva il PDF generato
2. Firma il PDF con dispositivo di firma digitale
3. Ottieni il file **.p7m**
4. Carica il .p7m come allegato alla pratica

### Allegare alla pratica

**Dove caricare**:
- Nella sezione **"Quadro riepilogativo della documentazione"** della pratica
- Solitamente nella voce "Procura/Delega" o "Documenti liberi"

**Procedura**:
1. Vai alla [compilazione della pratica](compilare-istanza.html#quadro-riepilogativo-della-documentazione)
2. Trova il documento richiesto (es. "Procura") o usa "Documenti liberi"
3. Carica il PDF (firmato se richiesto)
4. Prosegui con la compilazione

---

## Esempi pratici

### Esempio 1: Delega per pratica specifica

**Scenario**: Stai compilando un Permesso di Costruire per il Sig. Verdi. Ti serve la delega firmata.

**Procedura**:
1. Menu → Le mie istanze → Autocompilazione modelli
2. Seleziona "Modello di delega alla presentazione della pratica"
3. Scegli **"Da Pratica"**
4. Seleziona la pratica del Permesso di Costruire (in compilazione)
5. Il sistema precompila: Nome Verdi, indirizzo intervento, tipo pratica
6. Aggiungi la data odierna
7. Salva i dati → Genera PDF
8. Stampa, fai firmare al Sig. Verdi, scannerizza
9. Carica nella pratica come allegato "Procura/Delega"

### Esempio 2: Procura generica da anagrafica

**Scenario**: Il Sig. Rossi ti dà una procura generale per presentare qualsiasi pratica per suo conto.

**Procedura**:
1. Menu → Le mie istanze → Autocompilazione modelli
2. Seleziona "Procura generale"
3. Scegli **"Da Anagrafica"**
4. Seleziona "Rossi Mario" dall'anagrafica richiedenti
5. Il sistema precompila i dati anagrafici di Rossi
6. Compila: Data, eventuali limitazioni della procura
7. Salva i dati → Genera PDF
8. Stampa, fai firmare, scannerizza
9. **Conserva** il documento per usarlo in future pratiche di Rossi

---

## Rigenerare un modello

Se hai bisogno di rigenerare lo stesso tipo di documento (es. perché hai sbagliato qualcosa):

**Procedura**:
1. Torna su Menu → Autocompilazione modelli
2. Seleziona di nuovo lo stesso modello
3. Ricarica i dati (da anagrafica o pratica)
4. Modifica i dati corretti
5. Salva → Genera PDF

{: .note }
> Non c'è limite al numero di volte che puoi generare un modello. Ogni generazione crea un nuovo PDF indipendente.

---

## Differenze tra autocompilazione e compilazione manuale

| Aspetto | Autocompilazione modelli | Compilazione manuale |
|---------|-------------------------|---------------------|
| **Tempo** | Pochi secondi | Diversi minuti |
| **Errori** | Ridotti (dati da fonte affidabile) | Possibili errori di battitura |
| **Formattazione** | Standard e corretta | Varia in base al template usato |
| **Personalizzazione** | Possibile prima di generare PDF | Totale |
| **Conformità** | Garantita dal template dell'Ente | Da verificare manualmente |

---

## Consigli pratici

### Popola l'anagrafica prima

Per sfruttare al massimo l'autocompilazione:

✅ **Carica i richiedenti** ricorrenti nell'[anagrafica](gestione-anagrafiche.html)  
✅ **Mantieni aggiornati** i dati anagrafici  
✅ **Verifica sempre** i dati precompilati prima di generare il PDF  

### Verifica prima di stampare

Prima di stampare per la firma:

✅ **Controlla tutti i dati** siano corretti  
✅ **Verifica le date** (non devono essere future se non ha senso)  
✅ **Controlla l'indirizzo** dell'intervento (se applicabile)  
✅ **Leggi il testo completo** del modello generato  

### Usa "Da Pratica" quando possibile

Se hai già la pratica in compilazione:

✅ Usa **"Da Pratica"** invece di "Da Anagrafica"  
✅ **Più dati** vengono precompilati automaticamente  
✅ **Coerenza** garantita tra documento e pratica  
✅ **Meno errori** di trascrizione  

---

## Domande frequenti

### Posso modificare il template del modello?

**No**, i template sono predefiniti e non modificabili direttamente.

Puoi:
- ✅ Modificare i **dati** nel form prima di generare il PDF
- ❌ Modificare la **struttura** o il **testo fisso** del template

### Posso generare modelli per pratiche già inviate?

**No**, l'autocompilazione funziona solo con pratiche **in compilazione**.

### I dati vengono salvati dopo la generazione del PDF?

**No**, i dati inseriti nel form servono solo per generare il PDF specifico. Non vengono salvati permanentemente.

Se generi di nuovo lo stesso modello, dovrai ricompilare o ricaricare i dati.

### Posso generare più copie dello stesso documento?

**Sì**, puoi rigenerare lo stesso modello quante volte vuoi. Ogni volta genera un nuovo PDF identico (se usi gli stessi dati).

### Il PDF generato è modificabile?

**No**, il PDF generato è un documento statico. Non puoi modificarlo dopo la generazione.

Se serve una modifica:
1. Torna all'autocompilazione
2. Rigenera il modello con i dati corretti

### Devo allegare il modello generato a una pratica?

**Dipende dal tipo di documento**:

- **Procura/Delega**: Sì, obbligatoria come allegato alla pratica

### Posso generare modelli per altri professionisti?

**Si**, l'autocompilazione usa i **tuoi dati** come professionista delegato ma puoi modificarli. Non è consigliato, ma puoi farlo.

---

## Prossimi passi

- [Gestione anagrafiche](gestione-anagrafiche.html) per popolare i dati da usare nell'autocompilazione
- [Compilare un'istanza](compilare-istanza.html) per usare i documenti generati
- [Visualizzare il dettaglio di una pratica](dettaglio-istanza.html)

---

**Hai bisogno di aiuto?** Contatta l'assistenza tecnica per supporto sull'autocompilazione dei modelli.
