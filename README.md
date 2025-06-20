# Project: Deploying a Private Ethereum Blockchain

This repository documents a project from the **41900 Cryptography** course that involved building and interacting with a private Ethereum blockchain network from scratch. The project demonstrates a practical understanding of how core cryptographic concepts like hashing and digital signatures are combined to create a functional Proof-of-Work (PoW) blockchain.

The primary tool used was **geth (Go Ethereum)**, the official command-line interface for running a full Ethereum node.

### Project Workflow & Key Stages

The project involved setting up a single-node private network and performing fundamental blockchain operations:

**1. Initializing the Blockchain (The Genesis Block):**
*   Created a custom `genesis.json` file to define the initial state of the blockchain. This file configured parameters such as the `chainId`, `difficulty` (set low to accelerate mining), and initial account allocations.
*   Used `geth init` to process the genesis file and create the very first block, laying the foundation for the private network.

**2. Account Management and Mining:**
*   Used the `geth` JavaScript console to create multiple new Ethereum accounts (key pairs).
*   Designated one account as the `etherbase`, the recipient for mining rewards.
*   Initiated the mining process, which began solving the PoW puzzle to create new blocks and secure the network. Successfully observed the block number increasing.

**3. Executing Transactions:**
*   Verified account balances using `eth.getBalance()`.
*   Constructed and sent a transaction to transfer Ether from the `etherbase` account to a second account.
*   Observed the transaction entering the transaction pool (`txpool`) and subsequently being included in a new block by the miner.
*   Confirmed the success of the transaction by checking that the recipient's balance had increased.

### Core Skills & Technologies Demonstrated:

*   **Blockchain Fundamentals:** Practical knowledge of blocks, chains, transactions, and consensus mechanisms.
*   **Ethereum & geth:** Proficiency with the Go Ethereum client for node operation, account management, and network interaction.
*   **Proof-of-Work (PoW):** Hands-on experience with initiating and observing a PoW mining process.
*   **Cryptocurrency Transactions:** Understanding of how value is transferred on a blockchain network.
*   **Private Network Configuration:** Ability to define and launch a custom blockchain using a genesis file.
*   **Command-Line & JS Console Interaction:** Interacting with a complex application programmatically.

---
*This project was completed as part of the 41900 Cryptography course. The full report and the `genesis.json` file are included in this repository.*
