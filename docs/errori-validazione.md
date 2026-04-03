---
title: Errori di validazione
nav_order: 25
parent: Le mie istanze
description: Guida agli errori di validazione - processo di validazione ed errori comuni
keywords: [errori, validazione, campo obbligatorio, errore compilazione]
has_children: true
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Errori di validazione

Guida completa agli errori che possono apparire durante la **validazione** di una pratica.

---

## Come funziona la validazione

### Quando validare

La **validazione** è l'ultimo passaggio prima della firma e dell'invio della pratica all'Ente. Serve a verificare che:
- Tutti i **campi obbligatori** siano compilati
- I **dati** siano nel **formato corretto**
- Gli **allegati richiesti** siano stati caricati
- I **pagamenti** (se previsti) siano stati effettuati

### Pulsante "Valida e Salva"

Trovi il pulsante **"Valida e Salva"** in fondo alla pratica, dopo aver compilato tutte le sezioni.

Quando clicchi:
1. Il sistema **controlla** tutti i dati
2. Se trova **errori**, appare un **messaggio rosso** in cima alla pagina relativo al primo errore che viene individuato. Il sistema posiziona il cursore nel punto esatto in cui è presente l'errore
3. La pratica **NON** viene salvata finché non correggi tutti gli errori
4. Se **tutto OK**, la pratica viene salvata e puoi procedere all'invio

---

## Come leggere i messaggi di errore

### Formato tipico

I messaggi di errore iniziano sempre con **"ATTENZIONE !"** e descrivono cosa manca o cosa è sbagliato:

```
ATTENZIONE ! Codice Fiscale del Titolare non inserito.
```

```
ATTENZIONE ! CAP di residenza del Titolare non valido.
```

### Dove appare

Il messaggio di errore appare:
- In cima alla pagina (in rosso)

### Cosa fare

1. **Leggi attentamente** il messaggio
2. **Identifica** la sezione e il campo indicati
3. **Cerca** il messaggio in questa guida (Ctrl+F)
4. **Segui** la soluzione passo-passo
5. **Riprova** la validazione

---

## Tipi di errori

### 1. Errori comuni (tutte le pratiche)

Questi errori possono apparire in **qualsiasi tipo di pratica**:
- Dati anagrafici Titolare
- Dati Professionista
- Codice Fiscale, Partita IVA
- Email, CAP
- Date

👉 Vedi la sezione [Errori Comuni](#errori-comuni) qui sotto.

### 2. Errori specifici per pratica

Ogni tipo di pratica ha validazioni specifiche: nei prossimi rilasci del manuale ci saranno sezioni apposite.

---

## Errori Comuni

Questi errori possono apparire in **qualsiasi tipo di pratica**. Sono controlli di base sui dati anagrafici e documenti.

**Totale errori comuni**: 43

### ATTENZIONE ! CAP di residenza del Professionista non inserito.

**Causa**: Il CAP è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **CAP**
2. Inserisci il CAP
3. Riprova **"Valida e Salva"**

{: .warning }
> **IMPORTANTE**: CAP errato è una delle cause principali del blocco IUV PagoPA! Se lo IUV non si genera, verifica il CAP.

---

### ATTENZIONE ! CAP di residenza del Professionista non valido.

**Causa**: Il CAP non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **CAP**
2. **NO** 4 cifre (es. `0121` → SBAGLIATO)
3. **NO** spazi (es. `10121 ` → SBAGLIATO)
4. Esempio corretto: `10121` ✅
5. Riprova **"Valida e Salva"**

{: .warning }
> **IMPORTANTE**: CAP errato è una delle cause principali del blocco IUV PagoPA! Se lo IUV non si genera, verifica il CAP.

{: .warning }
> **IMPORTANTE**: il CAP è sempre riferito ad un codice nazionale italiano. Se si deve inserire un CAP estero, è necessario che tale valore sia di 5 cifre.
Se ad esempio il CAP è di sole 3 cifre, si può fare un'aggiunta di due zeri iniziali per portarlo a 5 cifre. Oppure si può inserire un CAP del tipo "00000"

---

### ATTENZIONE ! CAP di residenza del Titolare non inserito.

**Causa**: Il CAP è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **CAP**
2. Inserisci il CAP
3. Riprova **"Valida e Salva"**

{: .warning }
> **IMPORTANTE**: CAP errato è una delle cause principali del blocco IUV PagoPA! Se lo IUV non si genera, verifica il CAP.

---

### ATTENZIONE ! CAP di residenza del Titolare non valido.

**Causa**: Il CAP non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **CAP**
2. **NO** 4 cifre (es. `0121` → SBAGLIATO)
3. **NO** spazi (es. `10121 ` → SBAGLIATO)
4. Esempio corretto: `10121` ✅
5. Riprova **"Valida e Salva"**

{: .warning }
> **IMPORTANTE**: CAP errato è una delle cause principali del blocco IUV PagoPA! Se lo IUV non si genera, verifica il CAP.

{: .warning }
> **IMPORTANTE**: il CAP è sempre riferito ad un codice nazionale italiano. Se si deve inserire un CAP estero, è necessario che tale valore sia di 5 cifre.
Se ad esempio il CAP è di sole 3 cifre, si può fare un'aggiunta di due zeri iniziali per portarlo a 5 cifre. Oppure si può inserire un CAP del tipo "00000"

---

### ATTENZIONE ! Campo obbligatorio non inserito.

**Causa**: Campo obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DELLA DITTA/SOCIETA'/ENTE/ALTRO** o nella sezione **DATI DEL PROCURATORE / DELEGATO** in un campo mancante
2. Compila o correggi il dato richiesto
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Città di residenza del Professionista non inserita.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Città**
2. Compila il campo richiesto
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Città di residenza del Titolare non inserita.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Residente in**
2. Compila il campo richiesto
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale del Procuratore/Delegato non valido.

**Causa**: Il Codice Fiscale non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL PROCURATORE / DELEGATO** all'interno del campo **Codice Fiscale**
2. Verifica che il CF sia di **16 caratteri** esatti
3. Usa solo lettere e numeri
4. **Nessuno spazio** o carattere speciale
5. Esempio corretto: `RSSMRA80A01H501U`
6. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale del Professionista non inserito.

**Causa**: Il Codice Fiscale è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Codice Fiscale**
2. Inserisci il Codice Fiscale completo
3. Formato: **16 caratteri** alfanumerici
4. Esempio corretto: `RSSMRA80A01H501U`
5. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
6. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale del Professionista non valido.

**Causa**: Il Codice Fiscale non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Codice Fiscale**
2. Verifica che il CF sia di **16 caratteri** esatti
3. Usa solo lettere e numeri
4. **Nessuno spazio** o carattere speciale
5. Esempio corretto: `RSSMRA80A01H501U`
6. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale del Titolare non inserito.

**Causa**: Il Codice Fiscale è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Titolare** all'interno del campo **Codice Fiscale**
2. Inserisci il Codice Fiscale completo
3. Formato: **16 caratteri** alfanumerici
4. Esempio corretto: `RSSMRA80A01H501U`
5. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
6. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale del Titolare non valido.

**Causa**: Il Codice Fiscale non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Titolare** all'interno del campo **Codice Fiscale**
2. Verifica che il CF sia di **16 caratteri** esatti
3. Usa solo lettere e numeri
4. **Nessuno spazio** o carattere speciale
5. Esempio corretto: `RSSMRA80A01H501U`
6. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Codice Fiscale della Ditta/Società/Ente non valido.

**Causa**: Il Codice Fiscale non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DELLA DITTA/SOCIETA'/ENTE/ALTRO** all'interno del campo **Codice Fiscale**
2. Verifica che il CF sia di **16 caratteri** esatti
3. Usa solo lettere e numeri
4. **Nessuno spazio** o carattere speciale
5. Esempio corretto: `RSSMRA80A01H501U`
6. Verifica su [calcolatore CF](https://www.codicefiscale.com/)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Cognome del Professionista non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Cognome**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Cognome del Titolare non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Cognome**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Comune di nascita del Professionista non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Comune Nascita**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Comune di nascita del Titolare non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Titolare** all'interno del campo **Nato a**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Data di Nascita del Professionista non inserita.

**Causa**: La data è obbligatoria ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Data Nascita**
2. Inserisci la data richiesta (nel formato GG/MM/AAAA) oppure usa il calendario
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Data di Nascita del Titolare non inserita.

**Causa**: La data è obbligatoria ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Nato il**
2. Inserisci la data richiesta (nel formato GG/MM/AAAA) oppure usa il calendario
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Data di nascita del Professionista non valida (gg/mm/aaaa).

**Causa**: La data è nel formato sbagliato.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Data Nascita**
2. Usa il formato **GG/MM/AAAA**
3. Esempio: `01/01/1980`
4. Usa il **calendario** (clicca sull'icona)
5. Verifica che giorno (01-31), mese (01-12), anno (4 cifre)
6. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Data di nascita del Titolare non valida (gg/mm/aaaa).

**Causa**: La data è nel formato sbagliato.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Nato il**
2. Usa il formato **GG/MM/AAAA**
3. Esempio: `01/01/1980`
4. Usa il **calendario** (clicca sull'icona)
5. Verifica che giorno (01-31), mese (01-12), anno (4 cifre)
6. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo di residenza del Professionista non inserito.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Indirizzo**
2. Compila il campo richiesto
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo di residenza del Titolare non inserito.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Indirizzo**
2. Compila il campo richiesto
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail certificata del Procuratore/Delegato non valido.

**Causa**: L'indirizzo di posta elettronica certificata non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL PROCURATORE / DELEGATO** all'interno del campo **PEC**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail certificata del Professionista non inserito.

**Causa**: L'indirizzo di posta elettronica certificata è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **E-Mail Certificata**
2. Inserisci l'indirizzo email valido
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail certificata del Professionista non valido.

**Causa**: L'indirizzo di posta elettronica certificata non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **E-Mail Certificata**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail certificata del Titolare non valido.

**Causa**: L'indirizzo di posta elettronica certificata non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **PEC**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail certificata della Ditta del Titolare non valido.

**Causa**: L'indirizzo di posta elettronica certificata non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DELLA DITTA/SOCIETA'/ENTE/ALTRO** all'interno del campo **PEC**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail del Procuratore/Delegato non valido.

**Causa**: L'indirizzo email non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL PROCURATORE / DELEGATO** all'interno del campo **posta elettronica**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail del Professionista non inserito.

**Causa**: L'indirizzo email è obbligatorio ma mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **E-Mail**
2. Inserisci l'indirizzo email valido
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail del Professionista non valido.

**Causa**: L'indirizzo email non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **E-Mail**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail del Titolare non valido.

**Causa**: L'indirizzo email non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **posta elettronica**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Indirizzo e-mail della Ditta del Titolare non valido.

**Causa**: L'indirizzo email non è valido.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DELLA DITTA/SOCIETA'/ENTE/ALTRO** all'interno del campo **posta elettronica**
2. Verifica formato: `nome@dominio.ext`
3. **Nessuno spazio** prima o dopo
4. Un solo simbolo **@**
5. Esempi corretti:
   - `mario.rossi@gmail.com` ✅
   - `studio@pec.architetti.it` ✅
6. Esempi SBAGLIATI:
   - `mario rossi@gmail.com` ❌ (spazio)
   - `mario@@gmail.com` ❌ (doppio @)
7. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Nome del Professionista non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Nome**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Nome del Titolare non inserito.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Nome**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Numero civico di residenza del Professionista non inserito.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Civico**
2. Inserisci solo il numero civico (es. `15`, `22/A`)
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Numero civico di residenza del Titolare non inserito.

**Causa**: Dato di indirizzo/residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **n.**
2. Inserisci solo il numero civico (es. `15`, `22/A`)
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Numero dello scontrino della marca da bollo non inserito.

**Causa**: Numero scontrino marca da bollo mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato in alto, nella sezione realtiva alla *Marca da Bollo* all'interno del campo **Numero Scontrino**
2. Inserisci il numero identificativo della marca da bollo (14 cifre)
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Partita IVA della Ditta/Società/Ente non valida (11 caratteri numerici).

**Causa**: La Partita IVA non è valida.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DELLA DITTA/SOCIETA'/ENTE/ALTRO** all'interno del campo **P.IVA**
2. Verifica che la P.IVA sia di **11 cifre** esatte
3. Usa **solo numeri**, nessuna lettera
4. **Nessuno spazio** o carattere speciale
5. Esempio corretto: `12345678901`
5. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Provincia di nascita del Professionista non inserita.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Provincia**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Provincia di nascita del Titolare non inserita.

**Causa**: Dato anagrafico obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Prov.**
2. Inserisci il dato richiesto come da documento d'identità
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Provincia di residenza del Professionista non inserita.

**Causa**: Dato di provincia di residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **Dati del Professionista** all'interno del campo **Provincia**
2. Inserisci la provincia di residenza
3. Riprova **"Valida e Salva"**

---

### ATTENZIONE ! Provincia di residenza del Titolare non inserita.

**Causa**: Dato di provincia di residenza obbligatorio mancante.

**Soluzione**:
1. Il sistema dovrebbe averti posizionato nella sezione **DATI DEL TITOLARE** all'interno del campo **Prov.**
2. Inserisci la provincia di residenza
3. Riprova **"Valida e Salva"**

---



---

## Indice pratiche

{: .note }
> Le pratiche saranno aggiunte progressivamente.

---

## Consigli generali

### Prima di validare ✅

- **Compila tutte le sezioni** dall'inizio alla fine
- **Verifica campi gialli** (obbligatori) siano compilati
- **Controlla formati**:
  - Codice Fiscale: 16 caratteri MAIUSCOLI
  - Partita IVA: 11 cifre
  - CAP: 5 cifre esatte
  - Email: nome@dominio.ext
- **Usa Anagrafica** per autocompilare dati ricorrenti
- **Salva frequentemente** durante la compilazione

### Se ricevi errori ⚠️

1. **Non farti prendere dal panico** - è normale in prima compilazione
2. **Leggi il messaggio** con attenzione
3. **Cerca in Errori Comuni** (sopra) o nella guida della tua pratica
4. **Correggi** seguendo la soluzione
5. **Salva** dopo ogni correzione
6. **Riprova validazione**

### Top 5 errori più frequenti 🔍

1. **CAP errato o incompleto** → Blocca generazione IUV PagoPA
2. **Codice Fiscale non valido** → Verifica 16 caratteri, maiuscole, no spazi
3. **File caricato in sezione sbagliata** → Usa "Documenti obbligatori", non "liberi"
4. **Email formato non valido** → Verifica nome@dominio.ext
5. **Dati catastali mancanti** → Inserire Foglio + Particella

---

## Non trovi l'errore? 🆘

Se il messaggio che vedi **non è** negli Errori Comuni né nella guida specifica della tua pratica:

1. **Verifica** di aver cercato nella pratica giusta
2. **Copia** il messaggio esatto (Ctrl+C) e cerca in tutto il manuale
3. Consulta [Troubleshooting](troubleshooting.html) per problemi tecnici
4. Consulta [FAQ](faq.html) per domande generali
5. Contatta [Assistenza tecnica](assistenza-tecnica.html) con:
   - Messaggio errore completo
   - Tipo pratica (SCIA, CILA, PdC, ecc.)
   - Numero pratica

---

## Prossimi passi

- [Compilare un'istanza](compilare-istanza.html) - Guida completa alla compilazione
- [Troubleshooting](troubleshooting.html) - Problemi tecnici comuni
- [FAQ](faq.html) - Domande frequenti
- [Assistenza tecnica](assistenza-tecnica.html) - Come contattare il supporto

---

**Ultima revisione**: Marzo 2026  
**Errori comuni documentati**: 43
