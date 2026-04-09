---
title: Inviare un'istanza
nav_order: 22
parent: Le mie istanze
description: Guida completa alla compilazione di pratiche edilizie su GeoTecSUE - inserimento dati, soggetti, localizzazione, allegati, pagamenti e invio
keywords: [inviare istanza, trasmettere istanza, validazione completata, firmata, invio]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Inviare un'istanza

Questa sezione spiega come trasmettere un'istanza edilizia su **GeoTecSUE** verso l'Ente di riferimento.

## Quando usi questa guida

Puoi trasmettere un'istanza all'Ente quando:
- [Hai completato una nuova istanza](compilare-istanza.html)
- [Hai completato una pratica duplicata](nuova-istanza.html#metodo-2-duplicare-una-pratica-esistente)
- Hai completato una comunicazione all'interno del [dettaglio di una pratica](dettaglio-istanza.html#comunicazioni-verso-lente)
- [Hai completato una pratica di Notifica Preliminare](notifica-preliminare.html) (solo per la Regione Piemonte)

## Dove ti puoi trovare per poter inviare un'istanza

La trasmissione dell'istanza verso l'Ente può essere effettuata solo da due punti:
- Sei nella sezione **Le mie istanze** - **Elenco Istanze** nel serbatoio *Lista Pratiche in fase di compilazione* (caso invio Pratica)
- Sei all'interno del **dettaglio** di una pratica:
  - nel serbatoio *Lista comunicazioni in fase di compilazione* (caso invio Comunicazione)
  - nella sezione *Richiesta integrazioni attiva* (caso Richiesta Integrazioni)
  - nella sezione *Invio documentazione all'Ente (integrazioni spontanee)* (caso Invio libero di documentazione, se previsto dall'Ente)

## Invio Pratica

Se la pratica in fase di compilazione ha correttamente superato la fase di **validazione** (vedere la sezione apposita [Valida e salva](compilare-istanza.html#valida-e-salva-pulsante-verde-con-dischetto-e-spunta)) si trova in stato **Completata**.

### Procedura di invio

**1. Generazione del PDF**

Clicca sul bottone **Genera** presente nella colonna **PDF** del serbatoio *Lista Pratiche in fase di compilazione*.
Il sistema procederà alla generazione del PDF e, al termine del processo, il file sarà disponibile per il download. A questo punto, l'icona nella colonna **PDF** diventerà cliccabile per scaricare il documento.

**2. Download del PDF**

Prima di scaricare il file:
- **Pulisci la cartella Download** del tuo computer per evitare file duplicati
- Clicca sull'icona **PDF** per scaricare il file generato
- Il file avrà un nome simile a: `DOCUMENTOISTANZA_999999_c67723cf-b83a-4174-ba06-d092c255c9ad.pdf`

**3. Firma digitale CAdES**

Nella maggior parte dei casi, l'Ente richiede che il PDF venga firmato digitalmente in modalità **CAdES**:

- **IMPORTANTE**: NON spostare né rinominare il file appena scaricato
- Firma il file direttamente dalla cartella Download usando il tuo software di firma digitale
- Al termine della firma, il file avrà estensione `.pdf.p7m` (esempio: `DOCUMENTOISTANZA_999999_c67723cf-b83a-4174-ba06-d092c255c9ad.pdf.p7m`)
- **Attenzione**: alcuni software di firma creano file con estensione solo `.p7m` invece di `.pdf.p7m` - verifica che l'estensione sia `.pdf.p7m`

**4. Caricamento del file firmato**

- Clicca sul bottone di sfoglia nella colonna **P7M**
- Seleziona il file firmato (con estensione `.pdf.p7m`)
- Clicca sul bottone di *upload*
- Se i passaggi precedenti sono stati completati correttamente, in questa fase la pratica passerà allo stato **Firmata**

**5. Invio della pratica**

Se il sistema non rileva incongruenze tra il file PDF generato e quello firmato digitalmente, il bottone **Invia** (di colore verde) sarà disponibile nell'ultima colonna.

Cliccando il bottone **Invia**, la pratica *cambia di stato* (vedi [ciclo di vita](nozioni-di-base.html#stati-di-lavorazione-dellente)), passando allo stato **Inviata** e verrà inserita nel serbatoio *Lista Pratiche inviate*.

## Invio Comunicazione

L'invio della comunicazione ricalca quanto visto nella sezione dell'[invio pratica](#invio-pratica).
Una volta trasmessa la comunicazione, questa comparirà nella sezione *Comunicazioni Inviate collegate alla Pratica*.

## Richiesta Integrazioni

All'interno del dettaglio della pratica, se l'Ente ha fatto una *richiesta di integrazioni*, è possibile caricare e trasmettere i documenti verso l'Ente.

A differenza della trasmissione di una pratica o di una comunicazione, in questo caso **non è necessario** generare il PDF e firmarlo, ma è sufficiente procedere con il caricamento degli allegati.

Una volta caricati tutti i documenti richiesti, è possibile cliccare il bottone **Invio Documenti Integrativi**.

Quando i documenti vengono trasmessi, la pratica *cambia di stato*, passando allo stato **Invio Integrazioni** in attesa che l'Ente proceda con la registrazione delle stesse.

Una volta trasmesse le integrazioni, queste vengono registrate nella sezione *Dati Ente* in *Storico richieste integrazioni*.

Nel caso in cui l'Ente lo consenta, è possibile anche caricare più file di quanti richiesti.

## Invio libero di documentazione

Nel dettaglio della pratica, se l'Ente lo consente, è possibile trasmettere delle *integrazioni spontanee* dalla sezione **Invio documentazione all'Ente (integrazioni spontanee)**.

Cliccando il bottone **Nuovo Invio** il sistema consentirà il caricamento di uno (o più) file che soddisfino i requisiti di dimensione e di (eventuale) firma.

Caricato il documento (o i documenti) è possibile cliccare il bottone **Invia documenti** per trasmetterli all'Ente. Come nel caso della *richiesta integrazioni* **non è necessario** generare il PDF e firmarlo.

Una volta trasmessi i documenti, l'*Invio documentazione libera* verrà registrata nella sezione *Comunicazioni Inviate collegate alla Pratica* (come per le comunicazioni).

## Risoluzione problemi

### Errore: "Il file firmato digitalmente non corrisponde all'originale"

Questo è l'errore più frequente durante la fase di invio della pratica e si verifica quando il file PDF generato e il file firmato digitalmente CAdES non sono congruenti.

**Possibili cause:**
- È stato firmato un file PDF diverso da quello generato dal sistema
- Il file firmato non ha l'estensione corretta `.pdf.p7m`
- Il file PDF è stato spostato dalla cartella di download prima della firma
- Il file PDF è stato rinominato prima della firma
- Sono presenti file duplicati nella cartella di download (con suffisso tipo "(1)" nel nome che il browser aggiunge automaticamente)

**Come risolvere:**

1. **Genera nuovamente il PDF** cliccando sul bottone **Genera** nella colonna **PDF**
2. **Pulisci la cartella Download** del computer per evitare file duplicati che potrebbero avere suffissi come "(1)" aggiunti automaticamente dal browser
3. **Scarica nuovamente il file** cliccando sull'icona **PDF**
4. **NON spostare** il file dalla cartella Download del computer
5. **NON rinominare** il file PDF
6. **Firma digitalmente il file** in modalità CAdES direttamente dalla posizione in cui è stato scaricato
7. **Verifica l'estensione** del file firmato: deve essere `.pdf.p7m` (non solo `.p7m`)
8. **Carica il file firmato** nella colonna **P7M**

> **Nota importante**: Il sistema riconosce automaticamente la corrispondenza tra il PDF generato e quello firmato solo se il file originale non è stato né spostato né rinominato prima della firma digitale.

### Problemi con il formato della firma digitale

Se il sistema non accetta il file firmato:

- Verifica di aver utilizzato una firma **CAdES** (e non PAdES o altri formati)
- Controlla che il certificato di firma sia valido e non scaduto
- Assicurati che il software di firma sia aggiornato
- Se il file ha estensione solo `.p7m`, prova a rinominarlo aggiungendo `.pdf` prima di `.p7m` (es: `file.p7m` → `file.pdf.p7m`)

### Non trovo il file scaricato

Se non trovi il PDF generato nella cartella Download:

- Controlla le impostazioni del browser per verificare la cartella di download predefinita
- Verifica che il download sia stato completato correttamente
- Prova a rigenerare il PDF e attendi il completamento del download prima di procedere
