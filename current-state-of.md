## Current State of the Art

Especially following the collapse of the DAO, the need for mediation and arbitration on blockchain-based smart contracts has spurred teams to investigate what frameworks may be developed to build this necessary part of the blockchain ecosystem. Two projects in particular serve as compelling starting points for discourse and improvement, and have been taken into consideration while developing Juris.

#### DAMN

In May, 2016, pre DAO hack, Third Key Solutions, founded by Pamela Morgan and notable Bitcoin advocate Andreas M. Antonopoulos released a proposal for DAMN: a Decentralized Arbitration and Mediation Network[^1]. The proposal was brief, and outlined an open source project intended to create a network similar to Juris on many fronts, in particular the adherence to United Nations arbitration standards. Their proposal was submitted to the DAO for funding approval and sentiment regarding the proposal was largely positive[^2]. The last activity on the project Github repo was in late May, 2016, with the DAO hack taking everyone’s attention shortly thereafter.

#### Kleros

Released as a concept whitepaper 2017, Kleros represents a more focused advance of the state of the art in the underlying reasoning of smart contract arbitration. Drawing its game theoretic underpinnings on Ethereum founder Vitalik Buterin’s initial proposals of SchellingCoin, Kleros proposed to incentivize arbiters to collaboratively vote as to reach truth, where truth \(or a proxy of it\) must emerge from a costly voting process and incentives apropos. Juris seeks to improve on several of the components outlined by Kleros. For example, game theoretical challenges emerge when voters are asked to vote how they think everyone else will vote. This problem, known as the Beauty Pageant Problem, remains unaddressed in both SchellingCoin and Kleros. Additionally, the top-down segmentation of the judicial system into sub-categories and sub-courts of dispute proposes an unnecessary quantity of operational overhead on the project, as does the selection of arbiters according to a cryptographic hash function. Kleros does present well an example of the use cases for a decentralized arbitration system, and outlines the attack risks against the system \(bribery, surreptitiously controlling the majority of tokens, and a Sybil Attack\).

#### Platform Specific Dispute Resolution

Part of the initial excitement for smart contracts, was the elimination of ambiguity and human jusgement from the process of contract execution. But most of the community has retreated from that view[^1] and many of todays most promising blockchain aplications pivot arround matters of judgement \(cround funding, freelancing, content licensing, etc\). Did a croud funded team hit there milstone? Did a freelancer deliver what they promised? The best players in each of these spaces has reconized that the reliance on matters of judgement implies that there will be disputes, and have therefore outlined dispute resolution \(DR\) mechanisms. However, these platforms are not at heart about DR and they have accordingly given little attention to design of their DR systems. Many lack any incentives; many are vulnerable to simple attack patters; and all nessesarily use members of thier general comunity to ajudicate disputes.

Juris is first-and-formost a tool for these platforms to get out of the side business of DR, so that they can focus on thier core value. By integrating Juris in to thier platform, they are outsoursing a highly technical existential problem.

[^1]: https://github.com/thirdkey-solutions/damn/blob/master/proposal.asciidoc

[^2]: https://dao.consider.it/decentralized-arbitration-and-mediation-network?results=true

