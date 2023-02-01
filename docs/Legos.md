---
title : "Legos"
description: "List of Legos Useful to the Open Data Community"
---

### List of Useful Legos

Legos
Below is a list curated to highlight some of the Legos useful to the ODC Landscape.

legos are literally "pieces that can be joined together to make models of many different objects" and more importantly Legos in this context are said to be **components of the data mesh which have consistent input and outputs which can easily duplicate analysis and other repeated functions used to better empower communities collective decision making [more](https://github.com/Fraud-Detection-and-Defense/lego-docs) and [more](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546) on Legos**


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

**On-chain Footprint Lego**

- How It Works : The TDD (Transaction Date Mean Difference) metric is utilized by this Lego, and it is computed by subtracting each transaction date from the following one to obtain the difference, then dividing by the total number of transactions (i.e., the mean difference or average difference).
- This Lego was developed to counter any attempts by a Sybil attacker to get around transaction count-based security measures by carrying out insignificant transactions in a short period of time to increase the number of transactions, avoid detection, and carry out their attack.

**Address Correlation Lego**
 
 - How It Works: The "address correlation Lego" is a pattern-identification Lego that is intended to be used against previously known sybil patterns that will be stored in a readable format (currently using a pandas dataframe). Its purpose is to judge the correlation between the activities of an address and those of sybil addresses using the Spearman's rank correlation coefficient.



**Resources**

- [Public goods legos roadmap](https://gov.gitcoin.co/t/public-goods-legos-roadmap/12546)
- [Legos for Prioritization](https://docs.google.com/spreadsheets/d/1FIYR7wtFEGfZTjMNXDMbkRDyfdtgkWJvbvsLpAD5eSE/edit#gid=354684328)
- [Open Data COmmunity Discord](https://discord.gg/Ye3QrWf6fG)
- [Gitcoin Governace Forum](https://discord.gg/gitcoin)





