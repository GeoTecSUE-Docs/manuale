---
title: Notifiche al professionista
parent: Le mie istanze
nav_order: 80
description: Elenco degli eventi che generano una notifica al professionista, dei canali di invio e di dove trovarle nel portale
keywords: notifiche, tracciabilità, email, PEC, stato pratica
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale GeoTecSUE
---

# Notifiche al professionista

Ogni variazione rilevante dello stato di una pratica genera una notifica per il professionista. Le notifiche vengono sempre riportate nella **tracciabilità della pratica** e nella **sezione Notifiche** del portale, che è il canale ufficiale; in base alla configurazione dell'Ente, vengono anche inviate via **email** o **PEC** come servizio di cortesia (vedi sotto).

## Quando viene generata una notifica

In linea di massima, il sistema invia una notifica in corrispondenza dei seguenti eventi:

- **Invio** della pratica o di una comunicazione
- **Protocollazione**
- **Registrazione**
- **Acquisizione integrazioni** (l'Ente ha ricevuto e preso in carico un'integrazione inviata)
- **Richiesta integrazioni** (l'Ente richiede documentazione o chiarimenti aggiuntivi)
- **Rilascio del provvedimento**
- **Cancellazione del rilascio del provvedimento**
- **Archiviazione**
- **Cancellazione archiviazione**
- **Diniego**
- **Cancellazione diniego**
- **Pubblicazione documenti**
- **Pareri e rilasci**
- **Revoca del delegato**
- **Invio IUV da Ente**

{: .note }
> L'elenco copre gli eventi principali legati al ciclo di vita della pratica. Non tutte le tipologie di pratica generano tutte le notifiche elencate: dipende dall'iter previsto per quel tipo di pratica e dalla configurazione dell'Ente.

Per il dettaglio completo delle fasi e degli stati che una pratica può attraversare, consulta [Il ciclo di vita della pratica](https://geotecsue-docs.github.io/manuale/docs/appendici/ciclo-vita-dettagliato.html).

## Dove trovare le notifiche

### Tracciabilità della pratica

Ogni evento notificato viene registrato nella tracciabilità della singola pratica, con data e ora: è lo storico completo e permanente di tutto ciò che è accaduto sulla pratica.

### Sezione Notifiche

Tutte le notifiche ricevute sono raccolte anche in un'unica sezione dedicata, consultabile indipendentemente dalla singola pratica: utile per avere una visione d'insieme su tutte le pratiche in carico.
Tale sezione è raggiungibile dal menu in alto a destra alla voce *Notifiche*, dove a fianco si trova un numero che indica le notifiche ancora non lette.

Ogni notifica riporta:

- **Mittente**: chi ha generato la notifica (es. "GeoTec SUE" oppure "Comune di...")
- **Oggetto**: il tipo di evento (es. "Pubblicazione documento")
- **Numero pratica**: la chiave della pratica di riferimento
- **Tipo Pratica**: la tipologia della pratica (es. Permesso di Costruire, C.I.L.A., ...)

Su ogni singola notifica sono disponibili le seguenti azioni:

- **Cestino rosso**: elimina la notifica
- **Stellina**: segna la notifica come non letta
- **Leggi** (bottone verde): apre il messaggio della notifica, da cui è anche possibile accedere direttamente al dettaglio della pratica a cui la notifica si riferisce

### Email o PEC

Oltre alla visualizzazione nel portale, ogni notifica viene inviata anche via email: a seconda di come l'Ente ha configurato il servizio, l'invio può avvenire tramite **email ordinaria**, tramite **PEC** oppure **entrambe** (sia email ordinaria che PEC).

{: .warning }
> L'invio via email/PEC è un **servizio di cortesia**, non il canale ufficiale di comunicazione. Il canale ufficiale resta sempre e solo il **portale**. Per questo motivo, l'email non contiene mai i documenti pubblicati (es. provvedimenti, pareri, allegati): riporta solo l'avviso che sul portale sono stati pubblicati dei documenti, che vanno consultati e scaricati direttamente da lì.

{: .note }
> L'indirizzo a cui vengono recapitate le notifiche è quello configurato nel profilo dell'utente che opera sulla pratica in quel momento. Se gestisci più anagrafiche o più indirizzi PEC, verifica quale email è impostata sul profilo che stai utilizzando.

### Non ricevo le email di notifica

Se non ricevi le email di notifica, verifica innanzitutto che l'**indirizzo email inserito nella pratica** sia corretto e privo di errori di digitazione.

Se l'indirizzo risulta corretto, è possibile che le comunicazioni inviate da **noreply@servizipubblicaamministrazione.it** siano state recapitate nelle cartelle **Spam**, **Posta indesiderata** o **Promozioni** del tuo client di posta. Controlla anche queste cartelle e, se necessario, aggiungi il mittente tra quelli attendibili.
