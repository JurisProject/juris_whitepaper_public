# The Reputation System

## Introduction

If Juris is to be the go-to adjudication mechanism for smart contracts, parties must have confidence that their cases are arbitrated fairly by reputable and experienced individuals. The system must allow for the on-boarding and advancement of new Jurists. Yet, it must do so without sacrificing fairness to inexperienced input on decisions. Additionally the system must require a minimum demonstration of experience for a Jurist to have material impact on case outcome in order to resist attack via mass new account creation.

This presents a challenge: how do we gauge fairness and reputability in a decentralized, anonymous, autonomous environment, while leaning minimally on proof of previous credentials? As a solution to this challenge, we propose a trust framework—a _reputation system_—tightly integrated with the Juris platform, but executed as its own blockchain. In this chapter we explore the existing literature on similar systems, before describing the Juris Reputation Blockchain \(hereafter, the _repchain_\) in detail.

## Background

The Juris Repchain is an evolution of existing systems with significant prior art.

In the digital realm, the problem of reputation has been tackled from many angles, and effective execution has contributed to the success of such platforms as Reddit and Stack Overflow. In real world academic and professional context we handle the notion of reputation by issuing credentials like degrees or certifications, tracking notable publications, awards, or recommendations. In the context of justice and the law, there already exists a hierarchy of certification, experience, and reputation. This makes arbitration, and dispute resolution the ideal first case scenario for the implementation of a bespoke repchain.

### Reputation Systems

A _reputation system_ is a program that enables a community to collaboratively determine the trustworthiness of its members. More formally, a reputation system defines a trust metric, provides the framework for computing that metric, and calls the metric _reputation_.

### Trust Metrics

The concept of measurable \(or computable\) trust has been studied extensively within the contexts of sociology and computer science, and is known as a _trust metric_. Defined simply, a _trust metric_ is the quantification of the emotion _Trust_. That is, the extent to which one party expects that any other party will do as they promise. However, Trust, being both abstract and subjective, has no formal and universal identity as a numerical quantity. It follows that trust metrics are proxies; they are numerical quantities that attempt to indicate the magnitude of trust between parties in a given context.

The context dependence of trust metrics means that it's exceedingly difficult to directly map existing trust metrics to new systems, while retaining the original metric's meaning[^1]. Therefore the details of our trust metric will require a lot of tuning and adjustment to the use case, and as Juris matures. Before giving a detailed implementation specification, we will define our priorities and process.

## Priorities for The Repchain

Broadly, the Juris repchain should have the following qualities:

### Useful Proxy

In the Juris system "reputation" gauges the degree to which a person is capable of effectively and fairly arbitrating cases.

_An individual's capacity to effectively arbitrate cases:_ our trust metric. Reputation is a proxy that gauges this capacity.

### Verifiable

Rep must be readily calculable, deterministic, and open.

_Readily calculable:_ This should not be conflated with "computationally or algorithmically simple." Instead, we mean **right-sized for the execution engine**. If the execution engine is Ethereum, then "readily calculable" does translate to "computationally simple" due to the cost of computing on the Ethereum platform.

_Deterministic:_ Repeatable rep computations. Starting from the same base state, the rep algorithm will always compute the same rep for a given point in the rep transaction log.

_Open:_ Rep algorithm and log of rep-changing transactions are both public. If rep computations are readily calculable and deterministic, and the rep transaction logs available and the algorithm known, then anybody can verify the accuracy of reputation scores quickly and easily.

### Achievable When Warranted

Earning rep legitimately should be straightforward, although difficult.

_Straightforward:_ Knowledge of the repchain's implementation is neither necessary nor advantageous for earning rep.

_Legitimate:_ An individual who, using a single identity, is committed to resolving smart contract disputes through the fair and impartial application of knowledge and judgement, is **earning rep legitimately**.

\_Difficult: E\_arning rep requires considerable human action.

### Unachievable When Unwarranted

Earning rep illegitimately should be so difficult as to be effectively impossible.

\_Illegitimate: \(D\_efinition by negation.\) An individual using multiple identities, or multiple individuals using a single identity, who manipulate the outcome of contract disputes through unfair and/or biased application of knowledge and judgement, is/are **earning rep illegitimately**.

### Identity-Based

Rep must be non-transferrable and unsusceptible to commodification.

_Non-transferrable:_ Down to the smallest denomination, rep is permanently tied to one 'account' identifier.

_Unsusceptible to commodification:_ Rep cannot be earned quid pro quo. Transfer of an account from one entity to another must be impossible, or there must be significant barriers to execution.

### Promotes Cooperation

The system must have a sensible incentive structure: Jurists are rewarded for sound judgement, fruitful contribution, and effective prosecution. Jurists punished for poor judgement, bad behavior, or extended failure to engage in the system demonstrating, at least, continued attention to the system.

* implies that _quality_ of action more important than _quantity_ of action; therefore, the system needs quality metrics

_Punishment:_ The system must provide for the increase _and decrease_ of reputation.

### Attack-Resistant

The system should be resistant to malicious actors, sybil attacks, and abuse through collusion.

* malicious actors: system should be decentralized, both correctness and incorrectness should be provable
* sybil attacks: creating many accounts must be extremely difficult. it must always more effective to concentrate rep in one account instead of many.
* collusion: just as one person with many accounts less effective than same person with one account, many legitimate accounts with low rep must be less impactful than one legitimate account with high rep

### Self-Perpetuating

After initialization, the system should be fully autonomous and decentralized.

* computed by a computer \(duh\)
* decentralized: implies some kind of peer-to-peer
* autonomous: \(maybe not? initial governance is not autonomous\)

## Earning Reputation

This is the section that will be of the greatest interest to Jurists. Earning rep keeps you in good standing and earning a lot of rep makes you elegable to participate in PANELs.

SNAP is structured to profide lots of opertunities for

\(1\) Jurists to demonstrate good judgement, and  
\(2\) Jurists to implicitly endorce each others judgement.

These implicict endrocements can then be used as the raw data for a directed weighted graph \(DWG\). By applying graph analitical techniques to these DWGs we can infer our _Trust Metric._

### The Easy Stuff

Finish what you start. This stuff doesn’t really prove that you have good judgement, but failing to do it proves that you’re a bit of a flake and shouldn’t be trusted to make good judgement. So if you make an opening vote, and don’t make a final vote or endorse an opinion, you get dinged hard.

### Contributing to Discussions and Opinions

Is a pull request an implicit endorsement of the commits all ready on that chain?  
If a fork ends up being popular, the person who started that fork should get a lot of rep. They started a movement that stuck.

### PANEL Peer Review

PANEL's don't have as many opertunitres for Juritst to show off . . . . \[yada yada yada\]

### Graph Analysis

[^1]:  [Ziegler, Cai-Nicolas, and Georg Lausen. "Propagation models for trust and distrust in social networks." Information Systems Frontiers 7.4-5 \(2005\): 337-358.](https://link.springer.com/article/10.1007/s10796-005-4807-3)

