# W3F Grant Proposal

- **Project Name:** ThreeFold Decentralised KYC
- **Team Name:** TFTech nv
- **Payment Address:** x BTC / USD / ... 
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 3

## Project Overview :page_facing_up:

ThreeFold Tech has developed technology to empower a global scalable peer2peer Internet. This open-source peer-to-peer Internet empowers the digital workloads of tomorrow. Our vision is of a digital economy that guarantees data sovereignty, privacy and ownership for all, delivers equality regardless of borders, gender or race and is based upon an infrastructure that is truly decentralised, ecologically and economically sustainable for our beautiful planet. Doing good for the world and growing a successful software company can go hand in hand. 

Our peer-to-peer internet technology is a blockchain-driven, self-healing cloud storage, compute and network platform. Addressing multiple target groups (e.g. blockchain organisations, developer community, banking, telco operators, government, enterprise etc) and enabling sustainable cloud infrastructure that is decentralised, quantum safe, scalable,  self-healing, regenerative and ultra cost-effective. 

ThreeFold Grid now in 3e generation, our primary use case, is live today with 90+ PB of storage and 31k+ CPU cores available across 60 countries and growing day-to-day. ThreeFold Grid has attracted 20+ fantastic partners who are building added value on this universal network of decentralised capacity.

This **project** intends to ... 

<!-- ## Project Overview :page_facing_up:

### Overview

#### Introduction

**SubDAO is a Cross-chain Platform built by SubDAO Labs to link DAO and DApp on Polkadot.**  It will be the infrastructure to maintain DAO and to connect DApp with DAO in the world of Web3.0 powered by Substrate and Polkadot.

The SubDAO will run as a parachain to provide specific services. The various DAO templates and SubDAO Airfone will alleviate the burden on developers to maintain DAOs and to create very DApps linked with DAOs. 

The initial governors of a DAO can easily create a cross-chain DAO by only a few clicks without any tech skills at all. Developers who are willing to build DApps can give the governance to communities by using SubDAO to create the very DAO connected to DApp through SubDAO Airfone.

#### Integration

SubDAO is a customized chain based on the Substrate 2.0 Framework and will run as a parachain on Polkadot. The OCW (Off-chain Worker) provides the ability to access the off-chain world, which would empower the DAOs to access external data rather than only On-chain data, such as the price of stable coins, the contributions on Github, and so on.

#### Team Interest

The initial members of the SubDAO Labs team are big fans of Web3.0 technology. They come from different areas, ranging from full-stack developer, product manager, project management to cryptocurrency early adopters. DAO is the ideal governance model in the mind of the team. Creating and maintain a DAO is not so easy, especially to make a DAO working across different chains. But with the help of Substrate 2.0 and Polkadot, the team thinks it is the time now.

Creating a DAO is not a new thing to the guys involved in the blockchain world, just like shooting a man to the Moon is not news to the fiction novel readers nor people. But the opportunity for everyone to easily travel forth and back between the Moon and the earth is making a big difference! All the team trying to do is to build a cheap, reliable, and fast enough vessel for people to travel between the Moon and the earth even further between Mars and the Earth. The team wants to provide a cheap, reliable, and fast enough way to let everyone being able to create DAOs and DApps across different chains.

### Project Details

#### Architecture

With the state-of-art technology, SubDAO Labs can achieve the goal based on Substrate 2.0 and the Polkadot. The SubDAO project contains SubDAO node, Template Library, SubDAO Guard, Asset Vault, SubDAO Airfone, and Front End.

![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/SubDAO%20Architecture.jpg)

* **SubDAO Node** is the customized chain node for the SubDAO network built by Substrate 2.0. It's the fundament of the SubDAO network that contains the basic functionalities as a normal chain node but also provides the ability to fetch external data needed for DAO governance with the OCW (Off-chain Worker) from Substrate 2.0 Framework. 

* **Template Library** is the key component of the SubDAO network. It is comprised of multiple contracts. The main functionalities of **Template Library** are managing and providing various DAO Templates for different types of organizations. Everyone has the right to define new DAO Templates according to their needs, and the SubDAO network provides some default DAO Templates such as Voting Template, Fund Template, VC (Venture Capital) Template and so on. 

* **SubDAO Guard** is the original DAO of the SubDAO network. It provides basic management functionalities. Every member of the SubDAO network can get involved in the SubDAO network governance through SubDAO Guard.

* **Asset Vault** is the smart contract providing the basic features of manage assets for each DAO. Working together with **DAO Template**, the **Asset Vault** manages all kinds of assets, including the assets needed by creating a new DAO, the assets deposited by the governors of a DAO, and other assets.

* **SubDAO Airfone** is the SDK for developers to connect their DApps with the DAOs created by themselves or others. It will be provided as a Javascript library at the beginning, and in other languages later. Developers can use the SubDAO Airfone to interact with the SubDAO network directly or built their DApps with the connection to DAO.

* **Front End** provides Web UI for everyone to interact with the SubDAO network. All the users need to do is open the webpage deployed by the SubDAO Labs team or by users themselves and click the buttons following the manual. **Front End** will provide such functionalities as creating a new DAO, define a new DAO template, withdraw personal assets,  voting in DAO, and so on. Front End will be built with NodeJS.

* **SubDAO Token $SDT** is the native token of the SubDAO Network, and it will play the role of governance and other utilities. **$SDT** is necessary to secure and power the SubDAO Network. The SubDAO Network may hold an IPO and reward community members for helping our auction with **$SDT** tokens during the Parachain Auction.

#### Scenarios

*  **Scenario to Create a New DAO**  
![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/flow1.jpg)

As shown above, the steps to create a new DAO are marked. The DAO governor calls the smart contract of the SubDAO Guard to choose a proper DAO template from the DAO Template Library. After the governor fills the basic information required by template such as name, description, the rules of governance, initial members, and so on and deposits the initial fund to the Asset Vault, the SubDAO Guard contract will create the very DAO according to the chosen template and filled information. All extra information, such as images, texts, and files, will be stored in a decentralized storage network like IPFS.

*  **Scenario to Attend a New DAO**  
![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/flow2.jpg)

Generally speaking, there are two kinds of ways to interact with DAO contracts. The first way to get involved with a specific DAO is using the **Front End** created by the SubDAO Labs to interact with all the DAOs on the SubDAO Network. The second way is using the **SubDAO Airfone**. The SubDAO Airfone will hide all the details of calling smart contracts for users and is used by DApps since the developers of DApps can customize their scenario according to their needs.


#### The Open SDK

Our ultimate goal is to provide an essential open SDK (**the SubDAO Airfone**) from a high-level perspective together with the above components, fully powering the ecosystem of DAO across chains on Polkadot.  With the functionality of the Open SDK, anyone involved can utilize DAO and DApp.

The benefits of an open SDK are beyond criticism. The Open SDK will be an extension of both the DAO's capabilities and the value of the DApps through the whole Polkadot universe.  We hope to build a framework whereby any Decentralized Autonomous Organizations can live, and any Decentralized Apps can use in the  Polkadot ecosystem.

### Substrate / Polkadot Integration

The whole SubDAO Network builds on top of the Substate 2.0, and the Polkadot ecosystem is essential to what SubDAO Network is trying to achieve. The SubDAO Network will be connected to the Polkadot ecosystem as a parachain, sharing the Polkadot underlying consensus, and protected by the network performance of Polkadot and Substrate. 

The off-chain worker is a new feature in the Substrate Framework that allows the SubDAO Network to interact with off-chain data. 

The node in the SubDAO Network is built with OCW (Off-chain Worker) enabled. The figure below shows how it will work with external data (for example, the contributions on Github).

![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/Integration.jpg)

In the figure above, the SubDAO Node includes an OCW pallet that interacts with external HTTP service (Github Http Wrapper). Since the OCW pallet is a general component, most of the processing work of external data is moved out of OCW to decrease the complexity of implementation and give the ability to the DAO governors who wanna use specific data sources for their DAO. The external HTTP service (Github Http Wrapper) will fetch the data such as contributions for a user in a project or repository from Github.com and feed the OCW pallet in the SubDAO Node.

All smart contracts mentioned above will be implemented with **Ink** or **EVM**. Since the SubDAO Node includes **OCW (Off-chain Worker)**, **Ink** is essential due to **Ink** is the only way to interact with pallets currently. Thanks to Ethereum, **Solidity** is widely used over several years, and most of the developers are already familiar with **EVM**.  So in the SubDAO Network, most of the smart contracts will be implemented using **EVM** to decrease the difficulties for new developers on the Polkadot ecosystem.  

![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/Pallets.jpg)

As shown above, those contracts interacting with pallets will be implemented with **Ink**, and others will be with **EVM**. Later in future versions, when developers get familiar with **Ink**, the whole project will upgrade to use **Ink** only. 

For **EVM**, we will choose [Frontier](https://github.com/paritytech/frontier) as the evm pallet.

#### The Pallet Implementation

The function provided by the pallet to get off-chain data is `requestOffchainData`.

**1. requestOffchainData**

- `desc:` smart contract requests the off-chain data, the SubDAO network nodes will send data to the SubDAO chain through OCW integrated later.
- `params:` HTTP wrapper URL, JSON params
- `return:` dataId


### Ecosystem Fits

Most of the current L1 blockchain frameworks run on centralized cloud infrastructure, like Amazon AWS, Microsoft Azure etc. Centralisation of hardware infrastructure for running decentralized workloads goes against the nature of the cryptospace, to have as much decentralization as possible. 

There are initiatives focused on decentralisation of storage (Filecoin, SIA, Storj, ...) on the one hand, and other initiatives decentralizing compute capacity (Golem, SONM, ...). Other initiatives like Dfinity/ICP aim to build a 

**ThreeFold** is, to our knowledge, the only project that decentralizes the full spectrum of cloud infrastructure, while respecting privacy by design, full-fledged security, ability to run at the edge. 
We achieve this by have all hardware resources (CPU, memory, HDD, SSD, network, IP addresses) be orchestrated by a federated, neutral and Linux-based operating system, called Zero-OS. 

Th
 -->

### Overview

Please provide the following:

- If the name of your project is not descriptive, a tag line (one sentence summary).
- A brief description of your project.
- An indication of how your project relates to / integrates into Substrate / Polkadot / Kusama.
- An indication of why your team is interested in creating this project.

### Project Details

We expect the teams to already have a solid idea about your project's expected final state. Therefore, we ask the teams to submit (where relevant):

- Mockups/designs of any UI components
- Data models / API specifications of the core functionality
- An overview of the technology stack to be used
- Documentation of core components, protocols, architecture, etc. to be deployed
- PoC/MVP or other relevant prior work or research on the topic
- What your project is _not_ or will _not_ provide or implement
  - This is a place for you to manage expectations and to clarify any limitations that might not be obvious

### Ecosystem Fit

The project already has TFChain running as the blockchain component of the project. TFChain is running in Parity Substrate. 
It is the trust component which, combined with the Zero-OS operating system, the Quantum-Safe Storage and the Planetary Network, is the foundation of the peer-to-peer internet. Anyone requiring internet capacity for deploying his workloads can make use of decentralised capacity connected to the Threefold Grid. 

To our knowledge, a truly Decentralised and Autonomous Internet infrastructure platform has never been created, not in the Substrate ecosystem, but neither anywhere else. Traditionally, information technology is very people-intensive which adds to its complexity, risk and cost. Our technology approach is unique in many aspects including a fully decentralised operating system able to federate any digital network, compute and storage infrastructure, quantum safe storage, planetary network, carbon-negative sustainability, significant cost efficiency etc.

The project brings true decentralisation and brings back the internet to a state that is in line with how it was started. Over the years, internet has been monopolized by big tech hyperscalers, which have abused their power to their own financial benefit.  

Most of the current L1 blockchain frameworks run on centralized cloud infrastructure, like Amazon AWS, Microsoft Azure etc. Centralisation of hardware infrastructure for running decentralized workloads goes against the nature of the cryptospace, to have as much decentralization as possible. 

There are initiatives focused on decentralisation of storage (Filecoin, SIA, Storj, ...) on the one hand, and other initiatives decentralizing compute capacity (Golem, SONM, ...). Other initiatives like Dfinity/ICP aim to build a 

**ThreeFold** is, to our knowledge, the only project that decentralizes the full spectrum of cloud infrastructure, while respecting privacy by design, full-fledged security, ability to run at the edge. 
We achieve this by have all hardware resources (CPU, memory, HDD, SSD, network, IP addresses) be orchestrated by a federated, neutral and Linux-based operating system, called Zero-OS. 

Th

<!-- Help us locate your project in the Polkadot/Substrate/Kusama landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
- Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
  - If so, how is your project different?
  - If not, are there similar projects in related ecosystems? --> 

## Team :busts_in_silhouette:

### Team members

- Kristof De Spiegeleer : CEO
- Geert Machtelinckx : Project Lead 
- Rob Van Mieghem : Lead Engineer 
- Dylan Verstraete : Full-stack and blockchain developer
- Maxime Verstraete : Full-stack developer
- Lee Smet : System Architect 

### Project Websites

- General : https://www.threefold.io 
- Wiki : https://library.threefold.me  

### Contact

- **Contact Name:** Geert Machtelinckx
- **Contact Email:** geert@threefold.tech
- **Website:** www.threefold.io

### Legal Structure

- **Registered Address:** Antwerpse Steenweg 19, 9080 Lochristi, Belgium
- **Registered Legal Entity:** TFTech nv

### Team's experience

**Kristof**

- Founder and CEO of ThreeFold Tech
- Passionate social entrepreneur who believes that respect & transparency is the basis for solid business. We believe that doing good for the world & providing return for investors can co-exist. 
- Serial tech entrepreneur with 6 Successful Exits > USD 500 million

**Rob**

- 21 years of expertise in Development and Management
- Mentioned in the release notes of Bitcoin version 0.11.0: https://github.com/bitcoin/bitcoin/blob/452bb90c718da18a79bfad50ff9b7d1c8f1b4aa3/doc/rele ase-notes/release-notes-0.11.0.md#credits

**Geert**

- 23 years of experience in IT Project Management and Architecture
- Currently busy on Project Management and Business Development with ThreeFold Tech

**Dylan**

- Main engineer on TFChain, the ThreeFold blockchain in Parity Substrate 
- 4 years of experience in Blockchain technology. Passionate about learning about new technologies and getting hands on experience with them.

**Lee**

- Lead Architect of ThreeFold Tech
- 6 years of expertise in IT Cloud Architectures and Operating Systems

**Maxime**

- 7 years of expertise in Operating Systems, Storage 

### Team Code Repos

- https://github.com/threefoldtech
- https://github.com/threefoldfoundation
- https://github.com/threefoldtech/tfchain
- https://github.com/threefoldtech/tfchain-pallets

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- https://github.com/<team_member_1>
- https://github.com/<team_member_2>

### Team LinkedIn Profiles (if available)

- https://www.linkedin.com/in/despiegk/
- https://www.linkedin.com/in/robvanmieghem/
- https://www.linkedin.com/in/geert-machtelinckx-a72453b/
- https://www.linkedin.com/in/dylan-verstraete-229539a4/
- https://www.linkedin.com/in/lee-smet-4a279a136/

## Development Status :open_book:

If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- links to improvement proposals or [RFPs](https://github.com/w3f/Grants-Program/tree/master/rfp-proposal) (requests for proposal),
- academic publications relevant to the problem,
- links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
- references to conversations you might have had related to this project with anyone from the Web3 Foundation,
- previous interface iterations, such as mock-ups and wireframes.

## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month.

For each milestone,

- make sure to include a specification of your software. _Treat it as a contract_; the level of detail must be enough to later verify that the software meets the specification.
- include the amount of funding requested _per milestone_.
- include documentation (tutorials, API specifications, architecture diagrams, whatever is appropriate) in each milestone. This ensures that the code can be widely used by the community.
- provide a test suite, comprising unit and integration tests, along with a guide on how to set up and run them.
- commit to providing Dockerfiles for the delivery of your project.
- indicate milestone duration as well as number of full-time employees working on each milestone.
- **Deliverables 0a-0d are mandatory for all milestones**, and deliverable 0e at least for the last one. If you do not intend to deliver one of these, please state a reason in its specification (e.g. Milestone X is research oriented and as such there is no code to test).

> :zap: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Teams that submit others' work without attributing it will be immediately terminated.**

### Overview

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Implement Substrate Modules

- **Estimated duration:** 1 month
- **FTE:**  2
- **Costs:** 8,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| 0a. | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| 0b. | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.)
| 1. | Substrate module: X | We will create a Substrate module that will... (Please list the functionality that will be implemented for the first milestone) |  
| 2. | Substrate module: Y | We will create a Substrate module that will... |  
| 3. | Substrate module: Z | We will create a Substrate module that will... |  
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |  


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1
- **Costs:** 4,000 USD

...


## Future Plans

Please include here

- how you intend to use, enhance, promote and support your project in the short term, and
- the team's long-term plans and intentions in relation to it.


## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website / Personal recommendation by Substrate Builder Program team members. 

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- Work you have already done.
- If there are any other teams who have already contributed (financially) to the project.
- Previous grants you may have applied for.
