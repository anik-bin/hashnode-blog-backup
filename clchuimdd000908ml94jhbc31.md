---
title: "What Is Proof Of Work (POW) In Blockchain"
seoTitle: "What Is Proof Of Work (POW) In Blockchain"
seoDescription: "Proof of Work is a consensus mechanism used in blockchain networks to validate transactions. Learn more about it by reading the article"
datePublished: Wed Jan 04 2023 16:00:16 GMT+0000 (Coordinated Universal Time)
cuid: clchuimdd000908ml94jhbc31
slug: what-is-proof-of-work-in-blockchain
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1672848440448/eef697a1-bb63-4526-a2e0-19bff1becb9e.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1672848462227/fd1dee6f-ac4f-4a7d-b41c-c2105e77058d.png
tags: blockchain, bitcoin, ethereum

---

Proof of Work is a consensus mechanism cryptocurrencies use to validate transactions and add new blocks in a [blockchain](https://blog.aniketbindhani.com/what-is-blockchain-technology-explained) network.

In a blockchain network there are nodes all around the world that participate in the network and ensure that the network is stable and running correctly. <mark>This ensures the decentralisation of a network</mark>.

# What is Consensus Mechanism

First, let us understand what a **<mark>consensus mechanism</mark>** is. The major problem that bitcoin solved in decentralisation was the **double spending** problem. Double spending means that suppose Anil sends Pooja a bitcoin and then again sends the same bitcoin to Shubham before the transaction is recorded. Since bitcoin is a digital currency it was a very big problem. This would decrease the value of the coin.

The double spending problem does not happen with physical currency because we have banks maintain a ledger to verify the transactions but in a blockchain network there is no middleman.

So, bitcoin introduced Proof of Work which is a consensus mechanism in which all the nodes participating in the network verify all the transactions that are happening and choose which transactions are legitimate and add them to the network.

*Let us discuss how this process works more in detail*

## How does this work?

First, you need to know how a transaction happens in a blockchain

You can refer [here](https://blog.aniketbindhani.com/what-is-blockchain-technology-explained). This article has explained this in detail.

Now each node is given a complex mathematical puzzle that they need to solve and whoever solves first is rewarded with bitcoins. In this way, new coins are generated in the market and blocks are added to the blockchain. Some blockchains have different processes but overall the idea is the same.

A miner needs to find a **<mark>NONCE</mark>** ( number only used once ) by using computational power and if he/she finds it the transaction is validated by all the other nodes present in the network and if everyone agrees then it is added to the blockchain.

The problem of double spending is solved here since each node maintains a ledger containing all the transactions which are updated whenever a transaction happens. So even if one node tries to double spend, the transaction would get invalid as the ledgers would not match with the rest of the nodes.

This is known as Proof of Work.

# Downsides

The proof of Work mechanism requires a lot of computational power to work. The more complex the problem the more power is required. This increases the cost for the miners since more hardware is required and more energy is consumed.

According to some news reports, this is ultimately harmful to the environment since a high amount of energy is consumed by the miners.