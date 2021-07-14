Vault-Bot Creation Protocol
===============================

#### What is a Vault-Bot?
A Vault-Bot is an algorithmic trading bot written in typescript that automatically rebalances crypto-assets within an Enzyme Smart Vault according to the strategy encoded in the program.

All Smart Vaults offered by RHC will be algorithmically managed by its own Vault-Bot.

Tuck works closely with Vault-Bots by monitoring their performance and maintaining records of the profits and fee-structure in order to trigger the payment of dividends into the Commons-Fund. Initially, this will take place off-chain, but in future versions, Tuck will have an on-chain component that transparently records and collects profit for the Commons-Fund, a ratio of the DAO Bank reserved for commons-building grant awards.

This document outlines the route by which members of the DAO can take in order to propose and create Vault-Bots that they will ultimately get compensated for in Loot if their bot is deployed by the DAO.


### Step One: Application
Vault-Bots are proposed before they are implemented following the DAO Governance Proposal Protocol. Though maintaining a similar structure to the general proposal format, they also include the following additional fields: 

- strategy thesis: investment thesis
- strategy specification: detailed description of strategy
- allocation requested: amount of capital to place in new fund.
- fee structure: management fee, performance fee, and entrance fee
- commons-share: percent of profits to be diverted into the commons fund
- compensated proposed: amount in DAI to be awarded to team or individual that implements the strategy

### Step Two: Proposal Protocol
Since this is documented in detail elsewhere, i will simply list the major steps in the interest of brevity.

1. Proposal Drafting
2. Community Discussion
3. Final Draft Submission
4. DaoHaus Proposal 
5. Proposal Sponsorship
6. Governance Call
7. DaoHaus Voting
8. Grace Period for Rage Quitting
9. Proposal Processing
10. Implementation

For a more detailed description, see the Governance Section

### Step Three: A Passing Vault-Bot Proposal
After the DAO has decided that this is a Vault-Bot they would like to have implemented, the proposer is responsible for assigning and overseeing a team of developers to implementing the strategy into an automated investment bot. In exchange for implementing the strategy, the team is awarded the proposed compensation for the strategy.

To build the Vault-Bot, the team will be using enzyme finance's Software Development Kit for typescript. 


### Interacting with the Funds
Members and non-members alike can invest in the various Smart-Vaults managed by the DAO's Vault-Bots by using https://enzyme.finance/.

### An Example 
Consider a simple example of the creation of a crypto-long-volatility index fund its life-cycle within the DAO.

1. A member named Alice has the idea for a long-volatility crypto-asset vault-bot!
2. Alice starts by drafting up some notes and sending some messages in the mattermost server to ask for opinions and comments on her new idea
3. After piecing together a proposal draft with the help of the community input she received when asking for opinions, alice submits the draft on github and asks for more feedback.
4. Once alice has finalized her proposal, she resubmits the final draft and uses DAOHaus to officialy submit her proposal on the smart-contract.
5. At this time, another member named bob recognizes and appreciates alice's proposal as having value, and sponsors it by depositing 10 DAI into escrow by the smart-contract
6. Having received a sponsorship, alice's long volatility Vault-Bot proposal will now receive an official vote, and have a governance call scheduled by tuck during the voting period.
7. During the 7 days following bob's sponsorship, all members can vote on alice's strategy
8. After the voting period, a 7-day grace period begins in which all members who are unhappy with the outcome and voted on the opposition have the right to exit and redeem all of their shares before the new strategy is contracted.
9. If alice's Vault-Bot passed a vote, the board will now assign a team to implement the algorithm which will be transparently available to all members through the github.
10. Once the Vault-Bot is implemented, it is deployed and connected to the enzyme smart-contract, automatically managing the funds according to the proposal. 
11. At this point, members and non-members alike can now visit enzyme finance and invest in the Smart Vault.
