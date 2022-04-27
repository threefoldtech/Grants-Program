# W3F Grant Proposal

- **Project Name:** ThreeFold Thin Provisioning of Blockchain Infrastructure
- **Team Name:** TFTech nv
- **Payment Address:** x BTC / USD / ... 
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 3

## Project Overview :page_facing_up:

ThreeFold Tech has developed technology to empower a global scalable peer2peer Internet. This open-source peer-to-peer Internet empowers the digital workloads of tomorrow. Our vision is of a digital economy that guarantees data sovereignty, privacy and ownership for all, delivers equality regardless of borders, gender or race and is based upon an infrastructure that is truly decentralised, ecologically and economically sustainable for our beautiful planet. Doing good for the world and growing a successful software company can go hand in hand. 

Our peer-to-peer internet technology is a blockchain-driven, self-healing cloud storage, compute and network platform. Addressing multiple target groups (e.g. blockchain organisations, developer community, banking, telco operators, government, enterprise etc) and enabling sustainable cloud infrastructure that is decentralised, quantum safe, scalable,  self-healing, regenerative and ultra cost-effective. 

ThreeFold Grid now in 3e generation, our primary use case, is live today with 90+ PB of storage and 31k+ CPU cores available across 60 countries and growing day-to-day. ThreeFold Grid has attracted 20+ fantastic partners who are building added value on this universal network of decentralised capacity.

We consider the ThreeFold Technology as the missing foundational layer for a decentralized internet. Basically any IT workload can run on top of the TFGrid. 

![](https://github.com/threefoldfoundation/info_threefold_pub/blob/development/wiki/tfgrid/grid_concepts/img/missing_layer_.jpg)

#### Thin Provisioning

This **project** intends to benefit from the decentralised storage and compute capabilities developed in the ThreeFold Grid to do Thin Provisioning of any blockchain node deployment in the Polkadot ecosystem. 

In order to get a thin provisioning efficiently done, we need a way to start a filesystem in a well known existing state and modify this filesystem without modifying existing original layer.

Using 0-db database, we can give access to a database populated with a well known state of a filesystem. This database should be available only in read-only access in order to avoid any part to modify it. This database can be read by multiple reader in the same time.

While using this layer as base image, it will be possible to expose a remote filesystem available only in read-only, by using a solution like overlayfs, we can mount a write-layer locally, which will enable read-write without touching the source filesystem.

## Project Overview :page_facing_up:

### Overview

#### Introduction

**SubDAO is a Cross-chain Platform built by SubDAO Labs to link DAO and DApp on Polkadot.**  It will be the infrastructure to maintain DAO and to connect DApp with DAO in the world of Web3.0 powered by Substrate and Polkadot.

The SubDAO will run as a parachain to provide specific services. The various DAO templates and SubDAO Airfone will alleviate the burden on developers to maintain DAOs and to create very DApps linked with DAOs. 

The initial governors of a DAO can easily create a cross-chain DAO by only a few clicks without any tech skills at all. Developers who are willing to build DApps can give the governance to communities by using SubDAO to create the very DAO connected to DApp through SubDAO Airfone.

#### Integration

TF-Chain is a customized chain running in the Parity Substrate Framework. It stores the agreements between node providers and consumers for any workload to be deployed on the ThreeFold Grid. 

> TO DO : ... weblet (easy-to-deploy), terraform script, ... ***

#### Team Interest

The team is very experienced in cloud technology, ThreeFold Tech is the result of 20 years of open-source technology in the cloud sector, resulting in 6 exits for a total amount of about 500 million EUR. ThreeFold Tech is now combining this experience to create the world's first truly decentralized internet infrastructure. 

With this ambition, the team has made the technology to rebuild the internet in a way it was intended at conception, which is truly decentralized, stable, secure, fully privacy-enabling, sustainable and where an individual's data can't be exploited by the big tech giants. 

### Project Details

#### Architecture

With the state-of-art technology, SubDAO Labs can achieve the goal based on Substrate 2.0 and the Polkadot. The SubDAO project contains SubDAO node, Template Library, SubDAO Guard, Asset Vault, SubDAO Airfone, and Front End.

![img](https://raw.githubusercontent.com/SubDAO-Network/graphics/main/SubDAO%20Architecture.jpg)

* **Zero-OS** 

Zero-OS is our own Linux-based operating system. It has a Linux kernel inside, so it’s compatible for running any Linux workload on it: containers, Kubernetes clusters, all types of storage, any application. All around the kernel has been rebuilt in order to make it federated/multi-user, secure and privacy enabling. 
Features built around the kernel hold : 
  - An authentication mechanism using a public/private key pair :  Access to this OS, both as a provider and as a user, happens through a public-private key pair, the same as is used to secure blockchain identities. So it’s really decentralised, no longer requiring user names and passwords, source of many hacks. 
So every user (human, but it can also be an IoT device) has his own identity, represented by his own private keys, interacting directly on OS level. 

We got rid of hacking surface of this operating system, as it runs only in memory, there is no shell, and it completely separates the capacity providing side from the usage and data running on it. Meaning that a cloud provider has no insight whatsoever on the workload and the data running on his infrastructure. Which is essential to have privacy implemented by design. 

![](https://github.com/threefoldfoundation/info_threefold_pub/blob/development/wiki/technology/zos/img/zos_overview_compute_storage.jpg)

* **Quantum-Safe Storage** 

Quantum-safe storage is persistent storage where data can be dispersed intelligently over different hardware storage devices, which could be owned by different CSPs, in a way that hacking into a hard drive becomes useless, as data is incomplete (and encrypted). It’s why we call it quantum-safe: with incomplete data, even a quantumcomputer cannot reveal the original information.

* **Planetary Network** 

The network component which runs by design end-to-end encrypted communications, with strong authentication features to connect, this network can securely interconnect any 2 hardware devices over IPv6 and with a secure protocol.

* **TF-Chain** 

This blockchain component uses the Parity Substrate framework, and is the layer that stores all info required to run the ThreeFold Grid, holding all farms, hardware nodes (equipment), contracts between providers and consumers, agreements between farmers and capacity consumers, billing reports, ... 

Minting of TFT, as a reward for having hardware capacity connected to the ThreeFold Grid, is currently paid out on Stellar, but will be implemented on-chain on Parity Substrate soon. 
Payment for hired capacity happens in hourly cycles in TFT on TF-Chain. 

* **Smart Contract for IT** 

The 'Smart Contract for IT' is a process that allows on-chain reservation of cloud capacity in a fully automated way, and manages the payment of this capacity through hourly cycles. 

![](https://library.threefold.me/info/threefold/technology/threefold__smart_contract_it_.jpg)


* **TFT** is the utility token and a representation of the internet capacity connected to the ThreeFold Grid. TFTs are 'farmed' by providers of dedicated hardware capacity, and are used as a medium of exchange for cloud capacity. 

#### Deploy a workload

*  **Thin Provisioning**  

### Substrate / Polkadot Integration

TF-Chain has been implemented in the Parity Substrate framework, and be expanded and improved, benefiting from the Polkadot ecosystem to achieve consensus and to run the sis essential to what SubDAO Network is trying to achieve. The TF-Chain will be connected to the Polkadot ecosystem as a parachain, sharing the Polkadot underlying consensus, and protected by the network performance of Polkadot and Substrate. 

> __TO DO__ : The technology allows to suybstantially extend the Off-chain storage capabilities in the polkadot ecosystem compared to the Off-chain worker. 
> __TO CONFIRM__ : Parachain ? 

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

There are initiatives focused on decentralisation of storage (Filecoin, SIA, Storj, ...) on the one hand, and other initiatives decentralizing compute capacity (Golem, SONM, ...). Other initiatives like Dfinity/ICP aim to build a network to interconnect data centers, but do not offer security and privacy by design, nor capability to run at the edge, and require product-specific workloads to be created. 

**ThreeFold** is, to our knowledge, the only project that decentralizes the full spectrum of cloud infrastructure, while respecting privacy by design, full-fledged security, ability to run at the edge. 
We achieve this by have all hardware resources (CPU, memory, HDD, SSD, network, IP addresses) be orchestrated by a federated, neutral and Linux-based operating system, called Zero-OS. 

Th

---- 

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
