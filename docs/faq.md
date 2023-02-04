---
title: "FAQ"
description: "Answers to frequently asked questions."
lead: "Answers to frequently asked questions."
date: 2022-12-25T21:55:02-03:00
lastmod: 2022-12-25T21:55:02-03:00
draft: false
weight: 50
images: ["avatar.jpg"]
categories: []
tags: []
contributors: [""]
menu:
  docs:
    parent: "FAQ"
weight: 610
toc: true
---

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

## Can I submit a no-code solution, such as an entire static MVP like a really good design?

Yes, absolutely. It just has to be really good!
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

## How Ocean Protocol resist Sybil attacks ?

Ocean Protocol is a decentralized data exchange platform designed to provide secure and transparent access to data. It fights against Sybil attacks by using blockchain technology and cryptographic mechanisms to ensure the authenticity of participants on the network. Here are some ways in which Ocean Protocol resists Sybil attacks:
(i) Decentralization: By using a decentralized network, Ocean Protocol reduces the risk of a single point of failure and makes it more difficult for a malicious actor to control the network.
(ii) Token Economics: Ocean Protocol uses a token-based economy to incentivize good behavior on the network. This makes it more difficult for a malicious actor to control the network, as they would need to own a significant amount of tokens to do so.
(iii) Identity Management: Ocean Protocol uses decentralized identity management systems to ensure that participants are who they say they are. This makes it more difficult for a malicious actor to create multiple identities and conduct a Sybil attack.
(iv) Consensus Mechanisms: Ocean Protocol uses consensus mechanisms, such as proof-of-stake, to validate transactions on the network. This helps to prevent malicious actors from conducting Sybil attacks by controlling a large number of nodes.
By using these mechanisms, Ocean Protocol aims to provide a secure and transparent platform for data exchange, and to resist Sybil attacks.

## What is Ocean Protocol ?
Ocean Protocol is an open-source decentralized platform for data sharing that enables secure and private exchange of data assets. It is built on blockchain technology and aims to provide a secure and transparent marketplace for data assets.

## How can I use the Ocean Protocol?

Ocean Protocol allows for the decentralized sharing of data and algorithms at large scale. 

**DataBuilder Hackathon participants are strongly encouraged to use the Ocean Protocol.**  It is free, other than minor gas fees, and preferred by the judges as an easy way to show your commitment to resisting centralization as the data layer. 

Ocean provides a free and easy way to decentralize access control to algorithms and/or deploy ERC725Y as soulbound tokens for preventing misuse of DAO proposal mechanisms.

Ocean Protocol has authored a step-by-step guide for DataBuilder Hackathon participants here:  
[https://github.com/oceanprotocol/data-challenges/blob/main/DataBuilders%20Hackathon.md](https://github.com/oceanprotocol/data-challenges/blob/main/DataBuilders%20Hackathon.md)

Ocean Protocol experts will also be available on the DataBuilder hackathon Discord within the OpenData Community.

And the Ocean Protocol has extensive documentation here:
[https://docs.oceanprotocol.com/](https://docs.oceanprotocol.co)

NOTE: If you have any issues getting your data from ocean (maybe your download won't start), do try to download again, if it persist, we recommend using the Firefox browser and to be a bit more patient as it may take sometime.

## How does Ocean Protocol work?

   Ocean Protocol operates on a decentralized network, where data providers can securely and privately share their data assets with data consumers. It uses blockchain technology to ensure secure and transparent transactions, and smart contracts to enforce rules and regulations for data sharing.


## Hackathon FAQ:  How can I use Pocket Network ?

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

##  Who can use Trueblock with Gitcoin?

Anyone who is involved in the Gitcoin grants process can use Trueblock to provide transparency and accountability in their projects. This includes grantees, grant makers, and anyone else who is interested in tracking the progress of Gitcoin grants.

## What are the benefits of using Trueblock with Gitcoin?

By using Trueblock with Gitcoin, grantees can increase transparency and accountability in their projects, and Gitcoin can ensure that funds are being used effectively. Some of the key benefits include:
(i) Increased transparency: Trueblock allows grantees to report on their progress and for Gitcoin to verify that progress, providing a more transparent view of how funds are being used.
(ii) Improved accountability: Trueblock helps to ensure that grantees are using funds as intended and making progress on their projects, which helps to improve accountability in the grants process.
(iii) Better project management: By using Trueblock, grantees can more effectively track their progress and make adjustments as needed, improving the overall management of their projects.

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

## What's LEGO and how can it help control sybil Attacks?

The term "Lego" refers to discrete, modular units of code that carry out a specific task and can be assembled to make new things. Legos need to be tightly scoped, open and accessible, permissionless, have few dependencies, be modular, have open governance, take well defined inputs, and provide certain known outputs in order to be composable. ERC-20/721 token standards and Ethereum smart contracts are two examples of assembleable Legos. By giving the community the resources for innovative new solutions, the objective is to introduce freedom and agency to the funding of public goods. The gitcoin passport is one example of aUp Lego.

An anti-Sybil tool called the Gitcoin Passport uses stamps to act as a means of identification. For the retroactive squelching of Sybils, a trained machine learning pipeline is employed, but it is centralized and operated by a small group of specialists. By creating a standardized framework for modeling and model auditing, users will be able to train their own models, turning this into a set of assembleable Sybil defensive legos. To counter Sybil assaults, additional tools can be created, such as rules for resolving conflicts and governance legos. The decision to use Gitcoin models or train one's own models rests with the user.

##  How do LEGO bricks work in Gitcoin Grants?

In Gitcoin Grants, individual contributions are aggregated to support open source projects and initiatives. Contributors can make small donations, or "LEGO bricks," which are combined to provide funding for the project. This allows for a large number of individuals to collectively support the project, even if they cannot make a large individual contribution.

## What  are the benefits of using LEGO bricks in Gitcoin Grants?

Using LEGO bricks in Gitcoin Grants provides several benefits, including:
Increased accessibility: Small contributions make it easier for individuals to support open source projects, even if they cannot make a large individual donation.
Increased engagement: By allowing individuals to contribute small amounts, Gitcoin Grants encourages more engagement and participation from a wider range of contributors.
Increased funding: The aggregation of small contributions can result in significant funding for projects and initiatives, which can help drive open source development.

## Who can contribute LEGO bricks in Gitcoin Grants?

Anyone can contribute LEGO bricks to Gitcoin Grants. The platform is open to anyone who wants to support open source projects and initiatives, regardless of their location or financial resources.

## How can I contribute LEGO bricks to a Gitcoin Grant?

To contribute LEGO bricks to a Gitcoin Grant, you simply need to make a donation through the Gitcoin platform. You can choose the amount you want to donate and your contribution will be combined with others to support the project or initiative.

## What is OpenData Community (ODC) ?
The OpenData Community (ODC) is a new initiative originally founded by Gitcoin. Through activities like hackathons, knowledge curation, and others, we hope to create, capture and distribute value to those building decenlatrized solutions for an Open Data Layer for web3 and to promote decentralization of web3. 

## How can I help ODC ?

Anyone can help ODC reach its objectives through participating in the active projects at Github. (1) Bootstrapping the ODC Community. (2) Data-Builder Hackthon ending January 31st. (3) The Landscape a useful curation of decentralized data solutions in web3 and (4) Building FAQs and other contributions such as useful curated datasets, website improvements, and design of community voting mechanisms.
For more information join our Discord channel https://discord.com/invite/fmcSubzNwv. 

## What is Landscape relating to ODC ?

The "landscape" in the context of Open Data Community (ODC) refers to the overall view of the different data sets, projects, organizations, and initiatives that exist within the ODC. A landscape analysis provides a comprehensive overview of the different actors, initiatives, and activities that make up the ODC, including the various types of data being collected and shared, the different use cases and applications, and the various challenges and opportunities faced by the ODC.
The purpose of a landscape analysis is to help organizations and individuals better understand the ODC and how they can contribute to or benefit from it. By providing a comprehensive view of the ODC, a landscape analysis can help organizations identify new opportunities, identify gaps in the data, and develop new initiatives and collaborations that can help advance the ODC.



