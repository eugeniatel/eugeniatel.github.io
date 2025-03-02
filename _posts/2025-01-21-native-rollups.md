---
title: 'Superpowers from L1 Execution'
date: 2025-01-21
permalink: /native-rollups
tags:
  - Native
  - Ultrasound Rollups
---

Almost two years after the [first Based Rollup post by Justin Drake](https://ethresear.ch/t/based-rollups-superpowers-from-l1-sequencing/15016) emerged, the [first Native Rollup post is here](https://ethresear.ch/t/native-rollups-superpowers-from-l1-execution/21517).


## Defining Native Rollups

The post compiles ideas around native rollups, a new type of rollups that use Ethereum for execution.

Native Rollups effectively aim to scale L1 through rollups that use an exact copy of its virtual machine, eliminating the need to keep up with Ethereum upgrades, enjoying Ethereum’s client diversity and benefiting from its security.

> A native execution rollup, or “native rollup” for short, is a rollup which uses `EXECUTE` to verify EVM state transitions for batches of user transactions.


### How does it use an exact copy of the EVM?

Within the EVM a precompile could be exposed that allows for people to deploy copies of the EVM, deploying a native rollup. Each copy can be customized with own fees, own governance mechanism and even sequencer.

The precompile takes as input the previous state root, post state root, gas used and trace. If executing a well formatted `trace` using `gas_used` starting from the previous root results in post root, the `EXECUTE` returns true.


## Based ≠ Native

This post came days after [Uma Roy’s post](https://x.com/pumatheuma/status/1880286929956270261) on “finally getting” Native Rollups and a couple of weeks after the [first Native Rollup Call.](https://x.com/pumatheuma/status/1880286929956270261) I won’t try to explain differences between based and native rollups as both sources explain it clearly.

Instead I’ll leave this quote:

> Based rollups and native rollups are orthogonal concepts: “based” relates to L1 sequencing whereas “native” relates to L1 execution. A rollup that is simultaneously based and native is whimsically called an “ultra sound rollup".


## Native ≠ Execution Shards

Though they might seem the same since they are also copies of L1 EVM, shards are _enshrined_ copies and are non-programmable. Native rollups bring a great benefit that shards are not able to: customization. Native Rollups can exist with custom governance and custom sequencing independant to that of Ethereum.

This also illuminates a path for existing L2s to upgrade into a native or ultrasound version. An opportunity to benefit from L1 security on execution while still retaining some of their qualities.

Justin Drake’s post also goes deeper into the precompile, the execute gas limit (max computational work a block is allowed to consume) and target, and zkVMs. But today’s short post ends here.


### Resources:

* [Sequencing and Preconf Calls (I believe #6 goes into this)](https://www.youtube.com/playlist?list=PLJqWcTqh_zKHDFarAcF29QfdMlUpReZrR)
* [Native Rollup #0 Call](https://www.youtube.com/watch?v=MNtzDe9Ck0c&t=2s)
