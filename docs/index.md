---
title: ConsenSys Rollups
---

# ConsenSys Rollups

## What is ConsenSys Rollups?

ConsenSys Rollups is a framework for implementing [rollups](Concepts/Rollups/Overview.md) for the Ethereum blockchain.
Rollups are layer 2 scaling solutions that improve the scalability of Ethereum networks by performing mass transaction
validation offchain.
ConsenSys Rollups supports any EVM-based protocol, including proof of work (PoW) and proof of authority (PoA) protocols.

ConsenSys Rollups currently implements [partially anonymous rollups](Concepts/Rollups/Partially-Anonymous-Rollups.md),
with plans to add support for other types of rollups (consensus-rollups and optimistic-rollups).

![Architecture](Images/ConsenSys-Rollups-Overview.png)

ConsenSys Rollups introduces a centralized actor called an operator which consists of a manager and engine.
The operator receives and executes transactions, manages the state, and submits batch transactions
to the Ethereum network. The blockchain nodes do not re-execute the transactions.

![ConsenSys Rollups workflow](Images/Operator_Flow.png)

## Why use ConsenSys Rollups?

ConsenSys Rollups provides approximate speeds of 10,000 transactions per second (TPS)
with 100 million accounts, on a private blockchain with immediate finality producing 1 block per
second.
