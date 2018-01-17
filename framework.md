## The Juris Framework

#### Dispute Triggers

All disputes will be triggered manually, and the ability to trigger a dispute will be limited to a direct party to the contract, or other parties to which the ability has been delegated via the CDK at the time of contract creation. Dispute triggers will be accessible only to these parties through the CDK. The Juris Foundation, its agents, arbitrators, and Jurists are unable to trigger a dispute on behalf of another party.

#### Contract Freeze

The moment that a dispute is triggered the CDK code freezes smart contract processes. The contract code will not continue to run. If the contract is a public contract, or a contract with a massive number of parties, and a previously agreed upon dispute threshold is reached, processes are frozen and additional parties are unable to access the contract until the disputes are resolved.

#### Evidence, Arguments, and Discussion

When a dispute is triggered, the triggering party will be required by the Juris platform to include itemized claims, their desired resolution, and their initial arguments for that resolution \(together, the "Formal Complaint"\). Additionally, they will be able to provide any details or evidence regarding the case that may fall outside of the smart contract logs \("Supplementary Evidence"\). All of these details will be attached to the smart contract through the CDK, and will follow the case through the Juris system.

The counter-party to the dispute will have a designated amount of time to respond to the claims of the triggering party. They will be required to provide a direct response to each item of the claim, as well as their initial arguments for their preferred resolution. Here they will also be able to provide any additional details or evidence for their case that may fall outside of the smart contract logs. If there is no response from the counter-party \(and one is required to proceed,\) the system may issue a default judgement in the favor of the other party.

The argument submission process will be locked following the response from the defending party, and the submission of additional evidence will be locked before the case proceeds to open discussion. New evidence may be submitted with majority High Jurist approval. Further discussion and questioning regarding the case, case details, and evidence will take place via resolution processes outlined below.

#### Holding Wallets

As soon as a Formal Complaint is filed, the CDK code generates a neutral blockchain wallet address into which the funds associated with the contract are moved. The funds can only be released from this wallet via the Juris CDK, and the use of one of the available resolution mechanisms. The neutral wallet address is maintained internally by the CDK code within the smart contract itself and is not known or accessible to contract parties, the Juris Foundation, or Jurists involved at any time.

#### Smart Contract Logs \("Hard Evidence"\)

One of the most critical pieces of evidence provided to the Jurists will be the history of logs and transactions associated with the smart contract in question. This is especially true when a bug in the smart contract is what lead to Juris dispute resolution. At the moment that the dispute is initiated the Juris CDK collects and freezes all transaction logs, contract execution logs, contract state, and the contract code itself. These logs will be automatically summarized and made available to Jurists as evidence.

## Resolution Mechanisms

#### SELF \(Self-Enforced Library Functions\) Judgement

**Problem it solves:** Something has gone wrong with a smart contract, and a dispute has been triggered. All parties to the contract are able to agree what should happen next. This could be caused by a bug, a broken oracle feed, or any other unforeseen event. Whether right away, or after brief negotiation, the parties have a solution and they agree that the solution is fair. But, current smart contract structure does not allow for an adjusted outcome.

**How JRS moves:** No JRS changes hands when the self-mediation toolkit is activated, but all funds in the initial contract are locked.

**From the parties' perspective:** This is a free and fast way to amicably resolve a contract that has resulted in a dispute or undesired outcome.

**From the Jurists’ perspective:** This keeps trivial matters off the docket.

**How it works \(figure 9.1\):** The incorporation of the Juris CDK allows the protocol to alter the outcome of a smart contract. Through the Juris dashboard, the parties to the contract have access a package of self mediation tools, which provide for the implementation of basic operations to designate a different outcome for the smart contract: void the contract, give all assets to party A, split assets evenly, etc. Once and outcome is selected, the details are incorporated into a new resolution smart contract which is uploaded to the blockchain, and executed. These tools will be open source and free.![](/assets/IMG_0061.jpg)_figure 9.1_

#### SNAP \(Simple Neutral Arbitrator Poll\) Judgement

_Based on the Delphi method._[^15]

**Problem it solves:** If parties are unable to settle on an outcome on their own, and believe that a disagreement in their contract will be resolved by a quick review of the facts by a third party, they can escalate to a SNAP. This provides the opportunity to break a deadlock without escalating to binding arbitration.

**How JRS moves:** The minimum fee for a SNAP is covered by the pre-attached JRS, but the party initiating the SNAP may also attach additional JRS to incentivize Jurists to take the case. 5% of the fee goes to the Juris Foundation, the rest is split equally amongst all of the Jurists in good standing who take part in the SNAP.

**From the parties' perspective:** This is a cheap way to get a fast judgement and a lot of input from different perspectives. It may have the power to quickly resolve a negotiation stalemate.

**From the Jurists’ perspective:** SNAP’s don’t pay as well, but they do offer a lot of opportunities to earn reputation. Jurists will always be on the hunt for a contract where their unique expertise will be decisive in order to earn increased reputation. Because everyone has to split the arbitration fee, it pays to look into disputes with fewer initial votes. Because every action impacts reputation, it pays to vote reasonably, be attentive, contribute, and choose cases where you have domain experience in order to increase or maintain your standing.

**How it works \(figure 9.2\):** After a dispute has been triggered, parties may initiate a SNAP. From the date the SNAP is initiated, the parties have a window in which to provide the additional details mentioned above for their Formal Complaint. This is added to the "Case Brief" containing itemized \(e.g. bulleted\) complaints, written arguments, and optionally itemized additional facts the parties would like to present during the judgement. At the close of this window, case briefs are anonymized posted to JRS Token holders publicly for review, and are all available to both parties.

Jurists may access any case brief without obligation to participate in the case, but must pass a Captcha test \(or equivalent\) before being given access to further evidence, or logs. If an individual chooses to join a SNAP as a participating Jurist, they are given access to further evidence and logs, and are required to cast their initial vote using only the information available. When casting their vote, a Jurist must cite justification from at least one of \(a\) an item of Hard Evidence, \(b\) an item of a Formal Complaint, or \(c\) an item of Supplementary Evidence. As part of their judgement, an arbitrator must also provide a short \(255 characters or less\) summary of their opinion. After submitting the above, their "Independent Judgement," an arbitrator formally becomes a Jurist for the given SNAP.

Independent Judgements remain hidden from both the disputing parties and other Jurists until everyone has submitted theirs, or a time limit has been reached. \(The number of Jurists that have joined the SNAP may be displayed publicly in a manner to incentivize Jurists to select cases with fewer assigned Jurists.\) At the end of a designated period of time the case details are no longer public, and open discussion begins among SNAP Jurists.

At this time all participants are made privy to the SNAP’s tally of votes, the tally of evidence selected as justification, and the Independent Opinions, all of which are anonymized. During discussion, Jurists make material contributions to the discussion in the form of: questions posed for other participants, submission of general comments, citations of case history, comments on any item in the Case Brief or supporting materials, written responses to any of the above and to other written responses, and atomic responses \(up/down vote\) to any of the above.

After a designated period the window for discussion is closed, at which point interaction between and among all participants ceases for a period of deliberation. In this time, Jurists have an opportunity to independently review the case details and all additional supporting and discussion materials. After deliberation, each Jurist must cast a final vote, select one or more pieces of supporting evidence, and compose a written summary of their opinion no longer than 500 characters \(collectively, their "Informed Judgement"\). Until the close of the deliberation period, all informed Judgements are hidden from other parties as they are submitted.

At the end of the deliberation period, all of the Informed Judgements are closed for modification, and each Jurist is immediately placed into a group of peers \(a “Consensus Group”\) who voted in favor of the same disputing party. Each Consensus Group is firewalled from both the other Consensus Group and from the disputing party. Each group will have a designated amount of time to confer amongst its members and write an opinion on their ruling \(the “Final Opinion”\). The Jurist with the highest reputation within an individual Consensus Group is automatically selected as the leader of their cohort. Optionally, the default lead Jurist may appoint another Jurist within their Consensus Group as the opinion writer.

During opinion composition, all Jurists retain access to all case briefs, evidence, and discussion details. The Jurists in a given Consensus Group collaborate in the same manner as the earlier discussion. Before the end of the opinion composition, each Consensus Group compiles these Opinion Artifacts into a Final Opinion.

With the submission of the Final Opinion, communication between all participants ceases, and the Final Opinions from both Consensus Groups are delivered to all parties to the contract along with a breakdown of the final voting split. All voting data, discussion records, and opinions are additionally attached to the contract recorded in case of further escalation.

At this point the disputing parties are again given access to the CDK resolution tools to implement an agreed upon dispute solution.![](/assets/IMG_0062.jpg)_figure 9.2_

#### PANEL \(Peremptory Agreement for Neutral Expert Litigation\) Judgement

_Based on UNCITRAL Arbitration Rules_[^16]

**Problem it solves:** While the SNAP procedure provides assistance in dispute resolution, it does not rise to the level of due process required for a binding judgement under United Nations standards. Disputes reaching this level will be complex, will have a lot at stake, or will require binding legal resolution. UN rules thus require a small number of people to take their time examining all of the evidence, and hearing all of the arguments.

**How JRS moves:** The party\(s\) to the contract requesting the PANEL pay the market rate in JRS to convene a panel. 5% of that fee goes to the Foundation, the rest is split equally amongst the Jurists on the panel at the close of proceedings.

**From the parties' perspective:** For complex disputes that require deep attention of the most skilled jurists, or to break a deadlock with a final and legally binding decision, it’s worth paying for a PANEL.

**From the Jurists’ perspective:** This is more labor intensive, but this is where the real money is as fees are higher and split among fewer Jurists. In order to get put on a panel, you need to have High Jurist standing. All of that work spent in SNAPs pays off here.

**How it works: **Similar to normal court systems, this is considered an escalation. Parties cannot proceed to a PANEL judgement without first running a SNAP. If one or both parties are unable to use the assistance of the SNAP to come to a resolution, they may choose to escalate to a PANEL judgement by \(1\) indicating their intent to escalate and \(2\) attaching the required JRS. At this time, all other parties to the contract will be notified of the case escalation, and their required actions. If, at any time, in the PANEL process a party fails to meet a required deadline, a default judgement may be declared at the discretion of the High Jurists.

_**Arbitration Panel Selection:**_ Based on the domain specialties marked on the arbitration agreement, a list of ten available High Jurists will be provided to each party. The High Jurists will be notified at this time of their inclusion on this list, will have access to the case brief, and will be invited to remove themselves if there is a potential conflict of interest. Parties will have 30 days from the delivery of the High Jurist list after which they will be required to select three \(or submit three alternatives\), numbered by preference. If a party chooses alternative arbitrators, any arbitrator not registered through the Juris Foundation will be required to register and provide proof of credentials before the end of the 30 day period. At this time, each list of preferred High Jurists will be shared with the opposing party, which will have 15 days to eliminate up to two of the opposing party's choices. The remaining Jurists will select a third -- neutral -- "Presiding High Jurist," to complete a final panel of three High Jurists. If either party fails to provide a list within the designated 30 day period the Juris system will randomly assign an available High Jurist.

_**Hearing Process:**_ All previous SNAP materials, opinions, evidence, and claims will be made available for review by panel high jurists. The High Jurists will be able to ask any questions of either party, and parties will be required to provide answers \(and may be found in default if they fail to respond.\) If relevant, this may extend as far as the coordination of video-based hearings. At this time, the parties will be allowed, at the discretion of the Jurists, to submit additional evidence, make additional arguments or counter arguments, provide witnesses, and amend previous materials. Any new materials, or communications, will be made available to all other parties at the time of submission.

_**Judgement:**_ At the end of 30 days, \(unless an extension is requested or granted by the panel,\) the High Jurists will render a binding judgement on the facts of the case. Through the Juris dashboard the Jurists will input their decision, and the CDK will unlock the smart contract, and execute the code, automatically enforcing the judgement.

