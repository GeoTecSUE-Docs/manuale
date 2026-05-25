---
title: Errori Inizio Lavori - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 42
description: Errori di validazione specifici per la Comunicazione di Inizio Lavori Nazionale - Tutte le regioni (art. 65 e artt. 93/94 D.P.R. 380/2001, D.Lgs. 81/2008)
keywords: [inizio lavori, comunicazione inizio lavori, art. 65 DPR 380/2001, art. 93, art. 94, amianto, piano di lavoro, zona sismica, contributo di costruzione, certificatore energetico, Titolo IV, D.Lgs. 81/2008, direttore lavori, notifica preliminare, nazionale]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 1101 }  # Valle d'Aosta - Inizio Lavori
  - { Reg: 4, Prat: 4101 }  # Lombardia - Inizio Lavori
  - { Reg: 6, Prat: 6101 } # Veneto - Inizio Lavori
  - { Reg: 8, Prat: 8101 } # Emilia-Romagna - Inizio Lavori
  - { Reg: 12, Prat: 12101 } # Lazio - Inizio Lavori
  - { Reg: 13, Prat: 13101 } # Abruzzo - Inizio Lavori
  - { Reg: 15, Prat: 15101 } # Campania - Inizio Lavori
  - { Reg: 16, Prat: 16101 } # Basilicata - Inizio Lavori
  - { Reg: 17, Prat: 17101 } # Puglia - Inizio Lavori
  - { Reg: 18, Prat: 18101 } # Calabria - Inizio Lavori
  - { Reg: 19, Prat: 19101 } # Sicilia - Inizio Lavori
Fonte: Manuale
---

# Errori di validazione - Comunicazione di Inizio Lavori
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per la **Comunicazione di Inizio Lavori** applicabile su tutto il territorio nazionale, relativa ai titoli abilitativi edilizi (Permesso di Costruire, SCIA, titolo unico) e alla contestuale dichiarazione degli adempimenti previsti dagli artt. 65, 93, 94 del D.P.R. 380/2001 e dal D.Lgs. 9 aprile 2008, n. 81.

{: .note }
> La Comunicazione di Inizio Lavori Nazionale è una pratica strutturata con molte sezioni in cascata. Le caratteristiche principali sono: la sezione **Inizio lavori** con 2 tipi di riferimento (titolo unico o pratica edilizia); la sezione **Amianto** con piano di lavoro condizionale; la sezione **Interventi strutturali/sismici** con **due radio group indipendenti** (art. 65 e artt. 93/94); la sezione **Tutela salute/sicurezza** con anagrafica del responsabile completa e struttura sicurezza a **4 livelli**. È richiesto obbligatoriamente un **Direttore Lavori (DR)** nei soggetti coinvolti. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Inizio lavori — tipo pratica e data](#1-inizio-lavori--tipo-pratica-e-data)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Amianto](#3-amianto)
4. [Interventi strutturali e/o in zona sismica](#4-interventi-strutturali-eo-in-zona-sismica)
5. [Contributo di costruzione](#5-contributo-di-costruzione)
6. [Tecnici incaricati — Certificatore Energetico](#6-tecnici-incaricati--certificatore-energetico)
7. [Impresa esecutrice dei lavori](#7-impresa-esecutrice-dei-lavori)
8. [Tutela salute e sicurezza — Anagrafica responsabile](#8-tutela-salute-e-sicurezza--anagrafica-responsabile)
9. [Tutela salute e sicurezza — Titolo IV D.Lgs. 81/2008](#9-tutela-salute-e-sicurezza--titolo-iv-dlgs-812008)
10. [Direttore Lavori nei soggetti coinvolti](#10-direttore-lavori-nei-soggetti-coinvolti)

---

## 1. Inizio lavori — tipo pratica e data

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Inizio lavori'.

**Dove si trova**: Sezione "Inizio lavori" → 2 radio button sotto "ai sensi del Regolamento Edilizio Comunale, che i lavori relativi al"

**Causa**: Non hai indicato il tipo di pratica a cui si riferisce l'inizio lavori.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **a_1 — "titolo unico pratica"** → inserisci numero e data del titolo unico
- ⚪ **a_2 — "pratica edilizia"** → seleziona il tipo pratica dal menu, poi inserisci numero e data

---

### Opzione a_1 — Titolo unico

#### ATTENZIONE ! Campo obbligatorio 'Numero Titolo Unico' non inserito.

**Causa**: Hai selezionato "titolo unico pratica" ma non hai compilato il campo numero.

**Soluzione**: Inserisci il numero del titolo unico nel campo "n." accanto al radio button.

---

#### ATTENZIONE ! Campo obbligatorio 'Data Titolo Unico' non inserito.

**Causa**: Hai compilato il numero ma non la data del titolo unico.

**Soluzione**: Inserisci la data nel campo "presentata in data" nel formato **GG/MM/AAAA**.

---

### Opzione a_2 — Pratica edilizia

#### ATTENZIONE ! Campo obbligatorio 'Tipo Pratica' non selezionato.

**Causa**: Hai selezionato "pratica edilizia" ma non hai selezionato il tipo dal menu a discesa (il campo interno `txtTipoPratica` ha ancora valore "0").

**Soluzione**: Seleziona il tipo di pratica edilizia dal menu a discesa "tipo pratica" (es. Permesso di Costruire, SCIA, SCIA alternativa al PdC).

---

#### ATTENZIONE ! Campo obbligatorio 'Numero Pratica' non inserito.

**Causa**: Hai selezionato il tipo pratica ma non hai compilato il numero.

**Soluzione**: Inserisci il numero della pratica nel campo "n."

---

#### ATTENZIONE ! Campo obbligatorio 'Data Pratica' non inserito.

**Causa**: Hai compilato tipo e numero ma non la data della pratica.

**Soluzione**: Inserisci la data nel campo "presentata in data" nel formato **GG/MM/AAAA**.

---

### Data inizio lavori (comune a entrambe le opzioni)

#### ATTENZIONE ! Campo obbligatorio 'Data Inizio Lavori' non inserito.

**Dove si trova**: Riga "avranno inizio in data" nella sezione Inizio lavori, dopo i campi del tipo pratica

**Causa**: Il campo `txtDataInizioLavori` è vuoto.

**Soluzione**: Inserisci la data prevista di inizio lavori nel formato **GG/MM/AAAA**.

{: .note }
> La data di inizio lavori è sempre obbligatoria, indipendentemente dall'opzione selezionata (titolo unico o pratica edilizia). Si riferisce alla data in cui i lavori avranno effettivamente inizio. Non viene verificato che sia una data futura — il sistema accetta qualsiasi data nel formato corretto.

---

## 2. Localizzazione dell'intervento

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

## 3. Amianto

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Amianto'.

**Dove si trova**: Sezione "Amianto" → 2 radio button nel testo "che le opere"

**Causa**: Non hai dichiarato se i lavori interessano parti di edifici con presenza di amianto.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **c_1** — "non interessano parti di edifici con presenza di fibre di amianto"
- ⚪ **c_2** — "interessano parti di edifici con presenza di fibre di amianto e che è stato predisposto... il Piano di Lavoro di demolizione o rimozione dell'amianto" → seleziona il sotto-radio Piano di Lavoro

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Piano di Lavoro'.

**Causa**: Hai selezionato c_2 (con amianto) ma non hai indicato lo stato del Piano di Lavoro.

**Soluzione**: Seleziona **uno dei due sotto-radio**:
- ⚪ **c_2_1** — "già trasmesso in sede di richiesta del Permesso di Costruire/titolo unico"
- ⚪ **c_2_2** — "presentato alla Azienda Sanitaria Locale in data ___" → inserisci la data di presentazione all'ASL

---

### ATTENZIONE ! Campo obbligatorio 'Data presentazione ASL' non inserito.

**Causa**: Hai selezionato c_2_2 ma non hai compilato la data di presentazione del Piano di Lavoro all'ASL.

**Soluzione**: Inserisci nel campo data accanto al radio button la data in cui il Piano di Lavoro è stato presentato all'Azienda Sanitaria Locale, nel formato **GG/MM/AAAA**.

{: .note }
> Il Piano di Lavoro per la rimozione dell'amianto è previsto dall'art. 256, commi 2 e 5, del D.Lgs. 81/2008. Deve essere predisposto prima dell'inizio dei lavori e presentato all'ASL competente per territorio. La data da inserire è quella di presentazione del piano all'ASL, non quella di approvazione.

---

## 4. Interventi strutturali e/o in zona sismica

Questa sezione contiene **due radio group completamente indipendenti** che devono essere entrambi compilati: il primo riguarda le strutture in cemento armato/metallica (art. 65), il secondo la zona sismica (artt. 93/94). Gli errori di entrambi i gruppi usano lo stesso messaggio generico.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Interventi strutturali e/o in zona sismica'. (primo radio group — art. 65)

**Dove si trova**: Prima parte della sezione → testo "che l'intervento" → 3 radio button

**Causa**: Non hai indicato se l'intervento prevede opere in cemento armato o struttura metallica (art. 65 D.P.R. 380/2001).

**Soluzione**: Seleziona **uno dei tre radio button**:
- ⚪ **d_1** — "non prevede la realizzazione di opere di conglomerato cementizio armato, normale e precompresso ed a struttura metallica"
- ⚪ **d_2** — "prevede la realizzazione di opere di conglomerato cementizio armato... la documentazione tecnica relativa alla denuncia di cui all'articolo 65... è già stata depositata con prot. ___ in data ___" → inserisci n. protocollo + data
- ⚪ **d_21** — "prevede la realizzazione di opere di conglomerato cementizio armato... la documentazione tecnica relativa alla denuncia di cui all'articolo 65 verrà depositata prima dell'inizio delle opere strutturali"

---

#### ATTENZIONE ! Campo obbligatorio 'Numero Protocollo' non inserito. (art. 65, denuncia già depositata)

**Causa**: Hai selezionato d_2 (denuncia art. 65 già depositata) ma non hai inserito il numero di protocollo.

**Soluzione**: Inserisci il numero di protocollo della denuncia nel campo "prot." accanto al radio button.

---

#### ATTENZIONE ! Campo obbligatorio 'Data Protocollo' non inserito. (art. 65, denuncia già depositata)

**Causa**: Hai inserito il numero ma non la data di deposito.

**Soluzione**: Inserisci la data nel campo "in data" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Interventi strutturali e/o in zona sismica'. (secondo radio group — artt. 93/94)

**Dove si trova**: Seconda parte della sezione → testo "e che l'intervento" → 4 radio button

**Causa**: Non hai indicato se l'intervento è soggetto a denuncia o autorizzazione sismica (artt. 93/94 D.P.R. 380/2001).

**Soluzione**: Seleziona **uno dei quattro radio button**:
- ⚪ **d_3** — "non prevede opere da denunciare o autorizzare ai sensi degli articoli 93 e 94 del d.P.R. n. 380/2001 o della corrispondente normativa regionale"
- ⚪ **d_4** — "prevede opere in zona sismica da denunciare ai sensi dell'articolo 93... e la relativa denuncia dei lavori in zona sismica è già stata depositata con prot. ___ in data ___" → inserisci n. protocollo + data
- ⚪ **d_41** — "prevede opere in zona sismica da denunciare ai sensi dell'articolo 93... e la relativa denuncia dei lavori in zona sismica verrà depositata prima dell'inizio delle opere strutturali"
- ⚪ **d_5** — "prevede opere strutturali soggette ad autorizzazione sismica ai sensi dell'articolo 94..." → seleziona il sotto-radio autorizzazione sismica

---

#### ATTENZIONE ! Campo obbligatorio 'Numero Protocollo' non inserito. (art. 93, denuncia già depositata)

**Causa**: Hai selezionato d_4 (denuncia art. 93 già depositata) ma non hai inserito il numero di protocollo.

**Soluzione**: Inserisci il numero nel campo "prot." accanto al radio button d_4.

---

#### ATTENZIONE ! Campo obbligatorio 'Data Protocollo' non inserito. (art. 93, denuncia già depositata)

**Causa**: Manca la data di deposito della denuncia sismica.

**Soluzione**: Inserisci la data nel campo "in data" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Autorizzazione Sismica'.

**Causa**: Hai selezionato d_5 (autorizzazione sismica art. 94) ma non hai indicato se l'autorizzazione è allegata o già ottenuta.

**Soluzione**: Seleziona **uno dei due sotto-radio**:
- ⚪ **d_5_1** — "si allega la documentazione necessaria per il rilascio dell'autorizzazione sismica"
- ⚪ **d_5_2** — "la relativa autorizzazione è già stata ottenuta con prot. ___ in data ___" → inserisci n. protocollo + data

---

#### ATTENZIONE ! Campo obbligatorio 'Numero Protocollo' non inserito. (art. 94, autorizzazione già ottenuta)

**Causa**: Hai selezionato d_5_2 (autorizzazione già ottenuta) ma non hai inserito il numero di protocollo.

**Soluzione**: Inserisci il numero nel campo "prot." accanto al radio button d_5_2.

---

#### ATTENZIONE ! Campo obbligatorio 'Data Protocollo' non inserito. (art. 94, autorizzazione già ottenuta)

**Causa**: Manca la data dell'autorizzazione sismica.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**.

---

## 5. Contributo di costruzione

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Contributo di costruzione'.

**Dove si trova**: Sezione "Contributo di costruzione" → 2 radio button

**Causa**: Non hai dichiarato se il contributo di costruzione è dovuto.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **e_1** — "è a titolo gratuito"
- ⚪ **e_2** — "è a titolo oneroso e pertanto allega la ricevuta della prima rata del costo di costruzione"

---

## 6. Tecnici incaricati — Certificatore Energetico

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tecnici incaricati'.

**Dove si trova**: Sezione "Tecnici incaricati" → 2 radio button relativi al Certificatore Energetico

**Causa**: Non hai dichiarato la situazione del Certificatore Energetico.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **f_1** — "di non aver nominato il Certificatore Energetico in quanto le opere previste non sono soggette all'applicazione dell'articolo 125 del d.P.R. n. 380/2001 e del d.lgs. n. 192/2005"
- ⚪ **f_2** — "di aver nominato il Certificatore Energetico ai sensi della LR 13/2007 e D.G.R. 4/08/2009 n. 45-11965"

{: .note }
> La scelta tra le due opzioni dipende dalla tipologia e dall'entità dell'intervento. Gli interventi di nuova costruzione e quelli di ristrutturazione rilevante sono in genere soggetti alla certificazione energetica. Per interventi di manutenzione ordinaria o straordinaria di modesta entità, si sceglie generalmente f_1.

---

## 7. Impresa esecutrice dei lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Impresa esecutrice dei lavori'.

**Causa**: Non hai indicato chi eseguirà i lavori.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **g_1** — "che i lavori saranno eseguiti dalla/e impresa/e indicata/e alla sezione 3 dell'allegato 'SOGGETTI COINVOLTI'"
- ⚪ **g_2** — "che, in quanto opere di modesta entità che non interessano le specifiche normative di settore, i lavori saranno eseguiti in prima persona, senza alcun affidamento a ditte esterne"

---

## 8. Tutela salute e sicurezza — Anagrafica responsabile

La sezione "Tutela della salute e della sicurezza nei luoghi di lavoro" richiede l'anagrafica completa del committente o responsabile dei lavori. Questi campi vengono validati **prima** della selezione del radio Titolo IV.

---

### ATTENZIONE ! Inserire il Cognome.

**Dove si trova**: Sezione "Tutela della salute e della sicurezza nei luoghi di lavoro" → campo `txtCognomeTut`

**Causa**: Il campo Cognome del committente/responsabile dei lavori è vuoto.

**Soluzione**: Inserisci il cognome del soggetto che sottoscrive la dichiarazione di sicurezza (committente o responsabile dei lavori).

---

### ATTENZIONE ! Inserire il Nome.

**Soluzione**: Inserisci il nome nel campo corrispondente.

---

### ATTENZIONE ! Inserire la Città.

**Dove si trova**: Sezione "Residenza" all'interno della tutela sicurezza → campo `txtCittaResTut`

**Soluzione**: Inserisci la città di residenza del committente/responsabile.

---

### ATTENZIONE ! Inserire la Provincia.

**Soluzione**: Inserisci la sigla della provincia (2 caratteri, es. `TO`).

---

### ATTENZIONE ! Inserire l'Indirizzo.

**Soluzione**: Inserisci l'indirizzo di residenza nel campo "Indirizzo".

---

### ATTENZIONE ! Inserire il Civico.

**Soluzione**: Inserisci il numero civico nel campo "Civico".

---

### ATTENZIONE ! Inserire il CAP.

**Soluzione**: Inserisci le 5 cifre del CAP nel campo "CAP".

---

### ATTENZIONE ! Inserire la PEC/Posta Elettronica.

**Soluzione**: Inserisci l'indirizzo email o PEC nel campo "PEC/Posta Elettronica".

---

### ATTENZIONE ! Inserire il Telefono fisso/Cellulare.

**Soluzione**: Inserisci un recapito telefonico nel campo "Telefono fisso/Cellulare".

{: .note }
> Il menu **"committente/titolare" / "responsabile dei lavori"** (`cmbRuoloTut`) non è validato dal codice — non genera errori se lasciato sul valore di default. Analogamente, i campi dell'ordine professionale (`txtOrdineTut`, `txtOrdineDiTut`, `txtOrdineNumTut`) da compilare solo se il responsabile dei lavori è un tecnico non sono validati. Inserire il ruolo corretto è comunque importante per la correttezza documentale.

---

## 9. Tutela salute e sicurezza — Titolo IV D.Lgs. 81/2008

Dopo l'anagrafica, il validatore controlla la dichiarazione relativa al Titolo IV del D.Lgs. 81/2008 con una struttura a 4 livelli di profondità.

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tutela della salute e della sicurezza nei luoghi di lavoro'.

**Causa**: Non hai indicato se l'intervento ricade nell'ambito del Titolo IV del D.Lgs. 81/2008.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **i_1** — "non ricade nell'ambito di applicazione del Titolo IV del d.lgs. n. 81/2008"
- ⚪ **i_2** — "ricade nell'ambito di applicazione del Titolo IV del d.lgs. n. 81/2008 e pertanto:" → seleziona documentazione imprese

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Documentazione Imprese Esecutrici'.

**Causa**: Hai selezionato i_2 (ricade nel Titolo IV) ma non hai specificato la situazione della documentazione delle imprese.

**Soluzione**: Seleziona **uno dei due radio button** (consultare la tabella riepilogativa nel modulo):
- ⚪ **i_2_1** — "dichiara che l'entità presunta del cantiere è inferiore a 200 uomini-giorno ed i lavori non comportano i rischi particolari di cui all'allegato XI del d.lgs. n. 81/2008 e di aver verificato..." (certificato CCIAA, DURC, autocertificazione contratto collettivo)
- ⚪ **i_2_2** — "dichiara che l'entità presunta del cantiere è pari o superiore a 200 uomini-giorno o i lavori comportano i rischi particolari di cui all'allegato XI..." → seleziona notifica preliminare

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Notifica preliminare'.

**Causa**: Hai selezionato i_2_2 (≥ 200 UG o rischi particolari) ma non hai indicato se la notifica preliminare è dovuta.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **i_2_2_1** — "dichiara che l'intervento non è soggetto all'invio della notifica"
- ⚪ **i_2_2_2** — "dichiara che l'intervento è soggetto all'invio della notifica e pertanto" → seleziona modalità notifica

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Comunicazione/Estremi Notifica'.

**Causa**: Hai indicato che la notifica è dovuta ma non hai specificato se viene allegata o se si comunicano gli estremi di una notifica già trasmessa.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **i_2_2_2_1** — "allega alla presente comunicazione la notifica, il cui contenuto sarà riprodotto su apposita tabella, esposta in cantiere..."
- ⚪ **i_2_2_2_2** — "indica gli estremi della notifica, già trasmessa in data ___ con prot./cod. ___" → inserisci data + protocollo notifica

---

### ATTENZIONE ! Campo obbligatorio 'Data estremi notifica' non inserito.

**Causa**: Hai selezionato i_2_2_2_2 (estremi notifica già trasmessa) ma non hai inserito la data di trasmissione.

**Soluzione**: Inserisci nel campo data la data in cui la notifica preliminare è stata trasmessa, nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Campo obbligatorio 'Prot. estremi notifica' non inserito.

**Causa**: Hai inserito la data ma non il numero di protocollo/codice della notifica.

**Soluzione**: Inserisci nel campo "con prot./cod." il numero di protocollo o codice identificativo della notifica preliminare già trasmessa.

---

## 10. Direttore Lavori nei soggetti coinvolti

### ATTENZIONE ! Non è stata selezionato nessun Tecnico come Direttore Lavori.

**Causa**: Nessun tecnico con ruolo **DR (Direttore Lavori)** è presente tra i soggetti coinvolti della pratica principale a cui è collegata questa comunicazione di inizio lavori.

**Soluzione**: Vai alla pratica principale → **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi un tecnico con ruolo **DR – Direttore Lavori** (delle opere architettoniche).

{: .note }
> Il Direttore Lavori è obbligatorio per tutte le tipologie di lavori oggetto di comunicazione di inizio lavori. Il controllo avviene sui soggetti della pratica principale (Permesso di Costruire, SCIA, ecc.) a cui questa comunicazione è collegata, non su soggetti inseriti direttamente nella comunicazione stessa.

---

## Consigli pratici — Inizio Lavori Nazionale

### Prima di validare ✅

- [ ] Seleziona il **tipo di riferimento** (titolo unico o pratica edilizia) e compila i campi relativi
- [ ] Inserisci la **data di inizio lavori** (GG/MM/AAAA)
- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona la voce **amianto** (e il piano di lavoro se con amianto, e la data ASL se presentato)
- [ ] Seleziona la voce **art. 65** (cemento/metallo): no / già depositato con n.+data / verrà depositato
- [ ] Seleziona la voce **artt. 93/94** (sismica): no / già depositato / verrà depositato / autorizzazione art. 94 (con eventuali sotto-selezioni)
- [ ] Seleziona il **contributo di costruzione** (gratuito o oneroso)
- [ ] Seleziona la voce **certificatore energetico** (nominato o non necessario)
- [ ] Seleziona la voce **impresa esecutrice** (soggetti coinvolti o in proprio)
- [ ] Compila l'**anagrafica del committente/responsabile lavori** (cognome, nome, città, provincia, indirizzo, civico, CAP, email, telefono)
- [ ] Seleziona la voce **Titolo IV** e completa le sotto-dichiarazioni se applicabile
- [ ] Verifica che la pratica principale abbia un **Direttore Lavori (DR)** nei soggetti coinvolti

### Campi presenti ma non validati ℹ️

- **Menu ruolo** (`cmbRuoloTut`): committente/titolare vs responsabile dei lavori — non validato
- **Ordine professionale** del responsabile lavori (`txtOrdineTut`, `txtOrdineDiTut`, `txtOrdineNumTut`) — non validati
- **Formato date**: nessuna data viene verificata nel formato (a differenza di altre pratiche) — il sistema accetta qualsiasi testo nel campo
- **Sezioni "Rispetto normativa privacy"**: non generano errori

### Gerarchia della sezione Interventi strutturali ⚠️

La sezione "Interventi strutturali e/o in zona sismica" ha **due radio group separati** che devono essere entrambi compilati. Il primo (`$Intervento1`) riguarda le strutture in cemento armato/metallo (art. 65), il secondo (`$Intervento2`) riguarda la zona sismica (artt. 93/94). Un errore su uno dei due group genera lo stesso messaggio generico "Non è stata selezionata nessuna voce per 'Interventi strutturali e/o in zona sismica'." — verificare entrambi i gruppi.

### Errori frequenti 🔍

1. **Data pratica e numero pratica confusi con la data di inizio lavori** → nella sezione a) ci sono fino a 3 date distinte: n./data del titolo di riferimento + data inizio lavori; la data inizio lavori è sempre l'ultima del gruppo ed è separata visivamente
2. **Secondo radio group sismico non compilato** → dopo aver selezionato il radio art. 65 ci si dimentica del secondo gruppo artt. 93/94 che genera un errore identico; scorri la sezione per verificare entrambi i gruppi
3. **Anagrafica responsabile lavori parziale** → la sezione tutela sicurezza chiede 9 campi obbligatori prima della selezione del Titolo IV; spesso ci si ferma a compilare solo cognome e nome
4. **Nessun DR nei soggetti coinvolti della pratica principale** → l'errore Direttore Lavori si riferisce ai soggetti della pratica madre (PdC, SCIA) non alla comunicazione stessa; verificare prima di compilare la comunicazione di inizio lavori
5. **Struttura a 4 livelli Titolo IV non completata** → dopo aver selezionato ≥ 200 UG occorre selezionare anche notifica → modalità notifica; se si sceglie "estremi notifica" occorre inserire data + protocollo

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
**Fonte**: Analisi codice ValidaDatiInizioLavoriNazionale e DatiInizioLavoriNaz.ascx
