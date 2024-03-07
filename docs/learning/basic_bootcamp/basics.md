---
title: 'Lesson 1: Blockchain Basics'
icon: material/flag-checkered
---

### Basics

!!! tip

    The first thing you need to invest is your time. Since the publication of the course, many things have evolved or appeared, this first chapter is much more important than it seems, take time, several days if necessary, to discover this ecosystem and things that are not mentioned in the video such as [Starknet](https://www.starknet.io/en), Zero-knowledge proof, Account Abstraction, etc.

!!! warning
    In case you also intend to invest, take the time to understand the current rules associated with your Country regarding cryptocurrency taxation

In the opening chapter of Patrick Collins course, we delve into the transformative world of smart contracts and their pivotal role in the **blockchain** landscape. This section, guides us through the evolution and potential of blockchain technology and its applications. Here's a refined overview of the key discussions:

**Web3** marks the dawn of a new internet era, a paradigm shift towards **decentralized networks**. This revolutionary concept aims to empower users with sovereignty over their data, identity, and transactions, moving away from the traditional centralized internet services to a more open, blockchain-based framework. This shift paves the way for direct, intermediary-free interactions between individuals.

Drawing an intriguing comparison, **Bitcoin**(1) is portrayed as the digital equivalent of gold. This analogy serves to introduce blockchain technology and Bitcoin, its first and most notable application. Much like gold, Bitcoin is valued for its scarcity, decentralization, and role as a digital store of value, free from the control of any single entity.
{ .annotate }

1.  :ninja: The creator of Bitcoin is Satoshi Nakamoto, his identity is unknown

The narrative then transitions to **Ethereum** (1), a trailblazing blockchain platform that builds upon the basic principles of blockchain, much like Bitcoin, but introduces the innovative concept of **smart contracts**. These are contracts that are automatically executed, with the terms directly embedded in code, facilitating transactions and agreements without the need for trust.
{ .annotate }

1.  :man_technologist: Ethereum's creator is Vitalik Butherin

Ethereum is celebrated for being the most popular platform for deploying smart contracts, thanks in part to **Solidity**, its dedicated programming language. This segment underscores Ethereum's significant influence on the development and proliferation of decentralized applications (dApps).

**DApps** are explored as decentralized applications that operate on a blockchain network. Typically anchored by smart contracts, these applications enable peer-to-peer transactions without central oversight, embodying the essence of decentralized protocols and smart contracts.
The discourse then introduces the idea of hybrid smart contracts, which marry on-chain code with off-chain data and computations. This innovative approach broadens the scope of smart contracts, allowing them to engage with the real world and external systems more effectively.

**Chainlink** emerges as a decentralized **oracle** network in this narrative, offering a secure bridge between smart contracts and external data sources. Its blockchain-agnostic nature ensures it can integrate with any blockchain, heralding a future of interconnected smart contracts. The indispensable role of oracles in delivering reliable, tamper-proof data to smart contracts is highlighted.

Finally, smart contracts are eloquently described as "unbreakable promises." This characterization emphasizes their immutable and self-sufficient nature, ensuring that once a smart contract is deployed, it will operate exactly as coded, immune to downtime, censorship, fraud, or interference.

This chapter not only sets the foundation for understanding smart contracts but also paints a vivid picture of their indispensable role in fostering a decentralized, trustless digital ecosystem through blockchain technology.

!!! abstract

    It is possible and preferable to learn more about [Bitcoin](https://bitcoin.org/bitcoin.pdf) and [Ethereum](https://ethereum.org/en/whitepaper/) by reading their respective whitepapers.

    Additional research is also recommended to fully understand the role of [Blockchain](https://andersbrownworth.com/blockchain/), [Smart Contract](https://chain.link/education/smart-contracts), [Hybrid Smart Contract](https://chain.link/education-hub/hybrid-smart-contracts) & [Oracle](https://betterprogramming.pub/what-is-a-blockchain-oracle-f5ccab8dbd72) concept.

### The purpose of Smart Contract

Smart contracts, is like the age-old concept of a "pinky swear", built on the foundation of trust and agreement. However, unlike the simple and purely honor-based promise represented by the intertwining of pinky fingers, smart contracts elevate the concept into the digital realm with a robust, secure, and enforceable framework. This leap is made possible through blockchain technology, which serves as the impartial digital ledger that records, verifies, and executes the terms of a contract automatically, without the need for intermediaries.

<figure markdown="span">
  ![](https://zupimages.net/up/24/10/dlcv.png)
  <figcaption>https://site.ieee.org/sb-ritb/why-are-smart-contracts-so-important/</figcaption>
</figure>

At their core, smart contracts function similarly to traditional contracts by encoding the terms of an agreement. However, the key distinction lies in their execution. Imagine two children agreeing to a pinky swear, where one promises to exchange their toy car for the other's action figure the following day. In the traditional sense, this agreement relies heavily on trust and personal integrity. Should one party renege on their promise, the aggrieved party's recourse is limited, primarily to social sanctions or seeking adult intervention.

Smart contracts revolutionize this concept by embedding the agreement into code. Once the contract's conditions are met, such as the confirmation of the toy car's delivery in our example, the smart contract automatically executes the agreed-upon action, in this case, transferring ownership of the action figure. This automation not only minimizes the risk of breach but also eliminates the need for a third-party enforcer, thus reducing potential conflicts and costs associated with dispute resolution.

The immutable nature of blockchain technology ensures that once a smart contract is deployed, its terms cannot be altered, much like the unbreakable vow of a pinky swear. However, unlike the latter, which relies on personal honor, the trust in smart contracts is placed in the technology's capability to impartially and reliably execute the agreement. This technological trust is underpinned by the decentralized and transparent nature of the blockchain, where each transaction is verified by a network of computers and recorded across multiple copies of the ledger, making fraud or interference exceedingly difficult.

The evolution from simple, trust-based agreements like the pinky swear to complex, code-enforced smart contracts signifies a monumental shift in how agreements are made and upheld. While the essence of making a promise remains unchanged, the mechanisms to ensure its fulfillment have been dramatically enhanced. This advancement not only streamlines transactions of all kinds but also introduces a new era of trust and security in agreements, moving beyond the limitations of human integrity to the reliability of code.

### Purpose of Gas

Gas refers to a unit that measures the amount of computational effort required to execute operations, like transactions and smart contracts, on a blockchain network. The concept of gas is crucial in managing and maintaining blockchain networks, especially those that support complex operations and decentralized applications (dApps).

**Resource Allocation:** Gas serves as a mechanism for allocating resources on a blockchain network. Since every operation, from a simple transaction to the execution of a smart contract, requires computational power provided by the network's nodes, there needs to be a way to limit and pay for these resources. Gas ensures that users pay for the computing energy they consume, preventing wasteful or malicious use of network resources.

**Transaction Processing:** Gas is used to prioritize transactions. In networks like Ethereum, users can specify a gas price for their transactions. Miners, who validate and add transactions to the blockchain, prioritize transactions with higher gas prices because they stand to earn more from these transactions. This system creates an efficient market for transaction processing, where users can choose how much they are willing to pay to have their transaction processed faster.

**Security:** Gas also plays a crucial role in network security. By requiring a fee for every computation, the gas system discourages spam transactions and potential denial-of-service (DoS) attacks. If an attacker attempts to flood the network with transactions or execute a smart contract loop indefinitely, they would need to supply a significant amount of gas, making such attacks prohibitively expensive.

**Smart Contract Execution:** For smart contracts, gas is essential not just for deploying them onto the blockchain, but also for executing their functions. Each operation within a smart contract has a base gas cost, and complex contracts require more gas to execute. This ensures that developers optimize their code to be as efficient as possible, reducing unnecessary computational strain on the network.

When initiating a transaction, users set a gas limit and a gas price. The gas limit is the maximum amount of gas the user is willing to consume for the transaction. The gas price is the amount of the blockchain's native cryptocurrency (e.g., ETH in Ethereum) that the user is willing to pay per unit of gas. The total transaction fee is the product of the gas consumed and the gas price.

In some cases, not all the gas limit set for a transaction is used. Unused gas is refunded to the user's account. This system encourages users to set a realistic gas limit for their transactions.