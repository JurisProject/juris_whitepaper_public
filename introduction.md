## Introduction

### Abstract

Contract disputes occur. **Off the blockchain**, we resolve them through the court system or a form of Alternative Dispute Resolution \(ADR\). The more structured form of ADR, called “arbitration,” involves the airing of grievances before a panel of neutral jurists, who assess the facts and provide a decision. The power of arbitration is recognized internationally, with ~150 countries required by UN treaty to enforce arbitration judgements. In the United States neutral arbitration is a for-profit business. **On the blockchain**, there does not yet exist a protocol for the fair and efficient resolution of disputes in smart contracts. In this paper we introduce the **Juris Protocol**, an open source arbitration protocol built for the blockchain, and **JurisCoin \(JRS\),** a utility token to facilitate and incentivize Juris platform activity. Through the use of Juris' Mediation Tools, Contract Development Kit \(CDK\), and Adjudication Protocol, the disputed outcome of any smart contract may be contested through United Nations compliant neutral arbitration. The Juris Protocol combines a novel reputation system based on prior certification, ongoing community activity, machine learning, and graph analysis. The protocol is intended to facilitate the inclusion of both professional human arbiters and a larger community of novices. In this paper we review Juris' improvements on the current state of the art, explore Juris as a framework, and describe a governance model for launch and future development. As a platform, Juris seeks to improve both the safety and security of smart contracts. This will reduce the risk in the transition of traditional transactions onto blockchain-based alternatives and, in turn, increase broad adoption of blockchain technology.

### Calamity on the Blockchain

In May 2016, the DAO, or “Decentralized Autonomous Organization” launched the largest crowdfunding campaign in history.[^1] Not just on the Ethereum Blockchain -- but **ever**. They raised 150 million dollars worth of Ether by the end of 28 days. But, their success was short lived: on June 17th, 2016, we saw what happens when the intention behind a “Smart Contract” diverges from its codified implementation. Several errors inside the smart contract code written by the DAO team allowed a single bad actor to drain 50 million dollars worth of Ether from the DAO wallets overnight. The remainder of the funds were saved only because a group of “white hat” hackers moved them to a friendly wallet via the same exploit.

The breach was significant enough to drastically undermine investor confidence in Ether. Immediately following the DAO's theft, Ether's price cratered and lost nearly 63% of its value. Beyond just a price drop, the impact of the DAO was forceful enough to crack Ethereum into two entire separate blockchains: Ethereum, on which the DAO transactions were erased, and Ethereum Classic, where they were not. The split took place because this "hack" wasn't strictly illegal, or even really a hack. These bad actors didn't break anything; they noticed errors and exploited them to make the contract function in a way other than intended. The community was split on how to handle this: should they stick to the "four corners" of the contract terms, or stick to the intent of the smart contract code? After much debate there was a "Hard Fork" of the Ethereum Blockchain[^1]. The fork happened because the Ethereum Foundation decided to honor the intent of the contract over the literal code written. This type of dispute is not new. **This is contract law.**

Had the set of smart contracts that constituted the DAO been constructed with an adjudication platform available as insurance \(in the way court systems safeguard ink and paper contracts\) the events that unfolded, ranging from the loss of market cap to the “Hard Fork” of Ethereum[^2], may have been preventable. It is to avoid catastrophes like these, and engender a better confidence in smart contracts at large, that we propose **Juris**: a decentralized adjudication platform for blockchain smart contracts.

### Mission

* To make “smart contracts” on all blockchains safe, robust, and human.  
* To create a protocol, token, and reputation system for fair dispute resolution, justice, and judgement.  
* To make justice as efficient, effective, and accessible as the Internet.











