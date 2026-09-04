# Private Ethereum Proof-of-Work Lab

A historical university lab documenting a single-node private Ethereum network built with **Geth 1.9.15**. The
exercise was completed for UTS 41900 Cryptography and reflects the Proof-of-Work tooling available in that legacy
environment.

## Lab workflow

1. Defined a custom genesis configuration with a private chain ID and low test difficulty.
2. Initialised a local chain data directory with `geth init`.
3. Created two local accounts through the Geth JavaScript console.
4. Selected an etherbase account and mined blocks in the isolated network.
5. Submitted a test transaction, inspected the transaction pool and resumed mining.
6. Confirmed the resulting transaction and account balances.

```text
genesis configuration
        |
        v
single local Geth node
        |
        +-- account creation
        +-- legacy PoW mining
        +-- local transaction pool
        +-- balance and transaction checks
```

## Evidence

The [lab report](docs/Private-Ethereum-PoW-Lab-Report.pdf) contains the captured commands and results from the
exercise. The original `genesis.json` is not included in this repository; its relevant configuration is visible in
the report.

## Historical scope

This repository demonstrates foundational blockchain mechanics in an isolated learning environment. It does not
represent a current Ethereum deployment pattern, smart-contract application or production blockchain network.

