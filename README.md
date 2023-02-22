# Cryptography

## Blockchain Cryptograhy Docuementation

## Blockchains

Purpose of Blockchain :

- No person or organization can control a particular process

Why Blockchain? :

- Blockchain was invented to solve for trust and to create a system that is completely safe and secure from various harms

Cryptographic Hash Functions :

- Conversion of any input of any size converted into fixed size output is known as function of Cryptographic Hash Function
- Best method for hashing is Modulo Division Method (according to Wikipedia)

# Digital Signatures

Public Key Cryptography :

Cryptography

- Cryptography in early stages was study of encrypting message so that they could not be decrypted even if intercepted and it was used for important secrets.
  Symmetric-Key Cryptography :

- Symmetric-key cryptography refers to encryption methods in which both the sender and reciever share the same key

Personal Computing

- Public Key was introduced to make the blockchain more secure rather than sharing keys directly.

- Public Key Cryptography is considered as Asymmetric Encryption in that only one party has access to private key.

- And only the person having key can decrypt the message sent to him!

RSA and ECDSA Algorithms

- Both Algorithms used for public key cryptography

- RSA algorithm is very difficult to be decrypted and is still an unsolved mystery in Computer Science.

- ECDSA algorithm uses Elliptic Curves and provide same level of security as other public key algorithms with smaller key sizes

- It is the Digital Signing Algorithm used by Bitcoin, specially the `secp256k1` curve

- `secp256k1` is used in Bitcoins public-key crpytography. `secp256k1` was constructed in a special non-random way which allows for especially efficient computation. As a result, it is often more than 30% faster than other curves if the implementation is sufficiently optimized.

- _Diffie-Hellman Key Exchange_ is used to get that Secret Key

# Proof of Work and Mining

Consensus Mechanisms :

- Consensus means coming to general agreement.
- Blockchain consensus typically means at least 51% of nodes are in agreement over the current global state of the network.

Proof-of-work and Minning :

- POW networks will typically have some sort of target_difficulty
- If a Miner wants to add a new block then must find a POW lower than the network target difficulty.
- If Miner follows all consensus rules then his block gets valid and miner gets paid for mining a valid transaction.

How does Bitcoin use Proof of Work?

- POW act as a security of the Bitcoin system. Thousands of nodes are working to find hashes of data. And if you want to hash data more than other miners then you should come up with more computing power than all the nodes in the entire system.
- This is referred to as a 51% attack because you need 51% of the total hashing power in the network.

Hashcash Concept :

- Hashcash is a POW system used to limit E-mail spam and denial of service attacks.
- Hashcash is a cryptographic hash based POW algorithm that requires a selectable amount of work to compute, but the proof can be verified efficiently.

# Blockchain Structure

Blockchain Architecture

- A blockchain is a distributed database of a list of validated blocks.
- Collection of distributed nodes arranged as a peer-to-peer network without any supernode is a structure of blockchain and due to Consensus mechanism Bitcoin network decides validity of new data based on who is able to produce a valid POW.

- Mallory : Crypto term of malicious actor!

# Blockchain Storage

## UTXO and Accound Models

- UTXO stands for "Unspent Transaction Output". Bitcoin uses the UTXO model to keep track of user balances.
- Ethereum and EVM chains use the account model to keep track of user balances.

For Merkle Tree Data Structure in Blockchain : [Click Here](https://www.linkedin.com/posts/aadit-palande-839a8b22a_blockchain-cryptocurrency-bitcoin-activity-7016400048452169728-1Dne?utm_source=share&utm_medium=member_desktop)

Merkle Proofs :

- A merkle proof confirms specific transactions represented by a leaf or branch hash within a Merkle hash root

# Patricia Merkle Tries

Important Ethereum Block Properties :

- State Root
- Transaction Root
- Receipt Root

Trees in Ethereum :

- Ethereum makes use a data structure called a radix trie also referred to as a Patricia trie or radix tree and combines this data structure to form Patricia Merkle Tree.

- Patricia Merkle Trees is a data structure that stores key-value pairs, just like hash table. It allows us to verify data integrity and the inclusion of a key-value pair.

# Introduction to Ethereum

What is Ethereum?

- It is an open source, globally decentralized computing infrastructure that executes programs called smart contracts.

Properties of the Ethereum Computer :

- Ethereum -> Truly Global Singleton : Not located at one location

- Censorship Resistance -> No one can govern Ethereum Computer

- Ethereum -> Ubiquitous and Accessible

- Natively Multi-User

- It is Verifiable and Auditable

**Difference between Ethereum and Bitcoin**

| Types                   |            Ethereum             |                     Bitcoin |
| :---------------------- | :-----------------------------: | --------------------------: |
| Consensus Mechanism     |         Proof of Stake          |               Proof of work |
| Accounting System       |          Account Model          |                  UTXO Model |
| Public Key Cryptography |    secp256k1 elliptic curve     |    secp256k1 elliptic curve |
| Stale/Orphan Blocks     |            Rewarded             |                Not Rewarded |
| Block Time              |     Approx every 12 seconds     |     Approx every 10 minutes |
| Network Difficulty      |      Adjusted every block       |           Every 2016 blocks |
| Language Support        | Turing Complete smart contracts | non-Turing Complete scripts |

**EIP** :
If there are any changes or any update is there in EVM (Ethereum Virtual Machine) , EIP (Ethereum Improvement Proposal) stores the history of updates.

**POS**

1. More Secure
2. Less energy intensive
3. Greater scalability

**JSON RPC**
It is the bridge we to connect any dApp we use or build to an Ethereum node, and thus the greater Ethereum network.

**Nodes and Clients**

A "node" is any instance of Ethereum client software that is connected to other computers also running Ethereum software, forming a network. A client is an implementation of Ethereum that verifies data against the protocol rules and keeps the network secure.

**Post Merge Ethereum**

1. Execution Client : listens to new transactions broadcasted in the network, executes them in EVM, and holds the latest state and database of all current Ethereum data.
2. Consensus Client : implements the proof-of-stake consensus algorithm, which enables the network to achieve agreement based on validated data from the execution client.
