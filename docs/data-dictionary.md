---
title: "Data Dictionary"
description: "Data Dictionary"
lead: "Data dictionaries for all the datasets provided by the ODC"
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
weight: 620
toc: true
---

## [Fantom round data](https://market.oceanprotocol.com/asset/did:op:d4b54f5ab4f171aec585b83189931625eab3803981e9658fe472a87ddc039b0b)

### fantom_round_votes

| Field | Description |
| :---- | :---------: |
| id | record_id |
| source_wallet | contributor/voter wallet |
| token | the token contributed |
| amount |the amount contributed (token) |
| destination_wallet| project wallet |
| created_at |	the time of creation |

### fantom_grant_applications

| Field | Description |
| :---- | :---------: |
| id | record id (off-chain) |
| project | project ID |
| status | status of the grant application |
| updated_at | the time of latest update by the grantee |
| created_at | the time of creation |
| application_round | grant round ID|
| application_recipient | recipient of grant funds |
| title | the project title |
| description | the description of the grant |
| website | project website |
| github_user | guthib user if available |
| project_github | project github repo |
| project_twitter | project twitter account |
| previous_funding | previous project funding sources |
| team_size | size of the team working on the project |
| live_on_other_chains | project live on other chains |
| project_value | value/innovation does the project bring to the Fantom ecosystem and community |
| improvements_to_existing_project	| improvements made if project is a fork of an existing codebase or otherwise directly derived from an existing project|


## [UNICEF round data](https://market.oceanprotocol.com/asset/did:op:d4b54f5ab4f171aec585b83189931625eab3803981e9658fe472a87ddc039b0b)

### unicef_round_votes

| Field | Description |
| :---- | :---------: |
| id | record_id |
| source_wallet | contributor/voter wallet |
| token | the token contributed |
| amount |the amount contributed (token) |
| destination_wallet| project wallet |
| created at |	the time of creation |

### unicef_grant_applications

| Field | Description |
| :---- | :---------: |
| id | record id (off-chain) |
| project | project ID |
| status | status of the grant application |
| updated_at | the time of latest update by the grantee |
| created_at | the time of creation |
| application_round | grant round ID|
| application_recipient | recipient of grant funds |
| title | the project title |
| description | the description of the grant |
| website | project website |
| github_user | guthib user if available |
| project_github | project github repo |
| project_twitter | project twitter account |


## [Gitcoin gr15 round data](https://market.oceanprotocol.com/asset/did:op:f40b1d9c08b737b72d25f705389ca6f3a42c0320887c0276eb28641357dffdf0)

### hackathon-contributions-dataset

| Field | Description|
| :---: | :---------:|
| txn_id | an internal ID for a contribution (off-chain) |
| user_id | an internal ID for a contributor |
| address | the wallet address used to contribute |
| grant_id | the ID of a grant on gitcoin |
| chain | the chain used for the contribution (eth, zksync, polygon...) |
| txn_hash | the hash of the transaction (on-chain) |
| network |	 mainnet or testnet |
| token | the token contributed |
| amount_in_usdt | the equivalent amount contributed in usdt |
| timestamp | the time of the contribution |

### grants_applications_gr15	

| Field | Description|
| :---: | :---------:|
| grant_id 	| the ID of a grant on gitcoin |
| active | is it active at the moment of export (end of round) will it receive its matching or not |
| approved |  was approved (illegible for matching) |
| address | the wallet address to receive the contributions |
| title | the title of the grant (name) |
| url | the url of the grant on Gitcoin website |
| description | the description of the grant |
| created_on | the time of creation |

### gr15_grants	

| Field | Description|
| :---: | :---------:|
| grant_id | the ID of a grant on gitcoin |
| active | is it active at the moment of export (end of round) will it receive its matching or not |
| title | the title of the grant (name) |
| address | the wallet address to receive the contributions |
| amout_received |	The total amount received all-time (usdt) |
| amount_received_in_round 	| the amount recieved this round (usdt) |
| contribution_count | the number of contributions |
| contributor_count | the number of contributors |
| description | the description of the grant |
| website | the website of the grant (not gitcoin page) |
| github_project_url | the github of the grant |
| twitter_handle_1 | the twitter handle of grant |
| twitter_handle_2 | the twitter handle of grant |
| twitter_verified | whether the twitter account was verified |
| created_on | the time of creation |
| last_update | the time of latest update by the grantee |