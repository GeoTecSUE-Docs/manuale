---
title: Troubleshooting
nav_order: 20
parent: Assistenza, risoluzione problemi e FAQ
description: Problemi comuni su GeoTecSUE e soluzioni immediate basate su oltre 1.500 ticket reali - risolvi autonomamente i problemi più frequenti
keywords: [troubleshooting, problemi comuni, errori, soluzioni, risoluzione problemi, FAQ tecnica, fix, debug]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Troubleshooting

Questa sezione contiene i **problemi più comuni** riscontrati su GeoTecSUE e le relative **soluzioni immediate**.

{: .note }
> **Basato su dati reali**: Questa guida è stata creata analizzando **1.542 ticket** di assistenza effettivi. I problemi sono ordinati per frequenza e le soluzioni sono quelle che l'assistenza ha fornito ai casi reali.

## Come usare questa guida

1. **Cerca il tuo problema** nell'indice qui sotto
2. **Segui la soluzione** passo-passo
3. **Se non risolve**, contatta l'[assistenza tecnica](assistenza-tecnica.html)

---

## Indice problemi per frequenza

Basato su analisi di 1.542 ticket reali:

| # | Problema | Frequenza | Vai a |
|---|----------|-----------|-------|
| 1 | Comunicazioni mancanti (menu scomparso) | 25.0% | [↓](#1-comunicazioni-mancanti-menu-scomparso) |
| 2 | Caricamento file/allegati | 11.2% | [↓](#2-caricamento-file-e-allegati) |
| 3 | Pagamenti PagoPA / IUV | 11.1% | [↓](#3-pagamenti-pagopa-e-iuv) |
| 4 | Validazione pratica | 6.1% | [↓](#4-validazione-pratica) |
| 5 | Accesso (SPID/CIE) | 4.5% | [↓](#5-accesso-spid-e-cie) |
| 6 | Pratiche collegate / Varianti | 3.6% | [↓](#6-pratiche-collegate-e-varianti) |
| 7 | Protocollazione e ricevute | 3.1% | [↓](#7-protocollazione-e-ricevute) |
| 8 | Voltura / Cambio professionista | 1.9% | [↓](#8-voltura-e-cambio-professionista) |
| 9 | Generazione PDF | 1.4% | [↓](#9-generazione-pdf) |
| 10 | Annullamento / Archiviazione | 0.5% | [↓](#10-annullamento-e-archiviazione) |

---

## 1. Comunicazioni mancanti (menu scomparso)

**Frequenza**: 25.0% dei ticket (problema più comune in assoluto!)

### Problema 1.1: Menu "Comunicazioni" non compare

**Sintomo**: Apro il dettaglio della pratica registrata ma non vedo il menu a tendina per inviare Inizio Lavori, Fine Lavori, ecc. Vedo solo "Invio documentazione libera".

**Esempio reale**:
> "NELLE PRATICHE REGISTRATE NON COMPARE PIU' LA TENDINA CON LA POSSIBILITA' DI CONSEGNARE LA DOCUMENTAZIONE DI FINE LAVORI, COLLAUDO, ECC MA C'E' SOLO LA POSSIBILITA' DI INVIARE DOCUMENTAZIONE LIBERA."

**Causa**: L'Ente **non ha attivato** le comunicazioni per quella tipologia di pratica (es. CILAS, Denuncia Sismica).

**Soluzione**:

**NON è un problema tuo - è configurazione dell'Ente che manca**.

1. Contatta l'Ente (telefonicamente, via mail, di persona)
2. Specifica:
   - Numero pratica
   - Tipo di pratica (es. CILAS, Denuncia Sismica)
   - Comune
   - Comunicazione che devi inviare (es. Fine Lavori)

3. L'Ente potrà operare in autonomia attivando la comunicazione (oppure dando indicazioni sul motivo per il quale la comunicazione non può essere attivata)
4. Non appena l'Ente attiva la comunicazione puoi ricaricare la pagina e procedere con la comunicazione

{: .note }
> **Soluzione rapida**: L'Ente può attivare la funzionalità in pochi minuti. Questo è il problema più comune e più rapido da risolvere. Se l'Ente non è in grado di operare in autonomia, può richiedere supporto a **SISCOM**

**Tipologie di pratica più colpite**:
- ✅ **CILAS** (Comunicazione fine lavori)
- ✅ **Denuncia Sismica** e **Denuncia Sismica Semplificata** (Fine lavori, Collaudo, Relazione a struttura ultimata)

### Problema 1.2: Comunicazioni scomparse dopo aver iniziato a compilarle

**Sintomo**: Avevo iniziato a compilare Inizio Lavori, poi l'Ente ha richiesto integrazioni e adesso non la trovo più.

**Causa**: Alcuni Enti configurano il sistema per nascondere le comunicazioni durante le integrazioni.

**Soluzione**:
1. **Non preoccuparti**: La comunicazione NON è persa
2. **Rispondi alle integrazioni** richieste dall'Ente
3. Quando le integrazioni sono acquisite, la pratica torna a "Registrata"
4. Il sistema **ripropone automaticamente** tutte le comunicazioni che avevi iniziato
5. Potrai riprendere e completare

{: .note }
> Questa è una configurazione intenzionale. Le comunicazioni sono al sicuro e riappariranno automaticamente.

---

## 2. Caricamento file e allegati

**Frequenza**: 11.2% dei ticket

### Problema 2.1: "File non caricato" ma l'ho caricato!

**Sintomo**: Carico un allegato obbligatorio, lo vedo nell'elenco, ma quando valido il sistema dice "ATTENZIONE! Non è stato caricato il file per: [nome documento]".

**Esempio reale**:
> "URGENTE!!!! Dopo aver caricato i file firmati .p7m quando faccio 'valida e salva' mi esce la seguente scritta 'ATTENZIONE ! Non è stato caricato il file per: ELABORATO GRAFICO DI INQUADRAMENTO GENERALE DELLO STATO DI FATTO E PROGETTO'."

**Causa**: Hai caricato il file nella sezione **SBAGLIATA** → "Documenti liberi" invece di "Documenti obbligatori".

**Soluzione**:

1. Vai alla sezione **"Quadro riepilogativo della documentazione"**
2. **NON usare** la sezione "Elenco dei documenti liberi"
3. Trova il documento nell'elenco **"Elenco dei documenti obbligatori richiesti"**
4. Clicca **"Sfoglia"** o **"Carica"** sulla **riga specifica** del documento richiesto
5. Seleziona il file
6. Verifica che appaia con icona ✅ nella colonna "Documenti obbligatori"
7. **Se l'hai caricato come "libero"**: Elimina da lì e ricarica nella sezione obbligatori

{: .warning }
> **Errore comune**: Pensare che "Documenti liberi" sia equivalente a "Documenti obbligatori". Il sistema NON riconosce documenti obbligatori caricati come liberi!

**Procedura corretta**:
```
❌ SBAGLIATO:
Quadro riepilogativo documentazione
  └─ Elenco dei documenti liberi ← NON QUI!
       └─ Aggiungi → Carica "Relazione tecnica"

✅ CORRETTO:
Quadro riepilogativo documentazione
  └─ Elenco dei documenti obbligatori richiesti
       └─ [Relazione tecnica asseverata] ← Clicca "Carica" QUI!
           └─ Sfoglia → Seleziona file
```

### Problema 2.2: File troppo grande

**Sintomo**: "Il file supera la dimensione massima consentita" (solitamente 10-25 MB).

**Soluzione**:

**Opzione A - Comprimi il PDF**:
1. Usa tool online: iLovePDF, Smallpdf, PDF Compressor
2. Riduci qualità immagini a 70-80%
3. Ricarica

**Opzione B - Dividi il documento**:
1. Se il documento accetta più file (es. Elaborati grafici)
2. Dividi in TAV01.pdf, TAV02.pdf
3. Carica separatamente

**Opzione C - Riduci risoluzione**:
1. Se contiene immagini ad alta risoluzione
2. Riduci a 150-200 DPI (sufficiente)
3. Esporta nuovamente

### Problema 2.3: Formato file non accettato

**Sintomo**: "Formato file non valido" o "Estensione non supportata".

**Causa**: Stai caricando un file che non rispetta il formato richiesto.

**Soluzione**:
1. Verifica che il file abbia il formato richiesto e se ne viene richiesta la firma
2. Ricarica

**Formati accettati**:
- Dipendono dalle impostazioni dell'Ente. Buona norma è però quella di usare il .pdf

---

## 3. Pagamenti PagoPA e IUV

**Frequenza**: 11.1% dei ticket

### Problema 3.1: Non riesco a generare IUV

**Sintomo**: Clicco "Crea IUV" ma non viene generato o ricevo errore generico.

**Esempio reale**:
> "Buongiorno, non riesco a generare lo IUV per il pagamento di 30 euro. Spiegatemi come si fa ed eventualmente sbloccare il sistema."

**Causa più comune**: Qualche campo è errato o malformato.

**Soluzione**:

1. Prova a fare un "Valida e Salva"
2. Verifica dove viene indicato l'errore (normalmente è un campo con sfondo giallo)
3. **Correggi** l'errore
4. **Salva** la pratica
5. **Riprova** la generazione IUV

**Campi da verificare**:
- Email titolare (deve essere valida)
- Codice Fiscale titolare (formalmente corretto)
- Indirizzo completo (via, numero civico)

{: .note }
> **CAP errato** è la causa dell'80% dei problemi di generazione IUV. Verifica sempre questo campo per primo!

### Problema 3.2: Stato pagamento non aggiornato dopo aver pagato

**Sintomo**: Ho pagato ma il sistema mostra ancora "IUV generato" invece di "Pagamento eseguito".

**Soluzione**:
1. **Attendi 10-15 minuti** dopo il pagamento
2. Torna alla pratica
3. Sezione **"PagoPA"** → Clicca **"Aggiorna stato"** (pulsante arancione)
4. Il sistema interroga PagoPA

**Se dopo 1 ora non si aggiorna**:
1. Verifica addebito sul conto bancario
2. Controlla di aver pagato il codice IUV **corretto**
3. Attendi 24 ore
4. Contatta l'Ente per sapere se lo IUV è stato correttamente pagato anche sui loro sistemi

Per tutti gli stati PagoPA: [Appendice Stati PagoPA](appendici/pagopa-stati.html)

### Problema 3.3: IUV scaduto

**Sintomo**: Stato: "Pagamento scaduto (40)".

**Causa**: Non hai pagato entro la scadenza (30-60 giorni).

**Soluzione**:
1. Clicca **"Elimina"** sul pagamento scaduto (pulsante rosso)
2. Clicca **"Crea IUV"** per generare nuovo codice
3. Paga il nuovo IUV entro la nuova scadenza

{: .warning }
> IUV scaduti NON sono pagabili. Devi sempre generarne uno nuovo.

---

## 4. Validazione pratica

**Frequenza**: 6.1% dei ticket

### Problema 4.1: "Campo obbligatorio non compilato" senza indicare quale

**Sintomo**: Clicco "Valida e Salva", ricevo errore generico ma il sistema non mi dice quale campo manca.

**Soluzione**:

**Procedura sistematica**:
1. Al click sul pulsante, il sistema si posiziona esattamente nel punto in cui viene rilevato l'errore
2. Cerca campo con errore e risolvilo

**Campi spesso dimenticati**:
- ✅ Email titolare
- ✅ Telefono titolare
- ✅ Almeno un dato catastale (Fabbricato O Terreno)
- ✅ Destinazione d'uso (almeno una)
- ✅ Soggetti obbligatori (progettista, direttore lavori, impresa)

**Verifica allegati**:
- "Quadro riepilogativo documentazione"
- TUTTI i documenti obbligatori con icona ✅

**Verifica pagamenti**:
- Pagamenti obbligatori in stato "Pagamento eseguito"

### Problema 4.2: Errore "Non è stata selezionata alcuna voce per documentazione imprese esecutrici"

**Sintomo**: Validazione fallisce con questo messaggio specifico.

**Esempio reale**:
> "Buonasera, dovrei inviare con urgenza una pratica ma al momento della validazione compare l'errore 'Attenzione! Non è stata selezionata alcuna voce per documentazione imprese esecutrici'"

**Causa**: Nella sezione **"Rispetto degli obblighi in materia di salute e sicurezza nei luoghi di lavoro"** hai selezionato "ricade nell'ambito di applicazione..." ma **non** hai selezionato una delle due opzioni successive.

**Soluzione**:
1. Il sistema ti posiziona nella sezione "Rispetto obblighi salute e sicurezza"
2. Hai già spuntato: "ricade nell'ambito di applicazione delle norme (D.Lgs. 81/2008)"
3. **Devi selezionare** una delle due opzioni:
   - ☑️ "dichiara che l'entità presunta del cantiere è **inferiore** a 200 uomini-giorno..."
   - ☑️ "dichiara che l'entità presunta del cantiere è **pari o superiore** a 200 uomini-giorno..."
4. Seleziona quella appropriata
5. Salva e valida di nuovo

---

## 5. Accesso SPID e CIE

**Frequenza**: 4.5% dei ticket

### Problema 5.1: Devo usare SPID anche se ero già registrato prima

**Sintomo**: Accedevo con username e password, ora mi chiede SPID.

**Esempio reale**:
> "Sono registrato a diversi comuni, solo per quest'ultimo devo inserire la partita IVA per il login invece del Codice Fiscale. Questo mi obbliga ad entrare con SPID invece che con username e password. Come posso risolvere?"

**Causa**: **Normativa AGID** (28 febbraio 2021): le P.A. devono usare SPID/CIE come unico sistema di identificazione.

**Risposta**: **Non si può risolvere - è obbligatorio per legge**.

**Spiegazione**:
- Dal 28/02/2021, tutte le P.A. devono integrare SPID/CIE
- L'accesso con username/password è stato **dismesso**
- Per **primo accesso** a un nuovo Comune sei OBBLIGATO a usare SPID o CIE
- Nessun'altra modalità è prevista

{: .note }
> Questa non è una scelta di GeoTecSUE ma un **obbligo di legge** stabilito da AGID (Agenzia per l'Italia Digitale).

---

## 6. Pratiche collegate e varianti

**Frequenza**: 3.6% dei ticket

### Problema 6.1: Come creo una variante collegata a una pratica esistente?

**Sintomo**: Devo fare una variante a una SCIA/Permesso già presentato ma non trovo come collegarla.

**Esempio reale**:
> "Buongiorno, devo fare un'istanza collegata alla SCIA numero 99999999. Come si crea un'istanza collegata? Se facessi una nuova CILA sarebbe errato perché c'è la SCIA aperta e quindi non riesco a capire come creare un'istanza collegata."

**Risposta**: **La variante è una pratica NUOVA**, non si crea "dentro" la pratica principale.

**Soluzione**:
1. Vai su **"Nuova istanza"**
2. Seleziona il tipo di pratica di interesse (SCIA, Permesso di Costruire...)
3. Compila normalmente
4. Nella sezione dedicata, indica la pratica esistente a cui la variante si riferisce inserendo numero e data (o selezionandola dall'elenco, se disponibile)
5. Si può utilizzare anche la sezione **"Descrizione dell'intervento"**, in cui inserire (ad esempio):
   - "Variante alla SCIA n. [numero pratica] del [data]"
   - Oppure: "Variante al Permesso di Costruire n. [numero] - Pratica [anno/numero]"
6. L'Ufficio Tecnico vedrà il riferimento e collegherà le due pratiche nel proprio gestionale

{: .note }
> Il collegamento tra pratiche è gestito dall'Ente nel proprio sistema. Tu devi solo indicare chiaramente nella descrizione a quale pratica si riferisce la variante oppure spuntare opportuna voce se prevista dal modello.

{: .note }
> **Attenzione**: il D.P.R. 380/2001 disciplina le varianti distinguendo tra modifiche non rilevanti e variazioni essenziali. Tuttavia, non tutte le pratiche edilizie ammettono la presentazione di varianti: la possibilità dipende dal tipo di titolo edilizio e dalla normativa regionale applicabile. Devi quindi verificare caso per caso se la variante è consentita oppure se è necessario presentare una nuova pratica

### Problema 6.2: Denuncia Sismica collegata a SCIA

**Sintomo**: Devo presentare Denuncia Sismica per una SCIA ma non so se farla separata o collegata.

**Esempio reale**:
> "Dopo aver caricato una SCIA, devo creare una denuncia sismica semplificata da collegare alla SCIA, però nella pagina della SCIA già caricata non vi è possibilità di creare tale pratica collegata..."

**Risposta**: La Denuncia Sismica va creata come **pratica separata**.

**Soluzione**:
1. Presenta la **SCIA** normalmente
2. Crea una **Nuova istanza** → "Denuncia Sismica Semplificata"
3. Nella descrizione scrivi: "Denuncia sismica relativa alla SCIA n. [numero pratica]"
4. L'Ente collegherà le due pratiche

---

## 7. Protocollazione e ricevute

**Frequenza**: 3.1% dei ticket

### Problema 7.1: Ricevuta senza data e numero protocollo

**Sintomo**: Scarico ricevuta di invio o protocollo ma mancano data/numero protocollo.

**Esempio reale**:
> "Invia documentazione libera. Sia la ricevuta di invio che la ricevuta di protocollo presentano questa scritta L'OGGETTO NULLABLE DEVE AVERE UN VALORE. Sulle ricevute non compare ne la data ne il numero di protocollo."

**Causa**: Bug temporaneo del sistema (già risolto, ma se capita ancora).

**Soluzione**:
1. **Attendi** che l'assistenza risolva (solitamente entro 24 ore)
2. Torna nel dettaglio della pratica
3. Nella sezione **"Ricevute"**
4. Clicca il pulsante **"Rigenera ricevuta"** (icona refresh)
5. Scarica la ricevuta corretta

{: .note }
> Se capita, contatta subito [assistenza](assistenza-tecnica.html). È un bug noto che viene risolto rapidamente.

### Problema 7.2: Pratica inviata ma non protocollata

**Sintomo**: Ho inviato la pratica giorni fa ma è ancora "Inviata", non "Protocollata".

**Causa**: La protocollazione è eseguita dall'**Ente**, non automatica.

**Soluzione**:
1. **Contatta l'Ufficio Tecnico** dell'Ente per sollecitare
2. La protocollazione **non dipende** da GeoTecSUE
3. Tempi tipici: poche ore / pochi giorni (dipende dall'Ente)

{: .note }
> GeoTecSUE trasmette la pratica all'Ente. La protocollazione è un'operazione manuale dell'Ufficio Protocollo dell'Ente.

---

## 8. Voltura e cambio professionista

**Frequenza**: 1.9% dei ticket

### Problema 8.1: Come passo la pratica a un altro professionista?

**Sintomo**: Non sono più il professionista incaricato, come trasferisco la pratica al nuovo professionista?

**Esempio reale**:
> "In riferimento alla pratica PdC intestata al sig. Mario Rossi, non essendo il sottoscritto più delegato dalla proprietà e progettista delle opere, richiedo quale procedura attivare per consentire al nuovo progettista di gestire direttamente l'iter della pratica."

**Risposta**: Devi richiedere una **VOLTURA** della pratica.

**Soluzione**:

**Procedura completa**:
1. Prepara documento di **richiesta voltura** firmato da:
   - Professionista **uscente** (tu)
   - Professionista **entrante** (nuovo professionista)
   - **Proprietà** (titolare della pratica)
   Eventualmente chiedi all'Ente cosa correttamente presentare

2. Nel [dettaglio della pratica](dettaglio-istanza.html):
   - Vai a "Invio documentazione all'Ente"
   - Clicca **"Nuovo invio"** (documentazione libera/volontaria)
   - Carica il documento di richiesta voltura
   - Invia

3. L'**Ente** riceve la richiesta
4. Se approva, l'Ente "sposta" la pratica dalla tua scrivania a quella del nuovo professionista
5. Il nuovo professionista potrà operare direttamente

{: .warning }
> Solo l'**Ente** può eseguire volture. Tu puoi solo richiedere, serve l'autorizzazione dell'Ente.

### Problema 8.2: Come subentro ad altro professionista?

**Sintomo**: Devo sostiruire il professionista originale. Come posso fare?

**Esempio reale**:
> "In riferimento alla pratica PdC intestata al sig. Mario Rossi, come posso subentrare al collega Luigi Verdi nella gestione della pratica?"

**Risposta**: Devi richiedere una **VOLTURA** della pratica.

**Soluzione**:

**Procedura completa**:
1. Prepara documento di **richiesta voltura** firmato da:
   - Professionista **uscente** (tu)
   - Professionista **entrante** (nuovo professionista)
   - **Proprietà** (titolare della pratica)
   Eventualmente chiedi all'Ente cosa correttamente presentare

2. Trasmetti l'istanza via PEC all'Ente

3. L'**Ente** riceve la richiesta
4. Se approva, l'Ente "sposta" la pratica dalla tua scrivania a quella del nuovo professionista
5. Il nuovo professionista potrà operare direttamente

{: .warning }
> Solo l'**Ente** può eseguire volture. Tu puoi solo richiedere, serve l'autorizzazione dell'Ente.

---

## 9. Generazione PDF

**Frequenza**: 1.4% dei ticket

### Problema 9.1: PDF con campi vuoti dopo autocompilazione

**Sintomo**: Genero PDF da "Autocompilazione modelli" (es. procura) ma i campi sono tutti vuoti.

**Causa**: Bug risolto con aggiornamento sistema.

**Soluzione**:
1. Se capita ancora:
   - Ricarica la pagina (Ctrl+F5)
   - Ricompila il modello
   - Clicca "Salva i dati"
   - Genera PDF

2. Se persiste, contatta [assistenza](assistenza-tecnica.html)

### Problema 9.2: Caratteri strani con apostrofo

**Sintomo**: Quando scrivo parole con apostrofo (es. "dell'intervento") appaiono caratteri strani nel PDF o durante il salvataggio.

**Esempio reale**:
> "Durante la compilazione dei campi di qualsiasi modello se si usa il carattere apostrofo (') si generano erroneamente dei caratteri alfanumerici in fase di salvataggio."

**Causa**: Bug risolto con aggiornamento 6.9.12

**Soluzione**:
- Il problema è stato risolto
- Se capita ancora, contatta [assistenza](assistenza-tecnica.html)

---

## 10. Annullamento e archiviazione

**Frequenza**: 0.5% dei ticket

### Problema 10.1: Come annullo una pratica inviata per errore?

**Sintomo**: Ho inviato una pratica sbagliata e voglio annullarla.

**Esempio reale**:
> "POICHE' HO PRESENTATO UNA PRATICA CIL AL COMUNE DI XXXXX A CAUSA DI UN ERRORE DI PRESENTAZIONE DELLA MEDESIMA VORREI SAPERE COME ANNULLARE LA SEGUENTE PRATICA"

**Risposta**: Devi richiedere **Archiviazione** della pratica.

**Soluzione**:

1. Vai all'[elenco istanze](elenco-istanze.html) → Pratiche inviate
2. Clicca il **pulsante verde** (dettaglio) della pratica da annullare
3. In alto a destra, clicca **"Richiedi Archiviazione"** (se Registrata, altrimenti devi attendere)
4. Il sistema predispone l'**istanza di archiviazione**
5. Compila come una normale istanza:
   - Motivo dell'archiviazione
   - Eventuali allegati
6. Valida
7. Firma (se richiesto)
8. **Invia** all'Ente

9. L'Ente riceve la richiesta
10. Se approva, **archivia** la pratica (stato finale)

{: .warning }
> L'invio è irreversibile. Puoi solo RICHIEDERE archiviazione, ma l'Ente deve approvarla. Non è automatico.

---

## Problemi tecnici del sistema

### Problema: Portale lento / Errore 500 / Errore di connettività

**Sintomo**: Il portale è lentissimo, dà errori generici o timeout.

**Causa**: Possibili problemi temporanei di connettività o manutenzione.

**Soluzione**:
1. **Attendi 5-10 minuti** (potrebbe essere manutenzione)
2. **Ricarica la pagina** (F5)
3. **Svuota cache** (Ctrl+Shift+Canc)
4. **Riprova**

**Se persiste oltre 30 minuti**: Contatta [assistenza](assistenza-tecnica.html)

{: .note }
> Problemi di connettività vengono solitamente risolti entro poche ore.

---

## Browser supportati

### Browser consigliati ✅

| Browser | Versione minima | Note |
|---------|----------------|------|
| **Google Chrome** | 90+ | ⭐ Consigliato |
| **Mozilla Firefox** | 88+ | ⭐ Consigliato |
| **Microsoft Edge** | 90+ | ✅ Supportato |
| **Safari** | 14+ | ✅ Supportato (Mac) |

### Browser non supportati ❌

- ❌ Internet Explorer (dismesso)
- ❌ Edge Legacy (< 90)
- ⚠️ Browser mobile (funzionalità limitate - usa PC)

### Suggerimenti

1. **Mantieni aggiornato** il browser
2. **Disabilita estensioni** che bloccano script
3. **Abilita cookie** di terze parti per SPID/CIE
4. **Svuota cache** periodicamente

---

## Checklist rapida pre-assistenza

Prima di contattare assistenza, hai provato:

- [ ] Ricaricare la pagina (F5)
- [ ] Svuotare cache (Ctrl+Shift+Canc)
- [ ] Provare con browser diverso
- [ ] Controllare connessione internet
- [ ] Consultare questa guida Troubleshooting
- [ ] Attendere 15 minuti (per problemi temporanei)

### Se nessuna soluzione funziona

**Contatta [assistenza tecnica](assistenza-tecnica.html)** con:

✅ Numero pratica (se applicabile)  
✅ Tipo di pratica (SCIA, Permesso, ecc.)  
✅ Cosa stavi facendo  
✅ Messaggio di errore **esatto**
✅ Browser e versione  
✅ Telefono (se disponibile)  

---

## Statistiche e note finali

**Questa guida è basata su**:
- **1.542 ticket** reali analizzati
- Problemi e soluzioni **effettivamente verificati**
- Pattern ricorrenti identificati tramite analisi automatica

**Top 3 problemi che puoi risolvere DA SOLO**:
1. **File caricato ma non riconosciuto** → Carica in "Documenti obbligatori", non "Liberi"
2. **IUV non si genera** → Verifica CAP (5 cifre esatte)
3. **Validazione senza indicare campo** → Scorri tutta la pratica, cerca campi gialli vuoti

**Top 3 problemi che richiedono ASSISTENZA**:
1. **Menu comunicazioni mancante** → Assistenza attiva funzionalità per Ente
2. **Pratiche non protocollate** → Sollecita Ente (non dipende da GeoTecSUE)
3. **Bug del sistema** → Assistenza corregge e aggiorna

---

**Problema non risolto?**

Contatta [assistenza tecnica](assistenza-tecnica.html) con descrizione dettagliata e screenshot.

---

**Ultima revisione**: Febbraio 2026  
**Basato su**: Analisi 1.542 ticket reali  
**Aggiornato con**: Soluzioni verificate dall'assistenza
