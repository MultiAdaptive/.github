# Multichain

**[Our Data Availability solution on BTC and ETHEREUM](https://github.com/MultiAdaptive/document/blob/main/Domicon-Data-Availability-Solution.md)**

MultiAdaptive Testnet v1 on Ethereum is live as of March 1, 2024

Join MultiAdaptive as a broadcast node -> [click here](https://github.com/MultiAdaptive/document/blob/main/pages/add-domicon-from-source_english.md)

Build a new OP rollup with MultiAdaptive as the DA layer -> [click here](https://github.com/MultiAdaptive/document/blob/main/domiconRollup/Domicon-OP-Stack-EN.md)

Build a new Orbit rollup with MultiAdaptive as the DA layer -> [click here](https://github.com/MultiAdaptive/document/blob/main/domiconRollup/Domicon-Orbit-anytrust-EN.md)

Use existing rollup with MultiAdaptive as DA layer -> [click here](https://github.com/MultiAdaptive/document/blob/main/domiconRollup/publishDA-EN.md)

Find out more about MultiAdaptive -> [click here](https://github.com/MultiAdaptive/document)

A brief introduction to KZG polynomial commitment scheme -> [click here](https://github.com/MultiAdaptive/document/blob/main/KZG-Polynomial-Commitments.md)

## 1. What is MultiAdaptive (previously Domicon)?

MultiAdaptive is an Ethereum bandwidth scaling solution designed to provide secure and efficient **data availability** (DA) services for the Layer 2/Rollup ecosystem. It consists of a broadcast layer responsible for data broadcasting and a storage layer responsible for long-term data storage. Domicon's ingenious utilization of the Kate-Zaverucha-Goldberg (KZG) polynomial commitment enables data broadcasting, data sampling, and aggregated auditing of full data, truly ensuring the integrity and reliability of data in propagation and storage.

Build Rollup  with MultiAdaptive as the DA  layer will get the fastest data confirm experience, the most secure data protection, and the most cost-effective data fees.

## 2. Why MultiAdaptive?

### 2.1 MultiAdaptive is the safest

**More secure native bridge**

Most DA projects, such as Celestia, need to bridge the user's storage certificate across the chain to Ethereum to complete the final data confirmation. This increases the security assumptions required to remain honest across chain bridges. In past experience, cross-chain bridges have been easily targeted by hackers. In the DA scenario, hackers can gain the full power of the project sequencer by tampering with DA data, thereby profiting from it, resulting in the loss of user assets.

MultiAdaptive itself is built using the Rollup method, with its own native cross-chain bridge, which binds the security of DA and Ethereum, bringing the most secure data confirmation solution to clients.

**The safest way to audit**

How to store data safely and for a long time is a problem that all DA solution providers need to face.

Existing DA projects all claim to use sampling or partial challenge for random audit mode, and then audit the data through multiple challenges to ensure that the data reaches 99% storage security.

But in fact, DA data is different from general data. For example, if a picture loses some pixels, it does not affect the viewing and use of the picture. The purpose of long-term preservation of DA data is to reconstruct the world state for replay, so the loss of any data will cause the replay to fail. Therefore, we believe that it is meaningless to conduct random audits on DA data.

MultiAdaptive adopts a deterministic audit scheme and uses the KZG aggregation scheme to complete the audit on 10T of data within 1 second and generate a certificate to confirm the security of the data with 100% probability.

### 2.2 MultiAdaptive is the fastest

In the known DA layer projects, data and data commitments are processed separately. Generally speaking, the final data commitment will be uploaded to Ethereum, and the data will be saved in the DA layer project's network. The common process is that the project party first stores the data to DA, and after DA confirms receipt of the data, the data commitment and storage certificate are sent to Ethereum to confirm the data.

MultiAdaptive adopts an integrated processing solution and encourages broadcast nodes to provide data confirmation services.

Users only need to hand over the data and data commitment to the broadcast node, and the broadcast node will help the user upload the data commitment to Ethereum and return the corresponding txhash to the user.

Users only need to check that the transaction has been confirmed on the Ethereum network, and then the data processing can be completed.

### 2.3 MultiAdaptive is the most lightweight

In MultiAdaptive's network, we have designed an incentive mechanism to encourage and supervise nodes to provide external services. 

Taking the broadcast node as an example, if it does not undertake the responsibility of broadcasting and does not broadcast data, its deposited tokens will be slashed; if it provides external data confirmation services, it will receive additional token rewards.

MultiAdaptive uses Ethereum as its governance layer, and all governance activities are completed on Ethereum. Therefore, users can obtain the external information of all MultiAdaptive broadcast nodes and storage nodes by querying the relevant contracts of MultiAdaptive on Ethereum.

In other words, when using MultiAdaptive services, there is no need to build your own nodes or use third-party nodes like other blockchain infrastructures.

You only need an Ethereum node to enjoy MultiAdaptive services smoothly. Whether you want to build a new rollup using MultiAdaptive or transfer the existing DA to Domicon, it is an easy task.
