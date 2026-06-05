---
title: Errori Segnalazione Certificata di Agibilità - Tutte le regioni (Nazionale)
parent: Errori di validazione
nav_order: 52
description: Errori di validazione specifici per la Segnalazione Certificata di Agibilità Nazionale - Tutte le regioni (art. 24 D.P.R. 380/2001)
keywords: [segnalazione certificata agibilità, SCA, agibilità, nazionale, tutte le regioni, art. 24 DPR 380/2001, titolo edilizio, fine lavori, tecnico agibilità, TA, direttore lavori, SCIA agibilità]
IDRegione: 99        # Fallback (Nazionale)
IDTipoPratica: 9999  # Fallback (Generico)
IDTarget:
  - { Reg: 1, Prat: 112 }  # Valle d'Aosta - SCA
  - { Reg: 6, Prat: 612 } # Veneto - SCA
  - { Reg: 8, Prat: 812 } # Emilia-Romagna - SCA
  - { Reg: 12, Prat: 1212 } # Lazio - SCA
  - { Reg: 13, Prat: 1312 } # Abruzzo - SCA
  - { Reg: 15, Prat: 1512 } # Campania - SCA
  - { Reg: 16, Prat: 1612 } # Basilicata - SCA
  - { Reg: 17, Prat: 1712 } # Puglia - SCA
  - { Reg: 18, Prat: 1812 } # Calabria - SCA
  - { Reg: 19, Prat: 1912 } # Sicilia - SCA
Fonte: Manuale
---

# Errori di validazione - Segnalazione Certificata di Agibilità
## Tutte le regioni (Nazionale)

Guida completa agli errori specifici per la **Segnalazione Certificata di Agibilità (SCA) Nazionale** ai sensi dell'art. 24 del D.P.R. 380/2001, applicabile su tutto il territorio nazionale (escluse le regioni con modulo specifico come la Liguria).

{: .note }
> La SCA Nazionale ha una struttura simile alla [SCA Liguria](errori-sca-liguria.html) ma con alcune differenze importanti. Il titolo edilizio usa lo stesso **doppio binario** (esterno a GeoTecSUE vs interno a GeoTecSUE), ma la data del titolo esterno viene qui verificata nel **formato GG/MM/AAAA** (diverso dalla Liguria). La sezione **fine lavori** usa radio button invece di una checkbox, con la seconda opzione che apre una data e un radio tipo ultimazione. La **privacy** richiede la checkbox `chkPrivacy` (presente come nell'SCA Liguria, assente nella SCA Lombardia). Per i tecnici è richiesto un ruolo **TA o DR** come nella versione ligure. Per errori comuni, vedi [Errori Comuni](errori-validazione.html#errori-comuni).

---

## Indice sezioni

1. [Localizzazione dell'intervento](#1-localizzazione-dellintervento)
2. [Titolo edilizio di riferimento](#2-titolo-edilizio-di-riferimento)
3. [Dichiarazioni per fine lavori](#3-dichiarazioni-per-fine-lavori)
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
> Il campo "Coordinate" (`txtCoordinate`) è presente nel modulo come campo testo libero ma **non viene validato** — non genera errori se vuoto.

---

## 2. Titolo edilizio di riferimento

La sezione del titolo edilizio ha un **doppio binario**: titolo esterno a GeoTecSUE (immesso manualmente) oppure già presente su GeoTecSUE. Almeno uno deve essere compilato.

---

### ATTENZIONE ! Selezionare il titolo abitativo edilizio.

**Causa**: Entrambi i menu del titolo edilizio (`cmbTitoliAbitEdilizi` e `cmbTitoliAbitEdilizi1`) sono rimasti sull'opzione vuota.

**Soluzione**: Compila **almeno uno** dei due percorsi:

**Percorso 1 — Titolo esterno (non su GeoTecSUE):** seleziona il tipo dal primo menu (`cmbTitoliAbitEdilizi`), poi compila il numero e la data nel formato **GG/MM/AAAA**.

**Percorso 2 — Titolo su GeoTecSUE:** seleziona il tipo dal menu `cmbTitoliAbitEdilizi1`, poi seleziona la pratica specifica dal menu `cmbTitoloRif1` che si abilita.

---

### ATTENZIONE ! Selezionare il riferimento della pratica.

**Causa**: Hai selezionato un tipo nel menu `cmbTitoliAbitEdilizi1` ma non hai scelto la pratica specifica da `cmbTitoloRif1`.

**Soluzione**: Seleziona la pratica corrispondente dal menu `cmbTitoloRif1`.

---

### ATTENZIONE ! Inserire il numero.

**Causa**: Hai selezionato un tipo nel percorso esterno ma non hai compilato il campo "prot. / n."

**Soluzione**: Inserisci il numero di protocollo o numero del titolo nel campo "prot. / n."

---

### ATTENZIONE ! Inserire la data.

**Causa**: Hai selezionato il tipo nel percorso esterno e il campo data è vuoto.

**Soluzione**: Inserisci la data nel campo "del" nel formato **GG/MM/AAAA**.

---

### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (titolo edilizio)

**Causa**: La data del titolo edilizio esterno non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA** (es. `15/03/2022`).

{: .note }
> A differenza della [SCA Liguria](errori-sca-liguria.html), la SCA Nazionale **verifica il formato della data** del titolo edilizio esterno tramite `ControlloFormatoData`. I titoli aggiuntivi su GeoTecSUE (cmbTitoliAbitEdilizi2..5 con relativi riferimenti e campi) non vengono validati — sono opzionali.

---

## 3. Dichiarazioni per fine lavori

### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Dichiarazioni per fine lavori'.

**Dove si trova**: Sezione "DICHIARA" → 2 radio button relativi alla comunicazione di fine lavori

**Causa**: Nessuno dei 2 radio button è selezionato.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbComunicazFLa_1** — "che la comunicazione di fine lavori è stata già presentata prot. / n. ___ del ___" → compila n. e data fine lavori già presentata
- ⚪ **rdbComunicazFLa_2** — "che la presente segnalazione vale come comunicazione di fine lavori e a tal fine attesta che gli stessi sono stati ultimati in data ___" → compila data ultimazione e tipo ultimazione

{: .note }
> A differenza della [SCA Liguria](errori-sca-liguria.html) che usa una **checkbox** opzionale per la fine lavori, la SCA Nazionale usa **radio button** obbligatori: è necessario indicare obbligatoriamente se la fine lavori è già stata presentata separatamente o se viene presentata contestualmente all'agibilità.

---

### Opzione rdbComunicazFLa_1 — Fine lavori già presentata

#### ATTENZIONE ! Inserire il prot. / n. di pratica.

**Causa**: Hai selezionato rdb1 ma non hai inserito il numero della comunicazione di fine lavori già presentata.

**Soluzione**: Inserisci il numero di protocollo/pratica della comunicazione di fine lavori nel campo "prot. / n."

---

#### ATTENZIONE ! Campo obbligatorio 'Data pratica' non inserito.

**Causa**: Hai compilato il numero ma la data della fine lavori già presentata è vuota.

**Soluzione**: Inserisci la data nel campo "del" nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data fine lavori già presentata)

**Causa**: La data inserita non rispetta il formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

### Opzione rdbComunicazFLa_2 — Fine lavori contestuale

#### ATTENZIONE ! Campo obbligatorio 'Data fine lavori' non inserito.

**Causa**: Hai selezionato rdb2 ("la presente segnalazione vale come comunicazione di fine lavori") ma non hai compilato il campo della data di ultimazione lavori.

**Soluzione**: Inserisci la data in cui i lavori sono stati ultimati nel campo affiancato, nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Inserire la data nel formato gg/mm/aaaa. (data ultimazione lavori)

**Causa**: La data di ultimazione lavori non è nel formato corretto.

**Soluzione**: Correggi nel formato **GG/MM/AAAA**.

---

#### ATTENZIONE ! Non è stata selezionata nessuna voce per 'Tipo ultimazione lavori'.

**Causa**: Hai compilato la data di ultimazione ma non hai indicato se i lavori sono stati ultimati completamente o parzialmente.

**Soluzione**: Seleziona **uno dei due radio button**:
- ⚪ **rdbTipoUltimazionea_2_1** — "completamente"
- ⚪ **rdbTipoUltimazionea_2_2** — "in forma parziale come da planimetria allegata"

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
- ⚪ **rdbPresenta4** — "l'agibilità relativa all'immobile oggetto dell'intervento edilizio"
- ⚪ **rdbPresenta5** — "l'agibilità parziale relativa a singoli edifici o a singole porzioni della costruzione (art. 24, comma 4, lett. a)...)"
- ⚪ **rdbPresenta6** — "l'agibilità parziale relativa a singole unità immobiliari (art. 24, comma 4, lett. b)...)"

---

## 5. Privacy

### ATTENZIONE ! Selezionare la presa visione dell'informativa sul trattamento dei dati personali.

**Dove si trova**: Sezione "Informativa sulla privacy" → checkbox `chkPrivacy` incorporata nel testo dell'informativa GDPR in fondo al modulo

**Causa**: Non hai spuntato la dichiarazione di aver letto l'informativa.

**Soluzione**: Scorri fino alla sezione "Informativa sulla privacy" e spunta la checkbox `chkPrivacy` — "Il/la sottoscritto/a dichiara di aver letto l'informativa sul trattamento dei dati personali pubblicata sul sito istituzionale del SUAP/SUE".

{: .note }
> L'informativa citata fa riferimento al **Reg. UE n. 2016/679 del 27 aprile 2016** (GDPR). La checkbox è incorporata all'interno del lungo testo dell'informativa e può essere difficile da individuare visivamente senza scorrere fino in fondo alla sezione.

---

## 6. Tecnici nei soggetti coinvolti

### ATTENZIONE ! Non è stato selezionato nessun Professionista incaricato per Agibilità o come Direttore Lavori.

**Causa**: Nessun tecnico con ruolo **TA** (Professionista Incaricato Agibilità) o **DR** (Direttore Lavori) è presente tra i soggetti coinvolti.

**Soluzione**: Vai a **"Soggetti coinvolti"** → **"Tecnici"** → aggiungi almeno un tecnico con uno dei due ruoli:
- **TA — Professionista Incaricato Agibilità**: il tecnico abilitato che certifica la conformità dell'immobile
- **DR — Direttore Lavori**: il direttore dei lavori delle opere architettoniche

---

## Consigli pratici — SCA Nazionale

### Prima di validare ✅

- [ ] Seleziona **indirizzo**, inserisci **CAP** e **civico**
- [ ] Aggiungi almeno un **mappale**
- [ ] Seleziona la **destinazione d'uso**
- [ ] Compila il **titolo edilizio**: percorso esterno (menu + n. + data **GG/MM/AAAA** — formato verificato) **oppure** percorso GeoTecSUE (menu tipo + menu riferimento pratica)
- [ ] Seleziona il **radio fine lavori** (già presentata con n.+data / contestuale con data ultimazione e tipo completamento)
- [ ] Seleziona uno dei 6 **radio presentazione agibilità** (SCIA o SCIA Unica, totale o parziale)
- [ ] Spunta **chkPrivacy**
- [ ] Aggiungi nei soggetti almeno un tecnico con ruolo **TA** o **DR**

### Differenze SCA Nazionale vs SCA Liguria

Le differenze principali sono tre. La data del titolo edilizio esterno viene **verificata nel formato** GG/MM/AAAA nella Nazionale (non nella Liguria). La fine lavori usa **radio button obbligatori** (non una checkbox opzionale): è obbligatorio indicare se la fine lavori è già stata presentata o viene presentata contestualmente. Se si sceglie l'opzione "contestuale", bisogna anche selezionare il tipo di ultimazione (completa/parziale) — un livello in più rispetto alla Liguria.

### Errori frequenti 🔍

1. **Data titolo esterno non nel formato GG/MM/AAAA** → a differenza della SCA Liguria, qui il formato viene verificato; inserire es. `2022` o `marzo 2022` genera l'errore di formato
2. **Nessun radio fine lavori selezionato** → i due radio button sono obbligatori; non è sufficiente non selezionarne nessuno come nella versione Liguria con la checkbox opzionale
3. **Radio rdb2 senza tipo ultimazione** → dopo aver inserito la data di ultimazione, bisogna anche indicare se la fine lavori è completa o parziale; dimenticare il secondo radio genera un errore separato
4. **Privacy non spuntata** → la checkbox è in fondo al lungo testo del GDPR; scorrere fino alla fine prima di validare
5. **Tecnico TA/DR assente** → come nella Liguria, la SCA Nazionale richiede specificamente uno di questi due ruoli; verificare il ruolo assegnato ai tecnici nei soggetti

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
**Fonte**: Analisi codice ValidaDatiSCANazionale e DatiSCANaz.ascx
