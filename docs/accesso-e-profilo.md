---
title: Accesso al portale e gestione del profilo
nav_order: 10
parent: Introduzione
description: Come accedere a GeoTecSUE tramite SPID o CIE e gestire i dati del proprio profilo utente
keywords: [accesso, login, SPID, CIE, profilo, autenticazione]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Accesso al portale e gestione del profilo

Questa sezione spiega come accedere a **GeoTecSUE** e gestire i dati del proprio profilo.

## Sistemi di autenticazione

L'accesso a **GeoTecSUE** avviene esclusivamente tramite:

- **SPID** (Sistema Pubblico di Identità Digitale)
- **CIE** (Carta d'Identità Elettronica)

Come previsto dal [Decreto Legge "Semplificazione e innovazione digitale"](https://innovazione.gov.it/dipartimento/focus/linee-guida-decreto-semplificazione/){:target="_blank"}, questi sono gli unici sistemi di identificazione consentiti per i servizi digitali della Pubblica Amministrazione.

### Disponibilità dei pulsanti di accesso (CIE/SPID):

La presenza fisica dei pulsanti o delle mascherine di login ("Entra con SPID" o "Entra con CIE") nella pagina di accesso dipende esclusivamente dalle configurazioni attivate dal singolo Ente. 

Se non si visualizza la mascherina o il pulsante per la CIE (o per lo SPID), significa che l'Ente specifico non ha ancora abilitato quel canale sulla piattaforma. In questo caso è necessario contattare direttamente l'Ufficio Tecnico o l'assistenza dell'Ente affinchè proceda con l'attivazione. Sarà cura dell'Ente rivolgersi poi all'assistenza del **GeoTecSUE** per ricevere tutto il supporto necessario in fase di attivazione del servizio.

### Mancato accesso con un provider SPID specifico (es. InfoCert, Namirial, TIM, Poste, ecc.)

Se durante il tentativo di login tramite SPID il sistema restituisce un errore dopo aver selezionato il proprio gestore dell'identità digitale, il problema potrebbe essere legato a un disservizio temporaneo dell'Identity Provider scelto e non alla piattaforma **GeoTecSUE**.

In questo caso:
1. Se possiedi un'identità digitale con un secondo provider (es. accede alternativamente con PosteID o CIE se attiva), puoi tentare un accesso alternativo 
2. Se l'accesso alternativo va a buon fine o se si decide comunque di aprire una segnalazione all'assistenza, **specifica il nome del provider** (es. "Non riesco ad accedere tramite TIM ID") con cui si è verificato l'errore. Questo permette ai nostri tecnici di isolare immediatamente il problema e verificare lo stato dei gateway governativi di quel gestore (ed eventualmente aprire una segnalazione)

### Non hai SPID o CIE?

Se non possiedi ancora una di queste credenziali, consulta:
- [Come ottenere SPID](https://www.spid.gov.it/richiedi-spid){:target="_blank"}
- [Come richiedere la CIE](https://www.cartaidentita.interno.gov.it/){:target="_blank"}

## Accesso come Azienda / Persona Giuridica

Oltre all'accesso tramite **SPID** o **CIE** per le persone fisiche, è possibile registrarsi come **Aziende**, **Società tra Professionisti (STP)**, **Studi Associati** e altre **Persone Giuridiche**.

### Perché esiste questa modalità di registrazione?

I sistemi nazionali di autenticazione attualmente disponibili (**SPID** e **CIE**) consentono di identificare esclusivamente una **persona fisica** tramite il relativo Codice Fiscale e non prevedono un meccanismo di autenticazione diretto basato sulla **Partita IVA** di una società.

Per agevolare l'operatività delle persone giuridiche, **GeoTecSUE** mette quindi a disposizione una modalità di registrazione dedicata che consente di creare un account associato a una Partita IVA.

Questa funzionalità rappresenta una facilitazione fornita dalla piattaforma e non sostituisce i sistemi di autenticazione nazionali previsti per l'accesso ai servizi digitali della Pubblica Amministrazione.

### Registrazione

Durante la registrazione vengono richiesti alcuni dati identificativi, tra cui:

- Ragione Sociale
- Partita IVA
- Cognome e Nome del referente
- Codice Fiscale del referente
- E-mail
- Telefono

### Credenziali di accesso

Per gli utenti registrati come Persona Giuridica:

- la **Partita IVA** rappresenta l'identificativo principale dell'account;
- l'account viene associato in modo permanente alla Partita IVA indicata in fase di registrazione.

### Collegamento di SPID o CIE

Dopo la registrazione è possibile associare all'account aziendale uno o più utenti autenticati tramite **SPID** o **CIE**.

Una volta effettuato il collegamento, sarà possibile accedere utilizzando le modalità di autenticazione previste dalla normativa nazionale, mantenendo l'associazione con la medesima posizione aziendale.

### Modifica della Partita IVA

La **Partita IVA non può essere modificata** dopo la registrazione.

Poiché costituisce l'identificativo univoco dell'account aziendale, GeoTecSUE non può effettuare variazioni, sostituzioni o correzioni della Partita IVA associata all'utenza.

Qualora sia necessario operare con una Partita IVA differente, dovrà essere creato un nuovo account riferito alla nuova posizione aziendale.

### Perché esiste questa modalità di registrazione? 

I sistemi nazionali di autenticazione attualmente disponibili (**SPID** e **CIE**) consentono di identificare esclusivamente una **persona fisica** tramite il relativo Codice Fiscale e non prevedono un meccanismo di autenticazione diretto basato sulla **Partita IVA** di una società. 
Per agevolare l'operatività delle persone giuridiche, **GeoTecSUE** mette quindi a disposizione una modalità di registrazione dedicata che consente di creare un account associato a una Partita IVA. Questa funzionalità rappresenta una facilitazione fornita dalla piattaforma e non sostituisce i sistemi di autenticazione nazionali previsti per l'accesso ai servizi digitali della Pubblica Amministrazione. 

> **Importante**
> Sebbene questa modalità di accesso possa essere resa disponibile dall'Ente, il suo utilizzo è fortemente sconsigliato. Il quadro normativo vigente in materia di digitalizzazione della Pubblica Amministrazione, e in particolare il Decreto Legge "Semplificazione e innovazione digitale", individua in **SPID** e **CIE** gli strumenti di autenticazione di riferimento per l'accesso ai servizi online della Pubblica Amministrazione.
> Si raccomanda pertanto di associare quanto prima uno o più utenti autenticati tramite SPID o CIE all'account aziendale e di utilizzare tali modalità per gli accessi successivi.

## Primo accesso e completamento profilo

Al primo accesso, **GeoTecSUE** importa automaticamente alcuni dati anagrafici dal sistema di autenticazione utilizzato (SPID o CIE).

Dopo il login, il sistema potrebbe richiedere di completare il profilo con informazioni aggiuntive necessarie per l'utilizzo del portale (esempio: dati professionali, recapiti, ecc.).

## Modificare i dati del profilo

Per accedere al tuo profilo:

1. Clicca sul **menu personale** in alto a destra (dove appare "Bentornato, **Cognome Nome**")
2. Seleziona **"Il mio profilo"**
3. Modifica o integra i dati desiderati

### Dati modificabili

Puoi modificare:
- Dati di contatto (email, telefono, PEC)
- Indirizzo di residenza/domicilio
- Dati professionali (Ordine, numero iscrizione, ecc.)

**Non è possibile modificare**:
- Cognome e Nome
- Codice Fiscale

Questi dati provengono direttamente dal sistema di autenticazione e non sono editabili.

## Durata della sessione

Una volta autenticato, rimani connesso a **GeoTecSUE** fino a quando:

- Esegui il **logout** manualmente (dal menu personale → "Logout")
- Chiudi la finestra/tab del browser
