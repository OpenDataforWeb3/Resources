---
title : "Legos"
description: "List of Legos Useful to the Open Data Community"
---

Legos are **algorithms that are packaged typically as Docker containers and that have consistent input and output schemas; Legos make algorithmic analysis more modular due to their standarized inputs / outputs and their packaging as containers; Legos also make this analysis somewhat more transparent because it improves the ability to report on the flow of a wallet or other identifier through a pipeline of Legos, identifying specifically which algorithms predicted that a particular wallet or other identifier is likely a Sybil or otherwise flagged as questionsable by the algorithms packaged as Legos. Much [more](https://github.com/Fraud-Detection-and-Defense/lego-docs) and [more](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546) about Legos is available - both sources point to foundation documents authored by the the Gitcoin FDD.  **

Several Legos are already built and are being used to identify Sybils potentially attacking public goods funding via the [Gitcoin protocol](). These includes:

 **Passport Scoring**
[Gitcoin passport](https://passport.gitcoin.co/):
-How It Works: Gitcoin passport is a tool that enables users prove their identity by collecting stamps which are credentials from web2 such as Facebook, Twitter, and web3 i.e BrightID, ENS. 
The combination of stamps in a wallet can be used to create a trust score which can be calculated to use as evidence of personhood,the greater the score the more likely a user is trustable or genuine.
- [Link](https://github.com/gitcoinco/passport-scorer)


**Algorithmic Detection Lego**
- How It Works: Sybils are detected on how the user's spread fund in bulk (Bulk Transfers) and in what pattern they make donation to the same grant(Bulk Donations).
- Created by TrustaLabs in the last hackathon.
- [Github Repo](https://github.com/TrustaLabs/slaysybil)


### List of Useful Legos

Below is a list curated to highlight some of the Legos useful to the ODC Landscape.
### [Sybil-Scoring] 

**Shared IP:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_visitsIP.R)

- How It Works: *User IP addresses can also be checked to see if they are shared with many other users. Lots of addresses originating from the same IP could be a marker for Sybil attackers.*

**SAD Model:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_SAD.R)

- How It Works: *The user also has a Gitcoin account whose history can be analyzed using the SAD model to give another Sybil-likelihood score.*

**DonorDNA:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_DNA.R)

- How It Works: *When a donor connects their wallet their profile of past donations can be analyzed to see whether it is similar to groups of other users, which may be indicatative of Sybil rings.*

**GrantDNA:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_DNA.R)

- How It Works: *Each grant has a set of donors that can be represented as a set of binary data. This can be used to compare grants against flagged grants to see if they have similar donor profiles.*

**Onchain Intersectionality:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_intersectionality.R)

- How It Works: *It checks "How many out of a set of on-chain credentials does a user have?"*

 [Githup repo to sybil scoring LEGOs developed by the FDD](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs)

**Levenstein distance:**
- [Github](https://github.com/Fraud-Detection-and-Defense/Gitcoin-Sybil-LEGOs/blob/main/scripts_process/process_levenshtein.R)

- How It Works: *Every user has a username - when they sign up to Gitcoin grants the similarity of their name can be compared against all other usernames to generate a likelihood of the username being auto-generated - evidence of a Sybil account. This Lego will be deprecated in the grants protocol because usernames will no longer be available - only Ethereum addresses, wallet IDs and grant/round nonce.*

**On-Chain History:**

- How It Works: *This Lego returns a Yes or No value if a user engaged in certain web3 activities in a specific timeframe.*

- As a Grant Lego: *The project's activities in a specific time frame can be used here to make a well-informed decision by the round operator on sybil detection, and with allowance for customization of the project’s time span, greater flexibility is provided and a lot more specificity in analysis and decision-making for different.
When this lego is combined with several other Legos, a more robust and comprehensive result can be reached.*

- As a Donation Lego: *By Understanding the behavior of a donor's wallet, the wallet on-chain history in this particular case a more informed decision can be taken. It is proposed that this lego be also customizable for any specific time span.*


**Money-Mixer:**


- How It Works: *Returns a Boolean if a user has interacted with known money-mixers.*

- As a Grant Lego: *This lego checks for grant recipient addresses interaction with known money-mixer services. Could be a bad signal if grant recipient addresses have interacted with money-mixers.*

- As a Donation Lego: *This Lego checks for the donation wallet’s address interaction with known money-mixers. Might not be a particularly significant signal for donors.*


**High Frequency Trading:**

- How it works: *Returns boolean wallet activity timestamps over # of transactions;*

- Grant Lego: *The range of wallet activity timestamps over the number of transactions; often an indicator of bot-control or other automatic wallet-vetting scripts; The threshold for this metric is yet to be determined and may be set dynamically based on community averages. This dynamic approach allows for a more accurate representation of the range of wallet activity timestamps and a more effective way of detecting potential bot activity.*


**Social Presence:**

- How It Works: *Returns Boolean if a project is within 1 standard deviation from the dynamic mean.*

- Grant Lego: *Evaluates the relationship between the amount of unique donations received and the number of twitter followers. Returns a boolean if a particular project is within 1 standard deviation from the ratio of the number of Twitter followers for a specific grant to the number of unique donations received for that grant.*


**Farmer Boolean:**

- How It Works: *uses on-chain data to determine whether a user has >X ERC-20 tokens and an average transaction value <Y ETH)*

- Grant Lego: *This lego is fed from on-chain data with thresholds where the number of distinct assets held > 10 on ERC-20; avg transaction value < 0.01 ETH.*


**Funding Wallet Is Unique:**

- How It Works: *Returns Boolean for uniqueness of funding wallet*

- Grant Lego: *This can be utilized with other indicators that could determine duplicate grant creation more. Could be used as a proof to indicate high risk money-mixing activity.*

**Slaysybil**

- [Github](https://github.com/TrustaLabs/slaysybil)

- How it works: *Tracking bulk transfers and donations to detect sybils with observing sequential behaviour pattern and asset-transfer graph. Built by TrustaLabs*

**On-chain Footprint Lego**

- How It Works : The TDD (Transaction Date Mean Difference) metric is utilized by this Lego, and it is computed by subtracting each transaction date from the following one to obtain the difference, then dividing by the total number of transactions (i.e., the mean difference or average difference).
- This Lego was developed to counter any attempts by a Sybil attacker to get around transaction count-based security measures by carrying out insignificant transactions in a short period of time to increase the number of transactions, avoid detection, and carry out their attack.

**Address Correlation Lego**
 
 - How It Works: The "address correlation Lego" is a pattern-identification Lego that is intended to be used against previously known sybil patterns that will be stored in a readable format (currently using a pandas dataframe). Its purpose is to judge the correlation between the activities of an address and those of sybil addresses using the Spearman's rank correlation coefficient.

**Flagged Activity**

- How It Works: _Returns whether address is in close association with addresses flagged as phishing/scam on Etherscan (send or receive event; last 365 days)._

**Script-Call to API**

- How It Works: _Imitate Bankless' use of "bot-label" for any python, curl, etc. direct-access to Passport API_

**On-Trend / Off-Trend**

- How It Works: _Determines whether user donation array is within-range for statistical averages of the community_

### Other Anti-sybil Technology

**Upala**
- [Website](https://upalahq.notion.site/upalahq/Upala-dashboard-a46d88209ecb4a4cabf1560acc8673a2)
- [Github](https://github.com/upala-digital-identity/upala)
- Summary: *Upala is a decentralized digital identity. The protocol generates human uniqueness score for users. The score is measured in dollars. Each account score is determined by market. Incentives ensure that the score equals the costs of forging the account. The score directly reflects how valuable that identity is to the user and creates an entirely new way to measure reputability in the virtual and real world.*

**POAP - Proof of Attendance Protocol**
- [Website](https://poap.xyz/)
- [Github](https://github.com/poap-xyz/)
- Summary - The Proof of Attendance Protocol turns events or hackathons into collectibles. Using blockchain technology, POAP tokenizes your proof of participation, so they can be used as DIDs (decentralized Identifiers).

**UBI - Universal Basic Income**
- [Website](https://ubi.eth.limo/)
- [Github](https://github.com/DemocracyEarth/ubi)
- Summary: Universal basic income (UBI) aims to address economic inequality and provide security through streamed cash to every human on Earth. It is built on top of Ethereum and the Proof of Humanity protocol. Every human that gets verified by submitting a video of themseleves.

**Proof Of Humanity**
- [Website](https://proofofhumanity.id/)
- [Github](https://github.com/Proof-Of-Humanity)
- Summary: Humans who wish to be included in the registry submit information about themselves serving for verification. Then you can vouch for others and challenge suspicious users just like Kleros.

**Idena - Proof-of-Person blockchain**
- [Website](https://www.idena.io/)
- [Github](https://github.com/idena-network)
- Summary: The Idena blockchain is driven by Proof-of-Person consensus with every node linked to a cryptoidentity, one person with equal voting power. It suggests a novel way to formalize people on the Internet: Idena proves the humanness and uniqueness of its participants without collecting personally identifiable information by running a Turing test at the same time globally.

**BrightID**
- [Website](https://www.brightid.org/)
- [Github](https://github.com/BrightID)
- Summary: BrightID is building an identity lego that allows users to prove to applications that they only exist once in any given system. It's one of the legos used in Gitcoin Passport. You can get 50% bonus matching for all your Gitcoin grants by joining BrightID and connecting it to your Gitcoin Passport.
=======

**Resources**

- [Public goods legos roadmap](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546)
- [Legos for Prioritization](https://docs.google.com/spreadsheets/d/1FIYR7wtFEGfZTjMNXDMbkRDyfdtgkWJvbvsLpAD5eSE/edit#gid=354684328)
- [Open Data Community Discord](https://discord.gg/Ye3QrWf6fG)
- [Gitcoin Governace Forum](https://discord.gg/gitcoin)





