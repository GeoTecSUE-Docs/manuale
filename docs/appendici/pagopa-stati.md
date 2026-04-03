---
title: Stati PagoPA
parent: Appendici
nav_order: 2
description: Descrizione completa degli stati dei pagamenti PagoPA su GeoTecSUE con icone, codici e significato operativo per ogni fase del pagamento
keywords: [PagoPA, stati pagamento, IUV, codici pagamento, pagamento eseguito, pagamento scaduto, incasso, storno]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Stati PagoPA

Questa appendice descrive gli **stati dei pagamenti PagoPA** gestiti e visualizzati nel portale **GeoTecSUE**.

## Come funzionano gli stati

Gli stati derivano dal **sistema PagoPA** e vengono rappresentati nel portale tramite:
- **Icone visive** per identificazione rapida
- **Codici numerici** (interni al sistema)
- **Descrizioni testuali** chiare
- **Significato operativo** (cosa devi fare)

{: .note }
> Gli stati PagoPA sono gestiti dal sistema di pagamento. GeoTecSUE li visualizza in tempo reale interrogando la piattaforma PagoPA.

## Dove vedi gli stati

Gli stati PagoPA appaiono in due sezioni del [dettaglio pratica](../dettaglio-istanza.html):

1. **Pagamenti aperti**: Pagamenti in attesa o in corso
2. **Pagamenti completati**: Pagamenti conclusi (eseguiti o falliti)

## Come aggiornare lo stato

Per i pagamenti già generati, puoi **aggiornare lo stato** cliccando il pulsante "Aggiorna" (arancione) accanto al pagamento. Il sistema interroga PagoPA e mostra lo stato attuale.

{: .note }
> Dopo aver pagato, attendi qualche minuto prima di aggiornare. I sistemi PagoPA possono richiedere tempo per propagare l'informazione.

---

## Tabella completa degli stati

| Codice | Icona | Stato | Descrizione | Significato operativo |
|--------|-------|-------|-------------|----------------------|
| — | ❌ | **Senza IUV** | Nessun IUV associato | Pagamento non ancora generato. Clicca "Creazione IUV" per generarlo. |
| 0 | ❌ | **Senza IUV** | Pagamento privo di IUV | Nessuna operazione avviata. Genera lo IUV per procedere. |
| 2 | ⏳ | **In attesa di IUV** | Generazione IUV in corso | Il sistema sta creando il codice. Attendi qualche secondo. |
| 10 | ✔️ | **IUV generato** | IUV creato e disponibile | Puoi procedere al pagamento tramite PagoPA. |
| 14 | 🛣️ | **Pagamento inoltrato** | Pagamento avviato | Hai iniziato la procedura di pagamento. In corso. |
| 15 | 👍 | **Pagamento accettato** | Preso in carico dal PSP | Il Prestatore Servizi Pagamento sta elaborando. Attendi. |
| 16 | 👍 | **Pagamento autorizzato** | Autorizzato dal PSP | Il pagamento è stato autorizzato. Attesa conferma finale. |
| 17 | 🔄 | **Pagamento differito** | Esito differito | L'esito finale verrà comunicato successivamente. Verifica più tardi. |
| 19 | 🛣️ | **In attesa di esito** | In verifica | Il sistema sta verificando l'esito. Attendi. |
| 20 | 👍 | **Pagamento eseguito** | Pagamento completato | ✅ **Pagamento riuscito**. Importo incassato. |
| 21 | 👍 | **Pagamento eseguito parzialmente** | Pagamento parziale | ⚠️ Pagato solo parzialmente. Verifica importo residuo. |
| 30 | 👎 | **Pagamento non eseguito** | Pagamento fallito | ❌ Pagamento non riuscito. Riprova o usa altro metodo. |
| 31 | 👎 | **Non eseguito (termini)** | Scaduto per termini | ❌ Scaduto il tempo disponibile. Genera nuovo IUV. |
| 32 | 🔁 | **Pagamento stornato** | Storno effettuato | Importo restituito. Pagamento annullato e rimborsato. |
| 33 | 👎 | **Pagamento revocato** | Revocato | ❌ Pagamento revocato. Non più valido. |
| 40 | 👎 | **Pagamento scaduto** | IUV scaduto | ❌ IUV oltre la scadenza. Genera nuovo codice. |
| 90 | 👎 | **Pagamento annullato** | Annullato | ❌ Pagamento annullato. Non valido. |
| 100 | 💶 | **Pagamento incassato** | Incassato e contabilizzato | ✅ **Completato e registrato**. Pagamento concluso. |

---

## Stati per categoria

### Stati iniziali (generazione IUV)

#### Senza IUV (—, 0)
**Cosa significa**: Non hai ancora generato il codice di pagamento.

**Cosa fare**: 
1. Vai alla sezione "Pagamenti aperti" del dettaglio pratica
2. Compila eventuali campi richiesti (es. importo)
3. Clicca su "Creazione IUV"

#### In attesa di IUV (2)
**Cosa significa**: Il sistema sta generando il codice IUV.

**Cosa fare**: Attendi qualche secondo. Lo stato passerà automaticamente a "IUV generato".

#### IUV generato (10)
**Cosa significa**: Il codice di pagamento è pronto.

**Cosa fare**: 
1. Clicca su "Dettaglio" per vedere il codice IUV
2. Copia il codice o usa il QR code
3. Accedi al tuo home banking o app di pagamento
4. Inserisci il codice IUV nella sezione PagoPA
5. Completa il pagamento

{: .note }
> Puoi pagare tramite: home banking, app bancarie, tabaccherie abilitate, sportelli ATM, uffici postali.

### Stati in corso (pagamento avviato)

#### Pagamento inoltrato (14)
**Cosa significa**: Hai avviato la procedura di pagamento sul PSP (banca, Poste, ecc.).

**Cosa fare**: Segui le istruzioni del tuo sistema di pagamento per completare l'operazione.

#### Pagamento accettato (15)
**Cosa significa**: Il Prestatore Servizi Pagamento ha preso in carico la richiesta.

**Cosa fare**: Attendi il completamento dell'elaborazione (solitamente pochi minuti).

#### Pagamento autorizzato (16)
**Cosa significa**: Il PSP ha autorizzato il pagamento.

**Cosa fare**: Attendi la conferma finale. Il pagamento è quasi completato.

#### Pagamento differito (17)
**Cosa significa**: L'esito del pagamento sarà comunicato in un secondo momento.

**Cosa fare**: 
1. Attendi alcune ore
2. Torna su GeoTecSUE e clicca "Aggiorna"
3. Verifica il nuovo stato

#### In attesa di esito (19)
**Cosa significa**: Il sistema sta verificando l'esito del pagamento.

**Cosa fare**: Attendi e aggiorna periodicamente lo stato.

### Stati positivi (pagamento riuscito)

#### Pagamento eseguito (20)
**Cosa significa**: ✅ **Il pagamento è stato completato con successo**.

**Effetti**:
- L'importo è stato incassato
- Il pagamento è registrato su PagoPA
- L'Ente riceverà notifica dell'avvenuto pagamento

**Cosa fare**: Nulla. Il pagamento è concluso.

{: .note }
> Lo stato "Pagamento eseguito" (20) conferma che hai pagato correttamente. Conserva la ricevuta.

#### Pagamento eseguito parzialmente (21)
**Cosa significa**: ⚠️ Hai pagato solo una parte dell'importo dovuto.

**Quando succede**: 
- Pagamenti rateali (hai pagato solo alcune rate)
- Errore nell'importo inserito

**Cosa fare**:
1. Verifica l'importo residuo nella sezione "Pagamenti aperti"
2. Genera un nuovo IUV per il saldo
3. Completa il pagamento

#### Pagamento incassato (100)
**Cosa significa**: ✅ **Il pagamento è stato incassato e contabilizzato** dall'Ente.

**Effetti**:
- Importo accreditato sul conto dell'Ente
- Pagamento registrato contabilmente
- Procedura completamente conclusa

**Cosa fare**: Nulla. Questo è lo stato finale definitivo.

{: .note }
> La differenza tra "Pagamento eseguito" (20) e "Pagamento incassato" (100) è che il secondo indica la registrazione contabile completa da parte dell'Ente.

### Stati negativi (pagamento fallito)

#### Pagamento non eseguito (30)
**Cosa significa**: ❌ Il pagamento è fallito per motivi tecnici.

**Possibili cause**:
- Fondi insufficienti
- Carta scaduta o bloccata
- Timeout della transazione
- Errore di comunicazione con il PSP

**Cosa fare**:
1. Verifica la causa dell'errore
2. Risolvi il problema (es. ricarica carta)
3. Genera un nuovo IUV
4. Riprova il pagamento

#### Non eseguito per termini (31)
**Cosa significa**: ❌ È scaduto il tempo disponibile per completare il pagamento.

**Quando succede**: Hai iniziato ma non completato il pagamento entro i termini (solitamente 15-30 minuti dalla sessione).

**Cosa fare**: Genera un nuovo IUV e riprova immediatamente.

#### Pagamento stornato (32)
**Cosa significa**: Il pagamento è stato annullato e l'importo **restituito**.

**Quando succede**:
- Richiesta di storno da parte tua o dell'Ente
- Pagamento duplicato
- Errore nell'importo

**Cosa fare**: 
1. Verifica il rimborso sul tuo conto
2. Se ancora necessario, genera un nuovo IUV
3. Effettua un nuovo pagamento corretto

#### Pagamento revocato (33)
**Cosa significa**: ❌ Il pagamento è stato revocato e non è più valido.

**Quando succede**:
- Revoca da parte dell'Ente
- Annullamento della pratica
- Errore amministrativo

**Cosa fare**: Contatta l'Ente per chiarimenti. Se ancora necessario pagare, l'Ente genererà un nuovo IUV.

#### Pagamento scaduto (40)
**Cosa significa**: ❌ Il codice IUV è oltre la **data di scadenza**.

**Quando succede**: Gli IUV hanno una scadenza (solitamente 30-60 giorni). Se non paghi entro questa data, lo IUV scade.

**Cosa fare**:
1. Nella sezione "Pagamenti aperti", clicca "Creazione IUV"
2. Genera un nuovo codice aggiornato
3. Paga entro la nuova scadenza

{: .warning }
> Attenzione alle scadenze! Controlla sempre la data di scadenza dello IUV prima di pagare.

#### Pagamento annullato (90)
**Cosa significa**: ❌ Il pagamento è stato annullato.

**Quando succede**:
- Annullamento manuale
- Pratica ritirata o archiviata
- Pagamento non più dovuto

**Cosa fare**: Verifica con l'Ente se il pagamento è ancora necessario.

---

## Domande frequenti

### Quanto tempo ci vuole per vedere "Pagamento eseguito" dopo aver pagato?

**Normalmente**: Da pochi minuti a qualche ora.

**Procedura**:
1. Completa il pagamento sul tuo sistema bancario/app
2. Attendi 10-15 minuti
3. Torna su GeoTecSUE nel dettaglio della pratica
4. Il pagamento dovrebbe già esserea aggiornato, altrimenti clicca "Aggiorna" accanto al pagamento
5. Lo stato dovrebbe cambiare in "Pagamento eseguito" (20)

{: .note }
> Se dopo 24 ore non vedi ancora lo stato aggiornato, contatta l'assistenza con il codice IUV e la ricevuta di pagamento.

### Posso pagare uno IUV scaduto?

**No**, gli IUV scaduti (stato 40) **non sono pagabili**.

**Soluzione**: 
1. Se possibile, cancella lo IUV e generalo nuovamente
2. Paga il nuovo codice entro la scadenza

### Ho pagato ma lo stato è ancora "IUV generato". Cosa faccio?

**Possibili cause**:
1. Il pagamento non è ancora stato registrato da PagoPA (attendi)
2. Hai pagato ma non hai completato correttamente la procedura
3. Errore di comunicazione

**Cosa fare**:
1. Verifica sul tuo conto se l'importo è stato addebitato
2. Attendi almeno 1 ora
3. Clicca "Aggiorna" su GeoTecSUE
4. Se persiste, contatta l'assistenza con ricevuta di pagamento

### Cosa significa "Pagamento eseguito parzialmente"?

Significa che hai pagato **solo una parte** dell'importo totale dovuto.

**Cause comuni**:
- Pagamenti rateizzati (hai pagato solo la prima rata)
- Hai inserito un importo inferiore al dovuto

**Soluzione**: Verifica l'importo residuo e genera un nuovo IUV per il saldo.

### Posso annullare un pagamento già generato?

**Dopo la generazione dello IUV**: Sì, puoi eliminare lo IUV (pulsante rosso) prima di pagare.

**Dopo aver pagato**: No, non puoi annullarlo autonomamente. Devi richiedere lo storno all'Ente seguendo le loro procedure.

### La scadenza dello IUV è passata ma non ho ancora pagato. Cosa succede?

Lo IUV passa allo stato **"Pagamento scaduto" (40)** e non è più utilizzabile.

**Cosa fare**:
1. Genera un nuovo IUV
2. Paga il nuovo codice entro la scadenza

{: .warning }
> Non cercare di pagare IUV scaduti. Il sistema li rifiuterà automaticamente.

### Devo pagare di nuovo se lo stato è "Pagamento stornato"?

**Dipende**:
- Se hai ricevuto il **rimborso** sul conto: Sì, se il pagamento è ancora dovuto, genera un nuovo IUV
- Se il pagamento **non è più necessario** (pratica archiviata, errore dell'Ente): No

Verifica sempre con l'Ente prima di procedere.

---

## Riepilogo stati comuni

### ✅ Stati positivi (tutto ok)
- **IUV generato (10)**: Puoi pagare
- **Pagamento eseguito (20)**: Hai pagato con successo
- **Pagamento incassato (100)**: Completato e contabilizzato

### ⏳ Stati in attesa (attendi)
- **In attesa di IUV (2)**: Generazione in corso
- **Pagamento inoltrato/accettato/autorizzato (14/15/16)**: Elaborazione in corso
- **In attesa di esito (19)**: Verifica in corso

### ❌ Stati negativi (azione richiesta)
- **Pagamento non eseguito (30)**: Fallito, riprova
- **Pagamento scaduto (40)**: Genera nuovo IUV
- **Pagamento annullato/revocato (90/33)**: Non valido

---

## Prossimi passi

- [Visualizzare il dettaglio di una pratica](../dettaglio-istanza.html#pagamenti-aperti-pagopa) (sezione Pagamenti)
- [Ciclo di vita dettagliato](ciclo-vita-dettagliato.html)

---

**Hai problemi con un pagamento?** Contatta l'assistenza dell'Ente fornendo:
- Codice IUV
- Data del pagamento
- Ricevuta (se disponibile)
- Stato attuale visualizzato su GeoTecSUE
