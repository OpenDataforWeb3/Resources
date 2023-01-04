## Hackathon FAQ:  How can I use the Ocean Protocol?

Ocean Protocol allows for the decentralized sharing of data and algorithms.  

**DataBuilder Hackathon participants are strongly encouraged to use the Ocean Protocol.**  It is free, other than minor gas fees, and preferred by the judges as an easy way to show your commitment to resisting centralization as the data layer. 

Ocean provides a free and easy way to decentralize access control to algorithms and/or deploy ERC725Y as soulbound tokens for preventing misuse of DAO proposal mechanisms.

Ocean Protocol has authored a step-by-step guide for DataBuilder Hackathon participants here:  
[https://github.com/oceanprotocol/data-challenges/blob/GitcoinHackathon/DataBuilders%20Hackathon.md] (https://github.com/oceanprotocol/data-challenges/blob/GitcoinHackathon/DataBuilders%20Hackathon.md)

Ocean Protocol experts will also be available on the DataBuilder hackathon Discord within the OpenData Community.

And the Ocean Protocol has extensive documentation here:
[https://docs.oceanprotocol.com/](https://docs.oceanprotocol.co)


## Hackathon FAQ:  How can I use Pocket Network?

Pocket Network is an open-source decentralized RPC network with a contributor-friendly ecosystem governed by a high-performance DAO. It allows Web3 developers to remove the most important layer of centralization in their projects: connection to the blockchain. Instead of using a centralized service, Pocket's decentralized network of tens of thousands of nodes is run by the community.  DataBuilder Hackathon participants can use the Pocket Network to access blockchain data free from the centralization of many providers of blockchain nodes and data.  

**DataBuilder Hackathon participants are strongly encouraged to use Pocket Network.**  

All hackathon participants have access to the Pocket Network decentralized RPC endpoints. You can go to the Pocket Portal and sign up for a free account, and you'll be able to access any one of dozens of blockchains for up to 250,000 relays per day at no charge. [https://www.portal.pokt.network/](https://www.portal.pokt.network/) 

Users will also have access to Pocket's robust RPC API, with connections available to Ethereum and all other major blockchains.  More information about the Pocket Network APIs are available here: [https://docs.pokt.network/api-docs/](https://docs.pokt.network/api-docs/)  In order to query againsts these inputs you may choose to use True Blocks or another solution to create an index based on wallet ID.  

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
