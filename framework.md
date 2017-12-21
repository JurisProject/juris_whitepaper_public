# The Juris Framework

### Evidence, Arguments, and Discussion

When a dispute is triggered, the triggering party will be required by the Juris platform to include itemized claims, their desired resolution, and their initial arguments for that resolution \(together, the "Formal Complaint."\) Additionally they will be able to provide any details or evidence regarding the case that may fall outside of the smart contract logs \("Supplementary Evidence."\) All of these details will be attached to the smart contract through the CDK, and will follow the case through the Juris system.

The counter-party to the dispute will have a designated amount of time to respond to the claims of the triggering party. They will be required to provide a direct response to each item of the claim, and their initial arguments for their preferred resolution. Here they will also be able to provide any additional details or evidence for their side that may fall outside of the smart contract logs. If there is no response from the counter-party, and a response is required by the resolution mechanism, the system will issue a default judgement in the favor of the claimant.

The argument submission process will be locked following the response from the defending party, and the submission of additional evidence will be locked before the case proceeds to open discussion. New evidence may be submitted with majority High Jurist approval. Further discussion and questioning regarding the case, case details, and evidence, will take place via resolution processes outlined below.

### Smart Contract Logs \("Hard Evidence"\)

One of the most critical pieces of evidence provided to the Jurists will be the history of logs and transactions associated with the smart contract in question. This is especially true when a bug in the smart contract is what brought the contract to Juris. At the moment that the dispute is initiated the Juris plugin collects and freezes all transaction logs, contract execution logs, contract state, and the contract code itself. These logs will be automatically summarized and made available to Jurists as evidence.

## Three Resolution Mechanisms

### SELF \(Self-Enforced Library Functions\) Judgement

**Problem it solves:** Something has gone wrong with a smart contract. All parties to the contract agree what should happen next. This could be caused by a bug, a broken oracle feed, or any other unforeseen event. Whether right away, or after brief negotiation the parties have a solution and they agree that the solution is fair.

**How Juris moves:** No Juris changes hands when the self-mediation toolkit is activated. The parties “pre-paid” for them when they signed the contract and attached their JRS.

**From the parties perspective:** This is a free and fast way to amicably resolve a misbehaving contract.

**From the Jurists’ perspective:** This keeps trivial business out of the docket.

**How it works:** The incorporation of the Juris CDK allows the protocol to alter the outcome of a smart contract. Through the Juris dashboard the parties to the contract have access a package of self mediation tools which provide for the implementation of some basic operations to designate a different outcome for the smart contract, \(void the contract, give all assets to party A, etc\). These tools will be totally open source and free.

### SNAP \(Simple Neutral Arbitrator Poll\) Judgement

**Problem it solves:** If parties are unable to settle on an outcome on their own, and believe that a disagreement in their contract will be resolved by a quick review of the facts by a third party, they should opt for a SNAP.

**How Juris moves:** The party\(s\) to the contract requesting the SNAP pay whatever they want to activate the SNAP \(above a minimum covered by the already attached JRS.\) 5% of that fee goes to the Juris Foundation, the rest is split equally amongst all of the Jurists in good standing who take part in the SNAP.

**From the parties perspective:** It’s a cheap way to get a fast judgement and a lot of input from different perspectives. It may have the power to quickly resolve a negotiation stalemate.

**From the Jurists’ perspective:** SNAP’s don’t pay as well, but they do offer a lot of opportunities to earn reputation. Jurists are always on the hunt for a contract where their unique expertise will be decisive. Since everyone has to split the arbitration fee, it pays to look into disputes that no one else is looking at. You need to pay attention, vote reasonably, and contribute if you’re going to increase or maintain your standing.

**How it works:** After a contract has executed, parties to the contract have a designated amount of time to initiate a SNAP, this time period can also be extended by mutual agreement.  From the date the SNAP is initiated, the parties have a window in which to provide the details mentioned above for their Formal Complaint. This is used to create a "Case Brief" containing itemized \(e.g. bulleted\) complaints, written arguments, and optionally itemized additional facts the parties would like to present during the judgement. At the close of this window case briefs are posted to JRS Token holders publicly for review.

Jurists may access any case brief without obligation to participate in the case, but must pass a Captcha test \(or equivalent\) before being given access to further evidence, or logs. If an individual chooses to join a SNAP as a participating Jurist they are given access to further evidence and logs, and are required to cast their initial vote using only the information available. When casting their vote an arbitrator must cite justification from at least one of \(a\) an item of Hard Evidence, \(b\) an item of a Formal Complaint, or \(c\) an item of Supplementary Evidence. As part of their judgement, an arbitrator must also provide a short \(255 characters or less\) summary of their opinion. After submitting the above, their "Independent Judgement," an arbitrator formally becomes a Jurist for the given SNAP.

Independent Judgements remain hidden from both the disputing parties and other Jurists. However, the number of Jurists that have joined the SNAP is displayed publicly. At the end of a designated period of time the case details are taken down, and open discussion begins among participants.

At this time all participants are made privy to the SNAP’s tally of votes, the tally of evidence selected as justification, and the Independent Opinions, all of which are anonymized. During discussion, Jurists make material contributions to the discussion in the form of: questions posed for other participants, submission of general comments, citations of case history, comments on any item in the Case Brief or supporting materials, written responses to any of the above and to other written responses, and atomic responses \(up/down vote\) to any of the above.

After a designated window discussion is closed, at which point interaction between and among all participants ceases for a period of deliberation. In this time, Jurists have an opportunity to independently review the case deatials and all additional supporting and discussion materials. After deliberation, each Jurist must cast a final vote, select one or more pieces of supporting evidence, and compose a written summary of their opinion no longer than 500 characters \(collectively, their "Informed Judgement.\) Until the close of the deliberation period all Informed Judgements are hidden from other parties as they are submitted.

At the end of the deliveration period, all of the Informed Judgements are closed for modification, and each Jurist is immediately placed into a group of peers \(a “Consensus Group”\) who voted in favor of the same disputing party. Each Consensus Group is firewalled from both the other Consensus Group and from the disputing party. Each group will have a designated amount of time to confer amongst its members and write an opinion on their ruling \(the “Final Opinion”\). The Jurist with the highest reputation within an individual Consensus Group is automatically selected as the leader of their cohort. Optionally, the default lead Jurist may appoint another Jurist within their Consensus Group as the opinion writer.

During opinion composition, all Jurists retain access to all case brief, evidence, and discussion details. The Jurists of a Consensus Group collaborate by making material contributions in the same form as the earlier discussion. Before the end of the opinion composition, each Consensus Group compiles these Opinion Artifacts into a Final Opinion.

With the submission of the Final Opinion, communication between all participants ceases, and the Final Opinions from both Consensus Groups are delivered to all parties along with a breakdown of the final voting split.

At this point the disputing parties are again given access to the CDK resolution tools to implement an agreed upon dispute solution.

### PANEL \(Peremptory Agreement for Neutral Expert Litigation\) Judgement

**Problem it solves:** While the SNAP procedure provides assistance is dispute resolution, it does not rise to the level of due process required for a binding judgement under United Nations standards. When a dispute is complex, there is a lot at stake, and the decision if final, you want small number of people to take their time examining all of the evidence, and hearing all of the arguments.

**How Juris moves:** The party\(s\) to the contract requesting the PANEL pay the market rate to convene a panel. 5% of that fee goes to the Foundation,  the rest is split equally amongst the Jurists on the panel at the close of proceedings.

**From the parties perspective:** For complex disputes that require deep attention of the most skilled jurists, or to break a deadlock with a final binding decision, it’s worth paying for a PANEL.

**From the Jurists’ perspective:** This is more labor intensive, but this is where the real money is, as fees are higher and split among fewer Jurists. In order to get put on a panel, you need to have High Jurist standing. All of that work spent in SNAP’s is paying off here!

**How it works: **Similar to normal court systems, this is considered an escalation. Parties cannot proceed to a PANEL judgement without first running a SNAP. If one or both parties are unable to use the assistance of the SNAP to come to a resolution, they may choose to escalate to a PANEL judgement by indicating their intent to escalate and 



The party\(s\) requesting the PANEL sends a PANEL transaction with JRS attached into the contract. All of the assets in the contested contract are moved into escrow. Based on the domain specialties marked on the arbitration agreement, a panel of 3 arbitrators is randomly selected. The PANEL has 7 days to hear arguments and answer questions. At the end of those 7 days, they each issue a judgment. The Majority order is binding and causes the escrow to release the smart contract assets in accordance with the order.

