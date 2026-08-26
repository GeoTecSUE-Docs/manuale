---
title: Errori Procedura Abilitativa Semplificata (P.A.S.) - Tutte le regioni
parent: Errori di validazione
nav_order: 70
description: Errori di validazione per la Procedura Abilitativa Semplificata (PAS) per impianti da fonti rinnovabili - Tutte le regioni (D.Lgs. 190/2024, D.Lgs. 387/2003, art. 12)
keywords: [PAS, procedura abilitativa semplificata, fonti rinnovabili, impianti fotovoltaici, D.Lgs. 190/2024, D.Lgs. 387/2003, Allegato B, nuova costruzione, impianti esistenti, completamento, variante, regolarità urbanistica, data luogo]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9978
IDTarget:
  - { Reg: 2, Prat: 78 }  # Piemonte - P.A.S.
  - { Reg: 1, Prat: 178 }  # Valle d'Aosta - P.A.S.
  - { Reg: 3, Prat: 378 } # Liguria - P.A.S.
  - { Reg: 4, Prat: 478 } # Lombardia - P.A.S.
  - { Reg: 6, Prat: 678 } # Veneto - P.A.S.
  - { Reg: 8, Prat: 878 } # Emilia-Romagna - P.A.S.
  - { Reg: 12, Prat: 1278 } # Lazio - P.A.S.
  - { Reg: 13, Prat: 1378 } # Abruzzo - P.A.S.
  - { Reg: 15, Prat: 1578 } # Campania - P.A.S.
  - { Reg: 16, Prat: 1678 } # Basilicata - P.A.S.
  - { Reg: 17, Prat: 1778 } # Puglia - P.A.S.
  - { Reg: 18, Prat: 1878 } # Calabria - P.A.S.
  - { Reg: 19, Prat: 1978 } # Sicilia - P.A.S.
Fonte: Manuale
---

# Errori di validazione - Procedura Abilitativa Semplificata (P.A.S.)
## Tutte le regioni

Guida completa agli errori specifici per la **Procedura Abilitativa Semplificata (PAS)** per la costruzione, esercizio e modifica di impianti da fonti rinnovabili ai sensi dell'art. 8 del D.Lgs. 25 novembre 2024, n. 190 (Allegato B).

{: .note }
> La PAS è stata **completamente riscritta** con il recepimento del D.Lgs. 190/2024. Rispetto alla versione precedente, la struttura è radicalmente cambiata: la **sezione Titolarità è commentata** e non più presente; il modulo è ora organizzato attorno ai blocchi **RICORRE / COMUNICA / DICHIARA**. La sezione "RICORRE" raccoglie i riferimenti normativi all'Allegato B e all'Allegato A del D.Lgs. 190/2024 (4 campi obbligatori inline nel testo). La sezione "COMUNICA" include: classificazione intervento, dati atto precedente (se intervento su impianto esistente), categoria impianto, potenza risultante, connessione rete elettrica/gas, disponibilità aree opere connesse, atti di assenso (5 checkbox con tipologia e autorità competente), tipologia/classificazione area e — se area agricola — classificazione uso suolo e valore agricolo. Sono **rimosse** le sezioni Presentazione PAS, Territorio, Tipo intervento, Opere parti comuni, Regolarità urbanistica, Comunicazioni contestuali, Atti assenso, Impresa, Sicurezza D.Lgs. 81/2008. Rimane obbligatorio almeno un **Progettista** (`PR`) nei Soggetti coinvolti. Per errori comuni a tutte le pratiche, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Denominazione dell'impianto](#1-denominazione-dellimpianto)
2. [RICORRE — riferimenti normativi Allegato B e Allegato A](#2-ricorre--riferimenti-normativi-allegato-b-e-allegato-a)
3. [COMUNICA — classificazione dell'intervento](#3-comunica--classificazione-dellintervento)
4. [COMUNICA — potenza risultante](#4-comunica--potenza-risultante)
5. [COMUNICA — connessione rete elettrica e gas](#5-comunica--connessione-rete-elettrica-e-gas)
6. [COMUNICA — atti di assenso](#6-comunica--atti-di-assenso)
7. [DICHIARA — piena disponibilità aree opere connesse](#7-dichiara--piena-disponibilità-aree-opere-connesse)
8. [Localizzazione dell'intervento](#8-localizzazione-dellintervento)
9. [Data e luogo](#9-data-e-luogo)
10. [Tecnici incaricati — Progettista](#10-tecnici-incaricati--progettista)

---

## 1. Denominazione dell'impianto

### ATTENZIONE ! Inserire la denominazione dell'impianto.

**Dove si trova**: Sezione **"Denominazione dell'impianto"** in cima al modulo → campo di testo `txtDescrIntervento`

**Causa**: Non hai inserito la denominazione dell'impianto oggetto della PAS.

**Soluzione**: Inserisci la denominazione nel campo di testo (max **300 caratteri**). Esempi:
- `Impianto fotovoltaico a terra "Cascina Nuova" - 2,5 MWp - Comune di Alessandria`
- `Impianto agrivoltaico "Podere Rossi" - potenza 1,8 MWp`
- `Impianto eolico onshore "Monte Vento" - 6 aerogeneratori da 4,5 MW`

{: .note }
> Questo è il **primo controllo** eseguito dalla funzione di validazione: se vuoto, nessun altro errore viene mostrato. Nella versione precedente della PAS il primo controllo era la Titolarità; nella versione attuale la sezione Titolarità è commentata e non presente nel modulo.

---

## 2. RICORRE — riferimenti normativi Allegato B e Allegato A

Il blocco **RICORRE** contiene quattro campi obbligatori inline nel testo del modulo. Si tratta dei riferimenti normativi che qualificano l'intervento ai sensi del D.Lgs. 190/2024.

---

### ATTENZIONE ! Inserire la lettera di cui all'Allegato B sezione I/II.

**Dove si trova**: Blocco **"RICORRE"** → campo `txtRicorre21` inline nel testo "alla procedura abilitativa semplificata ai sensi dell'articolo 8 del decreto legislativo 25 novembre 2024, n. 190, per l'intervento di cui all'**Allegato B sezione I/II lettera** ___"

**Causa**: Non hai indicato la lettera dell'Allegato B (Sezione I o II) del D.Lgs. 190/2024 che qualifica l'intervento soggetto a PAS.

**Soluzione**: Inserisci la lettera nel piccolo campo di testo (es. `a`, `b`, `c`). Consulta l'Allegato B del D.Lgs. 190/2024 per individuare la sezione (I = nuove costruzioni, II = impianti esistenti) e la lettera corrispondente alla tipologia dell'impianto.

---

### ATTENZIONE ! Inserire informazioni relative all'intervento.

**Dove si trova** *(prima occorrenza)*: Campo `txtRicorre23` inline nel testo "relativo a ___"

**Causa**: Non hai inserito la descrizione dell'intervento a cui si riferisce la lettera dell'Allegato B.

**Soluzione**: Inserisci nel campo `txtRicorre23` una descrizione sintetica dell'intervento (es. `impianto fotovoltaico a terra da 2,5 MWp`, `impianto eolico da 27 MW`).

{: .note }
> Il messaggio "Inserire informazioni relative all'intervento" compare per **due campi distinti**: `txtRicorre23` (riferito all'Allegato B) e `txtRicorre25` (riferito all'Allegato A). Entrambi hanno lo stesso messaggio ma si trovano in punti diversi del blocco RICORRE. Se il messaggio compare inaspettatamente dopo aver già compilato il primo campo, verifica il secondo più in basso.

---

### ATTENZIONE ! Inserire la lettera/e di cui all'Allegato A sezione I/II.

**Dove si trova**: Campo `txtRicorre24` inline nel testo "ai sensi dell'articolo 7, comma 8, per l'intervento di cui all'**allegato A sezione I/II lettera/e** ___"

**Causa**: Non hai indicato la lettera (o le lettere) dell'Allegato A (Sezione I o II) del D.Lgs. 190/2024.

**Soluzione**: Inserisci la lettera o le lettere nel campo `txtRicorre24`. L'Allegato A del D.Lgs. 190/2024 classifica le attività in regime di comunicazione (art. 7, c. 8).

---

### ATTENZIONE ! Inserire informazioni relative all'intervento.

**Dove si trova** *(seconda occorrenza)*: Campo `txtRicorre25` inline nel testo "relativo a ___"

**Causa**: Non hai inserito la descrizione dell'intervento a cui si riferisce la lettera dell'Allegato A.

**Soluzione**: Inserisci nel campo `txtRicorre25` la descrizione dell'intervento ai sensi dell'Allegato A.

---

## 3. COMUNICA — classificazione dell'intervento

### ATTENZIONE ! Non è stata selezionata nessuna voce per la classificazione dell'intervento.

**Dove si trova**: Blocco **"COMUNICA"** → radio button `$ClassificazioneIntervento`

**Causa**: Non hai selezionato se si tratta di un intervento di nuova costruzione o su impianto esistente.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **"intervento di nuova costruzione"** → nessun campo aggiuntivo obbligatorio in questa sottosezione
- ⚪ **"intervento su impianto già abilitato/autorizzato con atto ___ del ___"** → si attivano: numero atto, data atto e categoria impianto

---

### ATTENZIONE ! Inserire numero atto dell'impianto già abilitato/autorizzato.

**Causa**: Hai selezionato *intervento su impianto esistente* ma non hai inserito il numero dell'atto abilitativo originario.

**Soluzione**: Inserisci il numero dell'atto (es. numero PAS, numero autorizzazione unica) nel campo accanto a **"con atto"**.

---

### ATTENZIONE ! Inserire data atto dell'impianto già abilitato/autorizzato.

**Causa**: Hai selezionato *intervento su impianto esistente* e inserito il numero atto, ma il campo data è vuoto.

**Soluzione**: Inserisci la data dell'atto nel campo **"del"** nel formato **GG/MM/AAAA**. Puoi usare l'icona calendario.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. *(data atto)*

**Causa**: La data dell'atto abilitativo è in un formato non valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `10/06/2022` ✅, `10-06-2022` ❌).

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per la categoria dell'impianto.

**Causa**: Hai selezionato *intervento su impianto esistente* ma non hai indicato la categoria dell'impianto.

**Soluzione**: Seleziona **una delle quattro categorie** che si attivano sotto il bottone:
- ⚪ "impianto esistente"
- ⚪ "impianto per il quale è stata avviata la realizzazione"
- ⚪ "impianto per il quale non è stata avviata la realizzazione, con titolo abilitativo in corso di validità"
- ⚪ "impianto per il quale non è stata avviata la realizzazione, con titolo abilitativo scaduto"

---

## 4. COMUNICA — potenza risultante

### ATTENZIONE ! Non è stata selezionata nessuna voce relativa alla potenza elettrica /potenza termica /capacità produttiva /capacità di accumulo risultante dall'intervento.

**Dove si trova**: Blocco **"COMUNICA"** → radio button `$PotenzaRisultante`

**Causa**: Non hai dichiarato la potenza o capacità risultante dall'intervento.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ "che la potenza elettrica / potenza termica / capacità produttiva / capacità di accumulo risultante dall'intervento è pari a ___" → inserisci il valore nel campo
- ⚪ "che la potenza elettrica / potenza termica / capacità produttiva / capacità di accumulo risultante dall'intervento nel caso di varianti è pari a ___" → inserisci il valore nel campo

---

### ATTENZIONE ! Indicare la potenza elettrica /potenza termica /capacità produttiva /capacità di accumulo risultante dall'intervento.

**Causa**: Hai selezionato *che la potenza elettrica / potenza termica / capacità produttiva / capacità di accumulo risultante dall'intervento è pari a ___* ma il campo relativo è vuoto.

**Soluzione**: Inserisci il valore della potenza o capacità nel campo che si attiva accanto al radio button (es. `2,5 MWp`, `27 MW`, `1,8 MWt`, `50 MWh`).

---

### ATTENZIONE ! Indicare la potenza elettrica /potenza termica /capacità produttiva /capacità di accumulo risultante dall'intervento nel caso di varianti.

**Causa**: Hai selezionato *che la potenza elettrica / potenza termica / capacità produttiva / capacità di accumulo risultante dall'intervento nel caso di varianti è pari a ___* ma il campo relativo è vuoto.

**Soluzione**: Inserisci il valore della potenza risultante dalla variante nel campo che si attiva accanto al radio button.

---

## 5. COMUNICA — connessione rete elettrica e gas

### ATTENZIONE ! Indicare se condivide il punto di connessione con un altro impianto (si/no).

**Dove si trova**: Blocco **"COMUNICA"**

**Causa**: Non hai dichiarato se l'impianto condivide il punto di connessione alla rete con un altro impianto.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — l'impianto condivide il punto di connessione con un altro impianto
- ⚪ **no** — l'impianto ha un punto di connessione dedicato

---

### ATTENZIONE ! Indicare se prevede interventi di connessione alla rete elettrica (si/no).

**Dove si trova**: Blocco **"COMUNICA"**

**Causa**: Non hai dichiarato se la PAS comprende interventi di connessione alla rete elettrica.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — la PAS include interventi di connessione alla rete elettrica
- ⚪ **no** — non sono previsti interventi di connessione alla rete elettrica

---

### ATTENZIONE ! Indicare se prevede interventi di connessione alla rete gas (si/no).

**Dove si trova**: Blocco **"COMUNICA"**

**Causa**: Non hai dichiarato se la PAS comprende interventi di connessione alla rete gas.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — la PAS include interventi di connessione alla rete gas
- ⚪ **no** — non sono previsti interventi di connessione alla rete gas

{: .note }
> I tre radio button (condivisione punto connessione, connessione rete elettrica, connessione rete gas) sono verificati in sequenza e richiedono tutti una risposta sì/no. Non sono previsti campi aggiuntivi condizionali: la selezione sì/no è sufficiente per ciascuno.

---

## 6. COMUNICA — atti di assenso

Il blocco **"COMUNICA"** include fino a 5 righe di atti di assenso. Per ogni checkbox spuntata diventano obbligatori i due campi della stessa riga.

---

### ATTENZIONE ! Inserire tipologia atto.

**Causa**: Hai spuntato una delle 5 checkbox degli atti di assenso ma non hai compilato il campo **"Tipologia atto"** della riga corrispondente.

**Soluzione**: Per ogni checkbox spuntata, inserisci la tipologia dell'atto di assenso nel campo di testo corrispondente (es. `Autorizzazione paesaggistica`, `Parere Soprintendenza`, `Nulla osta Ente Parco`, `Valutazione di incidenza`).

---

### ATTENZIONE ! Inserire autorità competente.

**Causa**: Hai spuntato una checkbox e compilato la tipologia atto, ma hai lasciato vuoto il campo **"Autorità competente"** della stessa riga.

**Soluzione**: Inserisci l'autorità competente al rilascio dell'atto nella stessa riga della tipologia (es. `Soprintendenza ABAP`, `Regione Lombardia`, `Ente Parco Nazionale`, `Comune di ___`).

{: .note }
> La validazione scorre tutte e 5 le righe nell'ordine 1→5. Per ogni riga spuntata verifica prima la tipologia poi l'autorità competente, poi passa alla riga successiva. Le righe non spuntate vengono saltate interamente.

---

## 7. DICHIARA — piena disponibilità aree opere connesse

### ATTENZIONE ! Indicare se si ha piena disponibilità delle aree interessate dalle opere connesse (si/no).

**Dove si trova**: Blocco **"DICHIARA"** → radio button accanto a "di avere la piena disponibilità delle aree interessate dalle opere connesse"

**Causa**: Non hai dichiarato se hai la piena disponibilità delle aree interessate dalle **opere connesse** all'impianto.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **sì** — hai la piena disponibilità delle aree delle opere connesse
- ⚪ **no** — non hai ancora la piena disponibilità

{: .note }
> Nel form è presente anche la dichiarazione fissa (non radio button) "di avere la piena disponibilità delle aree interessate dall'**impianto**" — questa è una dichiarazione testuale e non genera errori di validazione. Il controllo riguarda esclusivamente la piena disponibilità delle aree delle **opere connesse** (cablaggi, cabine di trasformazione, linee di connessione), che viene validata con radio sì/no.

---

## 8. Localizzazione dell'intervento

### ATTENZIONE ! Inserire indirizzo della località di intervento.

**Causa**: "Toponimo mancante" spuntato ma campo indirizzo libero non compilato.

**Soluzione**: Compila il campo di testo che si attiva accanto alla checkbox "Toponimo mancante".

---

### ATTENZIONE ! Selezionare l'indirizzo della località di intervento.

**Causa**: Nessun indirizzo selezionato dal menu a discesa e "Toponimo mancante" non spuntato.

**Soluzione**: Seleziona un indirizzo dal menu a discesa oppure spunta ☑ **"Toponimo mancante"** e inseriscilo manualmente.

---

### ATTENZIONE ! Inserire CAP della località di intervento.

**Causa**: Il campo CAP è vuoto.

**Soluzione**: Inserisci esattamente **5 cifre** nel campo **"CAP"** (es. `15100`).

{: .warning }
> **CRITICO**: CAP errato o mancante blocca la generazione IUV PagoPA!

---

### ATTENZIONE ! Inserire numero civico della località di intervento.

**Causa**: Il campo numero civico è vuoto.

**Soluzione**: Inserisci il numero civico nel campo **"N. Civico"** (per impianti in area agricola o aperta campagna è accettato anche un riferimento come `s.n.c.` o `snc`).

---

### ATTENZIONE ! Non è stata selezionato nessun mappale per i fabbricati e i terreni.

**Causa**: Nessun mappale catastale inserito né nella sezione Fabbricati né nella sezione Terreni.

**Soluzione**: Aggiungi almeno un fabbricato o un terreno:
1. Clicca **"Aggiungi Fabbricato"** oppure **"Aggiungi Terreno"**
2. Compila Sezione, Foglio, Mappale (e Subalterno per i fabbricati)
3. Salva con l'icona ✅

---

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Destinazione d'Uso'.

**Causa**: Nessuna destinazione d'uso selezionata.

**Soluzione**: Seleziona almeno una voce dal campo **"Avente destinazione d'uso (CTRL + click per selezionare più voci)"**.

---

## 9. Data e luogo

### ATTENZIONE ! Inserire la data.

**Dove si trova**: Riquadro in fondo al modulo

**Causa**: Il campo data di sottoscrizione è vuoto.

**Soluzione**: Inserisci la data nel formato **GG/MM/AAAA**. Puoi usare l'icona calendario.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa.

**Causa**: La data è presente ma in formato non valido.

**Soluzione**: Riscrivi nel formato **GG/MM/AAAA** (es. `20/07/2026` ✅, `20-07-2026` ❌).

---

### ATTENZIONE ! Inserire il luogo.

**Dove si trova**: Campo accanto al campo data

**Causa**: Il campo luogo di sottoscrizione è vuoto.

**Soluzione**: Inserisci il Comune in cui viene sottoscritta la PAS.

{: .warning }
> Come nella versione precedente, la PAS è tra le poche pratiche del sistema in cui sia **data** (con verifica formato) sia **luogo** sono obbligatori e validati. Non dimenticarli: sono gli ultimi due controlli prima della verifica del Progettista.

---

## 10. Tecnici incaricati — Progettista

### ATTENZIONE ! Non è stato selezionato nessun Tecnico come Progettista.

**Dove si trova**: Sezione **"Tecnici incaricati"** + scheda **"Soggetti coinvolti"** → tecnici

**Causa**: Nessun tecnico con ruolo **Progettista** (codice `PR`) nei soggetti coinvolti.

**Soluzione**:
1. Vai alla scheda **"Soggetti coinvolti"** → sezione **"Tecnici"**
2. Clicca **"Aggiungi Tecnico"**
3. Seleziona il ruolo **"Progettista"**
4. Compila i dati e salva
5. Torna al modulo PAS, clicca **"Salva"** e riprova **"Valida e Salva"**

{: .note }
> Il Progettista è l'**unico tecnico validato** nella nuova PAS. A differenza della versione precedente, non sono validati altri ruoli tecnici. Il controllo è l'**ultimo** eseguito dalla funzione: tutti gli altri errori devono essere corretti prima che questo compaia.

---

## Consigli pratici PAS

### Prima di validare ✅

- [ ] Inserisci la **denominazione dell'impianto** (max 300 caratteri)
- [ ] Nella sezione **RICORRE**: inserisci la **lettera Allegato B** (`txtRicorre21`)
- [ ] Nella sezione **RICORRE**: inserisci la **descrizione intervento Allegato B** (`txtRicorre23`)
- [ ] Nella sezione **RICORRE**: inserisci la **lettera/e Allegato A** (`txtRicorre24`)
- [ ] Nella sezione **RICORRE**: inserisci la **descrizione intervento Allegato A** (`txtRicorre25`)
- [ ] Nella sezione **COMUNICA**: seleziona la **classificazione intervento** (nuova costruzione o su impianto esistente)
- [ ] **Se impianto esistente**: inserisci **numero atto** + **data atto** (GG/MM/AAAA) + seleziona **categoria impianto**
- [ ] Seleziona la **potenza risultante** e inserisci il **valore**
- [ ] Dichiara se **condivide il punto di connessione** (sì/no)
- [ ] Dichiara se prevede **connessione rete elettrica** (sì/no)
- [ ] Dichiara se prevede **connessione rete gas** (sì/no)
- [ ] Per ogni **atto di assenso** spuntato: inserisci **tipologia** e **autorità competente**
- [ ] Dichiara la **piena disponibilità aree opere connesse** (sì/no)
- [ ] Seleziona l'**indirizzo** (menu a discesa o "Toponimo mancante")
- [ ] Inserisci il **CAP** (5 cifre esatte)
- [ ] Inserisci il **numero civico**
- [ ] Aggiungi almeno un **mappale** e salvalo con ✅
- [ ] Seleziona la **destinazione d'uso**
- [ ] Inserisci la **data** (GG/MM/AAAA)
- [ ] Inserisci il **luogo**
- [ ] Aggiungi il **Progettista** nei Soggetti coinvolti
- [ ] **Salva** frequentemente

### Errori frequenti PAS 🔍

1. **Quattro campi RICORRE inline** → sono integrati nel testo del modulo e visivamente poco evidenti; verificarli tutti e quattro prima di validare
2. **Messaggio "informazioni intervento" doppio** → compare sia per Allegato B sia per Allegato A; se il messaggio compare una seconda volta, compilare il secondo campo più in basso
3. **Intervento su impianto esistente** → la selezione di *"intervento su impianto già abilitato/autorizzato con atto ___ del ___"* attiva tre controlli in cascata (numero atto, data atto, categoria): compilarli tutti prima di validare
4. **Disponibilità aree connesse vs aree impianto** → la dichiarazione fissa sull'impianto non è validata; il radio button riguarda esclusivamente le aree delle **opere connesse**
5. **Data e Luogo** → posizionati in fondo al modulo, compaiono come errore solo dopo che tutti i controlli precedenti sono superati; inserirli prima di validare

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

**Ultima revisione**: Agosto 2026
**Fonte**: Analisi codice `ValidaDatiPAS` e `DatiPAS.ascx`
