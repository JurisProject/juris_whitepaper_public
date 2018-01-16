# The Reputation System

#### Background

The Juris Reputation Blockchain is an evolution of existing systems with significant prior art:

In the digital realm, the problem of reputation has been tackled from many angles, and effective execution has contributed to the success of such platforms as Reddit and Stack Overflow. In real world academic and professional context, we handle the notion of reputation by issuing credentials like degrees or certificates. We track notable publications, awards, or recommendations, and we award higher degrees. In the context of justice and the law, there already exists a well worn hierarchy of certification, experience, and reputation. There are certain bars to be cleared before the practice of law is allowed, with even further hurdles to become a judge and progress from there. Because of this pre-existing system, legal reputation is an ideal first case scenario for a bespoke reputation chain implementation. We will be able to use observations regarding the movement of participants through the legal hierarchy to craft our own system, taking into account the inevitable real world variables like certification.

#### Proof of Judgement

If Juris is to be the go-to adjudication mechanism for smart contracts, parties must have confidence that their cases are arbitrated fairly by reputable and experienced individuals. The system must allow for the on-boarding and advancement of new Jurists. But, inexperienced input on cases must not result in an unfair outcome. Additionally, in order to resist attack, the system must require a minimum demonstration of experience for a Jurist to have material impact on case outcome.

This presents a challenge: how do we gauge fairness and reputability in a decentralized, anonymous, autonomous environment, while acknowledging, but not overemphasizing, proof of previous credentials? As a solution to this challenge, we propose a trust framework—a _reputation system_—tightly integrated with the Juris platform. This framework will be executed as its own blockchain, meant to establish and measure a new metric: _Proof of Judgement._

#### Reputation Systems

A _reputation system_ is a program that enables a community to collaboratively determine the trustworthiness of its members. More formally, a reputation system defines a trust metric, provides the framework for computing that metric, and calls the metric _reputation_.

#### Trust Metrics

The concept of measurable \(or computable\) trust has been studied extensively within the contexts of sociology and computer science, and is known as a _trust metric_. Defined simply, a _trust metric_ is the quantification of the emotion _Trust_. That is, the extent to which one party expects that any other party will do as they promise. However, Trust, being both abstract and subjective, has no formal or universal identity as a numerical quantity. It follows that trust metrics are proxies; they are numerical quantities that attempt to indicate the magnitude of trust between parties in a given context.

The context dependence of trust metrics means that it's exceedingly difficult to directly map existing trust metrics to new systems, while retaining the original metric's meaning[^17]. Therefore, the details of our trust metric will require a lot of tuning and adjustment to the use case, and as Juris matures. Before giving detailed implementation specifics, we will define our priorities and process.

## Priorities for The Juris Repchain

Broadly, the Juris Repchain should have the following qualities:

#### Useful Proxy

**\(1\)** Reputation Score \(henceforth, "Rep"\) must be a useful proxy for the intended trust metric: _an individual's capacity to effectively arbitrate cases._

In the Juris system, Rep gauges the degree to which a person is capable of effectively and fairly rendering a judgement regarding the outcome of a case when presented with details, arguments, and discussion.

#### Verifiable

**\(2\)** Rep must be readily calculable, deterministic, and open.

_Readily calculable:_ This should not be confused with "computationally or algorithmically simple." Instead, we mean **right-sized for the execution engine**. If the execution engine is Ethereum, then "readily calculable" does translate to "computationally simple" due to the cost of computing on the Ethereum platform.

_Deterministic:_ Repeatable Rep computations. Starting from the same base state, the Rep algorithm will always compute the same Reputation for a given point in the Rep transaction log.

_Open:_ Rep algorithm and log of Rep-changing transactions are both public. If Rep computations are readily calculable and deterministic, the Rep transaction logs available and the algorithm known, then anybody can verify the accuracy of reputation scores quickly and easily.

#### Achievable When Warranted

**\(3\)** Earning Rep legitimately should be straightforward, although difficult.

_Straightforward:_ Knowledge of the repchain's implementation is neither necessary nor advantageous for earning Rep.

_Legitimate:_ An individual who, using a single identity, is committed to resolving smart contract disputes through the fair and impartial application of knowledge and judgement, is **earning Rep legitimately**.

_Difficult:_ Earning Rep requires considerable human action.

#### Unachievable When Not Warranted

**\(4\)** Earning Rep illegitimately should be so difficult as to be effectively impossible.

_Illegitimate:_ \(Definition by negation.\) An individual using multiple identities, or multiple individuals using a single identity, who manipulate the outcome of contract disputes through unfair and/or biased application of knowledge and judgement, is/are **earning Rep illegitimately**.

#### Identity-Based

**\(5\)** Rep must be non-transferrable and unsusceptible to commodification.

_Non-transferrable:_ down to the smallest denomination, Rep is permanently tied to one identity \(account\).

_Non-commodification:_ no quid pro quo. The reputation system must have barriers that limit the feasibility of selling an identity/account.

#### Promotes Cooperation

**\(6\)** The system must have a sensible incentive structure. Jurists are rewarded for sound judgement, fruitful contribution, and effective prosecution. Jurists are punished for poor judgement, bad behavior, or extended failure to engage in the system.

_Punishment:_ The system must provide for the increase _and decrease_ of reputation.

_Quantity of engagement:_ Continued engagement with system must be rewarded, and lack of engagement punished.

Q_uality of engagement:_ the system will measure not only the amount of engagement, but the quality and efficacy of that engagement via, among other tools, upvote/downvote systems, and peer review of opinions.

#### Attack-Resistant

**\(7\)** The system must be resistant to malicious actors, sybil attacks, and abuse through collusion.

_Malicious actors:_ The system should be decentralized. Both correctness and incorrectness should be provable.

_Sybil attacks:_ Creating many accounts must be extremely difficult. It must always be more effective to concentrate Rep in one account instead of many.

_Collusion:_ Just as one person with many accounts is less effective than same person with one account, many legitimate accounts with low Rep must be _less_ impactful than one legitimate account with high Rep.

#### Self-Perpetuating

**\(8\)** After initialization, the system should be fully autonomous and decentralized.

_Decentralized:_ as a blockchain based system it should be able to function on a peer-to-peer basis, without the requirement of a central oracle.

_Autonomous:_ Rep is awarded only based on system parameters. There is no way to earn Rep _other_ than taking part in the system, or through providing proof of previous credentials.

## Earning and Computing Juris Reputation

Earning Rep keeps a Jurist in good standing and earning a lot of Rep makes a Jurist eligible to participate in PANELs.

SNAP is structured to provide numerous opportunity for:

**\(1\) **Jurists to demonstrate good judgement, and  
**\(2\)** Jurists to implicitly or explicitly endorse the judgement of other Jurists.

These endorsements can be used as the raw data for a directed weighted graph \(DWG\). By applying graph analytical techniques to these DWGs we can infer our _Trust Metric._![](/assets/IMG_0048.jpg)_Figure 1.11.1_

#### Accounting for the Basics

It is important to take into account a subset of standard best practices, which may have little to do with judgement. Finish what you start. Be polite. Report conflicts of interest. These practices do not really prove that one has good judgement, but failing to do them impacts trustworthiness. So, if a Jurist makes an opening vote, and does not make a final vote, or endorse an opinion, they will lose Rep. If a Jurist is reported for bad, abusive, or clearly biased behavior, they will lose Rep.

#### Contributing to Discussions and Opinions

The structure of measurement in this space will take shape over time, but can begin simply with an upvote/downvote dynamic for comments and questions during SNAP proceedings. As opinions are moved to increasingly collaborative writing processes, the reputation systems can become increasingly fluid. Contributions can be quantified and rated similarly to GitHub repo contributions, with Rep awarded accordingly at the close of the SNAP. Points may be awarded for popular forks, and for merges back into the master. Implicit endorsements can be deduced from the persistence of changes to documents, which can be attributed to the party which committed those changes for the purpose of Rep awards.

#### PANEL Peer Review

PANEL's don't have as many inherent structured opportunities for Jurists to demonstrate their good judgement. They are, by their nature, much more freeform. Therefore in a PANEL, Jurists will endorse each other much more explicitly using peer review following PANEL proceedings. These peer reviews will be structured to elicit meaningful measures of endorsement, as well as feedback for the most skilled of the Jurist pool, allowing them to improve and maintain standing.

## Graph Analysis

All of the implicit endorsements produced during dispute mediation will be modeled as a weighted, directed graph. Rep earned will slowly 'rot' over time, ensuring that the graph remains current, and promotes ongoing engagement. By using various graph analytical techniques \(PageRank, AvoGatoTrust, EigenTrust, etc.\), we will be able to infer Jurists' Rep within the network. There is extensive academic literature on using graph analysis to infer 'trust' and 'reputation' within distributed systems. By drawing on this literature, and balancing different graph analytical techniques, we'll be able to achieve the goals set above.

## Repchain Attack Resistance

Simple point-based karma systems are vulnerable to many classes of attack. For example, it would be trivial to attack the Repchain by submitting fraudulent low stakes contracts and using sibyl accounts to mediate them. But, by using a graph based Rep score these fraudulent methods can be detected and factored out of the Rep calculation. A linear increase in fraudulent graph-based Rep would require an exponential increase in the size of the attack.

Nodes mining the Repchain would preform this graph analyses as part of their Proof-of-Work. It's much easier to check the result of a graph analysis, O\(n\), than it is to preform the analysis, O\(n^3\). This makes it a good fit for distributed proof of work.

