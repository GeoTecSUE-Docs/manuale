---
title: Errori Notifica Preliminare - Regione Piemonte
parent: Errori di validazione
nav_order: 44
description: Errori di validazione specifici per la Notifica Preliminare Cantiere - Regione Piemonte (art. 99 D.Lgs. 81/2008, sistema MUDE/SPRESALWEB)
keywords: [notifica preliminare, notifica cantiere, art. 99 D.Lgs. 81/2008, MUDE, SPRESALWEB, coordinatore sicurezza, CF, CZ, Piemonte, istanza MUDE, codice ISTAT, aggiornamento]
IDRegione: 2
IDTipoPratica: 2
Fonte: Manuale
---

# Errori di validazione - Notifica Preliminare Cantiere
## Regione Piemonte

Guida completa agli errori specifici per la **Notifica Preliminare Cantiere** ai sensi dell'art. 99 del D.Lgs. 9 aprile 2008, n. 81, relativa alla **Regione Piemonte**. La notifica viene trasmessa allo SPRESALWEB (servizio di prevenzione e sicurezza negli ambienti di lavoro) tramite il sistema MUDE.

{: .note }
> La Notifica Preliminare è una pratica con caratteristiche del tutto diverse dalle altre. Ha una sezione **Qualificazione** con validazione articolata del numero MUDE a 22 cifre (solo per gli aggiornamenti); una sezione **Comunicazioni** con 6 campi numerici e temporali validati, di cui 2 devono coincidere con i dati inseriti nella sezione Imprese; e una logica sui **coordinatori per la sicurezza** che dipende dal numero totale di imprese + lavoratori autonomi inseriti. La pratica al momento dell'invio viene trasmessa al sistema SPRESALWEB: eventuali errori di trasmissione generano un messaggio specifico descritto nella sezione apposita. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Qualificazione pratica — tipo invio e istanza MUDE](#1-qualificazione-pratica--tipo-invio-e-istanza-mude)
2. [Tipologia intervento e descrizione](#2-tipologia-intervento-e-descrizione)
3. [Natura dell'opera](#3-natura-dellopera)
4. [Titolo autorizzativo di riferimento](#4-titolo-autorizzativo-di-riferimento)
5. [Localizzazione dell'intervento](#5-localizzazione-dellintervento)
6. [Comunicazioni — dati cantiere](#6-comunicazioni--dati-cantiere)
7. [Dichiarazioni — amianto](#7-dichiarazioni--amianto)
8. [Coordinatori per la sicurezza nei soggetti coinvolti](#8-coordinatori-per-la-sicurezza-nei-soggetti-coinvolti)
9. [Errori di trasmissione al sistema MUDE/SPRESALWEB](#9-errori-di-trasmissione-al-sistema-mudespresalweb)

---

## 1. Qualificazione pratica — tipo invio e istanza MUDE

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Qualificazione pratica - intervento'.

**Dove si trova**: Sezione "Qualificazione pratica - intervento" → 2 radio button "Primo invio" / "Aggiornamento"

**Causa**: Non hai indicato se si tratta di una prima notifica o di un aggiornamento di una notifica già trasmessa.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **t_1 — "Primo invio"** → nessun campo aggiuntivo richiesto
- ⚪ **t_2 — "Aggiornamento"** → inserisci il numero MUDE della notifica originale

---

### Errori dell'istanza MUDE di primo invio (solo per Aggiornamento)

Se selezioni "Aggiornamento", il campo `txtIstanzaMUDEPrimoInvio` viene abilitato e deve contenere il numero MUDE della notifica preliminare originale. La validazione è molto articolata: il numero viene verificato a più livelli in sequenza.

---

#### ATTENZIONE ! Inserire il numero dell'istanza MUDE di primo invio.

**Causa**: Hai selezionato "Aggiornamento" ma il campo istanza MUDE è vuoto.

**Soluzione**: Inserisci il numero MUDE della notifica preliminare di primo invio nel campo "Istanza di primo invio". Il numero ha **22 cifre numeriche** in un formato strutturato (vedi tabella nel modulo).

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è del formato corretto (22 caratteri numerici).

**Causa**: Il numero inserito non è composto esattamente da 22 cifre numeriche (contiene lettere, spazi, punteggiatura, o ha una lunghezza diversa da 22).

**Soluzione**: Verifica e correggi il numero MUDE. Deve essere esattamente **22 cifre numeriche** senza spazi o separatori. La struttura è: `RRCCCCCCPPPPPPPPPPAAAA` dove:
- `RR` (pos. 1-2): codice ISTAT regionale → deve essere `01` per il Piemonte
- `CCCCCC` (pos. 3-8): codice ISTAT del comune (6 cifre)
- `PPPPPPPPPP` (pos. 9-18): numero progressivo dell'istanza (10 cifre, > 0)
- `AAAA` (pos. 19-22): anno dell'istanza (4 cifre, anno valido)

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è del formato corretto: i primi due caratteri non rappresentano il codice ISTAT regionale (01).

**Causa**: I primi due caratteri del numero MUDE non sono `01` (codice ISTAT della Regione Piemonte).

**Soluzione**: Verifica che il numero MUDE inizi con `01`. Le notifiche del Piemonte hanno sempre i primi due caratteri `01`. Se stai inserendo una notifica di un'altra regione, non è possibile utilizzarla come riferimento.

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è del formato corretto: il codice ISTAT inserito nel numero MUDE non rappresenta quello dell'Ente (XXXXXX).

**Causa**: I caratteri dalla posizione 3 alla 8 del numero MUDE contengono un codice ISTAT di Comune diverso da quello dell'Ente a cui stai presentando la pratica.

**Soluzione**: Verifica che il numero MUDE corrisponda a una notifica presentata allo stesso Ente. Il codice ISTAT nell'errore indica il codice atteso. Se stai aggiornando una notifica presentata a un Ente diverso, non è possibile farlo tramite questo sistema.

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è del formato corretto: il numero dell'istanza non è valido (XXXXXXXXXX).

**Causa**: Le 10 cifre del progressivo (posizioni 9-18) non sono valide: sono zero, o non sono un numero intero positivo.

**Soluzione**: Verifica le cifre del progressivo nel numero MUDE. Il progressivo deve essere un numero intero maggiore di zero.

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è del formato corretto: l'anno dell'istanza non è valido (AAAA).

**Causa**: Le ultime 4 cifre del numero MUDE (posizioni 19-22) non rappresentano un anno valido. L'anno deve essere compreso tra 1900 e l'anno corrente.

**Soluzione**: Verifica le ultime 4 cifre del numero MUDE. L'anno deve essere un anno valido compreso tra `1900` e l'anno in corso.

---

#### ATTENZIONE ! L'istanza MUDE di primo invio non è in stato 'Registrata da PA'.

**Causa**: Il numero MUDE inserito è formalmente corretto e corrisponde a un'istanza presente nel sistema, ma questa istanza non è in stato "Registrata da PA" (cioè non è ancora stata protocollata e registrata dall'ente destinatario).

**Soluzione**: Verifica lo stato della notifica di primo invio nel sistema. Per poter procedere con un aggiornamento, la notifica originale deve essere stata presa in carico dall'ente (stato "Registrata da PA"). Se la notifica è ancora in fase di elaborazione, attendi che venga registrata prima di procedere con l'aggiornamento.

---

## 2. Tipologia intervento e descrizione

### ATTENZIONE ! Non è stata selezionato nessun 'Tipo intervento'.

**Dove si trova**: Sezione "Tipologia intervento" → menu a discesa "Tipo intervento"

**Causa**: Il menu `ddlTipoIntervento` è rimasto sull'opzione vuota iniziale.

**Soluzione**: Seleziona il tipo di intervento dal menu a discesa.

---

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Causa**: Il campo `txtDescrIntervento` è vuoto.

**Soluzione**: Inserisci la descrizione sintetica del cantiere nel campo multiriga (max **300 caratteri**).

---

## 3. Natura dell'opera

### ATTENZIONE ! Non è stata selezionata nessuna 'Natura dell'opera'.

**Dove si trova**: Sezione "Natura dell'opera" → menu a discesa

**Causa**: Il menu `ddlNaturaOpera` è rimasto sull'opzione vuota iniziale.

**Soluzione**: Seleziona la natura dell'opera dal menu a discesa (es. Edilizia residenziale, Edilizia non residenziale, Opere stradali, ecc.).

---

## 4. Titolo autorizzativo di riferimento

La sezione "Titolo autorizzativo di riferimento" è **condizionale**: il menu tipo pratica (`ddlTipoPratica`) è opzionale. Se lasciato sull'opzione vuota, nessun campo viene validato. Se si seleziona un tipo di pratica, i campi protocollo e data diventano obbligatori.

---

### ATTENZIONE ! Inserire il protocollo del titolo autorizzativo di riferimento.

**Causa**: Hai selezionato un tipo di pratica dal menu ma non hai compilato il campo "prot./estremi".

**Soluzione**: Inserisci il numero di protocollo o gli estremi del titolo abilitativo di riferimento (es. `123/2024`, `PdC n. 45 del 10/03/2024`).

---

### ATTENZIONE ! Inserire la data del protocollo del titolo autorizzativo di riferimento.

**Causa**: Hai compilato il protocollo ma non la data.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (titolo autorizzativo)

**Causa**: La data inserita non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 5. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Soluzione**: Spunta "Toponimo mancante" e inseriscilo nel campo testo.

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Soluzione**: Seleziona l'indirizzo dal menu a discesa oppure usa "Toponimo mancante".

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Soluzione**: Inserisci le **5 cifre** del CAP.

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"**.

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Soluzione**: Aggiungi almeno un fabbricato o terreno, compilalo e salvalo con ✅.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Soluzione**: Seleziona almeno una voce dalla lista "Avente destinazione d'uso".

---

## 6. Comunicazioni — dati cantiere

La sezione "Comunicazioni" contiene i dati quantitativi del cantiere. Due dei campi numerici (**n. imprese** e **n. lavoratori autonomi**) vengono confrontati con i soggetti effettivamente inseriti nella sezione Imprese: se i numeri non coincidono, la validazione non passa.

---

### ATTENZIONE ! Inserire la data presunta d'inizio dei lavori in cantiere.

**Causa**: Il campo `txtDataPresuntaInizioLavori` è vuoto.

**Soluzione**: Inserisci la data presunta di inizio cantiere nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data presunta inizio lavori)

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la durata presunta dei lavori in cantiere (gg).

**Causa**: Il campo `txtGiorniPresuntiLavori` è vuoto.

**Soluzione**: Inserisci il numero di giorni lavorativi presunti nel campo "Durata presunta dei lavori in cantiere (gg)".

---

### ATTENZIONE ! La durata presunta dei giorni dei lavori in cantiere deve essere maggiore di 0.

**Causa**: Hai inserito `0` o un valore non numerico nel campo giorni.

**Soluzione**: Inserisci un numero intero positivo (almeno `1`).

---

### ATTENZIONE ! Inserire il numero massimo presunto dei lavoratori sul cantiere.

**Causa**: Il campo `txtNumMaxPresunto` è vuoto.

**Soluzione**: Inserisci il numero massimo di lavoratori presunti contemporaneamente presenti in cantiere.

---

### ATTENZIONE ! Il numero massimo presunto dei lavoratori sul cantiere deve essere maggiore di 0.

**Causa**: Hai inserito `0` nel campo.

**Soluzione**: Inserisci un numero intero positivo (almeno `1`).

---

### ATTENZIONE ! Inserire il numero presunto di imprese sul cantiere.

**Causa**: Il campo `txtNumPresuntoImprese` è vuoto.

**Soluzione**: Inserisci il numero di imprese previste in cantiere.

---

### ATTENZIONE ! Il numero di imprese presunte non coincide con le imprese inserite.

**Causa**: Il numero inserito nel campo `txtNumPresuntoImprese` non corrisponde al numero di soggetti con ruolo **IMPRESA** presenti nella sezione "Soggetti coinvolti" → "Imprese".

**Soluzione**: Verifica i due valori e riallineali:
- Controlla quante imprese hai inserito nella sezione Imprese dei soggetti coinvolti
- Inserisci lo stesso numero nel campo "Numero presunto di imprese sul cantiere"

Oppure, se il numero nel campo è corretto, aggiungi o rimuovi imprese dalla sezione soggetti fino a che coincidono.

---

### ATTENZIONE ! Inserire il numero presunto di lavoratori autonomi sul cantiere.

**Causa**: Il campo `txtNumPresuntoLavAut` è vuoto.

**Soluzione**: Inserisci il numero di lavoratori autonomi previsti in cantiere (inserire `0` se non ci sono lavoratori autonomi).

---

### ATTENZIONE ! Il numero di lavoratori autonomi presunti non coincide con i lavoratori autonomi inseriti (nella sezione Imprese).

**Causa**: Il numero inserito nel campo `txtNumPresuntoLavAut` non corrisponde al numero di soggetti con ruolo **LAVORATORE AUTONOMO** presenti nella sezione "Soggetti coinvolti" → "Imprese".

**Soluzione**: Verifica i due valori e riallineali esattamente come per le imprese. I lavoratori autonomi vengono inseriti nella stessa sezione "Imprese" dei soggetti coinvolti, ma con un ruolo distinto.

---

### ATTENZIONE ! Inserire almeno un'impresa o un lavoratore autonomo.

**Causa**: Sia il numero di imprese che il numero di lavoratori autonomi sono 0 (o entrambi vuoti), quindi il totale è 0.

**Soluzione**: Aggiungi almeno un soggetto tra imprese e lavoratori autonomi nella sezione "Soggetti coinvolti" → "Imprese", e aggiorna i campi numerici di conseguenza. Una notifica preliminare deve avere almeno un soggetto esecutore.

---

### ATTENZIONE ! Inserire l'ammontare complessivo presunto dei lavori (€).

**Causa**: Il campo `txtAmmontareComplessivo` è vuoto.

**Soluzione**: Inserisci il valore in euro dell'importo complessivo presunto dei lavori. Il campo accetta valori decimali con massimo 2 cifre decimali.

---

### ATTENZIONE ! L'ammontare complessivo presunto dei lavori (€) deve essere maggiore di 0.

**Causa**: Hai inserito `0`, un valore non numerico, o un importo negativo (che il sistema riporta automaticamente a 0).

**Soluzione**: Inserisci un importo positivo maggiore di zero (es. `150000`, `25000.50`).

{: .note }
> Il campo ammontare accetta numeri decimali. La virgola viene automaticamente convertita in punto. Valori negativi vengono riportati automaticamente a 0 da una funzione JavaScript nel modulo. Il valore inserito deve rispecchiare il quadro economico del cantiere.

---

## 7. Dichiarazioni — amianto

### ATTENZIONE ! Inserire la data della presentazione del Piano di Lavoro.

**Causa**: Hai spuntato la checkbox "che sono previsti interventi per la rimozione dell'amianto" ma non hai compilato il campo data del Piano di Lavoro.

**Soluzione**: Inserisci la data in cui il Piano di Lavoro per la rimozione dell'amianto è stato presentato all'ASL, nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (Piano di Lavoro amianto)

**Causa**: La data del Piano di Lavoro non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

## 8. Coordinatori per la sicurezza nei soggetti coinvolti

La presenza dei coordinatori è **condizionale al numero totale di soggetti esecutori** (imprese + lavoratori autonomi). Se il totale è 1, nessun coordinatore è richiesto. Se il totale è 2 o più, sia il Coordinatore della progettazione (CF) che il Coordinatore dell'esecuzione (CZ) diventano obbligatori.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Coordinatore per la sicurezza in fase di progettazione.

**Causa**: La somma di imprese + lavoratori autonomi inseriti nei soggetti è maggiore di 1, ma non è presente nessun tecnico con ruolo **CF** (Coordinatore per la sicurezza in fase di progettazione) nella sezione soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **CF – Coordinatore per la sicurezza in fase di progettazione**.

{: .note }
> Ai sensi dell'art. 99 c. 1 e dell'art. 90 del D.Lgs. 81/2008, quando i lavori coinvolgono più imprese esecutrici o lavoratori autonomi, il committente è obbligato a designare un coordinatore per la progettazione e uno per l'esecuzione. Il sistema verifica automaticamente questa condizione in base al numero di soggetti inseriti.

---

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Coordinatore per la sicurezza in fase di esecuzione.

**Causa**: La somma di imprese + lavoratori autonomi è maggiore di 1, ma non è presente nessun tecnico con ruolo **CZ** (Coordinatore per la sicurezza in fase di esecuzione).

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **CZ – Coordinatore per la sicurezza in fase di esecuzione**.

{: .note }
> CF e CZ possono essere lo stesso soggetto o persone diverse. In entrambi i casi devono comparire come due voci separate nei soggetti coinvolti, una con ruolo CF e una con ruolo CZ. Il ruolo **RL (Responsabile Lavori)** è presente nel modulo ma **non è validato** dal codice: non genera errori se assente.

---

## 9. Errori di trasmissione al sistema MUDE/SPRESALWEB

La Notifica Preliminare, a differenza di tutte le altre pratiche, viene trasmessa a un sistema esterno regionale (**SPRESALWEB**) tramite il protocollo MUDE. Il processo di invio può fallire per due tipologie di errore distinte dal normale flusso di validazione del modulo.

{: .warning }
> Questi errori non compaiono durante la compilazione ma **al momento dell'invio** della pratica, dopo aver superato tutta la validazione del modulo.

---

### Messaggio: "Il mancato invio è in fase di analisi: non è necessario riprovare la trasmissione, verrà effettuato un nuovo tentativo dai nostri sistemi automatici"

Questo messaggio viene mostrato quando la pratica ha superato la validazione del modulo ma la trasmissione al sistema MUDE/SPRESALWEB non è andata a buon fine. Le cause possono essere due:

**Causa 1 — Invio pratica su MUDE fallito**: il sistema GeoTecSUE ha tentato di trasmettere la notifica al sistema MUDE regionale ma la chiamata è andata in errore (es. servizio MUDE temporaneamente non disponibile, timeout di comunicazione, errore di rete).

**Causa 2 — Errore in fase di validazione del tracciato XML SPRESALWEB**: la notifica è stata trasmessa al sistema MUDE ma il tracciato XML generato non ha superato la validazione del sistema SPRESALWEB (es. valori fuori range accettati da SPRESALWEB, campi non conformi al tracciato atteso dalla piattaforma regionale).

**Cosa fare**: in entrambi i casi, **non riprovare a trasmettere la pratica**. I tecnici di GeoTecSUE analizzano automaticamente i log di errore, verificano la causa del mancato invio e provvedono a:
- risolvere il problema e ritrasmettere automaticamente la pratica, oppure
- contattare il professionista per comunicare le eventuali correzioni necessarie nel modulo

Il professionista non deve compiere nessuna azione aggiuntiva fino a che non riceve comunicazione dai tecnici di supporto.

{: .note }
> Lo stato della pratica in GeoTecSUE mostrerà "Inviata" o "In elaborazione" anche in caso di mancata trasmissione a SPRESALWEB. La ricevuta di invio GeoTecSUE non garantisce la protocollazione da parte di SPRESALWEB, che avviene in un secondo momento. Contatta [Assistenza](assistenza-tecnica.html) se non ricevi aggiornamenti entro 24 ore lavorative.

---

## Consigli pratici — Notifica Preliminare

### Prima di validare ✅

- [ ] Seleziona **"Primo invio"** o **"Aggiornamento"**; se aggiornamento: inserisci il numero MUDE a 22 cifre
- [ ] Seleziona il **tipo di intervento** dal menu e inserisci la **descrizione** (max 300 caratteri)
- [ ] Seleziona la **natura dell'opera** dal menu
- [ ] Se pertinente: seleziona il **tipo pratica** del titolo autorizzativo e compila **prot./estremi** + **data** (GG/MM/AAAA)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data presunta inizio lavori** (GG/MM/AAAA)
- [ ] Inserisci la **durata presunta** in giorni (> 0)
- [ ] Inserisci il **n. massimo presunto di lavoratori** (> 0)
- [ ] Inserisci il **n. presunto di imprese** (deve coincidere con le imprese nei soggetti)
- [ ] Inserisci il **n. presunto di lavoratori autonomi** (deve coincidere con i lav. autonomi nei soggetti)
- [ ] Inserisci l'**ammontare complessivo** in euro (> 0)
- [ ] Se amianto: spunta la checkbox e inserisci la **data del Piano di Lavoro** (GG/MM/AAAA)
- [ ] Se imprese + lav.aut. > 1: aggiungi **CF** e **CZ** nei soggetti tecnici

### Campi presenti ma non validati ℹ️

- **Tipologia committente** (`ddlTipologiaCommittente`): ha la classe `CampoObbligatorio` ma non viene verificato dal codice VB
- **Responsabile Lavori (RL)**: presente nella logica ma commentato — non genera errori
- **Note** (`txtNote`): facoltative
- **Titolarità** (`cmbTitoloSuImm`): menu presente ma non validato

### Il numero di imprese non coincide — come risolvere ⚠️

Il confronto avviene tra il campo `txtNumPresuntoImprese` e il conteggio dei soggetti con ruolo IMPRESA nella sezione soggetti coinvolti. L'unico modo per risolvere l'errore è allineare i due valori: o aggiungi/rimuovi imprese dai soggetti, o correggi il numero nel campo. Lo stesso vale per i lavoratori autonomi.

### Errori frequenti 🔍

1. **Numero MUDE non corretto** → il formato a 22 cifre è rigido; copiarlo dal sistema MUDE piemontese è il metodo più sicuro per evitare errori
2. **N. imprese nel campo ≠ n. imprese nei soggetti** → inserire prima tutte le imprese nei soggetti e solo dopo compilare il campo numerico; aggiungere o rimuovere imprese dopo aver già compilato il campo richiede di aggiornare manualmente anche il numero
3. **Ammontare = 0** → valori decimali inseriti con la virgola vengono convertiti automaticamente; se il sistema riporta a 0, verificare che il valore sia un numero positivo
4. **CF e CZ mancanti con 2+ imprese** → l'errore appare solo dopo aver superato tutti i controlli precedenti; verificare in anticipo il numero di imprese e i soggetti tecnici

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
**Fonte**: Analisi codice ValidaDatiNP e DatiNP.ascx
