Organizational Architecture
========================

## Organizational Stack
In our opinion, effective governance does not mean utilizing blockchain for all aspects of the process but instead, applying the technology to areas in which it provides the greatest benefit. 

The vast majority of social interaction between humans is far too dynamic to allow for completely lossless encoding into programmatic logic. For this reason, the concept of on-chain vs off-chain is widely used in the discussion of blockchain oriented systems. 

Off-chain simply refers to the aspects of the system that are not enforced by programmatic logic on a smart contract, whereas on-chain refers to portions of the process that actively utilize smart-contract execution on the Ethereum Virtual Machine, resulting in trustless decentralization of the procedure. 

### On-Chain Components
The on-chain components of our governance system are Molochv2, the DAO Bank, Gnosis-Safe, and Enzyme Finance.

#### Moloch v2
[Moloch v2](https://github.com/MolochVentures/moloch) is a smart-contract developed by MolochVentures which aims to be a 'minimally-viable DAO'.

Moloch provides us with a decentralized application that encodes our agreements and relationships as members and provides us with the organizational abilities to submit and vote on proposals, exit the DAO before implementation of a proposal whose outcome we voted against (known as rage-quitting, more on this later), grant ownership of crypto-assets to the DAO, and receive compensation in the form of 'Loot'. 

#### DAOHaus
[DaoHaus](https://daohaus.club/) is a platform for interacting with DAO enabling smart contracts.

In reality, our smart-contract exists only in the ethereum virtual machine, but using DaoHaus provides us with a channel of communication to nodes of that machine, so that whenever we want an action to be executed on the ethereum virtual machine our behalf, we can just use DaoHaus! Get familiar with the platform by exploring the [Robinhood DAO Home Page](https://app.daohaus.club/dao/0x2a/0x7d317054229031579483f0d09384e9c64982b346). 

#### The DAO Bank
Any entity that interacts with the blockchain must have an identity, whether it's a smart-contract, trading-bot, or a human. Thus, the DAO possesses its own identiy, or pair of public/private keys which it can use to buy, sell, or trade crypto-assets. The interesting idea here is that as opposed to a single owner needing to verify transactions and approve the use of their private keys for interacting with the blockchain, the use of the DAO's private keys is dictated by the democratic voting process outlined in the DAO Governance System. This means that the DAO can own assets, the same way a bank would, except instead of a single centralized group getting to call the shots on when and what purchases should be made, the coop decides together. To view the DAO Bank, click the 'View Bank' button on the DAO Home Page. 
![bank-button](../assets/bank-button.png)

#### Gnosis-Safe 
[Gnosis Safe](https://help.gnosis-safe.io/en/articles/3876456-what-is-gnosis-safe) is a smart contract wallet running on Ethereum that requires a minimum number of people to approve a transaction before it can occur (M-of-N). 

If for example you have 3 main stakeholders in your business, you are able to set up the wallet to require approval from all 3 people before the transaction is sent. This assures that no single person could compromise the funds.

In our case, in order to allow for board members to execute time-sensitive transactions on behalf of the DAO, the Coop Board will be in charge of a 3-of-3 Gnosis-Safe.

Every fiscal quarter, the board will submit a proposal outlining the subsequent quarter's budget and if approved, the specified funds will be sent from the DAO wallet to the Board Gnosis-Safe, allowing for operating transactions to be executed as efficiently as possible.

#### Enzyme Finance
[Enzyme](https://enzyme.finance/) is a decentralised asset management infrastructure built on Ethereum. Using Enzyme Smart Vaults, individuals and communities can build, scale and monetise investment (or execution) strategies that employ the newest innovations in decentralised finance.

Enzyme enables RHC to provide transparent asset management to non-members and members alike through the Enzyme Market Place. As an end-user of Enzyme, you can allocate capital to any strategy created by RHC, allowing the DAO to receive revenue in the form of management, performance, and entrance fees. 


### Off-Chain Components
The off-chain components of our governance system are Tuck, the RHC site, Mattermost, Discord, and Github.


#### Tuck
[Tuck](https://github.com/robinhoodcoop/Tuck) is our friendly robot-assistant that aims to make our life easier by integrating both the off-chain and on-chain aspects of our DAO smart-contract into our communication platform, Mattermost. In this version, Tuck will only be able to read data from the smart-contract and provide notifications of on-chain events within mattermost, but in future versions, Tuck will replace DAOHaus as the smart-contract user-interface and be able to automate aspects of the governance and community moderation process.

#### RHC Site 
The [RHC website](https://www.robinhoodcoop.org/) will primarily be used to host the membership application, newsletters, and educational content created by members.

#### Mattermost
[Mattermost](https://mattermost.com/) will be our primary platform for the social coordination and communication that is necessary to make organizations function efficiently. Upon becoming a member in the DAO, you'll receive an email with the access link, which will allow you to join the conversation straight from your browser or one of their [Mobile and Desktop Apps](https://mattermost.com/download/#). 

#### Discord
[Discord](https://discord.com/) will be our primary platform for external communication with potential members. The key difference between our use of discord and mattermost lies in the target audience and content discussed. Discord will serve as a place for potential members to ask questions and learn more about what it's like to be a part of the DAO, whereas mattermost will contain current members only, and will serve as the platform within which we discuss confidential DAO-related converstaions, proposals, vault-bots, Working Group projects, and more.

#### Github
[Github](https://github.com/) is a web service built on the open-source version-control tool, git. We will use github primarily to share proposals, membership applications, and other materials related to the development and operations of the coop.

In a future version, we will adopt [Radicle](https://radicle.xyz/), a peer-to-peer alternative to github that allows the DAO to integrate more tightly with the file-sharing system and file-related web3 protocols.


## Working Groups
In order to allow for effective collaboration and specialization within the organization, we have created a set of working groups that members can become a part of. In order to join a working group, one must submit a working group membership proposal, detailing the loot requested as compensation for their work, hours per week of commitment to the working group, and reasoning for their desire to be a part of the working group.

Upon having their working group membership proposal approved by the DAO, members will receive monthly payments from the Board as compensation for their contribution.

### Board
The Board will be resposible for general oversight of all operations and making sure that the organization continues to be aligned with it's primary goals, facilitating transparent mutual aid between members in the form of risking-together with long-volatility investment allocations, and empowering commons-oriented projects through grant funding.

In order to allow for the board to execute time-sensitive decisions without submitting an entire proposal and waiting for the completion of the ~8 day process, they will be given access to a 3-of-5 Gnosis-Safe. This wallet will allow the board to request funding for the day-to-day operational expenses as per the quarterly budget proposal and 'circuit-break', or, revoke the trading bots' vault access and exit all held investment positions.

Since the Gnosis-Safe is enabled by a smart-contract, the transactions made by the wallet are available for the community to view on any block explorer such as etherscan or tenderly. If at anytime, the board is found to be making transactions that are not aligned with the goals and interests of the DAO, members are able to view the transactions themselves and decide to propose the replacement of board members and deauthorize their addresses from accessing the Enzyme Vaults.
 
Every Fiscal Quarter, the board is required to provide a quarterly budget in the form of a proposal. The proposed budget along with the transactions from the past quarter will be used by the DAO in the DGP Protocol to evaluate whether or not the funds should be granted to the Board.

Every algorithmic trading bot deployed by the DAO will have it's own Smart Vault on Enzyme. The Board Multi-Sig and the trading bot will both be given access, but the DAO may revoke access at anytime from either of them. The Board is responsible for actively monitoring the vault, and 'circuit-breaking' in the event of bugs, hyper-volatility, or risk-guideline violations.

Key Tasks:

1. Maintaining day-to-day operations and ensuring the governance system is being used effectively
2. Maintaining effective and regulatory compliant accounting and creating quarterly budget proposals.
3. 'Circuit-breaking' or overriding the governance system when investment risk-guidelines are violated or bugs are exhibited in the trading bot. For example, if the Coop's investments begin to perform poorly enough such that an agreed upon (through the DGP Protocol) maximum level of portfolio drawdown is realized, the Board is responsible for liquidating positions to reduce exposure to excess risk and hyper-volatile events. 

### Community Management
The Community Management Working Group will be responsible for providing clear, prompt, and engaging communication with both current and potential members of the DAO. This team will work closely with the Design/UX Working Group as well as the Growth and Investor Relations Working Group in order to create and deliver content that allows for potential and current members to easily obtain a detailed illustration of the current ongoings within the DAO.

Key Tasks:

1. Creation and delivery of bi-weekly newsletters that describe the current state of affairs of the DAO.
2. Engaging with the DeFi and Crypto communities through the DAO social media accounts.
3. Moderating the Mattermost server.
4. Moderating and answering potential member questions in the Discord server.
5. Working with the Design/UX team to create Youtube tutorials, lessons, and educational material for the community.

### Design/UX
The Design and User Experience Working Group will be responsible for working with the Web 3.0 Engineering Working Group to ensure that our protocols and user interfaces are user-friendly, intuitive, and fun to use. In addition, the Design and UX Working Group will play a key role in helping the Community Management Working Group Create attractive and engaging material for communicating ideas and updates to members. 

Key Tasks:

1. Designing effective and intuitive user-interfaces for the governance system and its related protocols.
2. Synthesizing deliverables to be used for marketing, newsletters, social media posts, and educational materials.
3. Designing and mainting the RHC website.


### Growth and Grant Recipient/Investor Relations
The Growth and Investor Relations Working Group will be primarily focused on scaling the DAO both in the amount of members and the amount of capital. This working group will work closely with both the Design/UX and Community Management Working Groups in order to create investor pitches, grow relations with current members, maintain relationships with grand recipients, and build a closely-knit internal community.

Key Tasks:

1. Create and maintain relationships with potential and current investors.
2. Attend conferences and networking events on behalf of RHC.
3. Follow up with grant recipients and create reports detailing the results of grant funding.
4. Design and lead initiatives centered around creating a more unified community.
5. Create crypto state of the market reports detailing current trends and potential opportunities for the DAO.

### Strategy Design
The Strategy Design Working Group will be focused on creating investment hypotheses and their respective Vault-Bot specifications. The entirity of this groups responsibilites will entail researching current market trends and designing a strategy to exploit inefficiences while maintaing a long-volatility bias. 

The Financial Markets courses offered to members will serve as an experiential learning opportunity in which members can learn about strategy design and how to confidently explore different investment hypotheses. Once a hypothesis has been created, a specification is designed which details the logical requirements for an implemented strategy. An important idea is that the specification outlines *what* a strategy should do, not *how* it should do it, as the *how* is left to the Strategy Engineers.

Key Tasks:

1. Research current market environment.
2. Synthesize investment hypotheses for the current market environment.
3. Use investment hypotheses to create strategy specifications.

### Strategy Engineering
The Strategy Engineering Working Group will be responsible for taking a strategy specification created by the strategy designers and approved for implementation by the DAO and writing and deploying software that automatically rebalances an Enzyme Vault according to the rules put forth by the specification. These software projects are called Vault-Bots, and will primarily be written in TypeScript.

The Financial Programming in TypeScript Course will equip members with the skills necessary to implement a fully-fledged automated investment strategy based upon a strategy specification.

Key Tasks:

1. Write and deploy Vault-Bots for strategy specifications which are approved by the DAO

### Web 3.0 Engineering
The Web 3.0 Engineering Working Group will be responsible for adapting and upgrading the smart-contracts and off-chain integrations required for the DAO to organize in a decentralized, trustless, and transparent manner. 

Though most proposals for evolution of the DAO will come from members outside of this working group, this team will be concerned with how to efficiently and securely implement the proposed changes through the creation, use, and modification of web 3.0 software and tools.

Key Tasks:

1. Working with the design/UX team to create easy to use interfaces.
2. Implement proposed changes for evolution of the DAO Governance System.
3. Maintain and deploy software responsible for facilitating decentralized and transparent collaboration among members.

## DAO Update Calls

**DAO Update Calls** will occur on a monthly basis and will be used to discuss the current ongoings of the co-op, as well as current proposals, and new member applications. The time and date of the calls will be established once we onboard all legacy members and hold a vote.
