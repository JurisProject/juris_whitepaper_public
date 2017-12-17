# The Juris Framework

##Dispute Handling
#### Evidence, Arguments, and Discussion

When a dispute is triggered, the triggering party will be required by the Juris platform to include itemized claims, their desired resolution, and their initial arguments for the resolution. Additionally they will be able to provide any details or evidence regarding the case that may fall outside of the smart contract logs. All of these details will be attached to the smart contract through the CDK, and other parties will be notified that a dispute has been triggered.

The counter-party to the dispute will have a designated amount of time to respond to the claims of the triggering party. They will be required to provide a direct response to each item of the claim, and their initial arguments for their preferred resolution. Here they will also be able to provide any additional details or evidence for their side that may fall outside of the smart contract logs. If there is no response from the counter-party the system will issue a default judgement in the favor of the claimant. 

The argument submission process will be locked following the response from the defending party, and the submission of additional evidence will be locked before the case proceeds to open discussion. New evidence may be submitted with majority High Jurist approval. Further discussion and questioning regarding the case, case details, and evidence, will take place via resolution processes outlined in paragraph 6.4.

### Smart Contract Logs
One of the most critical peices of evidance provided to the Jurists will be the history of logs and transactions assiciated with the scart contract in question. This is especially true when a bug in the smart contract is what brought the contract to Juris. These logs will autmiatcally summarised and made available to Jurists as evidence.

## Resolution Mechanisms
What do you do when you have a dispute with someone off the blockchain? First, you try to work it out amongst yourselves. If you can’t, you’d seek advice. If that advice doesn’t help you solve things, you’ll ask someone neutral to make the choice for you. Juris works the same way. 

### SELF (Self-Enforced Library Functions) Judgement
Problem it solves: Something has gone wrong with a smart contract. All parties to the contract agree what should happen next. This could be caused by a bug, a broken oracle feed, or any other unforeseen event.
How Juris moves: No Juris changes hands when the self-mediation toolkit is activated. The parties “pre-paid” for them when they signed the contract. 
From the parties perspective: This is a free and fast way to amicably resolve a misbehaving contract. 
From the Jurists’ perspective: This keeps trivial business out of the docket. 
How it works: Often, people are able to solve their own disputes. In the case of software bug, or any time the parties agree what the contract should do, but that intended behavior is not the contract’s expected behavior, the parties just need the tools to force some very specific behavior out of the contract. 
For these users, we’re building a package of self mediation tools which implement some basic operations (void the contract, give all assets to party A, ect). These tools will be totally open source and free. 


### SNAP (Simple Neutral Arbitrator Poll) Judgement
Problem it solves: If parties believe that a disagreement in their contract will be resolved by a quick review of the facts by a third party, they should opt for a SNAP.
How Juris moves: The party(s) to the contract requesting the SNAP pay whatever they want to activate the SNAP (above a minimum). 5% of that fee goes to the Juris Foundation, the rest is split equally amongst all of the Jurists in good standing who vote in the SNAP. 
From the parties perspective: It’s a cheap way to get a fast judgement and a lot of input from different perspectives. 
From the Jurists’ perspective: SNAP’s don’t pay very well, but they do offer a lot of opportunities to earn rep. Jurists are always on the hunt for a contract where their unique expertise will be decisive. Since everyone has to split the arbitration fee, it pays to look into disputes that no one else is looking at. You need to pay attention, vote reasonably, and contribute if you’re going to increase or maintain your standing. 
How it works: All parties to a contract have 24 hours to submit an argument. Once they’re all in, any Jurist can see the arguments. To take a case a Jurist must vote based only on the arguments and submit a textual justification of their vote. After 24 hours, if the SNAP has had at least 5 votes the justifications are revealed to the jurists, and Discovery begins. The jurists can ask the parties any questions they have, vote on the questions and comment on the parties responses (very much like a Reddit AMA). By the end of discovery all jurists must vote again (or their opening vote will carry over and they will lose reputation). Then, the collective opinion phase begins, lasting 36 hours. Using the git source control system, Jurists collaboratively author an opinion for each position that received at least one vote. Based on the vote and opinion, the parties can decide to self mediate an outcome, or appeal for a PANEL. 


The format allows parties to provide opening arguments while also allowing the jurists to directly question the parties. This is designed to be a fusion of the anglo-american adversarial format with the east asian inquisitorial format.

This VOTE --> JUSTIFY --> DISCUSS --> VOTE → JUSTIFY model is based on the Delphi Method of collective decision making. The Delphi Method has been shown to be very effective at surfacing hidden profiles while producing judgements that have broad support and alignment with facts.  


### PANEL (Peremptory Agreement for Neutral Expert Litigation) Judgement
Problem it solves: When a dispute is complex or there is a lot at stake, you want a small number of people to take their time examining all of the evidence, and hearing all of the arguments. 
How Juris moves: The party(s) to the contract requesting the PANEL pay the market rate to convene the panel. 5% of that fee goes to the Foundation,  the rest is split equally amongst the Jurists on the panel. 
From the parties perspective: For complex disputes that require deep attention of the most skilled jurists, it’s worth paying for a PANEL. 
From the Jurists’ perspective: This is where the real money is. But in order to get put on a panel, you need to have very high rep. All of that work spent in SNAP’s is paying off here! 
How it works: The party(s) requesting the PANEL sends a PANEL transaction with JRS attached into the contract. All of the assets in the contested contract are moved into escrow. Based on the domain specialties marked on the arbitration agreement, a panel of 3 arbitrators is randomly selected. The PANEL has 7 days to hear arguments and answer questions. At the end of those 7 days, they each issue a judgment. The Majority order is binding and causes the escrow to release the smart contract assets in accordance with the order. 
