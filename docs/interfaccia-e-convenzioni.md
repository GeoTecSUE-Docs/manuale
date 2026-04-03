---
title: Interfaccia e convenzioni
nav_order: 30
parent: Introduzione
description: Guida alle icone, colori e convenzioni grafiche dell'interfaccia GeoTecSUE per navigare il portale in modo efficace
keywords: [interfaccia, pulsanti, icone, colori, convenzioni, modifica, cancellazione, visualizza, soggetti, azioni]
IDRegione: 99
IDTipoPratica: 9999
Fonte: Manuale
---

# Interfaccia e convenzioni

Questa sezione descrive gli elementi grafici e le convenzioni utilizzate nell'interfaccia di **GeoTecSUE** per aiutarti a riconoscere rapidamente le azioni disponibili.

## Sistema di identificazione visiva

**GeoTecSUE** utilizza un sistema coerente di **icone** e **colori** per rappresentare le azioni disponibili e il loro livello di impatto. Conoscere queste convenzioni ti permetterà di navigare il portale in modo più rapido ed efficace.

## Panoramica dei pulsanti

Ogni pulsante nel portale è identificato da:
- Un'**icona** che rappresenta il tipo di azione
- Un **colore** che indica l'impatto dell'operazione

### Tabella riepilogativa

| Icona | Colore | Azione | Impatto |
|-------|--------|--------|---------|
| Matita | Giallo | Modifica dati o accesso al dettaglio | Reversibile |
| Cestino | Rosso | Cancellazione definitiva | **Non reversibile** |
| Persona | Blu / Verde | Gestione soggetti compilatori | Reversibile |
| Lente | Verde / Giallo | Visualizzazione dettaglio | Solo lettura |

{: .note }
> Il colore di alcuni pulsanti può variare in base allo stato dell'elemento (es. blu se vuoto, verde se popolato).

## Azioni di modifica (giallo)

### Cosa fa

Il pulsante di modifica consente di:
- Modificare dati già inseriti
- Accedere al dettaglio di un'istanza per proseguirne la compilazione
- Correggere informazioni precedentemente salvate

### Comportamento

L'azione è **sempre reversibile**: cliccando il pulsante si accede alla schermata di modifica, ma le modifiche non vengono salvate finché non confermi esplicitamente.

### Dove si trova

- **Elenco istanze**: Accanto a pratiche e comunicazioni in compilazione
- **Dettaglio pratica**: Nella sezione delle comunicazioni in fase di compilazione
- **Compilazione istanza**:
  - Sezione "Localizzazione intervento" (modifica mappali)
  - Sezione "Soggetti coinvolti" (modifica titolari, tecnici, imprese)

{: .note }
> Quando vedi il pulsante giallo, puoi sempre modificare il dato senza rischi: le modifiche richiedono conferma esplicita.

## Azioni di cancellazione (rosso)

### Cosa fa

Il pulsante di cancellazione consente di eliminare **definitivamente**:
- Pratiche o comunicazioni in compilazione
- Allegati caricati
- Codici IUV di pagamenti PagoPA non ancora effettuati
- Soggetti inseriti nell'istanza (titolari, professionisti, imprese)

### Comportamento

{: .warning }
> **Attenzione**: L'operazione di cancellazione è **irreversibile**. Una volta confermata, non sarà possibile recuperare i dati eliminati.

Per le cancellazioni critiche (come l'eliminazione di un'intera istanza), il sistema richiede una conferma esplicita prima di procedere.

### Dove si trova

- **Elenco istanze**: Accanto a pratiche e comunicazioni in compilazione
- **Dettaglio pratica**: Nella sezione delle comunicazioni in fase di compilazione
- **Compilazione istanza**:
  - Sezione "Localizzazione intervento" (cancellazione mappali)
  - Sezione "Soggetti coinvolti" (rimozione titolari, tecnici, imprese)
  - Sezione "PagoPA" (cancellazione pagamenti non effettuati)
  - Sezione "Allegati" (rimozione file caricati)

{: .warning }
> Usa il pulsante rosso con cautela: assicurati sempre di voler eliminare definitivamente l'elemento prima di confermare.

## Gestione soggetti compilatori (blu/verde)

### Cosa fa

Questo pulsante consente di gestire i [soggetti compilatori](nozioni-di-base.html#soggetti-compilatori-aggiuntivi) della pratica:
- Aggiungere professionisti che possono collaborare alla compilazione
- Rimuovere collaboratori precedentemente aggiunti
- Modificare i ruoli assegnati (Amministratore o Utente Modifica)

### Comportamento

L'azione è **reversibile**: cliccando il pulsante si accede alla schermata di gestione, ma le modifiche richiedono conferma esplicita prima di essere salvate.

### Indicatore visivo dello stato

Il colore del pulsante comunica lo stato attuale:

- **Blu**: Nessun soggetto compilatore aggiunto alla pratica
- **Verde**: Almeno un soggetto compilatore è già presente

Questo ti permette di vedere a colpo d'occhio se la pratica è condivisa con altri professionisti.

### Dove si trova

- **Elenco istanze**: Accanto alle pratiche in compilazione
- **Dettaglio pratica**: In alto a destra, con etichetta "Gestione Soggetti"

{: .note }
> Per maggiori dettagli sul sistema di collaborazione tra professionisti, consulta la sezione [Soggetti compilatori aggiuntivi](nozioni-di-base.html#soggetti-compilatori-aggiuntivi).

## Visualizzazione dettaglio (verde/giallo)

### Cosa fa

Il pulsante di visualizzazione consente di:
- Accedere al dettaglio completo di un'istanza
- Visualizzare un allegato caricato
- Consultare i dati di un soggetto

### Comportamento

L'azione apre una schermata di **sola visualizzazione** o, nel caso di istanze, di accesso al dettaglio completo con ulteriori azioni disponibili.

### Indicatore visivo del contesto

Il colore del pulsante indica il tipo di visualizzazione:

- **Verde**: Dato consolidato o istanza già trasmessa (sola lettura)
- **Giallo**: Dato modificabile o istanza in compilazione

**Esempi**:
- Visualizzare una pratica inviata → **Verde** (dati consolidati)
- Visualizzare un allegato in un'istanza in compilazione → **Giallo** (puoi ancora eliminarlo o sostituirlo)

### Dove si trova

- **Elenco istanze**: Accanto a pratiche inviate, protocollate, registrate o importate
- **Compilazione istanza**:
  - Sezione "Allegati" (visualizzazione file caricati)
  - Sezione "Soggetti coinvolti" (dettaglio anagrafiche)

## Altre convenzioni dell'interfaccia

### Messaggi e notifiche

Il portale utilizza messaggi colorati per comunicare lo stato delle operazioni:

- **Verde**: Operazione completata con successo
- **Giallo**: Attenzione o informazione importante
- **Rosso**: Errore o operazione non riuscita

### Campi obbligatori

I campi obbligatori hanno uno sfondo giallo e devono essere compilati prima di poter validare e trasmettere l'istanza.

### Badge di stato

Le istanze nell'elenco delle pratiche inviate mostrano un badge colorato che indica uno stato *particolare* e che merita attenzione:
- **Verde**: Esecutiva
- **Giallo**: Richiesta integrazioni
- **Rosso**: Archiviata/Diniego

## Consigli per l'utilizzo

### Prima di cancellare

Prima di usare il pulsante rosso di cancellazione:
1. Verifica di aver selezionato l'elemento corretto
2. Assicurati di non averne più bisogno
3. Considera di scaricare una copia (per allegati) prima di eliminare

### Quando modificare

Usa il pulsante giallo di modifica quando:
- Devi correggere un errore di compilazione
- Vuoi aggiornare informazioni prima dell'invio
- Devi completare campi lasciati vuoti

### Condivisione pratiche

Usa il pulsante blu/verde di gestione soggetti quando:
- Lavori in team e vuoi condividere la compilazione
- Hai bisogno che un collega completi alcune sezioni
- Vuoi delegare l'invio a un altro professionista

{: .note }
> Ricorda: anche se condividi la pratica, tu rimani il [professionista principale](nozioni-di-base.html#professionista-principale) agli occhi dell'Ente.

## Accessibilità

Tutte le icone sono accompagnate da etichette testuali (tooltip) che appaiono passando il mouse sopra il pulsante. Questo garantisce che l'interfaccia sia utilizzabile anche senza distinguere i colori.

Se hai difficoltà a distinguere i colori, concentrati sulle icone e sui tooltip testuali per identificare le azioni disponibili.

---

**Prossimi passi**: 
- Consulta [Creazione di una nuova istanza](nuova-istanza.html) per vedere queste convenzioni in azione
- Torna a [Nozioni di base](nozioni-di-base.html) per ripassare i concetti fondamentali
