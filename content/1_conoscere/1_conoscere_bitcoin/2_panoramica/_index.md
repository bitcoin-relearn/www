+++
title = 'Panoramica'
author = 'Mattia'
date = 2024-10-30
weight = 2
draft = false
+++

> [!important] Brief:
> Questa sezione ti offre una panoramica per capire che cosa è bitcoin e che cosa sono i termini ad esso correlati.

> [!TIP]+ Con parole semplici
> ##### Che cosa è bitcoin
> Bitcoin è un software che consente di inviare e ricevere pagamenti digitali senza intermediari come banche, grazie a un registro condiviso chiamato blockchain. La blockchain è un registro che contiene tutte le transazioni che avvengono sulla rete Bitcoin, aggiornato ogni 10 minuti attraverso un processo chiamato mining, che previene il problema della doppia spesa.
> 
> Il mining non solo aggiunge nuove transazioni alla blockchain, ma genera anche nuovi Bitcoin come ricompensa per i miner. Le transazioni sono registrate come messaggi digitali, firmati con una chiave privata per garantirne la sicurezza. Possedere Bitcoin significa controllare una chiave privata associata a un indirizzo sulla blockchain, e per farlo, gli utenti utilizzano portafogli digitali sicuri.
> 
> In breve, Bitcoin offre un sistema decentralizzato di scambi digitali, protetto dalla potenza combinata di tutti i miner e dalla sicurezza della blockchain, che registra ogni transazione effettuata.

### Che cosa è Bitcoin?

Bitcoin è fondamentalmente un software che puoi scaricare ed eseguire anche sul tuo computer.

Quando avvii Bitcoin per la prima volta, il programma si collega ad altri computer che stanno eseguendo lo stesso software e inizia a scambiare con loro un file speciale, chiamato **blockchain**. La blockchain è come un grande registro, un elenco che contiene tutte le transazioni mai effettuate con Bitcoin.

Ogni volta che una nuova transazione viene creata, viene inviata attraverso la rete e distribuita a tutti i computer collegati. Poi, circa ogni 10 minuti, uno di questi computer (chiamato **nodo**) aggiorna il registro, aggiungendo le ultime transazioni alla blockchain e condividendo le novità con tutti gli altri.

In pratica, Bitcoin crea una rete di computer che collaborano per tenere aggiornato questo registro, rendendo possibile uno scambio di valore senza bisogno di banche o intermediari.

### Quale problema risolve Bitcoin?

Bitcoin è stato creato per risolvere un problema importante: rendere possibili i pagamenti digitali senza bisogno di un’autorità centrale, come una banca.

Prima di Bitcoin, inviare denaro attraverso una rete di computer era già tecnicamente possibile, ma c’era un problema: il rischio di spendere lo stesso importo due volte, detto _problema della doppia spesa_. Se una persona cercasse di inviare la stessa somma a due destinatari contemporaneamente, come farebbe la rete a sapere quale transazione è valida?

Bitcoin risolve questo problema grazie a un sistema in cui tutti i computer (o **nodi**) della rete tengono temporaneamente in memoria tutte le transazioni che ricevono. Ogni 10 minuti circa, un nodo della rete viene scelto casualmente per aggiungere queste transazioni alla blockchain, il registro ufficiale di Bitcoin. Una volta aggiornato, il registro viene condiviso con tutta la rete, e le transazioni in conflitto vengono scartate.

Questo processo, chiamato **mining**, è una sorta di competizione tra i nodi per aggiornare la blockchain. Grazie al mining, Bitcoin assicura che il registro delle transazioni sia sempre unico e aggiornato, impedendo la doppia spesa e garantendo che tutti i nodi abbiano la stessa versione delle transazioni.

### Che cosa è la rete Bitcoin?

La rete Bitcoin è formata da persone che utilizzano un programma speciale chiamato "client Bitcoin". Chiunque, con una connessione Internet, può scaricarlo e unirsi alla rete.

Questa rete funziona in modo _peer-to-peer_ (P2P), cioè tutti i partecipanti sono collegati tra loro e hanno lo stesso ruolo. Quando esegui il client Bitcoin, esso si collega agli altri utenti e inizia a scaricare una copia della blockchain, il registro che contiene tutte le transazioni verificate. Da quel momento, il tuo client inizia a ricevere nuove transazioni e a inoltrarle agli altri, contribuendo all’aggiornamento della rete.

In sostanza, ogni persona che usa un client Bitcoin diventa un **nodo** della rete, aiutando a mantenere aggiornata e sicura la blockchain, senza bisogno di un’autorità centrale.

### Che cosa è il mining?

Il **mining** è il processo che aggiunge nuovi gruppi di transazioni, chiamati blocchi, alla blockchain, il registro condiviso di Bitcoin.

Ogni computer (o **nodo**) nella rete Bitcoin tiene in memoria le ultime transazioni ricevute. Quando prova a fare mining, il nodo raccoglie queste transazioni in un contenitore, chiamato _blocco_. Per aggiungere il blocco alla blockchain, però, bisogna calcolare un valore speciale, detto _hash_.

Un **hash** è come un’impronta digitale unica, generata da un algoritmo. Questo algoritmo prende le informazioni del blocco e le trasforma in un numero unico e imprevedibile. Se si modifica anche un solo dettaglio nel blocco, l’hash cambia completamente.

Per poter aggiungere un blocco alla blockchain, l’hash del blocco deve essere inferiore a un certo valore (il _target_), un numero concordato da tutti i nodi della rete. Per ottenerlo, il nodo modifica i dati del blocco e calcola l’hash, ripetendo finché non ottiene un hash sotto il target. Quando finalmente uno dei nodi ci riesce, può aggiungere il blocco alla blockchain e condividerlo con il resto della rete.

Questo processo rende il mining una vera e propria competizione tra nodi, dove chi riesce per primo ad ottenere un hash valido aggiunge il blocco e guadagna una ricompensa. Così, nessun nodo ha il controllo completo sulla blockchain, garantendo un sistema distribuito e senza autorità centrale.

Sebbene sia ancora possibile per chiunque provare a estrarre blocchi, non è più competitivo farlo su un computer di casa. I minatori, per eseguire calcoli hash il più velocemente (e il più efficientemente) possibile, utilizzano hardware specializzato ed elettricità a basso costo.

### Da dove provengono i Bitcoin?

I Bitcoin vengono creati come **ricompensa** per i miner, cioè per coloro che usano la potenza di calcolo dei loro computer per aggiungere nuovi blocchi di transazioni alla blockchain. Ogni volta che un blocco viene aggiunto, vengono generati nuovi Bitcoin che prima non esistevano.

Questi nuovi Bitcoin vengono assegnati al miner che ha completato con successo il blocco, come compenso per il lavoro e l’energia spesi. In questo modo, il mining diventa anche un meccanismo per distribuire i Bitcoin.

### Che cosa è la blockchain?

La **blockchain** è un file condiviso tra tutti gli utenti della rete Bitcoin e contiene un elenco completo di transazioni. Questo file si aggiorna costantemente con le ultime transazioni, così che ogni utente abbia sempre una versione aggiornata.

Le transazioni non vengono aggiunte una alla volta, ma sono raggruppate in blocchi, collegati uno dopo l’altro in una “catena” dove ogni blocco si basa sul precedente. Questo collegamento impedisce di modificare blocchi già esistenti: ogni cambiamento romperebbe i collegamenti della catena. Da qui il nome “blockchain” (catena di blocchi).

I miner costruiscono sempre sulla "punta" della catena di blocchi più lunga e considerano valida solo questa versione della blockchain. Di conseguenza, per cambiare la cronologia delle transazioni, qualcuno dovrebbe ricostruire un'intera catena di blocchi più lunga di quella attuale, un'impresa che richiederebbe più potenza di calcolo di quella di tutta la rete messa insieme.

In breve, la blockchain rende la storia delle transazioni, e quindi il valore dei Bitcoin, sicura grazie all’energia combinata di tutti i miner.

### Che cosa sono le transazioni?

Le transazioni in Bitcoin sono il modo in cui gli utenti inviano e ricevono bitcoin sulla rete. Ogni transazione è come un messaggio digitale che sposta bitcoin da un indirizzo a un altro. Questo messaggio include informazioni importanti: l’indirizzo del mittente, l’indirizzo del destinatario e la quantità di bitcoin trasferiti.

Per rendere sicura ogni transazione, il mittente utilizza una **firma digitale**. La firma digitale è una sorta di password unica per quella transazione, che dimostra che il mittente è effettivamente il proprietario dei bitcoin inviati. Questa firma viene creata grazie a una **chiave privata** (una sequenza di numeri segreta) che solo il mittente conosce. Gli altri utenti della rete possono verificare la firma e confermare che il mittente ha autorizzato la transazione senza però conoscere la sua chiave privata.

Quando una transazione viene inviata, viene inoltrata alla rete e raccolta dai miner nel blocco successivo da aggiungere alla blockchain. Una volta confermata, la transazione diventa parte della blockchain e non può essere annullata, rendendo il trasferimento di bitcoin permanente.

### Come si possiedono i bitcoin?

Possedere bitcoin significa avere il controllo di una chiave privata che permette di utilizzare una certa quantità di bitcoin collegata a un indirizzo specifico sulla blockchain. In pratica, quando qualcuno ti invia bitcoin, la transazione viene registrata sulla blockchain, e gli altri utenti vedranno che quella quantità di bitcoin appartiene al tuo indirizzo.

Tuttavia, non possiedi realmente “bitcoin fisici” sul tuo computer. Invece, possiedi una **chiave privata** legata al tuo indirizzo Bitcoin. Questa chiave privata è una sorta di “chiave digitale” segreta, che ti permette di firmare e autorizzare transazioni, spostando bitcoin dal tuo indirizzo a quello di qualcun altro.

È importante proteggere la chiave privata, perché chiunque la possieda può accedere ai tuoi bitcoin e spenderli. Per questo motivo, gli utenti spesso utilizzano **wallet** (portafogli digitali) sicuri per conservare le loro chiavi private, garantendo che solo loro possano gestire i propri bitcoin.


