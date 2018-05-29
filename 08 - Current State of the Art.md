# Current State of the Art

Especially following the collapse of the DAO, the need for mediation and arbitration on blockchain-based smart contracts has spurred teams to investigate what frameworks may be developed to build this necessary part of the blockchain ecosystem. Two projects in particular serve as compelling starting points for discourse and improvement, and have been taken into consideration while developing Juris.

#### DAMN

In May of 2016, pre DAO hack, Third Key Solutions -- founded by Pamela Morgan and notable Bitcoin advocate Andreas M. Antonopoulos -- released a proposal for DAMN: a Decentralized Arbitration and Mediation Network[^12]. The proposal was brief, and outlined an open source project intended to create a network similar to Juris on many fronts, in particular the adherence to United Nations arbitration standards. Their proposal was submitted to the DAO for funding approval and sentiment regarding the proposal was largely positive[^13]. The last activity on the project Github repo was in late May of 2016, with the DAO hack taking everyone’s attention shortly thereafter.

#### Kleros

Released as a concept whitepaper in 2017[^14], Kleros represents a more focused look R the idea of smart contract arbitration, and presents an example of the use cases for a decentralized arbitration system. Additionally, it outlines the attack risks against such a system \(bribery, surreptitiously controlling the majority of tokens, and a Sybil Attack\). Drawing game theory underpinnings from Ethereum founder Vitalik Buterin’s initial proposals of SchellingCoin, Kleros proposed to incentivize arbiters to collaboratively vote as to reach "truth," where truth \(or a proxy of it\) must emerge from a costly voting process and incentives apropos. Game theory challenges emerge when voters are asked to vote how they think everyone else will vote. This problem, known as the Beauty Pageant Problem, remains unaddressed in both SchellingCoin and Kleros. Additionally, Kleros calls for the top-down segmentation of the judicial system into sub-categories and sub-courts of dispute. Escalation in the Kleros system calls for an increasing number of arbiters for each stage of a case, with those arbiters selected via cryptographic hash function. All of these factors impose an unnecessary operational overhead on the project.

#### Platform Specific Dispute Resolution Tools

Part of the initial excitement for smart contracts was the elimination of ambiguity and human judgement from the process of contract execution. But most of the community has retreated from that view, and disputes in many of today's most promising blockchain applications involve matters of judgement \(crowd-funding, freelancing, content licensing, etc\). Did a crowd-funded team hit their milestone? Did a freelancer deliver what they promised? All judgement. 

The best players in each of these spaces have recognized that there will be disputes, and have outlined dispute resolution procedures. However, these platform specific tools are often customer support oriented and not built to sound legal standards. Many lack any incentives, many are vulnerable to simple attack patterns, and all necessarily use members of their general community, or support personnel to adjudicate disputes. Not only do these systems frequently fail, or result in unsatisfactory wait times, but the decisions delivered by customer support or the community will still be open to legal challenge after the fact. This then becomes a source of possible liability for the platform itself.

Juris is first-and-foremost a tool for these platforms to get out of the business of dispute resolution so that they can focus on their core value. By integrating Juris into their platform, they are outsourcing a highly technical, possibly existential problem.

[^12]: [https://github.com/thirdkey-solutions/damn/blob/master/proposal.asciidoc](https://github.com/thirdkey-solutions/damn/blob/master/proposal.asciidoc)
[^13]: [https://dao.consider.it/decentralized-arbitration-and-mediation-network?results=true](https://dao.consider.it/decentralized-arbitration-and-mediation-network?results=true)
[^14]: [https://medium.com/kleros/kleros-a-decentralized-justice-protocol-for-the-internet-38d596a6300d](https://medium.com/kleros/kleros-a-decentralized-justice-protocol-for-the-internet-38d596a6300d)