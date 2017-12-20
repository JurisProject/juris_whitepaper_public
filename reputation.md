# The Reputation System

If Juris is to be the go-to adjudication mechanism for smart contracts, parties must have confidence that their cases are arbitrated fairly by reputable individuals. This presents a challenge: how do we gauge fairness and reputability in a decentralized, anonymous, autonomous environment? As a solution to this challenge, we propose a trust framework—a *reputation system*—tightly integrated with the Juris platform, but executed as its own blockchain. In this chapter we explore the existing literature on similar systems, before describing the Juris Reputation Blockchain (hereafter, the *repchain*) in detail.

## Background
The Juris repchain is an evolution of existing systems with significant prior art.
### Trust Metrics
The concept of measurable (or computable) trust has been studied extensively within the contexts of sociology and computer science, and is known as a *trust metric*. Defined simply, a *trust metric* is the quantification of the emotion *Trust*. However, Trust—being both abstract and subjective—has no formal and universal identity as a numerical quantity. It follows that trust metrics are proxies; they are numerical quantities that indicate the magnitude of trust between parties in a given context.

The context dependence of trust metrics means that it's exceedingly difficult to directly map existing trust metrics to new systems, while retaining the original metric's meaning.

### Reputation Systems
A *reputation system* is a program that enables a community to collaboratively determine the trustworthiness of its members. More formally, a reputation system defines a trust metric, provides the framework for computing that metric, and calls the metric *reputation*.

## The Repchain

Broadly, the Juris repchain should have the following qualities:

1. Rep gauges the degree to which a person is capable of effectively arbitrating cases
2. Rep must be readily calculable, deterministic, and open
3. Earning rep legitimately should be straightforward, although difficult
4. Earning rep illegitimately should be so difficult as to be effectively impossible
5. Rep must be non-transferable and unsusceptible to commodification
6. The system must have a sensible incentive structure: arbitrators are rewarded for sound judgement and effective prosecution, and punished for poor judgement or bad behavior
7. The system should be resistant to malicious actors, sybil attacks, and abuse through collusion
8. After initialization, the system should be fully autonomous and decentralized

From each of these qualities we derive requirements which, when viewed together, lead naturally to the technical solution of an off-platform blockchain with rep reified as a crypto token.

### Ability to effectively arbitrate
*An individual's capacity to effectively arbitrate cases*—our trust metric. Rep is a proxy that gauges this capacity.

### Readily calculable, deterministic, and open
*Readily calculable*—should not be conflated with 'computationally or algorithmically easy.' Instead, we mean *right-sized for the execution engine*. If the execution engine is Ethereum, then 'readily calculable' does translate to 'computationally simple,' simply due to the cost of computing on the Ethereum platform.

*Deterministic*—given a history of transactions, reputation for an individual at time *t* always resolves to the same score.

*Open*—log of rep-changing transactions, and the algorithm to compute rep, are open and free. If rep computations are readily calculable and deterministic, and the rep transaction logs available and the algorithm known, then anybody can verify the accuracy of reputation scores.

### Earning rep legitimately
- Straightforward: a person's knowledge of the *repchain system* should not improve their ability to earn rep; only their ability to effectively arbitrate should
- define "legitimate:" one person, committed to justice, knowledgable, and verified by their peers
- difficult: straightforward != easy. implies significant human interaction

### Earning rep illegitimately
- Define illegitimately: definition by negation of the above

### Non-transferrable
- Down to the smallest denomination, rep is permanently tied to one 'account'
- unsusceptible to commodification: rep cannot be earned quid pro quo. barriers to transferring an account from one entity to another (unresolved?)

### Sensible incentive structure
- implies that *quality* of action more important than *quantity* of action; therefore, the system needs quality metrics
- punished: reputation can be docked

### Resistant to attacks
- malicious actors: system should be decentralized, both correctness and incorrectness should be provable
- sybil attacks: creating many accounts must be extremely difficult. it must always more effective to concentrate rep in one account instead of many.
- collusion: just as one person with many accounts less effective than same person with one account, many legitimate accounts with low rep must be less impactful than one legitimate account with high rep

### Autonomous and decentralized
- computed by a computer (duh)
- decentralized: implies some kind of peer-to-peer
- autonomous: (maybe not? initial governance is not autonomous)

## Earning Reputation
This is the section that will be of the greatest interest to Jurists. Earning rep keeps you in good standing and earning a lot of rep makes you elev

###The Easy Stuff

Eat your vegetables and finish what you start. This stuff doesn’t really prove that you have good judgement, but failing to do it proves that you’re a bit of a flake and shouldn’t be trusted to make good judgement. So if you make an opening vote, and don’t make a final vote or endorse an opinion, you get dinged hard.

Contributing to Discovery
Contributing to Opinions
Is a pull request an implicit endorsement of the commits all ready on that chain?
If a fork ends up being popular, the person who started that fork should get a lot of rep. They started a movement that stuck.

PANEL Peer Review
