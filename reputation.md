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

- Reputation should be a reliable proxy for a person's ability to effectively arbitrate cases
- Reputation scores must be readily calculable, deterministic, and open
- Earning reputation legitimately should be straightforward, although difficult
- Earning reputation illegitimately should be so difficult as to be effectively impossible
- Reputation must be non-transferable and unsusceptible to commodification
- The system must have a sensible incentive structure: arbitrators are rewarded for sound judgement and effective prosecution, and punished for poor judgement or bad behavior
- The system should be resistant to malicious actors, sybil attacks, and abuse through collusion
- After initialization, the system should be fully autonomous and decentralized

The technical implementation of Juris' reputation system will be an off-platform blockchain, with reputation (or *rep*) reified as a crypto token.

## Earning Reputation
This is the section that will be of the greatest interest to Jurists. Earning rep keeps you in good standing and earning a lot of rep makes you elev

###The Easy Stuff

Eat your vegetables and finish what you start. This stuff doesn’t really prove that you have good judgement, but failing to do it proves that you’re a bit of a flake and shouldn’t be trusted to make good judgement. So if you make an opening vote, and don’t make a final vote or endorse an opinion, you get dinged hard.

Contributing to Discovery
Contributing to Opinions
Is a pull request an implicit endorsement of the commits all ready on that chain?
If a fork ends up being popular, the person who started that fork should get a lot of rep. They started a movement that stuck.

PANEL Peer Review
