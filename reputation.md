# The Reputation System

## Introduction

If Juris is to be the go-to adjudication mechanism for smart contracts, parties must have confidence that their cases are arbitrated fairly, by reputable individuals. This presents a challenge: how do we gauge fairness and reputability in a decentralized, anonymous, autonomous environment? As a solution to this challenge, we propose a trust framework—a _reputation system_—tightly integrated with the Juris platform, but executed as its own blockchain. In this chapter we explore the existing literature on similar systems, before describing the Juris Reputation Blockchain \(hereafter, the _repchain_\) in detail.

## Background

The Juris repchain is an evolution of existing systems with significant prior art:

### Trust Metrics

The concept of measurable \(or computable\) trust has been studied extensively within the contexts of sociology and computer science, and is known as a _trust metric_. Defined simply, a _trust metric_ is the quantification of the emotion _Trust_. However, Trust—being both abstract and subjective—has no formal and universal identity as a numerical quantity. It follows that trust metrics are proxies; they are numerical quantities that indicate the magnitude of trust between parties in a given context.

The context dependence of trust metrics means that it's exceedingly difficult to directly map existing trust metrics to new systems, while retaining the original metric's meaning[^1]. Therefore the details of our trust metric will require a lot of tuning and ajustment as Juris matures. So instead of giving a detailed implimentation specification we will define our priorities and process.

### Reputation Systems

A _reputation system_ is a program that enables a community to collaboratively determine the trustworthiness of its members. More formally, a reputation system defines a trust metric, provides the framework for computing that metric, and calls the metric _reputation_.

## Priorities for The Repchain

Broadly, the Juris repchain should have the following qualities.

### Useful Proxy

Rep gauges the degree to which a person is capable of effectively arbitrating cases.

_An individual's capacity to effectively arbitrate cases_—our trust metric. Rep is a proxy that gauges this capacity.

### Verifiable

Rep must be readily calculable, deterministic, and open.

_Readily calculable_—should not be conflated with "computationally or algorithmically simple." Instead, we mean **right-sized for the execution engine**. If the execution engine is Ethereum, then "readily calculable" does translate to "computationally simple" due to the cost of computing on the Ethereum platform.

_Deterministic_—repeatable rep computations. Starting from the same base state, the rep algorithm will always compute the same rep for a given point in the rep transaction log.

_Open_—rep algorithm and log of rep-changing transactions are both public. If rep computations are readily calculable and deterministic, and the rep transaction logs available and the algorithm known, then anybody can verify the accuracy of reputation scores.

### Achievable When Warranted

Earning rep legitimately should be straightforward, although difficult.

_Straightforward_—knowledge of the repchain's implementation is neither necessary nor advantageous for earning rep.

_Legitimate_—an individual who, using a single identity, is committed to resolving smart contract disputes through the fair and impartial application of knowledge and judgement, is **earning rep legitimately**.

_Difficult_—earning rep requires considerable human action.

### Unachievable When Wot Warranted

Earning rep illegitimately should be so difficult as to be effectively impossible.

_Illegitimate_—definition by negation. An individual using multiple identities, or multiple individuals using a single identity, who manipulate the outcome of contract disputes through unfair and/or biased application of knowledge and judgement, is/are **earning rep illegitimately**.

### Identity-Based

Rep must be non-transferrable and unsusceptible to commodification.

* Down to the smallest denomination, rep is permanently tied to one 'account'
* unsusceptible to commodification: rep cannot be earned quid pro quo. barriers to transferring an account from one entity to another \(unresolved?\)

### Promotes Cooperation

The system must have a sensible incentive structure: arbitrators are rewarded for sound judgement and effective prosecution, and punished for poor judgement or bad behavior.

* implies that _quality_ of action more important than _quantity_ of action; therefore, the system needs quality metrics
* punished: reputation can be docked

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

