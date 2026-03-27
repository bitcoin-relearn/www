
## Why run a node


**What is a Bitcoin node?**
A Bitcoin node is an application that run on your computer.
It downloads and verifies all transactions since the inception of Bitcoin. It gives you the ability to broadcast your transactions and check the status of them.

**Why run a Bitcoin node?**
- Verify your own balances and incoming transactions, no trusted third paties
- Broadcast your own transactions, without censorship
- Privacy
- Adds to the decentralisation of the network
- You are not earning or mining bitcoin running a node

**Ways to run a Bitcoin node**
https://thebitcoinhole.com/bitcoin-nodes
https://pcpartpicker.com/products/
https://ubuntu.com/download/server
(Dell Optiplex USFF, 8GB RAM, 2TB SSD. Bitcoin Core 700GB, Electrs 50GB)

BIOS
- boot sequence
- power management

**Pros**
- Minimal trusted parties - DIY approach
- No personal or identifiable information stored
- Light weight (both physical and software)
- Silent, small form factor
- Solid uptime / minimal downtime
- Learn new computing skills

**Cons**
- No inbuilt battery/UPS - power outages
- Takes time to learn & understand
- Manual updates and upgrades
- No trusted third parties to rely upon
- Must have physical access to router to plug into






## Electrum Servers
- What is an Electrum Server?
- Why do we need one?
- Choosing an Electrum Sever
- Diagram of typical setup

**What is an Electrum Server?**
- An electrum server is an additional database that sits upon Bitcoin Core and serves information about the status of the blockchain

**Why do we need one?**
- The Bitcoin Core database (700GB) is inefficient, slow and difficult to query against.
- An electrum sever is an efficient database, that can be queried quickly and by address.

**Choosing an Electrum Sever**
- Electrum Rust Server (electrs)* (trade off between disk space and wallet query requirements)
- ElectrumX
- Fulcrum

**Diagram of typical setup**
Hardware wallet holds private key
sparrow wallet on existing PC holds public key
Sparrow wallet queries electrum server
Electrum server is fed up to date information from Bitcoin Core