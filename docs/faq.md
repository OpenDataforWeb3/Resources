## What is a Hackathon?

In general a Hackathon is a social coding event that brings together computer programmers like software developers, analysts,  designers and user interface specialists along with industry process experts and professionals to identify issues and create software solutions within a specific period of time.

## Who can participate in the Open Data Community (ODC) hackathon?

Everybody is welcome to apply and be part of the Open Data Community (ODC) hackathon. We are looking for hackers, coders, makers but also for innovators, engineers, creative people, designers, data geeks and startups. Specifically, Data analysts and data scientists, software developers, and DevRel contributors are all well suited for the different bounties and contests of this hackathon.  

## Any prepared dataset for use during the hackathon?
Yes, we have prepared a dataset for your use that includes information about recent grants rounds with Unicef and with Fantom:

UNICEF and Fantom datasets [https://market.oceanprotocol.com/asset/did:op:d4b54f5ab4f171aec585b83189931625eab3803981e9658fe472a87ddc039b0b](https://market.oceanprotocol.com/asset/did:op:d4b54f5ab4f171aec585b83189931625eab3803981e9658fe472a87ddc039b0b)

Gitcoin gr15 datasets [https://market.oceanprotocol.com/asset/did:op:f40b1d9c08b737b72d25f705389ca6f3a42c0320887c0276eb28641357dffdf0](https://market.oceanprotocol.com/asset/did:op:f40b1d9c08b737b72d25f705389ca6f3a42c0320887c0276eb28641357dffdf0)

We have tied together all our datasets uploads here: [https://market.oceanprotocol.com/profile/0x6fd78613E08FCB92890e65eA14450750aCAFF7b5](https://market.oceanprotocol.com/profile/0x6fd78613E08FCB92890e65eA14450750aCAFF7b5)

## In the Anti-Sybil Dashboard bounty, are we expected to come up with new LEGOs  or work with the existing ones?

You can work with existing ones! To get started, you might want to go with mock ones of course.

## Where can I find an example dashboard screen that I may find useful in developing legos for the OpenData Community Hackathon?

[../sybil-image.png](../sybil-image.png)

For a fancy version, you can see the docs from TrustaLabs.  They just launched a commercial Sybil scoring project and are one of our sponsors here as well.  

[https://trustalabs.gitbook.io/trustscan/product-guides/details-of-the-sybil-risk-report](https://trustalabs.gitbook.io/trustscan/product-guides/details-of-the-sybil-risk-report)

More importantly,Program managers want to know how is my round doing and Is it getting attacked!
Here are some of the lego ideas.. [https://docs.google.com/spreadsheets/d/1sMgm3cg3pfMvRbmrteknpu44qsyuQlvn3vizgwnOgOU/edit#gid=2020378185](https://docs.google.com/spreadsheets/d/1sMgm3cg3pfMvRbmrteknpu44qsyuQlvn3vizgwnOgOU/edit#gid=2020378185)

## zkSync, bulk transactions and how it works

[https://v2-docs.zksync.io/dev/fundamentals/zkSync.html#prerequisites](https://v2-docs.zksync.io/dev/fundamentals/zkSync.html#prerequisites)zkSync is a layer2 solution for transferring Ether and ERC20 tokens. The L2 protocol positions itself as a scaling and privacy engine for Ethereum. The project is built on zero Knowledge (ZK) rollup architecture with the idea of “unlimited” Ethereum scaling.

Ethereum scaling is dependent on addressing inherent drawbacks of Ethereum - slow transactions and high gas fees due to limited throughput(i.e the amount of transactions that can happen at any given period of time). 

To ensure “unlimited” Ethereum scaling with zkSync, computation is performed off-chain and most data is stored off-chain. As all transactions are proven using what is known as validity proofs on the Ethereum mainchain, and users enjoy the same level of security as in Ethereum. What this allows is to batch many transactions together (i.e bulk transactions) and send them to the L1 (i.e Ethereum). Currently, a batch is guaranteed to be able to successfully process a max of 50 transactions.

There are many layer 2 solutions to solve Ethereum’s congestion problem. One of these solutions are rollups: ZK rollups (ex. zkSync) and Optimistic rollups. The rollup is basically an Ethereum extension designed to increase scalability. The extension rolls up many transactions into one batch and sends them all to Ethereum in one action. In other words, a roll-up block is a summary of changes reflecting all transactions in a single batch.

Collect Transactions > Generate Proofs > Send to L1

## Sybil Attacks

A Sybil attack is a kind of security threat on an online system where one person tries to take over the network by creating multiple accounts, nodes or computers. This can be as simple as one person creating multiple social media accounts, but in the world of cryptocurrencies, a more relevant example is where somebody runs multiple nodes on a blockchain network. 

## What problems can Sybil attacks cause?
Attackers may be able to out-vote the honest nodes on the network if they create enough fake identities (or Sybil identities). They can then refuse to receive or transmit blocks, effectively blocking other users from a network.

In really large-scale Sybil attacks, where the attackers manage to control the majority of the network computing power or hash rate, they can carry out a 51% attack. In such cases, they may change the ordering of transactions, and prevent transactions from being confirmed. They may even reverse transactions that they made while in control, which can lead to double spending. 

Over the years, computer scientists have dedicated a lot of time and research to figure out how to detect and prevent Sybil attacks, with varying degrees of effectiveness. For now, there’s no guaranteed defense.

A good question to ask is: In what ways can zkSync (ZK Rollups) help reduce Sybil attacks, or help increase the risks of a network having a Sybil attack?

For further reading: 
* [https://go.gitcoin.co/blog/a-community-based-roadmap-for-sybil-detection-across-web-3](https://go.gitcoin.co/blog/a-community-based-roadmap-for-sybil-detection-across-web-3)
* [https://www.youtube.com/watch?v=-EKhIBUQjcA](https://www.youtube.com/watch?v=-EKhIBUQjcA)
* [https://www.youtube.com/watch?v=_VolZn0y-FM](https://www.youtube.com/watch?v=_VolZn0y-FM)
* [https://vitalik.ca/general/2021/01/05/rollup.html](https://vitalik.ca/general/2021/01/05/rollup.html)
## Hackathon FAQ:  How can I use the Ocean Protocol?

Ocean Protocol allows for the decentralized sharing of data and algorithms.  

**DataBuilder Hackathon participants are strongly encouraged to use the Ocean Protocol.**  It is free, other than minor gas fees, and preferred by the judges as an easy way to show your commitment to resisting centralization as the data layer. 

Ocean provides a free and easy way to decentralize access control to algorithms and/or deploy ERC725Y as soulbound tokens for preventing misuse of DAO proposal mechanisms.

Ocean Protocol has authored a step-by-step guide for DataBuilder Hackathon participants here:  
[https://github.com/oceanprotocol/data-challenges/blob/main/DataBuilders%20Hackathon.md](https://github.com/oceanprotocol/data-challenges/blob/main/DataBuilders%20Hackathon.md)

Ocean Protocol experts will also be available on the DataBuilder hackathon Discord within the OpenData Community.

And the Ocean Protocol has extensive documentation here:
[https://docs.oceanprotocol.com/](https://docs.oceanprotocol.co)

NOTE: If you have any issues getting your data from ocean (maybe your download won't start), do try to download again, if it persist, we recommend using the Firefox browser and to be a bit more patient as it may take sometime.

## How to contribute to the hackathon

The ODC team has detailed how best to contribute to the hackthon here : [https://github.com/OpenDataforWeb3/Resources/blob/main/CONTRIBUTING.md](https://github.com/OpenDataforWeb3/Resources/blob/main/CONTRIBUTING.md)

## Hackathon FAQ:  How can I use Pocket Network?

Pocket Network is an open-source decentralized RPC network with a contributor-friendly ecosystem governed by a high-performance DAO. It allows Web3 developers to remove the most important layer of centralization in their projects: connection to the blockchain. Instead of using a centralized service, Pocket's decentralized network of tens of thousands of nodes is run by the community.  DataBuilder Hackathon participants can use the Pocket Network to access blockchain data free from the centralization of many providers of blockchain nodes and data.  

**DataBuilder Hackathon participants are strongly encouraged to use Pocket Network.**  

All hackathon participants have access to the Pocket Network decentralized RPC endpoints. You can go to the Pocket Portal and sign up for a free account, and you'll be able to access any one of dozens of blockchains for up to 250,000 relays per day at no charge. [https://www.portal.pokt.network/](https://www.portal.pokt.network/?utm_medium=cta&utm_source=odc&utm_campaign=data-builder-hackathon&utm_content=faq-page) 

Users will also have access to Pocket's robust RPC API, with connections available to Ethereum and all other major blockchains.  More information about the Pocket Network APIs are available here: [https://docs.pokt.network/api-docs/](https://docs.pokt.network/api-docs/pokt/?utm_medium=cta&utm_source=odc&utm_campaign=data-builder-hackathon&utm_content=faq-page) In order to query againsts these inputs you may choose to use True Blocks or another solution to create an index based on wallet ID.  

Pocket team members will be on-hand in the OpenData Community Hackathon Discord channel throughout the event to answer any questions you might have. 


## Hackathon FAQ:  How can I use TrueBlocks?

On-chain data is the foundation of crypto, the ultimate source of truth. However, on-chain data is difficult to work with natively, without any transformations, in part because it is not indexed based on account. As a result in the past many data analysts would rely on centralized sources of information, such as Etherscan or various commercial solutions, because of their ease of use. However, these solutions are typically not open source or decentralized and are out of the control of the data analyst, introducing the risk of lock-in or capture and limiting the opportunities for customization and control.  

TrueBlocks is an open-source project funded in part by the Gitcoin community and the Ethereum foundation that is dedicated to providing an index that improves with usage and that is thoroughly decentralized.

**DataBuilder Hackathon participants should strongly consider using TrueBlocks to provide a local index that can be used to query an RPC from any source, including the decentralized Pocket Network.**  

To get started, participants can Docker run a local copy of the index.
[https://github.com/TrueBlocks/trueblocks-docker](https://github.com/TrueBlocks/trueblocks-docker)

TrueBlocks engineers will be available on the DataBuilder Hackathon OpenData Community Discord.

TrueBlocks documentation which explains much more about how to build and contribute to the shared “unchained” index as well as how to use TrueBlocks and the index for data analysis is available here: [https://trueblocks.io/docs/]( https://trueblocks.io/docs/)


##  What is a Sybil Attack and why we should fight it?

A Sybil attack refers to a type of attack in which an attacker creates multiple fake identities, or "Sybils” to gain an unfair advantage within a decentralized network. This term is a reference to a [book entitled Sybil](https://en.wikipedia.org/wiki/Sybil_(Schreiber_book)). This book was also made into two television movies, the main character Sybil Dorsett endorsed different personalities.

In the context of systems/organizations, Sybil attacks happen when actions or rewards are calculated based on “one human, one identity”.
Fraudsters or 'Sybils' create multiple identities in an attempt to control (vote) or profit ( distributions of funds or rewards).
Fighting this kind of practice enables organizations to have democratic practices without the physical presence of its participants, for example, online voting in DAOs.   
For more in-depth discussion you can check:     
* [33 - Sybil Resistance with Bryan Ford](https://open.spotify.com/episode/0PEAQCYSRZTxDM5qddP4K0?si=bxdF437OTv2xAmRp6XKbp) ( at 14:00 they start to discuss possibilities in a world where we would already solved the sybil attack problem) 

## What is quadratic funding and matching? Why is it important to understand Sybil attacks?  

Quadratic funding is a mechanism used by Gitcoin to fund public goods. Contributions to a grant are matched in a quadratic way by a matching fund.

Check this 60 sec video by Gitcoin to better understand and come back here:  
* [WTF is Quadratic Funding? ](https://wtfisqf.com/?grant=&grant=&match=1)  

Nice, now that you understood, is easy to get why fraudsters create multiple accounts. The idea is simple, make really small contributions to their own project from different accounts in an attempt to maximize ROI, as the quadratic funding algorithm prioritizes distribution of matching funds pool to projects that received donations from the biggest number of community members.

Similarly, the quadratic mechanism can also be applied to voting (quadratic voting) where each voter votes with some tokens, then fraudsters are incentivized to vote for a proposal from many addresses rather than a single address.


## What is the price of forgery? 

The price (or cost) of forgery, as it says, is the cost paid to forge an identity in a system. There are a lot of discussions about economic games involved in Sybil defense. Most systems are designed to develop a high cost of forgery in an attempt to disincentivize Sybil attacks, making the attack expensive and not profitable. Some discussions argue that this could stop Sybil attacks focused on profit but if the motivation is other, like ideological, the cost could be not a barrier.  

In ep 36 of Green Pill podcast, Kevin Owocki and Petr Porobov, founder of Upala, have some discussion around the topic and how Upala is trying to understand the real price of forgery using incentives. 

* [36 - Creating Sybil Resistance with Upala Founder Petr Porobov]( https://open.spotify.com/episode/1Mz7efMzvziu1I8PZXS44O?si=rUpVFBQCSFOj88mK3ncw9Q)

## Where can I find more Sybil fighting content?  

* [Gitcoin Fraud Defense and Detection Forum](https://gov.gitcoin.co/tag/fdd)  
* [Green Pill Podcast](https://greenpill.party/#podcast)- Season 2 is dedicated to regenerative society, some episodes are focused on Digital Identities and Sybil Fighting   
* [BlockScience Blog](https://medium.com/block-science)- Articles with analyses of passed Gitcoin Grants Rounds and other complex system analyses.   
* [Prof. Brain Ford Papers](https://bford.info/pub/) - Prof Brian Ford has studies on decentralized systems, identity and blockchain. Special highlight to: 
 _Identity and Personhood in Digital Democracy: Evaluating Inclusion, Equality, Security, and Privacy in Pseudonym Parties and Other Proofs of Personhood_ 
