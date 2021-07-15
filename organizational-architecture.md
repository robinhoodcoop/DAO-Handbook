Organizational Architecture
========================

## Organizational Stack
In our opinion, effective governance does not mean utilizing blockchain for all aspects of the process but instead, applying the technology to areas in which it provides the greatest benefit. 

The vast majority of social interaction between humans is far too dynamic to allow for completely lossless encoding into programmatic logic. For this reason, the concept of on-chain vs off-chain is widely used in the discussion of blockchain oriented systems. 

Off-chain simply refers to the aspects of the system that are not enforced by programmatic logic on a smart contract, whereas on-chain refers to portions of the process that actively utilize smart-contract execution on the Ethereum Virtual Machine, resulting in trustless decentralization of the procedure. 

### On-Chain Components
The on-chain components of our governance system are Molochv2, Gnosis-Safe, and Enzyme Finance.

#### Moloch v2
[Moloch v2](https://github.com/MolochVentures/moloch) is a smart-contract developed by MolochVentures which aims to be a 'minimally-viable DAO'.

Moloch provides us with a decentralized application that encodes our agreements and relationships as members and provides us with the organizational abilities to submit and vote on proposals, exit the DAO before implementation of a proposal whose outcome we voted against (known as rage-quitting, more on this later), grant ownership of crypto-assets to the DAO, and receive compensation in the form of 'Loot'. 

#### DAOHaus
[DaoHaus](https://daohaus.club/) is a platform for interacting with DAO enabling smart contracts.

In reality, our smart-contract exists only in the ethereum virtual machine, but using DaoHaus provides us with a channel of communication to nodes of that machine, so that whenever we want an action to be executed on the ethereum virtual machine our behalf, we can just use DaoHaus!

#### Gnosis-Safe 
[Gnosis Safe](https://help.gnosis-safe.io/en/articles/3876456-what-is-gnosis-safe) is a smart contract wallet running on Ethereum that requires a minimum number of people to approve a transaction before it can occur (M-of-N). 

If for example you have 3 main stakeholders in your business, you are able to set up the wallet to require approval from all 3 people before the transaction is sent. This assures that no single person could compromise the funds.

In our case, in order to allow for board members to execute time-sensitive transactions on behalf of the DAO, the Coop Board will be in charge of a 3-of-3 Gnosis-Safe.

Every fiscal quarter, the board will submit a proposal outlining the subsequent quarter's budget and if approved, the specified funds will be sent from the DAO wallet to the Board Gnosis-Safe, allowing for operating transactions to be executed as efficiently as possible.


#### Enzyme Finance
[Enzyme](https://enzyme.finance/) is a decentralised asset management infrastructure built on Ethereum. Using Enzyme Smart Vaults, individuals and communities can build, scale and monetise investment (or execution) strategies that employ the newest innovations in decentralised finance.

Enzyme enables RHC to provide transparent asset management to non-members and members alike through the Enzyme Market Place. As an end-user of Enzyme, you can allocate capital to any strategy created by RHC, allowing the DAO to receive revenue in the form of management, performance, and entrance fees. 


### Off-Chain Components
The off-chain components of our governance system are Tuck, the RHC site, Mattermost, and Github.


### Tuck
[Tuck](https://github.com/robinhoodcoop/Tuck) is our friendly robot-assistant that aims to make our life easier by integrating both the off-chain and on-chain aspects of our DAO smart-contract into our communication platform, Mattermost. In this version, Tuck will only be able to read data from the smart-contract and provide notifications of on-chain events within mattermost, but in future versions, Tuck will replace DAOHaus as the smart-contract user-interface and be able to automate aspects of the governance and community moderation process.

### RHC Site 
The [RHC website](https://www.robinhoodcoop.org/) will primarily be used to host the membership application, newsletters, and educational content created by members.

### Mattermost
[Mattermost](https://mattermost.com/) will be our primary platform for the social coordination and communication that is necessary to make organizations function efficiently. Upon becoming a member in the DAO, you'll receive an email with the access link, which will allow you to join the conversation straight from your browser or one of their [Mobile and Desktop Apps](https://mattermost.com/download/#). 


### Github

[Github](https://github.com/) is a web service built on the open-source version-control tool, git. We will use github primarily to share proposals, membership applications, and other materials related to the development and operations of the coop.

In a future version, we will adopt [Radicle](https://radicle.xyz/), a peer-to-peer alternative to github that allows the DAO to integrate more tightly with the file-sharing system and file-related web3 protocols.


## Working Groups

#### Co-op Board

Board membership positions will be proposed and voted on in the same manner as all other proposals. Once a board is established, they will be resposible for general oversight of all operations and making sure that the organization continues to be aligned with it's primary goals, facilitating transparent mutual aid between members in the form of risking-together with long-volatility investment allocations, and empowering commons-oriented projects through grant funding. There are two main responsibilities of the board:

1. Maintaining day-to-day operations and ensuring the governance system is being used effectively
2. 'Circuit-breaking' or overriding the governance system when investment risk-guidelines are violated or bugs are exhibited in the trading bot. For example, if the Coop's investments begin to perform poorly enough such that an agreed upon (through the DGP Protocol) maximum level of portfolio drawdown is realized, the Board is responsible for liquidating positions to reduce exposure to excess risk and hyper-volatile events. 

In order to allow for the board to execute time-sensitive decisions without submitting an entire proposal and waiting for the completion of the ~8 day process, they will be given access to a 3-of-5 Gnosis-Safe. This wallet will allow the board to:

- request funding for the day-to-day operational expenses as per their quarterly budget proposal
- 'circuit-break', or, revoke the trading bots' vault access and exiting all held positions.

Since the Gnosis-Safe is enabled by a smart-contract, the transactions made by the wallet are available for the community to view on any block explorer such as etherscan or tenderly. If at anytime, the board is found to be making transactions that are not aligned with the goals and interests of the DAO, members are able to view the transactions themselves and decide to propose the replacement of board members and deauthorize their addresses from accessing the Enzyme Vaults.
 
#### Quarterly Budget Proposal
Every Fiscal Quarter, the board is required to provide a quarterly budget in the form of a proposal. The proposed budget along with the transactions from the past quarter will be used by the DAO in the DGP Protocol to evaluate whether or not the funds should be granted to the Board.

#### Administration of Enzyme Vaults
Every algorithmic trading bot deployed by the DAO will have it's own Smart Vault on Enzyme. The Board Multi-Sig and the trading bot will both be given access, but the DAO may revoke access at anytime from either of them. The Board is responsible for actively monitoring the vault, and 'circuit-breaking' in the event of bugs, hyper-volatility, or risk-guideline violations.


Key Tasks:

#### Community Management

Key Tasks:
#### Design/UX

Key Tasks:
#### Business Development

Key Tasks:
#### Growth and Investor Relations

Key Tasks:
#### Strategy Design

Key Tasks:
#### Strategy Engineering

Key Tasks:
#### Web 3.0 Engineering

Key Tasks:

