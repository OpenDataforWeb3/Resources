# Lego's 

Legos are composable building blocks that performs specific function and analysis by taking in inputs and returning outputs which can be used to protect public goods funding from Sybil's attack.

Several Lego’s are already built and are being used to manage Sybils. These includes:

### Passport Scoring 
[Gitcoin passport](https://passport.gitcoin.co/):
- Gitcoin passport is a tool that enables users prove their identity by collecting stamps which are credentials from web2 such as Facebook, Twitter, and web3 i.e BrightID, ENS. 
The combination of stamps in a wallet can be used to create a trust score which can be calculated to use as evidence of personhood,the greater the score the more likely a user is trustable or genuine.
- [Link](https://github.com/gitcoinco/passport-scorer)


### Algorithmic Detection Lego
- Created by TrustaLabs in the last hackathon. Sybils are detected on how the user's spread fund in bulk (Bulk Transfers) and in what pattern they make donation to the same grant(Bulk Donations).
- [Github Repo](https://github.com/TrustaLabs/slaysybil)


### Sybil-Scoring 
##### Shared IP:
- A user's IP address is checked to see if it is used by multiple users. Such IP with a lot of addresses could be marked as a sybil attacker.
- [Link]()

##### SAD Model:
- A user's gitcoin history can be analysed using a SAD model to give sybil likelihood scores.
- [Link]()

##### DonorDNA:
- A donor's past donations can be analysed when their wallet is connected to see whether it is similar to groups of other users, which may be indicative of Sybil rings.
- [Link]()

##### GrantDNA: 
- Each grant has a set of donors that can be represented as a set of binary data. This can be used to compare grants against flagged grants to see if they have similar donor profiles.
- [Link]()

##### Onchain Intersectionality: 
- Checks how many out of a set of on-chain credentials a user has.
- [Link]()


### Other Legos that could exist:

##### Farmer Boolean:
- Uses on-chain data to determine whether a user has >X ERC-20 tokens and an average transaction value <Y ETH.
                                                                                                          
##### Onchain History Boolean:
- Has a user engaged in certain web3 activities in a specific timeframe? Activities and timeframe can be customized by round owner.
                                                                                                          
##### Money-Mixer: 
- Does a user interact with mixers e.g. Tornado cash, Blender.io 

##### On-Trend / Off-Trend:
- Is the donation profile of a user similar to a grant’s target community?
                                                                                                          
##### Flagged Activity on Etherscan: 
- Checks if an address is associated with addresses flagged as phishing/spam on etherscan.

