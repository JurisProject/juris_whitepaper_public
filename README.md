# [Juris](https://juriscoin.io)

#### A Judicial Oracle for Blockchain Smart Contracts

#### Justitia usquam ex nusquam

---

[https://juriscoin.io](https://juriscoin.io)

Authors reachable on Telegraph

[@SudoDemosthenes](https://t.me/SudoDemosthenes) [@YoungSeneca](https://t.me/YoungSeneca) [@LockeItUp](https://t.me/LockeItUp) 
[@OdinGrimnir](https://t.me/OdinGrimnir) [@HammurabyteCode](https://t.me/HammurabyteCode) [@Sardonicu5](https://t.me/Sardonicu5)

---

### Table of Contents

- [Abstract](#abstract)
	- [Calamity on the Blockchain](#calamity-on-the-blockchain)
	- [Mission](#mission)
- [Introduction](#introduction)
- [Value Proposition](#value-proposition)
    - [Contract Parties](#contract-parties)
    - [Decentralized App Publishers](#decentralized-app-dapp-publishers)
    - [Jurists](#jurists)
- [Contracts](#contracts)
    - [Contracts](#contracts-1)
    - [Alternative Dispute Resolution](#alternative-dispute-resolution)
    - [Smart Contracts](#smart-contracts)
- [The Juris Platform for the Non-Technical](#the-juris-platform-for-the-non-technical)
- [Real World Use Cases](#real-world-use-cases)
- [SCAFT](#scaft)
- [The Juris Framework](#the-juris-framework)
- [Looking Forward](#looking-forward)
- [Conclusion](#conclusion)


---

## Abstract

Contract disputes occur. **Off the blockchain**, we resolve contract disputes through the court system or a form of Alternative Dispute Resolution (ADR). The more structured form of ADR, called “arbitration” involves the airing of grievances before a panel of neutral jurists, who assess the facts and provide a decision. The power of arbitration is recognized internationally, with 150 countries required by UN treaty to enforce arbitration judgements from other countries. In the United States neutral arbitration is a for-profit business. **On the blockchain**, there does not yet exist a protocol for the fair and efficient resolution of disputes in smart contracts. In this paper we introduce the **Juris Protocol**, an open source arbitration protocol built for the blockchain, and **JurisCoin** an utility token to facilitate and incentivize Juris platform activity. Through the use of Juris' Mediation Tools, Contract Development Kit (CDK), and Adjudication Protocol, the disputed outcome of any smart contract may be contested through United Nations compliant neutral arbitration. The Juris Protocol combines a novel reputation system based on prior certification, ongoing community activity, and merit. The protocol is intended to facilitate the inclusion of both professional human arbiters and a larger community of novices climbing as they gain experience. In this paper we review Juris' improvements on the current state of the art, explore Juris as a framework, and describe a governance model for launch and future development. As a platform, Juris seeks to improve both the safety and security of smart contracts. This will reduce the risk in the transition of traditional transactions onto blockchain-based alternatives and, in turn, increase broad adoption of blockchain technology.

## Introduction

### Calamity on the Blockchain

In May 2016, the DAO, or “Decentralized Autonomous Organization” launched the largest crowdfunding campaign in history. Not just on the Ethereum Blockchain -- but **ever**. They raised 150 million dollars worth of Ether by the end of 28 days. But, their success was short lived: on June 17th, 2016, we saw what happens when the intention behind a “Smart Contract” diverges from its codified implementation as several errors inside the smart contract code written by the The DAO team, allowed a single bad actor to drain 50 million dollars worth of Ether from the DAO wallets overnight. The remainder of the funds were saved only because of a group of “white hat” hackers who moved them to a friendly wallet via the same exploit. 

The breach was so significant as to drastically undermine investor confidence in Ether. Immediately following the DAO's theft, Ether's price cratered and lost nearly 63% of its value. Beyond just a price drop, the impact of the DAO was forceful enough to crack Ethereum into two entire separate blockchains: Ethereum, on which the DAO transactions were erased, and Ethereum Classic, where they were not. The split took place because this "hack" wasn't strictly illegal, or even really a hack. These bad actors didn't break anything, they noticed errors and exploited them to make the contract function in a way other than intended. The community was split on how to handle this: should they stick to the "four corners" of the contract terms, or stick to the intent of the smart contract code? After much debate there was a "hard fork" of the Ethereum Blockchain. The fork happened because the Ethereum Foundation decided to honor the intent of the contract over the literal code written. This type of dispute is not new. **This is contract law.**

Should the set of smart contracts that constituted the DAO been constructed with an adjudication platform available as a safeguard, as court systems safeguard non-smart contracts, the events that unfolded, ranging from the loss of market cap to the “Hard Fork” of Ethereum, may have been preventable. It is to avoid catastrophes like these, and engender a better confidence in smart contracts at large, that we propose **Juris**: a decentralized adjudication platform for blockchain smart contracts.

### Mission 
To make “smart contracts” on all blockchains safe, robust, and human.
To create an self-assembling global ecosystem of fair and thoughtful Jurists, supported and incentivized by the standard utility coin for fair dispute resolution, justice, and judgement.
To create a trust-less proof-of-judgement reputation chain.
To make access to justice as efficient, effective, and accessible as the internet.

--- 

## Value Proposition

### Contract Parties
The Juris platform will allow CDK, Mediation Tools, and Adjudication Protocol users to add a layer of human-based insurance to their smart contracts at minimal expense.   

### Decentralized App (dApp) Publishers
Dispute resolution is not the focus of most development teams, but can be a vital component of dApp function, especially when tokens are changing hands. Transaction disputes can be a sincere source of legal liability and thus existential risk for a fledgling application. By integrating Juris as their default dispute resolution mechanism, publishers can offload this risk -- for free.

### Jurists
By joining the Juris platform’s community of Jurists, legal professionals will increase the size of the market to which they are able to offer their services, while increasing the efficacy of the system, the value of time spent, and in turn their own JurisCoin holdings.

---

## Contracts

### Contracts

The contract is one of the foundational innovations of human society. Contracts, backed by rule of law, allow for the creation of trusted agreements between parties who may have limited ability to check backgrounds, or enforce promises without the help of a government. Contracts, and contract law, allow cooperation to scale beyond the village square. And in the past half-century, the ability to work together has given birth to even more advanced means of cooperation, as we’ve seen the progression from radio, to television, the internet, the web, social media, and now blockchain technology. Each of these innovations has resulted in more communication, taking place further and further from the comfort of the village square. This means more and more reliance on contracts to back our agreements.

Disputes under contract law arise when there is a perceived failure of cooperation. Fingers are pointed, and arguments are made about meaning and understanding. Contract law does its best to provide a peaceful solution, and codify results for future reference. But, disputes regarding intent, expression of intent, and understanding of that intent by all parties, are forever rooted in the vagaries and nuances of human life and language. For this reason, there will always be contract disputes. When these disputes occur, the parties call on the government and rule of law to resolve confusion and enforce resolution. 

### Alternative Dispute Resolution

As society has grown and technology has provided for more and more cooperation -- and corresponding legal agreements -- the frequency of such disputes has given rise to judicially recognized alternative dispute resolution (ADR) mechanisms. For the parties tied up in a dispute, these alternatives provide a means of peaceful resolution that is faster and cheaper than the court system. For the court system, ADR helps them keep their docket under control so they can worry about important matters like criminal trials. Modern contracts between parties frequently include “arbitration clauses” which stipulate that in the event of a dispute the parties agree to air their grievances before a neutral third party, and accept the decision rendered, rather than availing themselves of their right to pursue resolution via judicial system. 

Under most ADR systems, arbitration is overseen by a professional neutral arbiter, who is frequently provided by an organization like JAMS, the largest private ADR provider in the world. Arbitrators are usually experienced legal professionals, lawyers, or  retired judges. The Juris Platform will provide greater access to this class of professional assistance, and will allow an increasing number of legal professionals to weigh in, provide services, and establish themselves as skilled Jurists. 

For all their recognition and respect, ADR systems have fallen behind. The Juris CDK, Mediation Tools, and Adjudication Protocol are the next evolution of dispute resolution, built for the next wave of human communication, cooperation, and innovation. 

### Smart Contracts

Uniquely enabled by blockchain technology, the “smart contract” is a new evolution of cooperation via agreement. Over the past decade, blockchain has crept into the backbone of myriad previously centralized, analog processes. From currency exchanges and crowdfunding, to identity management and self-governance systems, activities previously reliant on central authority are leveraging blockchain’s distributed immutable recordkeeping to become more fault tolerant, more inclusively accessible, and more democratically operated. At the core all of this works in service of the same end as does contract law: increased ability to co-operate securely. It makes sense that blockchain would carry with it a new evolution of the contract itself, the “smart contract.”

The smart contract introduces new components to the contract structure. They aren't "contracts," really, they're computer programs, structured like contracts. They live, and run directly on a blockchain, like Ethereum, not on any one local machine. They are both an agreement between parties and distributed executable computer software. This means the drafter of a smart contract can not only program in the terms of an agreement, but write a program to execute those terms automatically. Standard contracts are documents that represent the agreement between two parties. When it comes to executing, it’s on the parties to hold up their side of the agreement, and the expectation that they will do so is backed by the ability to sue for enforcement. A smart contract doesn’t need the threat of legal action as backing. Execution is actually built into the program. If the terms are met by one party, the rest of the contract code simply executes, and the agreed upon outcome is enforced. Here, the agreement is enforced not by fear of the courts, or the police upon court order, but by the code's execution and persistence on a distributed immutable blockchain. Because of this, blockchain technologies, and smart contracts are sometimes called “trust-less,” as they enable a measure of enforcement without government backup. You don’t have to trust the other party to an agreement to fulfill their obligation, the code just does it. But this code is a “contract” insofar as it represents intent by multiple parties that a form of co-operation is to take place. In this way even smart contracts will inevitably, on occasion, fall prey to the same trappings of human frailty we encounter in the practice of contract law.

### Human Tools, Human Rights

Blockchain technologies and smart contracts present the world with a new way of structuring and executing agreements between parties. Yet, for all their revolutionary capacity, those technologies work in service of human ends, and will never be free of the aforementioned vagary and nuance. People will misunderstand or misrepresent. Intent and meaning will mis-match. Software will have bugs. And people will desire a mechanism to protect their right to a fair resolution of wrongdoing, disagreement, negligence, or conflict. Millennia of contracts, contract law, cooperation, and conflicts have given rise to modern international systems of arbitration. Held to United Nations convention standards, arbitration is a recognized means of dispute resolution. The Juris Protocol we propose evolves those systems for blockchain applications, and in doing so represents the next evolution of fair and peaceful dispute resolution and justice.

While creating Juris we hold it as truth that peaceful resolution of disagreements is a human right. We believe that the progress of further human cooperation and technological expansion will depend on the ability to feel secure in one’s agreements, and in one’s ability to seek justice when those agreements fall short. It is only a matter of time before this new form of cooperation, fed by the evolution of blockchain technology, progresses into the function of democracy, systems of law, and dispute resolution. As such, our goal for Juris is to digitize and decentralize the mediation and arbitration process, and to bring arbitration to decentralized contract systems such as the Ethereum smart contract. At maturity, an arbitration platform for the blockchain holds the potential be an indispensable part of participation in any smart contract, any contract, and any system of human cooperation.


### Bringing Rule of Law to the World

“The rule of law and development are strongly interrelated and mutually reinforcing[.] [T]he advancement of the rule of law at the national and international level is essential for sustained and inclusive economic growth, sustainable development, the eradication of poverty and hunger and the full realization of all human rights and fundamental freedoms, including the right to development, which in turn reinforce[s] the rule of law”. - UN Declaration on Rule of Law

Contracts have the power to facilitate cooperation only to the extent that they are backed by government legal systems, and rule of law. In countries without functioning courts, parties to contacts cannot be compelled to perform. Even in countries with strong civil law, getting an arbitration judgement is just half the battle. If the parties do not conform to the judgement, the aggrieved party can go to the court to get an order to seize assets, or garnish wages, for example. Globally, this process is often difficult, time consuming, complicated across borders, and still cannot happen in many places that suffer from weak rule of law.

Hence, the imperative for a system like Juris. Here we leverage the smart contract constraint that a token asset is inextricably linked to execution of the contract itself. Because of this link we are able to ensure that - should dispute arise - the process of performance is as automatically executable as the standard behavior of the contract would have been without dispute. Over the past decade, disruptive technologies like Bitcoin and Mpesa have distributed banking services to over 1 billion people. We see here the opportunity for a similar distribution of Rule of Law via Juris. When arbitrating a smart contract running through Juris, an arbitrator would be able to directly enforce their judgement regarding the assets described within the code of the smart contract, distributing the assets as law and justice require. This removes the need for judicial backup behind the terms of an agreement.


### The United Nations, Arbitration, and International Law

Carried out to United Nations standards, arbitration is well suited for dispute resolution in the distributed, often multi-jurisdictional context of blockchain and smart contracts. 157 of 193 UN countries are signatories to The New York Convention, which provides for the recognition of arbitral awards across borders if those awards are the result of arbitration proceedings which follow UN mandated minimum rules. Additionally, many countries have adopted UNCITRAL Model Arbitration Laws, which provide for the same. This treaty and these laws mean that any system of arbitration built to UN standards is already internationally enforceable via traditional means, if need be.

Built to parallel the UNCITRAL arbitration rules, the Juris CDK will provide a way to build UN standards for arbitration process, and jurisdiction independent arbitral award enforcement, into any smart contract. This will provide a globalized, decentralized system for dispute resolution, built to United Nations standards for due process.

The Juris platform seeks to provide global citizens with viable and reliable access to internationally enforceable options for contractual agreement, and conflict resolution. Smart contracts are able to reach the farthest corners of the connected world, creating the opportunity for an increasing number of people to take part in secure transactions that may have otherwise been questionable, or impossible. For citizens this means increased access to justice. For jurists this means access to new markets which will grow with the adoption of blockchain, mobile devices, and the web, instead of markets that grow only at the pace of stable government.


### All Software Has Bugs

Through decades of software development and the composition of billions of source lines of code by millions of programmers, at least one maxim has held true: where there is software, we will find bugs. Estimates vary, but at least one thorough study suggests that software defects cost us 1.1 trillion dollars in the year 2016 alone [https://www.tricentis.com/resource-assets/software-fail-watch-2016/]. Browse through the commit history of any one of thousands of open source projects on GitHub, and it will be readily apparent that bugs are both a) pervasive and b) not limited to novice programmers.

The second inference—that bugs are committed by experienced and novice programmers alike—has grave implications for the future of smart contracts. After all, smart contracts are just software. It would be an extraordinary claim to suggest that the increased adoption and correspondingly increased sophistication of smart contracts will reduce the incidence of bugs, when history has shown us otherwise. We can expect quite the opposite, actually; as smart contracts are adopted more widely, they’ll be applied to increasingly difficult problem domains, with an increase in complexity to match. Software defects will continue to be a fact of life, and will worm their way into smart contracts—often, with dire consequences. They already have.

That’s not to say that we should throw our hands up in defeat. On the contrary, the blockchain development community can (and must) work hard to limit the rate and potential impact of bugs in both smart contracts and the underlying blockchain platforms. These two mitigating strategies (limiting the rate of bugs to the fullest extent possible, and limiting the impact of bugs) are two distinct topics that deserve their own treatment.

<Move to "Implementation"> To help us catch bugs in smart contracts early and often, JurisCoin will leverage several strategies that have emerged in the field of software development. Before we discuss how JurisCoin facilitates the production of safe and bug-free smart contracts, let’s enumerate some of the most well-known approaches to limiting bugs:

**Static typing:** statically typed languages can provide certain guarantees on correctness and safety if they pass a static type checker.
**Software testing:** software tests often surface bugs during development, and reduce the likelihood of introducing new bugs during change.
**Code reviews and audits:** when more than one pair of eyes are on software before release, we aren’t as likely to hear “I accidentally killed it” [https://www.cryptocoinsnews.com/i-accidentally-killed-it-parity-wallet-bug-locks-150-million-in-ether/]
**Standardized libraries:** from Effective Java, 2nd Edition, Item 47: KNOW AND USE THE LIBRARIES:
	“By using a standard library, you take advantage of the knowledge of the experts who wrote it and the experience of those who used it before you.” </move>

---

## The Juris Platform for the Non-Technical

A smart contract is protected by the Juris Protocol when the Juris CDK code is included in the contract, and backed by the attachment of a small quantity of JurisCoin (JRS). The CDK provides for a minimum subset of “just in case” contract terms in the form of code to be included in the smart contract. The CDK and Juris Dashboard help make sure that the party writing the contract has outlined the necessary terms of possible dispute resolution, or is aware of default CDK settings. It also makes sure that any other parties accessing the smart contract are aware of these terms as well. The necessary terms include details like the amount of time the parties will have to dispute a transaction following the smart contract’s execution, time for default in arbitration, and other specifics The Jurist Foundation or the United Nations recommend.

Once the contract is written, the minimum JRS is attached, and the smart contract is live on a blockchain, that contract is protected by the Juris Protocol. For the life of the contract the JRS will remain attached, and the CDK terms will remain incorporated, unless otherwise outlined in the code. If the smart contract runs without dispute, and the time for a challenge expires, all attached JRS will be returned to the providing party.

In the event of a dispute, the challenging party accesses their contract through the Juris Dashboard, or via the command line, and initiates the Juris Protocol. The system freezes further activity within the smart contract, creates an individual address as a holding account for any funds, takes the details of their grievance, attaches them to the disputed smart contract along with any and all associated logs, and then notifies the other parties involved. They are immediately moved to the mediation and arbitration process with the following steps:

1. **SELF Mediation:** Through the Juris Dashboard the parties are given access to a range of popular mediation tools and techniques, intended to facilitation resolution of any conflicts. The CDK gives the parties the ability, with mutual agreement, to cause the contract to proceed as written, to return all parties back to their positions before the contract was executed, or any resolution in-between deemed fair by all parties.

2. **SNAP Judgement:** If the parties are not able to work the conflict out themselves, they can escalate to a SNAP Judgement. This will cost extra JRS, but will arm the conversation with a bit of data on expected outcome. When a dispute is escalated to a SNAP, the Juris protocol will facilitate a polling process of all available Jurists. They will have a limited amount of time to review the details of the case, each side’s story, and provide their judgement on an equitable solution via anonymous vote. The parties will be provided with a breakdown of poll results, and a brief opinion from the group. The JRS put up for the SNAP will be split among all Jurists who take part in the SNAP process. Armed with this new information, the disputing parties will still have the option to resolve the dispute on their own using the Juris CDK tools.

3. **Binding PANEL Judgement:** If the parties are unable to resolve their conflict to the satisfaction of all, one or more of the parties may choose to escalate further through the Juris Adjudication Protocol to a Juris PANEL judgement. Again, this will come at the cost of additional JRS, but will provide a binding judgement, enforceable by UN treaty in most of the world. When a case is escalated the Juris system will facilitate the selection a panel of three High Jurists: those at the highest level of reputation, classified by domain experience and any other factors outlined initially via CDK. This panel will be selected by Juris Foundation and UN mandated process, and convene virtually through the Jurist Platform. They will have a pre-determined amount of time to hear additional arguments from the parties, request, collect, and review additional evidence, consider arguments, etc. Once this panel has made their decision the presiding High Jurist will have the power via the CDK to execute the decision by immediately running the modified contract instructions. The dispute is marked resolved, and the additional JRS allocated for escalation is paid out evenly to the High Jurists who made up the panel.

### Jurists
Jurists are classified by their rank in The Juris Reputation System, and by their areas of demonstrated expertise. The reputation system is a blockchain based means of storing and representing, proof of certification, merit, competence, and engagement. This pool will initially be seeded by The Juris Foundation from existing, certified, arbitrators and legal professionals. But, anyone is welcome to sign up to start earning (or losing) reputation by voting on cases, taking part in discussion, and helping with opinions. Classified by expertise if specified, all Jurists are notified when there is a new case. If they take part in an initial SNAP vote they will be required to take part in the final vote, and are encouraged to take part in discussion.

Reputation bleeds over time, and may be docked for bad behavior, and anyone is subject to rank demotion. All Jurist signups require proof of identity, and proof of certification if applicable. There are three reputation ranks:

**High Jurists** are pre-certified and Juris Foundation vetted. They are arbitration professionals, and those who have earned advancement and maintained standing through the system. High Jurists are eligible for the more lucrative, but time consuming PANEL Judgements.

**Good Standing Jurists** started with a law degree or better, and have continued to contribute fruitfully to decisions and discussions on the Juris platform. Good Standing Jurists are able to vote in SNAP Judgements, and the outcome of their anonymous votes will be included in the case files and reports to involved parties. They are able to advance to High Jurist by gaining reputation.

**Novice Jurists** are new signups not able to demonstrate any prior experience. They are allowed to take part in SNAP judgements and discussions, contribute to opinions, and earn reputation to advance to Good Standing.Their votes are not included in case files or reports to the parties involved in a dispute.

---

## Real World Use Cases

### Ziggy Stardust

Ziggy plays guitar, he’s an independent singer and songwriter who puts out music along with his band The Spiders from Mars. He wants to sell his tunes, but he’s sick of dealing with iTunes and the streaming options. He only makes 30% of the purchase price there. He thought about selling his music direct, and taking payments through PayPal, but those transaction fees are pretty high as well. To compete he needs to offer his tracks at $.99, $1.50 max, and he’s losing $.30-.50 of that on each transaction. But Ziggy has been watching the evolution of blockchain tech, he thinks he can do even better. He finds a service built on Ethereum called Ujo that helps him set up a store based off Ethereum smart contracts. The contract sends an attached Mp3 file directly back to any anyone that sends in $1 worth of Ether. Easy, and he gets to keep way more of that dollar than he would have with any alternative. Brilliant!

Ziggy drops his first single using his new smart contract system. He teases the track on Twitter and his fans are excited. David, a huge fan, immediately sends in his ETH, and he gets the mp3 he expected, but when he listens he finds out the file is nothing but static. This also happened to a thousand other fans. It seems the file Ziggy uploaded was corrupted on export or delivery. Luckily Ujo had incorporated the Juris CDK. The company hasn't collected any money yet, it’s in a CDK created holding wallet for the contracted two days clearance before they pass it to Ziggy. On David’s receipt he has a button that says “Request Refund or Report Problem.” He hits it, and fills out the details on the problem with his mp3 file.

The platform operators and Ziggy get a notification right away that the smart contract outcome has been flagged, and the contract (and funds) are frozen. On their Juris Dashboard they can see that 800 other flags have come in for this issue. Ziggy immediately checks the file and sees what happened, this is an obvious screw up, they’ll need to make good. Ziggy exported the wrong track in his recording session, and Ujo didn’t catch it. Whoops, but accidents happen, good thing there was a backup system.
 
Ziggy outputs the right track, and lets the service know, they send the fixed Mp3 file to David and all of the other fans who have placed an order so far. David gets a ping that Ujo and Ziggy have marked the dispute as resolved, he agrees so he marks the conflict as resolved via the Juris Dashboard as well. The funds are unlocked, and the contract is able to run. In 2 days Ziggy’s ETH will show up on time. In that time the service has fixed the smart contract for Ziggy’s track so this won’t happen to the next buyer. As buzz grows 50,000 more tracks are sold in the next day, all smooth transactions. The CDK just saved Ziggy, Ujo, and thousands of fans a headache -- and possibly some lawsuits.

### 100k Twitter Followers?

Alfred, an aspiring London comedian, is looking to drastically grow his small presence on Twitter to reach new audiences. He currently has around 20k followers and dreams of hitting the low six figures. On CoinLancer, a popular Ethereum-based freelancing marketplace, he finds Barbara: a self-proclaimed social media guru in Chicago. Barbera advertises that for 4 Ether she can grow anyone's Twitter follower count by 100k followers within 30 days. Alfred's sold: the price per follower sounds much better than any other offer he's seen. CoinLancer’s system helps he and Barbara enter into a smart contract with one another, set to programmatically test Alfred's follower count in 30 days.

30 days later, Alfred's follower count is at 125k - and rising. The test clause of the smart contract has become active, and confirms that his Follower count has surpassed the success criteria to pay out to Barbara.

To Alfred's horror, 3 days later, he receives an email from Twitter notifying him that 80k of Alfred's 125k Followers were deactivated. His Follower count now falls drastically short of Barbara's promise. As far as he's concerned, this isn't what he paid for. He contacts Barbara. As far as she's concerned, she's fulfilled the contract as it was written and has rendered her services as agreed: she got him his 100k followers.

Relieved that CoinLancer suggested he include Juris CDK in the smart contract, Alfred activates the adjudication function in his Juris dashboard. All the Ether in the contract is temporarily frozen, and a request is sent to Juris to begin arbitration. He and Barbara have already talked about their disagreement, and they're getting nowhere, so Alfred decides to escalate to a SNAP Judgement.

Worldwide, holders of JurisCoin receive notification of a new contract in need of arbitration. As they enter their online Juris dashboard and examine the ticket, they're presented with a brief synopsis of case details provided by Alfred and Barbara, as well as a copy of the smart contract in question. Deng, a JurisCoin holder in Singapore, reviews the initial case brief. He's unfamiliar with bot protocols and Twitter, and he's not confident that he will be able to contribute to the discussion, this case isn't for him, he decides. But Juan, a social media manager in Acapulco, has dealt with this before - personally. He - and thousands of other token holders - accept the ticket. He reviews the case and contract, and swiftly casts his first vote. Within the day, thousands of votes have been cast worldwide, each voter tasked with the same mission: render the mediation decision NOW that you think would be rendered by an arbiter in a second round of binding arbitration. **<-- Doesn't exactly match new SNAP system, does it?**

Alfred awakes the next day and - to his delight - the Juris arbiters have rendered a judgement. His dashboard reports back that 64% of the arbiters in the top 25% of reputation score sided with him, 73% of the top 10% of arbiters, and 92% of the top 1% of arbiters. As a token holder - and occasional arbiter himself - he knows that's a very positive outcome for him. He also knows Barbara will see the same.

He submits to assent to the favorable opinion cast by the Juris arbiters. If Barbara assents also, the case will be marked resolved and he'll be refunded his Ether. He and Barbara can part ways. He knows that if she doesn't, a second round of arbitration, this time - binding - will happen. Seeing thousands of votes rendered in Alfred's favor, Barbara concedes and assents to the decision. The Ether tied up in the contract is returned to Alfred, and the JurisCoin used to power the arbitration function in the contract is divided equally amongst all the arbiters who cast their vote in favor of Alfred.

## SCAFT

Nearly all securities contracts use an arbitration clause, or agreement.

The Simple Agreement for Future Tokens (SAFT) has quickly become a popular funding mechanism for pre-sale Token Generation Events. They are a tool for the early sale of the tokens that will be generated and used by technology protocols for which funding is needed. They require a certain degree of interpersonal trust between founders and investors, as they are essentially a promise to produce, and deliver something at a future date. But what if you want to fund a Cambodian team with a promising idea? Or an anonymous distributed team? Because of this trust component the SAFT is a less effective device for unproven teams or inexperienced investors. Luckily the system is already primed for a trustless solution, a Smart Contract for Future Tokens.

But this SCaFT could still be too rigid for the fast changing and fuzzy world of startups and crypto-technology. Let’s see why:


Three investors would each like to pre-purchase 10K ETH of AwesomeCoin at a 20% discount. Each puts 10K ETH in to a smart contract which has the following expected behavior: It will release .5% of its contents every day until it receives [the correct number of tokens] from [specific wallet address] at which point it will dump all of the remaining funds into the company's account. 

Due to a technical problem while preparing for the TGE, the AwesomeCoin developers lose access to [specific wallet address]. This means the smart contracts will never trigger as specified in their code. Without intervention, AwesomeCoin will never receive the full balance of their funds, and the investors will never receive their tokens. AwesomeCoin does not want to disrupt their TGE timeline, so they push ahead, have the TGE and distribute tokens manually from their new address, as promised, to the 3 investors. Using the Juris self mediation tools, the developers propose that the money be transferred to their account even through the technical terms of the SC were not satisfied. Using the same tools, 8 of the investor's signal their assent; the developers signal their assent, and the transfer executes. Two of the investors invoke the SCAFT’s cancellation terms. All of the money left in the account is moved into a 72 hour escrow account. Given the implementation of the SC, they don’t see any reason to leave the money in the contract. The developers unilaterally tigger the Juris mediation clause. That freezes the escrow account and creates a ‘summary plebiscite’. Any jurist in good standing can vote for 24 hours. At the end of that period, the breakdown is as follows: 

At that point one of the invests signals their willingness to release funds. Both parties crypto-sign a judgement. The funds are released and those jurists who voted inline with the signed judgement, get a share of the Juris denominated mediation fee and an increase in their rep-score.

Investor #3 signals that they do not intend to assent to the judgement. This signals the formation of a panel. The smart contract doesn’t detail what kind of mediation they would like, so the default is used. From the pool of Jurists who are marked as active at the “high” level, three are selected at random (weighted for expertise). This panel sits for up to seven days to hear arguments and examine evidence. At the end of that period, the judges find 2-to-1 for the entrepreneurs. Using their dispute mediation tools, without the consent of the investor, they transfer the remaining funds to the investor. The panel members split the mediation fee rate each other's performance (those ratingings are used to update their rep scores). 

Any investors or entrepreneurs reading this exchange probably found it extremely unpleasant to read. But imagine if these parties hadn’t had access to fast, just mediation. 


### Current State of the Art

Especially following the collapse of the DAO, the need for mediation and arbitration on blockchain-based smart contracts has spurred teams to investigate what frameworks may be developed to build this necessary part of the blockchain ecosystem. Two projects in particular serve as compelling starting points for discourse and improvement, and have been taken into consideration while developing Juris.

#### DAMN

In May, 2016, pre DAO hack, Third Key Solutions, founded by Pamela Morgan and notable Bitcoin advocate Andreas M. Antonopoulos released a proposal for DAMN, a Decentralized Arbitration and Mediation Network. The proposal was brief, and outlined an open source project intended to create a network similar to Juris on many fronts, in particular the adherence to United Nations arbitration standards. Their proposal was submitted to the DAO for funding approval and sentiment regarding the proposal was largely positive. The last activity on the project Github repo was in late May, 2016, with the DAO hack taking everyone’s attention shortly thereafter.

#### Kleros

Released as a concept whitepaper 2017, Kleros represents a more focused advance of the state of the art in the underlying reasoning of smart contract arbitration. Drawing its game theoretic underpinnings on Ethereum founder Vitalik Buterin’s initial proposals of SchellingCoin, Kleros proposed to incentivize arbiters to collaboratively vote as to reach truth, where truth (or a proxy of it) must emerge from a costly voting process and incentives apropos. Juris seeks to improve on several of the components outlined by Kleros. For example, game theoretical challenges emerge when voters are asked to vote how they think everyone else will vote. This problem, known as the Beauty Pageant Problem, remains unaddressed in both SchellingCoin and Kleros. Additionally, the top-down segmentation of the judicial system into sub-categories and sub-courts of dispute proposes an unnecessary quantity of operational overhead on the project, as does the selection of arbiters according to a cryptographic hash function. Kleros does present well an example of the use cases for a decentralized arbitration system, and outlines the attack risks against the system (bribery, surreptitiously controlling the majority of tokens, and a Sybil Attack).


In-house Arbitration Systems
Current State of art:
CoinLancer
Bounty0x
Research one more
Benefits of a platform solution:
Arbiter pool
Future development: data network effects in AI systems (the ‘why’ of this is the ‘why’ of all SaaS and PaaS
Cost reduction
Liability Management

---

## The Juris Framework

### The CDK: Contract Development Kit



#### Evidence, Arguments, and Discussion

When a dispute is triggered, the triggering party will be required by the Juris platform to include itemized claims, their desired resolution, and their initial argument for that resolution. Additionally they will be able to provide any details or evidence regarding the case that may fall outside of the smart contract logs. All of these details will be attached to the smart contract through the CDK, and other parties will be notified that a dispute has been triggered.

The other parties to the contract will have a designated amount of time to respond to the claims of the triggering party. They will be required to provide a direct response to each item of the claim, and their initial arguments for their prefered resolution. Here they will also be able to provide any additional details or evidence that may fall outside of the smart contract logs. If there is no response the system will issue a default judgement in the favor of the claimant. 

The argument submission process will be locked following the response from the defending party, and the submission of additional evidence will be locked before the case proceeds to open discussion. New evidence may be submitted with majority High Jurist approval. Further discussion and questioning regarding the case, case details, and evidence will take place via resolution processes outlined in paragraph 6.4.

#### Smart Contract Logs

#### Three Resolution Mechanisms
What do you do when you have a dispute with someone in meatspace? First, you try to work it out amongst yourselves. If you can’t, you’d seek advice. If that advice doesn’t help you solve things, you’ll ask someone neutral to make the choice for you. Juris works the same way. 

###### SELF (Self-Enforced Library Functions) Judgement
Problem it solves: Something has gone wrong with a smart contract. All parties to the contract agree what should happen next. This could be caused by a bug, a broken oracle feed, or any other unforeseen event.
How Juris moves: No Juris changes hands when the self-mediation toolkit is activated. The parties “pre-paid” for them when they signed the contract. 
From the parties perspective: This is a free and fast way to amicably resolve a misbehaving contract. 
From the Jurists’ perspective: This keeps trivial business out of the docket. 
How it works: Often, people are able to solve their own disputes. In the case of software bug, or any time the parties agree what the contract should do, but that intended behavior is not the contract’s expected behavior, the parties just need the tools to force some very specific behavior out of the contract. 
For these users, we’re building a package of self mediation tools which implement some basic operations (void the contract, give all assets to party A, ect). These tools will be totally open source and free. 


###### SNAP (Simple Neutral Arbitrator Poll) Judgement
Problem it solves: If parties believe that a disagreement in their contract will be resolved by a quick review of the facts by a third party, they should opt for a SNAP.
How Juris moves: The party(s) to the contract requesting the SNAP pay whatever they want to activate the SNAP (above a minimum). 5% of that fee goes to the Juris Foundation, the rest is split equally amongst all of the Jurists in good standing who vote in the SNAP. 
From the parties perspective: It’s a cheap way to get a fast judgement and a lot of input from different perspectives. 
From the Jurists’ perspective: SNAP’s don’t pay very well, but they do offer a lot of opportunities to earn rep. Jurists are always on the hunt for a contract where their unique expertise will be decisive. Since everyone has to split the arbitration fee, it pays to look into disputes that no one else is looking at. You need to pay attention, vote reasonably, and contribute if you’re going to increase or maintain your standing. 
How it works: (The SNAP is the most structured of the three dispute resolution processes, so the description here will be brief. See XXXXXX for a longer explanation of the SNAP.) All parties to a contract have 24 hours to submit an argument. Once they’re all in, any Jurist can see the arguments. To take a case a Jurist must vote based only on the arguments and submit a textual justification of their vote. After 24 hours, if the SNAP has had at least 5 votes the justifications are revealed to the jurists, and Discovery begins. The jurists can ask the parties any questions they have, vote on the questions and comment on the parties responses (very much like a Reddit AMA). By the end of discovery all jurists must vote again (or their opening vote will carry over and they will lose reputation). Then, the collective opinion phase begins, lasting 36 hours. Using the git source control system, Jurists collaboratively author an opinion for each position that received at least one vote. Based on the vote and opinion, the parties can decide to self mediate an outcome, or appeal for a PANEL. 


The format allows parties to provide opening arguments while also allowing the jurists to directly question the parties. This is designed to be a fusion of the anglo-american adversarial format with the east asian inquisitorial format.  

This VOTE --> JUSTIFY --> DISCUSS --> VOTE → JUSTIFY model is based on the Delphi Method of collective decision making. The Delphi Method has been shown to be very effective at surfacing hidden profiles while producing judgements that have broad support and alignment with facts.  

[clarify that the money for a SNAP may be preloaded into the contract. ]




###### PANEL (Peremptory Agreement for Neutral Expert Litigation) Judgement
Problem it solves: When a dispute is complex or there is a lot at stake, you want a small number of people to take their time examining all of the evidence, and hearing all of the arguments. 
How Juris moves: The party(s) to the contract requesting the PANEL pay the market rate to convene the panel. 5% of that fee goes to the Foundation,  the rest is split equally amongst the Jurists on the panel. 
From the parties perspective: For complex disputes that require deep attention of the most skilled jurists, it’s worth paying for a PANEL. 
From the Jurists’ perspective: This is where the real money is. But in order to get put on a panel, you need to have very high rep. All of that work spent in SNAP’s is paying off here! 
How it works: The party(s) requesting the PANEL sends a PANEL transaction with JRS attached into the contract. All of the assets in the contested contract are moved into escrow. Based on the domain specialties marked on the arbitration agreement, a panel of 3 arbitrators is randomly selected. The PANEL has 7 days to hear arguments and answer questions. At the end of those 7 days, they each issue a judgment. The Majority order is binding and causes the escrow to release the smart contract assets in accordance with the order. 

#### Arbiter/Jurist Sorting and Selection

###### PANEL Jurists - ?
We provide a list of High Jurist with domain expertise, they get some time to do homework, eliminate unacceptable Jurists, and rank remaining? Top two from each list are offered the job, check down the list if they don’t bite. Those two pick a 3rd who is the “presiding Jurist” basically head jurist.


###### Earning Reputation
This is the section that will be of the greatest interest to Jurists. Earning rep keeps you in good standing and earning a lot of rep makes you elev



The Easy Stuff

Eat your vegetables and finish what you start. This stuff doesn’t really prove that you have good judgement, but failing to do it proves that you’re a bit of a flake and shouldn’t be trusted to make good judgement. So if you make an opening vote, and don’t make a final vote or endorse an opinion, you get dinged hard. 

Contributing to Discovery
Contributing to Opinions
Is a pull request an implicit endorsement of the commits all ready on that chain? 
If a fork ends up being popular, the person who started that fork should get a lot of rep. They started a movement that stuck. 

PANEL Peer Review

Attack Resistance


50%+1 Attack
[Normal stuff about why a 51% pos attack is hard (it’s hard to buy up the coin if a lot of it is tied up in contracts, the more you monopolize the more expensive it gets, etc]

The bicameral structure of governance makes juris much more resistant to a 51% attack. Even if someone could control a super majority of Juris PoS they would be blocked by the Judgment chamber from forcing any changes to the Foundation Contract.

Sybil Attack


The PoT algorithm makes it very expensive to produce high ranked Jurists without providing value to the network. 

The Reputation Blockchain 


Governance


Initial Governance

Initially, the platform will be governed analogously to how other open source software projects are at their inception. A single leader from the Juris Foundation’s founding team will, amongst other roles, facilitate development, recognize contributions of the community, drive platform consensus, and break deadlocks. For example, direct vote by community members will be used to set technical direction, and anyone can submit pull requests. The Foundation will, at the outset, be the sole authority for what updates to the Foundation of the Juris Framework will be manifest.

This model is necessary during the early days of the platform to prevent attacks until the value of the platform and the resilience for the Juris Reputation System are maturely established. Once they system is sufficiently stable, The Juris Foundation will activate a meritocratic, bicameral liquid democracy to transfer power of governance to the Juris community.


Bicameral Liquid Democracy


Proof-of-Work and Proof-of-Stake are popular and effective governance tools for many blockchain-based communities. They give governance power to those who either bear the cost of maintaining the system or stand to gain the most from its continued success (respectively). Therefore they are very effective incentive-alignment tools. Yet they are not without their limitations, namely that they encourage winner-take-all dynamics. Fortunately, the addition of a bicameral liquid democracy ameliorates these shortcomings.

There is a long tradition of separating judicial authority from monied interests. It is an affront to a common sense of justice that a judicial body should be governed by one-token, one-vote (Proof-of-Stake) system. As such, historically, judiciaries have governed themselves through bar associations. Rule-setting bodies that constitute “the whole body of lawyers, the legal profession.” Though, without popular oversight, a judiciary run by- and for- the bar would become solipsistic and self-serving. 

Therefore, we propose Juris be governed by a bicameral liquid democracy; one chamber will operate on proof-of-stake the other, by proof-of-judgment. The assent of both chambers will be required to make a change to the master contract that defines the operations of Juris.

A Liquid Democracy or Delegated Democracy vests voting power in assigned delegates instead of representatives.  This enables voters to take an active role and vote on issues directly or take a passive role and delegate voting power to a trusted power with domain expertise.  Through either direct voting or proper delegation, people with domain knowledge of the topic are able to better influence the outcome of decisions, which in turn leads to an overall better governance of the state. Because of this, a Liquid Democracy naturally evolves into a system where decisions are mainly made by those who have the expertise required to make well-informed decisions on issues.


---

## Looking forward


### Defensibility

Before you decide to commit your time to working on an open source project or stockpiling a utility token behind it, it would be really nice to know if it’s going to win in the long term. Every good idea has lots clones and forking iteration. Why is Juris going to win in the long term?

First mover advantage is nice. Bitcoin remained the dominant medium-of-exchange crypto currency despite thousands of competitors, many of which are technically superior. If all of the interested parties commit to the first mover, everyone has more of an incentive to improve the first mover, than to jump (alone) to an upstart platform. Juris has this advantage [Ramsay and Matt - expand]

Juris also has something more important. Stackoverflow was not the first place to talk about software and Github was not the first place to distribute sourcecode. But they are the dominant platform because they were a good place to develop a reputation, and you can’t take that reputation with you. This is Juris’ long term strength. Though most of the utility of the platform will be derived from open source CDK’s, the Juris foundation will be able to able to continue to derive because of the lock-in power of the reputation system -- a novel innovation, and first of its kind in the blockchain ecosystem. Though it is similar to earn.com’s leveraging of social networks. 

People will want to commit to Juris coin quickly because of ability of first movers to quickly accrue reputation. Everyone will be reluctant to leave, because you can’t take that reputation with you. Far better to stay and improve the system you’re invested in. 

### AI arbitration


### Beyond arbitration

---

## Conclusion


---
## APPENDIX For Future Directions




### APPENDIX FAQs

Why does this need a token? Why not run the economy on BTC or ETR?
This is the most important question to ask of the current generation of blockchain companies, and almost all of them fail it. 

 five reasons. 
 
1. The way that the currency interacts with the rep chain.
2. The token is used to mark jurists
3. It enables the governance mechanisms. 
4. A token that is only used to deliver dispute resolution can give all parties to a contract confidence that the contract is well faithfully enforced. 
5. The need for an independent monetary policy. The prices of crypto currencies (EHT included) move A LOT! Juris is going to need to run it’s own monetary policy. 
6. Tethering the token across contract chains. -- when Juris moves to NEO, having a ETH derivative coin (as opposed to straight up ETH) will make coupling it to the other chain easier. 
7. facilitate and mediate partnerships. (give a bunch of coin to a partner to achieve alignment)

###### Why does this need to be decentralized? Can’t you just run this on one server?

There’s actually two things we are decentralizing, justice and reputation. 
Justice:
Apple, Signal, Telegram, and Keybase enable distributed end-to-end encrypted communication because your communication is no one else's business. Strongly encrypted communications prevent identity theft, stalking, government censorship, and forged communications. 
The world needs strongly encrypted justice for the same reasons. Not everyone enjoys swift impartial contract enforcement; and no one enjoys it at a low cost. To prevent corrupt governments and criminal organizations from tampering in dispute resolution, we need strong encrypted and decentralized system where the assets and contracts are never under the control of the juris foundation. 
What were planning would be impossible to do in a centralized way. 
Extending the force for contract law (with the assets held in smart escrow) to the entire planet is a radical idea. 
If this were on a centralized server, it would mean that Juris would be subject to all sorts of legal constraints.  If control of the assets were constantly passing through a central server we controlled, we would be crushed under a constant barrage of seizure claims form regional governments. It would be impossible to bring the justice of contract law to the world under that framework. 

Reputation (proof-of-judgement):
A reputation chain is most valuable to people on the chain if it is visible to everyone. We could publish an open API, but that would incur high recurring security and attack resilience costs and Jurist would have to trust us that we would continue to make their proof-of-judgement public. By running reputation as a blockchain, we make it maximally available (forever) without having to deal with those costs. 
