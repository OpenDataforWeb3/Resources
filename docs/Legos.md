---
title : "Legos"
description: "List of Legos Useful to the Open Data Community"
---

### List of Useful Legos

Legos
Below is a list curated to highlight some of the Legos useful to the ODC Landscape.

legos are literally "pieces that can be joined together to make models of many different objects" and more importantly Legos in this context are said to be **components of the data mesh which have consistent input and outputs which can easily duplicate analysis and other repeated functions used to better empower communities collective decision making [more](https://github.com/Fraud-Detection-and-Defense/lego-docs) and [more](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546) on Legos**

### Gitcoin Passport
- [Website](https://go.gitcoin.co/passport)
- [Github](https://github.com/gitcoinco/passport)

- How It Works: *When a user connects a passport, a trust score can be calculated for them which is used as evidence of personhood - the greater the score the more likely they are to be a genuine user.*


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

**Resources**

- [Public goods legos roadmap](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546)
- [Legos for Prioritization](https://docs.google.com/spreadsheets/d/1FIYR7wtFEGfZTjMNXDMbkRDyfdtgkWJvbvsLpAD5eSE/edit#gid=354684328)
- [Open Data Community Discord](https://discord.gg/Ye3QrWf6fG)
- [Gitcoin Governace Forum](https://discord.gg/gitcoin)





