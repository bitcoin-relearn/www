+++
title = 'Firma digitale'
author = 'Mattia'
date = 2024-11-12
weight = 5
draft = false
+++

>[!important] Brief:
> Questa sezione ti aiuterà a capire cos'è la firma digitale e che ruolo gioca nelle transazioni.

> [!TIP]+ Con parole semplici
> ##### Cos'è la firma digitale?
> La firma digitale è un sistema che serve a dimostrare che sei davvero tu a inviare dei bitcoin, senza che nessuno possa vedere o copiare la tua "chiave segreta" (chiamata chiave privata). È un po' come firmare una lettera per dimostrare che l'hai scritta tu, ma senza che la tua firma possa essere usata per altri scopi.
> ##### Perchè è sicura?
> La tua chiave privata non viene mai condivisa o mostrata a nessuno. La rete usa un sistema matematico (chiamato crittografia) che rende impossibile scoprire la tua chiave privata dalla firma o dalla chiave pubblica.
> ##### Un esempio:
> Immagina di scrivere una lettera importante che solo tu puoi firmare con un timbro unico, che tieni al sicuro a casa tua.
>- **Il timbro unico** è come la tua chiave privata: solo tu lo possiedi e puoi usarlo per firmare.
>- **La firma lasciata dal timbro** è come la firma digitale: chiunque può vederla e verificare che proviene dal tuo timbro, ma nessuno può risalire al timbro stesso.
>
>Quando mostri la firma a qualcuno, possono confermare che è autentica, perché sanno come appare il tuo timbro, ma non hanno il timbro originale e non possono falsificarlo.
>
>Questa è l’idea alla base della firma digitale: dimostri che hai autorizzato qualcosa senza mai rivelare il tuo "timbro" segreto.

### Che cosa è la firma digitale?

Quando si effettua una transazione di Bitcoin, entra in gioco la **firma digitale**, che è un meccanismo crittografico che consente alla rete di confermare che chi invia i fondi è effettivamente il legittimo proprietario, proteggendo allo stesso tempo la segretezza della chiave privata.

La **firma digitale** consente alla rete di confermare che chi invia i fondi è effettivamente il legittimo proprietario, proteggendo allo stesso tempo la segretezza della chiave privata.

Ecco come funziona il processo:
1. **Creazione della firma**: Quando invii bitcoin, il software del portafoglio utilizza la tua chiave privata per creare una firma digitale. Questa firma è una stringa alfanumerica che conferma il possesso della chiave privata senza tuttavia rivelarla, ma che può essere verificata da chiunque utilizzi la tua chiave pubblica.
2. **Verifica della firma**: Una volta eseguita la transazione, la firma digitale viene verificata da altri nodi della rete Bitcoin utilizzando la tua chiave pubblica (nel momento in cui una transazione viene trasmessa, la chiave pubblica diventa disponibile per chiunque). Questi nodi possono confermare che la firma è stata creata da chi possiede la chiave privata associata alla chiave pubblica, senza che la chiave privata stessa venga esposta. In questo modo, la rete garantisce che solo il proprietario effettivo dei bitcoin possa spenderli, mantenendo al sicuro la chiave privata.

Questo sistema di firma digitale è il motivo per cui il Bitcoin è così sicuro: anche se la rete verifica le transazioni, nessuno può accedere ai fondi senza la chiave privata.

L’algoritmo crittografico utilizzato da Bitcoin per le firme digitali è l’**ECDSA** (Elliptic Curve Digital Signature Algorithm). Questo algoritmo crea una firma che è verificabile da chiunque conosca la chiave pubblica del mittente, ma senza mai rivelare la chiave privata.

**Scenario**: Supponiamo che Alice voglia inviare 1 bitcoin a Mattia. Ecco come si svolge il processo.
### Creazione della firma digitale

##### 1. Creazione della transazione

Alice apre il suo portafoglio Bitcoin e crea una transazione in cui specifica che vuole inviare 1 bitcoin all'indirizzo di Mattia. Il portafoglio di Alice raccoglie le informazioni necessarie, come l'ammontare da inviare e l'indirizzo del destinatario (l'indirizzo di Mattia).

##### 2. Generazione della firma digitale

Per autorizzare questa transazione, il portafoglio di Alice utilizza la sua chiave privata per firmare i dati della transazione. Il software del portafoglio crea prima un **hash della transazione** e poi usa la chiave privata per firmare questo hash, creando così una firma digitale univoca.

##### 3. Invio della transazione

La transazione firmata viene inviata alla rete Bitcoin, dove viene ricevuta dai nodi che eseguono la verifica.

### Verifica della firma digitale

Vediamo ora un esempio pratico di come avviene la verifica di una firma digitale in una transazione Bitcoin.

##### 4. Verifica della firma

Uno dei nodi riceve la transazione e inizia il processo di verifica:

- Il nodo calcola l'hash della transazione utilizzando i dati inviati da Alice.
- Utilizza poi la **chiave pubblica** di Alice (che è pubblicamente associata al suo indirizzo Bitcoin) per verificare che la firma digitale corrisponda all'hash della transazione. Questo passaggio conferma che solo Alice, che possiede la chiave privata associata alla chiave pubblica, avrebbe potuto firmare la transazione.

##### 5. Validazione e inclusione nella blockchain

Se la firma digitale è valida, il nodo accetta la transazione e la diffonde ulteriormente nella rete. Alla fine, la transazione di Alice viene inclusa in un blocco della blockchain, e 1 bitcoin viene trasferito da Alice a Bob. In tutto questo processo, la chiave privata di Alice non è mai stata rivelata.

#### 6. Perché la chiave privata non viene mai svelata

La chiave privata di Alice è utilizzata solo per generare la firma digitale, e non è mai condivisa con la rete. Grazie alla crittografia a chiave pubblica, la chiave privata non può essere dedotta dalla chiave pubblica o dalla firma digitale. Questo sistema garantisce che, anche se la transazione viene verificata pubblicamente, solo chi possiede la chiave privata può autorizzare l’invio di fondi.

#### 7. Conclusione

La verifica della firma digitale nelle transazioni Bitcoin è un processo crittografico sofisticato ma essenziale per la sicurezza della rete. Utilizzando la crittografia a chiave pubblica e l'algoritmo ECDSA, Bitcoin permette di verificare l'autenticità delle transazioni senza compromettere la segretezza della chiave privata. Grazie a questo sistema, gli utenti possono trasferire fondi in modo sicuro, mentre la rete mantiene la fiducia e l'integrità delle transazioni.









