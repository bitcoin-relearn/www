+++
title = 'Transazioni'
author = 'Mattia'
date = 2025-01-14
weight = 6
draft = true
+++

Crittografia a chiave pubblica nelle transazioni Bitcoin.

La crittografia a chiave pubblica è anche nota come crittografia asimmetrica perché utilizza 2 chiavi diverse, una coppia di chiave pubblica e una privata, invece di una per crittografare i dati.

Crittografia asimmetrica:
Chiave pubblica: mostrala alle persone con cui vuoi comunicare.
Chiave privata: tienila segreta, solo tu la conosci.

[IMMAGINE]

Quando ricevi un messaggio:
- Messaggio del mittente --- crittografa con la tua chiave pubblica ---> Testo cifrato
- Testo cifrato --- invia a ---> Te
- Te --- decrittografa con la tua chiave privata ---> Messaggio

L'obiettivo generale della crittografia a chiave pubblica è dimostrare di avere un segreto senza doverlo mostrare a nessuno. E il segreto è la tua chiave privata.
Non dover condividere la tua chiave privata è uno dei vantaggi di questo tipo di crittografia.

Firma digitale:
Quando usi la tua chiave privata per firmare un messaggio, crei una firma digitale.
Ciò può dimostrare che il messaggio è stato scritto dal proprietario della chiave privata. È un tipo di autenticazione.

[IMMAGINE]

Indirizzo Bitcoin:
L'indirizzo che utilizziamo in Bitcoin per ricevere denaro è in realtà una derivazione della tua chiave pubblica.
Quando invii denaro a un indirizzo, stai dicendo "i bitcoin possono essere utilizzati dal proprietario delle chiavi corrispondenti a questo indirizzo".

[IMMAGINE]

Transazioni Bitcoin

Il tipo più comune di transazione Bitcoin è chiamato Pay to Public Key Hash (P2PKH), che fondamentalmente significa "Paga a un indirizzo".
Una transazione è essenzialmente un messaggio che utilizza la crittografia a chiave pubblica per assicurarsi che la persona giusta possa sbloccarlo.

[IMMAGINE]

Pagamento a Mattia:

[IMMAGINE]

Ecco un esempio con la dinamica semplificata di come funziona la crittografia a chiave pubblica in una transazione Bitcoin P2PKH:
1) Alice ti invia bitcoin:
- Alice "blocca" i bitcoin con la condizione che venga presentata la firma corretta
- Trasmette la transazione alla rete
- La transazione viene convalidata dai nodi della rete e minata
2) Spendi i bitcoin:
- Sblocchi i bitcoin rispondendo alla condizione precedente (firmando la transazione) e poi blocchi i fondi con una nuova condizione (che venga presentata la firma del destinatario)
- Trasmetti la transazione alla rete
- La transazione viene convalidata dai nodi della rete e minata




---



---
