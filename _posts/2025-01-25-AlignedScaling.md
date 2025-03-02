---
title: 'On the Road to Aligned Scaling'
date: 2025-01-25
permalink: /aligned-scaling
tags:
  - Based
  - Blobs
  - Pectra
---

The best way to end any kind of week is with hopeium. And that’s what we got this Friday.

<br>

### [Vitalik’s post on scaling L1 & Solutions](https://vitalik.eth.limo/general/2025/01/23/l1l2future.html)

### Blob Speak

First up: blobs limiting Etherum’s scaling. Blob amount is critical to scale transactions on Ethereum. A 2x increase om blobs will come with Pectra, another 2x with Fusaka, and 8x eventually with PeerDAS.

In the mean time: all validators should increase the gas limit, as it still remains an individual validator parameter. Signaling to [pump the gas](https://pumpthegas.org/) is in an all time high with [41% validators adopting more than 30M gas limit](https://gaslimit.pics/).

<br>

### Improvements paths for L2s

Next: the rollup landscape with multiple implementations has given us composability and UX issues. How can we ensure L2 scale L1 as originally intended?

* Security:
    * Get L2s to Stage 2 and improve their verifiability with multiprovers and formal verification
    * Develop Native Rollups, where the EVM state transition function verification happens in protocol with EVM precompiles, ensuring flexibility in implementation.

* Interoperability
    * Addresses should have identifiers for both account + chain it lives on (aka. chain specific addresses).
    * Cross-chain bridges and messages, and synchronous reads.
    * Develop ZK-EVM provers and fast proof aggregation – Can we make this happen with zkASICS?
    * Based rollups and Shared Sequencing

* Ethonomics
    * Cement ETH as the primary asset
    * Ensure MEV flows back to L1, based rollups development helps here.
    * More blobs, consider a minimum blob price, and blobs as a revenue generator.
    * L2s supporting ETH: with burning or staking % of fees


This wasn’t intended as a TLDR but it became one. My main take away is the focus on ETH the asset, based rollups not as a goal in itself but also as something that can help us get other where we want: a greater alignment in the L1<>L2s relationship, where both support and scale each other.

<br>

## Alignment of L2s with Based Rollups

Sequencing Call #17 happened. It included participation and [testimonies of L2 teams](https://x.com/drakefjustin/status/1882861787491778998) on their vision on Based Rollups and their solidarity with the initiative.

Great highlights of the call was the two biggest L2 teams participation: Optimism and Arbitrum (through a member of Off Chain Labs statement). Their willingness to support based infrastructure will be key for the greater ecosystem’s acceptance and for actual MEV to flow back to L1.

We also got a FABRIC announcement from the team at [Commit Boost](https://github.com/Commit-Boost/).

<br>

## Pectra Date

We have an expected date! March 11ᵗʰ will bring us 2x on blobs. For more, visit [Christine Kim’s write up](https://www.galaxy.com/insights/research/ethereum-all-core-developers-consensus-call-149/) on ACD.

<br>

After weeks of Ethereum and EF drama this felt like a necessary write up. The future is bright.
