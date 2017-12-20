# The Juris Framework

### Evidence, Arguments, and Discussion

When a dispute is triggered, the triggering party will be required by the Juris platform to include itemized claims, their desired resolution, and their initial arguments for that resolution. Additionally they will be able to provide any details or evidence regarding the case that may fall outside of the smart contract logs. All of these details will be attached to the smart contract through the CDK, and other parties will be notified that a dispute has been triggered.

The counter-party to the dispute will have a designated amount of time to respond to the claims of the triggering party. They will be required to provide a direct response to each item of the claim, and their initial arguments for their preferred resolution. Here they will also be able to provide any additional details or evidence for their side that may fall outside of the smart contract logs. If there is no response from the counter-party the system will issue a default judgement in the favor of the claimant.

The argument submission process will be locked following the response from the defending party, and the submission of additional evidence will be locked before the case proceeds to open discussion. New evidence may be submitted with majority High Jurist approval. Further discussion and questioning regarding the case, case details, and evidence, will take place via resolution processes outlined in paragraph 6.4.

### Smart Contract Logs

One of the most critical pieces of evidence provided to the Jurists will be the history of logs and transactions associated with the smart contract in question. This is especially true when a bug in the smart contract is what brought the contract to Juris. These logs will be automatically summarized and made available to Jurists as evidence.

## Three Resolution Mechanisms

### SELF \(Self-Enforced Library Functions\) Judgement

**Problem it solves:** Something has gone wrong with a smart contract. All parties to the contract agree what should happen next. This could be caused by a bug, a broken oracle feed, or any other unforeseen event. Whether right away, or after brief negotiation the parties have a solution and they agree that the solution is fair.

**How Juris moves:** No Juris changes hands when the self-mediation toolkit is activated. The parties “pre-paid” for them when they signed the contract and attached their JRS.

**From the parties perspective:** This is a free and fast way to amicably resolve a misbehaving contract.

**From the Jurists’ perspective:** This keeps trivial business out of the docket.

**How it works:** The incorporation of the Juris CDK allows the protocol to alter the outcome of a smart contract. Through the Juris dashboard the parties to the contract have access a package of self mediation tools which provide for the implementation of some basic operations to designate a different outcome for the smart contract, \(void the contract, give all assets to party A, etc\). These tools will be totally open source and free.

### SNAP \(Simple Neutral Arbitrator Poll\) Judgement

**Problem it solves:** If parties are unable to settle on an outcome on their own, and believe that a disagreement in their contract will be resolved by a quick review of the facts by a third party, they should opt for a SNAP.

**How Juris moves:** The party\(s\) to the contract requesting the SNAP pay whatever they want to activate the SNAP \(above a minimum\). 5% of that fee goes to the Juris Foundation, the rest is split equally amongst all of the Jurists in good standing who take part in the SNAP. 

**From the parties perspective:** It’s a cheap way to get a fast judgement and a lot of input from different perspectives. It may have the power to quickly resolve a negotiation stalemate.

**From the Jurists’ perspective:** SNAP’s don’t pay very well, but they do offer a lot of opportunities to earn reputation. Jurists are always on the hunt for a contract where their unique expertise will be decisive. Since everyone has to split the arbitration fee, it pays to look into disputes that no one else is looking at. You need to pay attention, vote reasonably, and contribute if you’re going to increase or maintain your standing.

**How it works:** After a contract has executed, parties to the contract \(the “Disputants”\) have 24 hours, \(the “Initiation Opportunity”\) to initiate a SNAP, this time period can also be extended by mutual agreement, or via the CDK when the contract is  created. At the moment that the SNAP is initiated \(the “Initiation Date”\), the Juris plugin collects and freezes all transaction logs, contract execution logs, contract state, and the contract code itself \(together, the “Hard Evidence”\). From the Initiation Date, Disputants have 24 hours \(the “Preparation”\) to compose a document outlining their dispute \(the “Case Brief”\). A Case Brief contains itemized \(e.g. bulleted\) written arguments \(the “Formal Complaint”\), and optionally itemized additional facts \(the “Supplementary Evidence”\) the Disputant would like to present during the judgement. At the close of Preparation \(the “Publication Date”\), the Hard Evidence, and optionally the Case Briefs \(at the discretion of the Disputations\), are posted to JRS Token holders publicly \(the “Case Publication”\) for review, for a 24 hour period \(the “Jury Selection”\).

Arbitrators may access any Case Publication without obligation to participate in the case, but must pass a Captcha test \(or equivalent\) before being granted access to the Case Publication. If an individual chooses to join a SNAP as a participating arbitrator \(a “Jurist”\) after reading a Case Publication, that person must cast their initial vote \(the “Independent Vote”\) using only the information in the Case Publication. When casting their Independent Vote, an arbitrator must cite justification \(the “Independent Evidence Selection”\) from at least one of \(a\) an item of Hard Evidence, \(b\) an item of a Formal Complaint, or \(c\) an item of Supplementary Evidence \(together and separately, the “Case Publication Items”\). As part of the Independent Judgement, an arbitrator must also provide a short \(255 characters or less\) summary of their opinion \(the “Independent Opinion”\). Together, the Independent Vote, Supporting Evidence Selection, and Independent Opinion comprise the arbitrator’s individual analysis \(the “Independent Judgement”\) of the case. After submitting the Independent Judgement, an arbitrator formally becomes a Jurist for the given SNAP.

During Jury Selection, all Independent Judgements remain hidden from both the Disputants and the Jurists. However, the number of Jurists that have joined the SNAP is displayed publicly. At the end of Jury Selection \(the “Trial Date”\), the Case Publication is taken down, jury selection ceases, and a 24 hour window for open arguments begins \(the “Trial”\).

On the Trial Date, all Jurists and Disputants \(together and severally, the “Trial Participants”\) are made privy to the SNAP’s tally of votes, the tally of each Supporting Evidence Selection, and the Independent Opinions, all of which are anonymized. During the Trial, Jurists make material contributions to the arbitration \(the “Trial Artifacts”\) in the form of: questions posed for other Trial Participants, submission of general comments, citations of case history, comments on any item in the Case Publication, written responses to any of the above and to other written responses, and atomic responses \(up/down vote\) to any of the above.

After 24 hours from the Trial Date, the Trial ends \(the “Trial Close Date”\), at which point interaction between and among all Trial Participants ceases for a period of 12 hours \(the “Deliberation”\). In Deliberation, Jurists have an opportunity to independently review the Case Publication and all Trial Artifacts. After Deliberation, each Jurist must cast a final vote \(the “Informed Vote”\), select one or more pieces of supporting evidence \(the “Informed Evidence Selection”\) from any Case Publication Item or Trial Artifact, and compose a written summary of their opinion \(the “Informed Opinion”\) no longer than 500 characters. Together, the Informed Vote, Informed Evidence Selection, and Informed Opinion comprise the Jurist’s Informed Judgement. During Deliberation, the contents of the Informed Judgements remain hidden from all Trial Participants.

At the end of Deliberation \(the “Judgement Date”\), all of the Informed Judgements are closed for modification, and each Jurist is immediately placed into a group of peers \(a “Consensus Group”\) who voted in favor of the same Disputant. Each Consensus Group is firewalled from both the other Consensus Group and from the Disputant. Starting from the Judgement Date, each Consensus Group has 24 hours \(the “Opinion Composition”\) to confer amongst its members and write an opinion on their ruling \(the “Final Opinion”\). The Jurist with the highest reputation within an individual Consensus Group is automatically selected as the leader of their cohort \(the “Lead Opinion Writer”\). Optionally, the default Lead Opinion Writer may appoint another Jurist within their Consensus Group as the Lead Opinion Writer.

During Opinion Composition, each Consensus Group has access to the Case Publication, its member Jurists’ Independent Judgements, all of the Trial Artifacts, its member Jurists’ Informed Judgements, and the tally of Informed Votes for each Consensus Group. The Jurists of a Consensus Group collaborate during Opinion Composition by making material contributions \(the “Opinion Artifacts”\) in the same form as Trial Artifacts. Before the end of the Opinion Composition, each Consensus Group compiles these Opinion Artifacts into a Final Opinion.

At the end of Opinion Composition, communication between all Trial Participants ceases, and the Final Opinions from both Consensus Groups are delivered to all Trial Participants \(the “Verdict”\) along with a breakdown of the final voting split.

### PANEL \(Peremptory Agreement for Neutral Expert Litigation\) Judgement

**Problem it solves:** When a dispute is complex or there is a lot at stake, you want a small number of people to take their time examining all of the evidence, and hearing all of the arguments.

**How Juris moves:** The party\(s\) to the contract requesting the PANEL pay the market rate to convene the panel. 5% of that fee goes to the Foundation,  the rest is split equally amongst the Jurists on the panel.

**From the parties perspective:** For complex disputes that require deep attention of the most skilled jurists, it’s worth paying for a PANEL.

**From the Jurists’ perspective:** This is where the real money is. But in order to get put on a panel, you need to have very high rep. All of that work spent in SNAP’s is paying off here!

**How it works:** The party\(s\) requesting the PANEL sends a PANEL transaction with JRS attached into the contract. All of the assets in the contested contract are moved into escrow. Based on the domain specialties marked on the arbitration agreement, a panel of 3 arbitrators is randomly selected. The PANEL has 7 days to hear arguments and answer questions. At the end of those 7 days, they each issue a judgment. The Majority order is binding and causes the escrow to release the smart contract assets in accordance with the order.

