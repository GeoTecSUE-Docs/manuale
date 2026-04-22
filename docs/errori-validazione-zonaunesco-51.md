---
title: Errori Zona UNESCO - Regione Piemonte
parent: Errori di validazione
nav_order: 21
description: Errori di validazione specifici per la richiesta di parere in Zona UNESCO - Regione Piemonte (L.R. 32/2008)
keywords: [UNESCO, zona UNESCO, core zone, buffer zone, PRG vigente, PRG adottato, parere UNESCO, L.R. 32/2008, art. 49 L.R. 56/77]
IDRegione: 2
IDTipoPratica: 51
Fonte: Manuale
---

# Errori di validazione - Zona UNESCO
## Regione Piemonte

Guida completa agli errori specifici per la **richiesta di parere in Zona UNESCO**, ai sensi della L.R. 32 del 01/12/2008 e s.m.i., dell'art. 49, comma 7, della L.R. 56/77 e delle vigenti Norme Tecniche di Attuazione del P.R.G., relativa alla **Regione Piemonte**.

{: .note }
> La pratica Zona UNESCO è richiesta per interventi su immobili ricadenti nelle aree iscritte nella Lista del Patrimonio Mondiale UNESCO. È una pratica snella con controlli limitati: titolarità, localizzazione (incluse Zona PRG vigente e adottato), zona di appartenenza (Core Zone o Buffer Zone) e descrizione sintetica dell'intervento. Non include sezioni tecnici, imprese, sicurezza o contributo. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Titolarità dell'intervento](#1-titolarità-dellintervento)
2. [Localizzazione dell'intervento](#2-localizzazione-dellintervento)
3. [Zone di localizzazione dell'intervento](#3-zone-di-localizzazione-dellintervento)
4. [Descrizione sintetica dell'intervento](#4-descrizione-sintetica-dellintervento)

---

## 1. Titolarità dell'intervento

### ATTENZIONE ! Specificare la titolarità dell'intervento.

**Dove si trova**: Campo **"Specificare se altro"** nella sezione **"Titolarità Intervento"**

**Causa**: Hai selezionato dal menu a discesa la voce **"altro"** come titolo di presentazione della pratica, ma non hai compilato il campo di testo libero che specifica di quale titolo si tratta.

**Soluzione**:
1. Trova il campo **"Specificare se altro"** accanto al menu a discesa della titolarità
2. Inserisci il tipo di titolo che hai sull'immobile (es. `Locatario con autorizzazione del proprietario`, `Amministratore di condominio delegato`, `Procuratore`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il campo "Specificare se altro" è normalmente disabilitato e si attiva automaticamente solo quando si seleziona la voce "altro" dal menu a discesa. Per tutte le altre voci del menu (proprietario, usufruttuario, ecc.) questo campo non è richiesto e il controllo non viene eseguito.

---

## 2. Localizzazione dell'intervento

---

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: Hai spuntato ☑ **"Toponimo mancante"** ma non hai inserito l'indirizzo manualmente.

**Soluzione**: Compila il campo di testo che appare accanto a "Toponimo mancante" (es. `Via Po`, `Piazza Castello`).

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona la via dal menu a discesa, oppure spunta ☑ **"Toponimo mancante"** e inseriscila manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il CAP non è stato inserito.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `10122`). Nessuno spazio, nessun trattino.

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il numero civico non è stato inserito.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (es. `15`, `snc`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Non hai inserito almeno un mappale catastale.

**Soluzione**:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione (se presente), Foglio, Mappale e Subalterno (solo fabbricati)
3. Clicca l'**icona ✅ verde** per salvare la riga
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

---

### ATTENZIONE ! Inserire la zona di PRG vigente.

**Dove si trova**: Campo **"Zona PRG vigente"** nella sezione Localizzazione

**Causa**: Non hai inserito la zona del Piano Regolatore Generale vigente in cui ricade l'immobile.

**Soluzione**:
1. Trova il campo **"Zona PRG vigente"** nella sezione localizzazione
2. Inserisci la zona come indicata negli strumenti urbanistici del Comune (es. `Zona A - Centro storico`, `R3`, `Ambito di conservazione A`)
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La zona PRG vigente si ricava dalla cartografia urbanistica comunale o dal certificato di destinazione urbanistica. Per immobili in area UNESCO si tratta quasi sempre di zone di tipo storico-ambientale (Zone A o similari). Puoi trovare questa informazione consultando il SIT (Sistema Informativo Territoriale) del tuo Comune.

---

### ATTENZIONE ! Inserire la zona di PRG adottato.

**Dove si trova**: Campo **"Zona PRG adottato"** nella sezione Localizzazione

**Causa**: Non hai inserito la zona del Piano Regolatore Generale adottato (ovvero il PRG in fase di approvazione o di variante adottata ma non ancora vigente).

**Soluzione**:
1. Trova il campo **"Zona PRG adottato"** accanto al campo Zona PRG vigente
2. Inserisci la zona come indicata nel PRG adottato (es. `A - Centro storico`, `Ambito A1`, `invariata`)
3. Se il PRG adottato coincide con quello vigente o non ci sono varianti in corso, inserisci la stessa zona o la dicitura appropriata
4. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Entrambi i campi Zona PRG (vigente e adottato) sono **sempre obbligatori** indipendentemente dal fatto che il PRG adottato coincida o meno con quello vigente. Se non ci sono varianti in corso, inserisci la stessa zona in entrambi i campi, oppure usa la dicitura "nessuna variante adottata" o "coincidente con PRG vigente".

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**. Tieni premuto **CTRL** per selezionarne più di una.

---

## 3. Zone di localizzazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per la zona (Core/Buffer).

**Dove si trova**: Sezione **"Zone di localizzazione dell'intervento"** → due radio button

**Causa**: Non hai dichiarato se l'immobile si trova nella Core Zone o nella Buffer Zone dell'area UNESCO.

**Soluzione**:
1. Vai alla sezione **"Zone di localizzazione dell'intervento"**
2. Seleziona **una delle due opzioni**:
   - ⚪ **CORE ZONE** — zona centrale del sito UNESCO, soggetta alle tutele più stringenti
   - ⚪ **BUFFER ZONE** — zona tampone di protezione attorno alla Core Zone
3. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Per sapere se il tuo immobile è in Core Zone o Buffer Zone, consulta le mappe del sito UNESCO di riferimento (es. per Torino: le Residenze Sabaude) o il Piano Paesaggistico Regionale del Piemonte. Il Comune può fornire questa informazione tramite il Certificato di Destinazione Urbanistica o il SUE.

---

## 4. Descrizione sintetica dell'intervento

### ATTENZIONE ! Inserire la Descrizione sintetica dell'intervento.

**Dove si trova**: Campo di testo nella sezione **"Descrizione sintetica dell'intervento"**

**Causa**: Non hai inserito la descrizione sintetica delle opere previste.

**Soluzione**:
1. Vai alla sezione **"Descrizione sintetica dell'intervento"**
2. Inserisci una sintesi chiara delle opere da eseguire (max **300 caratteri**)
3. La descrizione deve essere coerente con la relazione tecnica allegata, che contiene il dettaglio completo
4. Esempi:
   - `Restauro e risanamento conservativo della facciata esterna con pulitura e tinteggiatura secondo i colori storici originali.`
   - `Sostituzione infissi esterni con modelli conformi alle NTA del PRG, senza modifica delle aperture esistenti.`
   - `Ristrutturazione interna con eliminazione di tramezze non portanti e rifacimento impianti, senza modifica dell'involucro esterno.`
5. Clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> La descrizione sintetica è distinta dalla relazione tecnica allegata, che deve contenere il dettaglio completo dell'intervento ai fini della valutazione del parere UNESCO. Nella descrizione sintetica è sufficiente indicare la tipologia e l'oggetto principale dell'intervento.

---

## Consigli pratici Zona UNESCO

### Prima di validare ✅

- [ ] Compila il menu a discesa **titolarità** (proprietario, usufruttuario, ecc.)
- [ ] Se hai selezionato "altro": compila il campo **"Specificare se altro"**
- [ ] Seleziona l'**indirizzo** della località (o spunta "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** (fabbricato o terreno)
- [ ] Inserisci la **Zona PRG vigente**
- [ ] Inserisci la **Zona PRG adottato** (entrambi i campi sono obbligatori)
- [ ] Seleziona la **destinazione d'uso**
- [ ] Seleziona la **zona UNESCO** (Core Zone o Buffer Zone)
- [ ] Inserisci la **descrizione sintetica** dell'intervento (max 300 caratteri)
- [ ] **Salva** frequentemente

### Caratteristiche peculiari della pratica UNESCO ⚠️

La pratica Zona UNESCO è una delle più snelle dell'intera piattaforma: non include sezioni tecnici, imprese, sicurezza, contributo di costruzione o qualificazione dell'intervento. I controlli si limitano alla titolarità, alla localizzazione (con i due campi PRG esclusivi di questa pratica), alla zona Core/Buffer e alla descrizione sintetica.

I **due campi Zona PRG** (vigente e adottato) sono esclusivi di questa pratica e non esistono in nessun'altra. Entrambi sono sempre obbligatori.

La **titolarità** ha un meccanismo diverso rispetto alle altre pratiche: non usa radio button ma un solo menu a discesa, con il campo "altro" che si attiva solo per il valore specifico `"altron"`. Non è richiesta la scelta tra titolarità esclusiva e non esclusiva.

La **selezione della zona Core/Buffer** era originariamente implementata con checkbox (visibili nel codice commentato dell'ASCX), poi migrata a radio button mutuamente esclusivi. Il controllo attuale verifica il gruppo `$Zone`.

### Errori frequenti UNESCO 🔍

1. **"altro" selezionato senza specificare** → il campo di testo libero si attiva solo per la voce "altro"; se si seleziona un'altra voce del menu, il campo rimane disabilitato e non è richiesto
2. **Zona PRG adottato vuota** → spesso dimenticata perché si pensa sia opzionale; è invece obbligatoria come quella vigente
3. **Core Zone / Buffer Zone non selezionata** → sezione separata dalla localizzazione, può essere trascurata
4. **Descrizione sintetica troppo generica o vuota** → deve essere sintetica ma significativa ai fini del parere

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
**Fonte**: Analisi codice ValidaDatiUNESCO e DatiUNESCO.ascx
