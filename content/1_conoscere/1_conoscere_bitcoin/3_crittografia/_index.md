+++
title = 'Crittografia'
author = 'Mattia'
date = 2024-11-12
weight = 3
draft = false
+++

> [!important] Brief:
> Questa sezione ti aiuterà a capire cos'è la crittografia e perchè è un concetto fondamentale per bitcoin e per la blockchain.

> [!TIP]+ Con parole semplici
> ##### Che cosa è la crittografia
> Bitcoin utilizza la crittografia per proteggere le transazioni e garantire che solo i veri proprietari possano accedere e gestire i fondi. In pratica, la crittografia permette di dimostrare di possedere un "segreto" (la chiave privata) senza doverlo rivelare.
> 
> Per creare un sistema sicuro, Bitcoin si affida a vari algoritmi crittografici:
> - **SHA-256**: algoritmo di hashing che crea una sorta di "impronta digitale" unica e irreversibile per ogni insieme di dati, rendendo impossibile alterare le informazioni senza essere scoperti.
> - **RIPEMD-160**: algoritmo usato per ridurre le dimensioni degli indirizzi Bitcoin in modo compatto e pratico, ma mantenendo l'unicità e la sicurezza.
> - **ECDSA**: algoritmo usato per generare firme digitali. Serve a confermare che una transazione è stata autorizzata dalla persona giusta, senza rivelare la chiave privata.
>
> Grazie alla crittografia, Bitcoin può garantire transazioni sicure, anonime e immutabili, rendendolo affidabile anche senza autorità centrali.


Il bitcoin è basato su *crittografia*: una branca della matematica ampiamente usata in sicurezza informatica, che permette di dimostrare la conoscenza di un segreto (chiave privata) senza doverlo rivelare e di provare l’autenticità dei dati (firma digitale).

> _La sicurezza di un sistema crittografico non deve dipendere dal tenere celato l'algoritmo, ma solo dal tenere celata la chiave._
> 
> _Auguste Kerchoffs_

La crittografia serve a garantire la sicurezza e la validità delle transazioni, oltre a proteggere l'identità degli utenti. Viene utilizzata nella creazione delle chiavi, nella generazione degli indirizzi e delle firme digitali.

### Algoritmo SHA-256: La Base dell’Hashing

SHA-256 è un algoritmo di hashing, ossia un meccanismo che trasforma una serie di dati in una sequenza di lunghezza fissa, detta hash. Gli hash sono come impronte digitali dei dati di partenza: unici e non reversibili. Anche una modifica minima nei dati genera un hash completamente diverso, proteggendo così l'integrità delle informazioni.

Immaginiamo di avere una frase semplice come "Bitcoin è fantastico". Passando questa frase attraverso SHA-256 otteniamo un hash:

**Frase originale**: "Bitcoin è fantastico"  
**Hash SHA-256**: `7281eead366d738a5b1e3f3aadec82a9fdacdef519ba30541fa50a6b29293579`

Ora cambiamo una singola lettera, scrivendo "Bitcoin è Fantastico". Anche con questa minima variazione, l'hash risultante sarà completamente diverso:

**Frase modificata**: "Bitcoin è Fantastico"  
**Hash SHA-256**: `3b43131a74100d17000660637881c9b0ba3dd24cfd5ccff0bc04ecdc79ec3a18`

Come si può notare, l’hash cambia radicalmente anche con una piccola modifica. Questo garantisce che i dati registrati su Bitcoin non possano essere manomessi senza che la modifica sia immediatamente rilevata.

{{% button href="" style="blue" %}}Demo interattiva:{{% /button %}} [Algoritmo SHA-256](ext/sha-256.html)

### Algoritmo RIPEMD-160: La Generazione degli Indirizzi

L’algoritmo **RIPEMD-160** è una funzione di hashing progettata per produrre un hash (o impronta digitale) di 160 bit. Viene utilizzato nella generazione degli indirizzi dagli hash delle chiavi pubbliche per rendere l'output più compatto, rendendolo più pratico da usare e riducendo i costi di memoria e di trasmissione dei dati.

è progettato per essere resistente a collisioni, dove due input diversi generano lo stesso output. Sebbene altre funzioni di hashing più recenti come SHA-256 siano considerati più sicuri, RIPEMD-160 resta affidabile nel contesto degli indirizzi Bitcoin, grazie alla sua combinazione con SHA-256: la chiave pubblica viene prima sottoposta a SHA-256, poi l’hash SHA-256 risultante viene ulteriormente passato attraverso RIPEMD-160.

RIPEMD-160, in breve, rappresenta uno dei tanti elementi che contribuiscono alla sicurezza e alla praticità di Bitcoin, trasformando le chiavi pubbliche in identificatori brevi e sicuri.

Immaginiamo di partire da una chiave pubblica in formato hash SHA-256:

**Hash SHA-256 della Chiave Pubblica**:  
`ab9c3e5a7f2b4b4b8a3e2d2c3e1a0b3f7e5c2f8d3e0b1a3c4e5d2b3f7a8d4b5c`

Quando applichiamo RIPEMD-160, otteniamo un hash finale di 160 bit, come segue:

**Hash RIPEMD-160**:  
`7c5b7b1e8a2b1c5d3e9a3f7c1d0a6b8d3f9c2e5b`

Questo risultato rappresenta l'indirizzo Bitcoin, un identificatore unico e compatto per la chiave pubblica.

### Algoritmo ECDSA
 
L’algoritmo **ECDSA** (Elliptic Curve Digital Signature Algorithm) è un sistema crittografico basato su curve ellittiche utilizzato per generare e verificare firme digitali. In Bitcoin, ECDSA svolge un ruolo fondamentale: consente di firmare le transazioni con la chiave privata e permette a chiunque di verificare l’autenticità della firma utilizzando la chiave pubblica senza rivelare la chiave privata.

Per firmare una transazione, l'ECDSA richiede la chiave privata del mittente e l’hash del messaggio usando SHA-256. Questo garantisce che l’input della firma sia una stringa di lunghezza fissa, indipendentemente dalla lunghezza del messaggio originale. La firma e l’hash del messaggio vengono inclusi nella transazione da inviare alla rete Bitcoin.

La verifica della firma permette a chiunque di confermare che la transazione sia stata effettivamente firmata dalla chiave privata associata alla chiave pubblica del mittente, senza bisogno di conoscere la chiave privata.

L'ECDSA è considerato sicuro ed efficiente per diversi motivi:

- **Irreversibilità**: La chiave pubblica non può essere usata per risalire alla chiave privata grazie alla complessità matematica della curva ellittica.
- **Sicurezza**: Ogni firma è unica per quella transazione, garantendo che non sia possibile risalire alla chiave privata.
- **Efficienza**: ECDSA richiede meno dati e calcoli rispetto ad altri algoritmi di firma come RSA, rendendolo ideale per Bitcoin.

Grazie a questi fattori, ECDSA consente a Bitcoin di garantire transazioni sicure, verificabili e completamente indipendenti da terze parti, assicurando che solo chi possiede la chiave privata possa autorizzare movimenti sui propri fondi.
