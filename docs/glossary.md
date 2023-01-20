---
title: "Glossary"
description: "Glossary."
lead: ""
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

## Grants
A grant is an amount of money that is given or awarded to an organization, student, or project. In the context of Gitcoin, grants are used to fund public goods. During Gitcoin grants rounds, eligible grants will be able to receive matching funds from a matching fund using quadratic funding.

## EOA - Externally Own Address 
An EOA is one of a public address derived from a private key. On the public registry, any transaction from or to that address will reference that address. For more details about Ethereum accounts, you can visit [Etherscan: Understanding Ethereum Accounts](https://info.etherscan.com/understanding-ethereum-accounts/#:~:text=An%20externally%20owned%20address%20is,the%20funds%20in%20an%20address.)

## FDD - Fraud Detection & Defense
FDD is part of GitcoinDao and is responsible for detecting and preventing Sybil attacks against Gitcoin Grants.
FDD uses lego to fight Sybil's attacks some of them include Gitcoin Passport, SDD, and human review.

You can find more resources on [Gitcoin blog](https://gov.gitcoin.co/t/introducing-the-fdd-review/11095).

## Gitcoin Passport
Gitcoin Passport is one of the Sybil defense lego built by Gitcoin. It allows a user to acquire stamps to prove his humanness. These stamps are proof of either on-chain activities such as a lens profile, or a POAP and off-chain hard-to-fake web2 actions such as a Twitter account with several followers, a GitHub account with many stars or contributions, a proof of identity with for example BrightId. These credentials are stored on the Ceramic and can be queried to build a trust score for an address.

Verify your credentials with Passport [here](https://passport.gitcoin.co/).

## Stamps
Stamps are credentials or proof of activities that can be acquired by a user by connecting and verifying ownerships of accounts both with Gitcoin Passport.

## SAD - Sybil Account Detection
SAD is a Sybil defense lego developed by Gitcoin that looks at the on-chain history of a grant contributor to score the EOA of the user. 

## Gitcoin
Gitcoin describes itself as a platform “to fund builders looking for meaningful, open source work”. Their mission is to build a more open, collaborative, and economically empowering world. By giving tools to communities, they help build and funds public goods and bring the future digital public infrastructure. 

## Squelched
We say that a user is "squelched" when he does not have his funds matched by quadratic funding because he has been detected as a Sybil attacker. 

## POAP  - Proof of Attendance Protocol
POAP is commonly used to describe a collectible that can be used, for example, to certify the presence in a physical or online event, the participation in a hackathon. Broadly, it describes the gift of an event organizer to people attending the event.
You can find more details about POAP in the [documentation](https://poap.zendesk.com/hc/en-us/articles/9494654007437-What-Is-POAP-)

## Lego
A Lego is a composable unit that performs a definite action. You can see it as a piece of software in which, for a given input, it will return an output. Gitcoin Passport scorer is an example of Sybil detection lego developed by Gitcoin that, from the stamps verified by a user returns a trust score.

You can find more details in this Gitcoin blog post: [Anti-Sybil Legos](https://gov.gitcoin.co/t/anti-sybil-legos/12265)

## What is Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) is a method of understanding data that utilises visualization and statistical techniques to help identify inconsistencies, as well as better understand patterns within the data, detect outliers or anomalous events, and discover interesting relationships between variables.

One example of an EDA tool would be [Raphtory](https://www.raphtory.com/), an analytics platform that combines graph structure capabilities with time-series analysis.

## Ceramic Network

To be completed

## zksync

To be completed

## Bulk transactions

To be completed

## DID's

To be completed
