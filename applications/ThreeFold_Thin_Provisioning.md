# W3F Grant Proposal

- **Project Name:** ThreeFold Thin Provisioning of Blockchain Infrastructure
- **Team Name:** TFTech nv
- **Payment Address:** x BTC / USD / ... 
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 3

## Project Overview :page_facing_up:

### Overview

This project intends to provide in 'Thin Provisioning', meaning the creation of a new blockchain instance that does not need to be fully synchronised, but can start from an off-chain stored version of the blockchain. Syncing then only needs to be done since this last backup, and any data that the node needs to retrieve which is older, can be retrieved directly from this back-up. This back-up is stored in Zero-DB's. Zero-DB is is a fast and efficient key-value store redis-protocol compatible, which makes data persistent inside an always append datafile, with namespaces support. 
We will offer Thin Provisioning as a Service on the ThreeFold Grid, even though Zero-DB's can also run locally. Reservation of capacity on the ThreeFold Grid, is orchestrated by the TF-Chain, a Parity Substrate blockchain. 

### Background

ThreeFold Tech has developed technology to empower a global scalable peer-to-peer internet, empowering the digital workloads of tomorrow. Our vision is of a digital economy that guarantees data sovereignty, privacy and ownership for all, delivers equality regardless of borders, gender or race and is based upon an infrastructure that is truly decentralised, ecologically and economically sustainable for our beautiful planet. Doing good for the world and growing a successful software company can go hand in hand. 

Our peer-to-peer internet technology is a blockchain-driven, and encompasses cloud storage, compute and network features, which are interacting in a fully secure way using a federated operating systrem called Zero-OS. It addresses multiple target groups (e.g. blockchain organisations, developer community, banking, telco operators, government, enterprise, ...) and enables a sustainable cloud infrastructure that is decentralised, quantum-safe, scalable, self-healing, regenerative and ultra cost-effective. 

ThreeFold Grid has been released in its third generation. Our primary use case is live today with 80+ PB of storage and 31k+ CPU cores available across 60+ countries and growing day-to-day. ThreeFold Grid has attracted 20+ fantastic partners who are building added value on this universal network of decentralised capacity.

See the [Grid Explorer](https://explorer.threefold.io/all) for an overview of the connected capacity. 

We consider the ThreeFold Technology as the missing foundational layer for a decentralized internet. Basically any IT workload can run on top of the TFGrid. 

![](https://github.com/threefoldfoundation/info_threefold_pub/blob/development/wiki/tfgrid/grid_concepts/img/missing_layer_.jpg)

#### Integration

TF-Chain is a customized chain running in the Parity Substrate Framework. It stores the agreements between node providers and consumers for any workload to be deployed on the ThreeFold Grid. 

#### Team Interest

The team is very experienced in cloud technology, ThreeFold Tech is the result of 20 years of open-source technology in the cloud sector, resulting in 6 exits for a total amount of about 500 million EUR. ThreeFold Tech is now combining this experience to create the world's first truly decentralized internet infrastructure. 

With this ambition, the team has made the technology to rebuild the internet in a way it was intended at conception, which is truly decentralized, stable, secure, fully privacy-enabling, sustainable and where an individual's data can't be exploited by the big tech giants. 

### Project Details

#### Thin Provisioning

This **project** intends to benefit from the decentralised storage and compute capabilities developed in the ThreeFold Grid to do Thin Provisioning of any blockchain node deployment in the Polkadot ecosystem. 

In order to get a thin provisioning efficiently done, we need a way to start a filesystem in a well known existing state and modify this filesystem without modifying existing original layer.

Using 0-db database, we can give access to a database populated with a well known state of a filesystem. This database should be available only in read-only access in order to avoid any part to modify it. This database can be read by multiple reader in the same time.

While using this layer as base image, it will be possible to expose a remote filesystem available only in read-only, by using a solution like overlayfs, we can mount a write-layer locally, which will enable read-write without touching the source filesystem.

#### Architecture

With the state-of-art technology, ThreeFold Tech architecture allows to an easy way to thin provision blockchain nodes in the Parity Substrate ecosystem. The main component to have the Thin Provisioning Working is Zero-DB. 

The components to provision them onto the ThreeFold Grid are Zero-OS, Quantum-Safe Storage, Planetary Network, TF-Chain and the Smart Contract for IT.

* **Zero-DB**

0-db is a fast and efficient key-value store redis-protocol compatible, which makes data persistent inside an always append datafile, with namespaces support.

Characteristics : 
- Backend engine for Storage
- Can do +50000 transactions/sec
- Can work on SSD and HDD
- Is optimised for (soft/green) easy operation on HD
- Works with reservations
- Is an always-append store, which can have unlimited history
- Master-slave replication built-in

Zero-DB is being used as backend storage for Quantum Safe Filesystem.

* **Zero-OS** 

Zero-OS is our own Linux-based operating system. It has a Linux kernel inside, so it’s compatible for running any Linux workload on it: containers, Kubernetes clusters, all types of storage, any application. All around the kernel has been rebuilt in order to make it federated/multi-user, secure and privacy enabling. 
Features built around the kernel hold : 
  - An authentication mechanism using a public/private key pair :  Access to this OS, both as a provider and as a user, happens through a public-private key pair, the same as is used to secure blockchain identities. So it’s really decentralised, no longer requiring user names and passwords, source of many hacks. 
So every user (human, but it can also be an IoT device) has his own identity, represented by his own private keys, interacting directly on OS level. 

We got rid of hacking surface of this operating system, as it runs only in memory, there is no shell, and it completely separates the capacity providing side from the usage and data running on it. Meaning that a cloud provider has no insight whatsoever on the workload and the data running on his infrastructure. Which is essential to have privacy implemented by design. 

![](https://github.com/threefoldfoundation/info_threefold_pub/blob/development/wiki/technology/zos/img/zos_overview_compute_storage.jpg)

* **Quantum-Safe Storage** 

Quantum-safe storage is persistent storage where data can be dispersed intelligently over different hardware storage devices, which could be owned by different CSPs, in a way that hacking into a hard drive becomes useless, as data is incomplete (and encrypted). It’s why we call it quantum-safe: with incomplete data, even a quantumcomputer cannot reveal the original information.

![](https://library.threefold.me/info/threefold/technology/qsss/threefold__qsss_intro_0_.jpg)

* **Planetary Network** 

The planetary network is an overlay network which lives on top of the existing internet or other Peer To Peer networks created. In this network, everyone is connected to everyone. End-to-end encryption between users of an app and the app running behind the network wall.

Each user end network point is strongly authenticated and uniquely identified, independent of the network carrier used. There is no need for a centralized firewall or VPN solutions, as there is a circle based networking security in place.

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

First implementation of this 'This Provisioning' mechanism will be implemented on TF-Chain, our own Parity Substrate based blockchain. However, the same mechanism can then be applied for any blockchain to be deployed in the Polkadot ecosystem, with a reference version with a known state hosted on the threeFold Grid decentralized cloud infrastructure.  

> __TO DO__ : The technology allows to suybstantially extend the Off-chain storage capabilities in the polkadot ecosystem compared to the Off-chain worker. 
> __TO CONFIRM__ : Parachain ? 


### Ecosystem Fits

Most of the current L1 blockchain frameworks run on centralized cloud infrastructure, like Amazon AWS, Microsoft Azure etc. Centralisation of hardware infrastructure for running decentralized workloads goes against the nature of the cryptospace, to have as much decentralization as possible. 

There are initiatives focused on decentralisation of storage (Filecoin, SIA, Storj, ...) on the one hand, and other initiatives decentralizing compute capacity (Golem, SONM, ...). Other initiatives like Dfinity/ICP aim to build a network to interconnect data centers, but do not offer security and privacy by design, nor capability to run at the edge, and require product-specific workloads to be created. 

**ThreeFold** is, to our knowledge, the only project that decentralizes the full spectrum of cloud infrastructure, while respecting privacy by design, full-fledged security, ability to run at the edge. 
We achieve this by have all hardware resources (CPU, memory, HDD, SSD, network, IP addresses) be orchestrated by a federated, neutral and Linux-based operating system, called Zero-OS. 

<!-- 

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
  - This is a place for you to manage expectations and to clarify any limitations that might not be obvious --> 

### Ecosystem Fit

The 'Thin Provisioning' nicely fits in the idea of a multi-blockchain ecosystem, where many blockchain nodes need to be deployed. Bringing the tooling to have this up and running brings several major benefits : 
- blockchain nodes are deployed in a substantially lower timeframe than traditionally needed;
- blockchain nodes require substantially lower storage than with the traditional sync process, while the benefits of running a full blockchain remains (all history are available in the Zero-DB filesystem);
- our technology makes deployment of blockchain nodes possible on a fully decentralized cloud infrastructure, making it possible to wisely choose the location and type of hardware infrastructure. 

Moreover, due to the fact that TF-Chain is running on Parity Substrate, the internet capacity reservation process can be integrated seamlessly with the deployment of any IT workload created by any project in the Polkadot ecosystem. 


And it solves an anomaly in the decentralization movement: most of the current L1 blockchain frameworks run on centralized cloud infrastructure, like Amazon AWS, Microsoft Azure etc. Centralisation of hardware infrastructure for running decentralized workloads goes against the nature of the cryptospace, to have as much decentralization as possible. 

**ThreeFold** is, to our knowledge, the only project that decentralizes the full spectrum of cloud infrastructure, while respecting privacy by design, full-fledged security, ability to run at the edge. 
We achieve this by have all hardware resources (CPU, memory, HDD, SSD, network, IP addresses) be orchestrated by a federated, neutral and Linux-based operating system, called Zero-OS. 

There are initiatives focused on decentralisation of storage (Filecoin, SIA, Storj, ...) on the one hand, and other initiatives decentralizing compute capacity (Golem, SONM, ...). 
One project in the Substrate ecosystem is working on Network, [Phala Network](https://www.phala.network/en/). Both projects are complementary and compatible: Phala is focusing on network and cloud functions. We build the 'layer 0' by connecting hardware infrastructure to a decentralized ecosystem. Moreover our focus is on storage and running any Linux workload inside VMs. Phala could use the hardware infrastructure offered in the ThreeFold Grid for their own services. 

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

- https://github.com/threefoldtech (full ThreeFold Tech repo)
- https://github.com/threefoldfoundation 
- https://github.com/threefoldtech/0-db (Zero-DB repo)
- https://github.com/threefoldtech/tfchain (TFChain repo)
- https://github.com/threefoldtech/tfchain-pallets (repo holding pallets used for TFChain)

Please also provide the GitHub accounts of all team members. If they contain no activity, references to projects hosted elsewhere or live are also fine.

- Kristof: https://github.com/despiegk
- Rob: https://github.com/robvanmieghem
- Maxime: https://github.com/maxux
- Geert: https://github.com/gmachtel
- Dylan: https://github.com/DylanVerstraete 
- Lee: https://github.com/LeeSmet

### Team LinkedIn Profiles (if available)

- Kristof: https://www.linkedin.com/in/despiegk/
- Rob: https://www.linkedin.com/in/robvanmieghem/
- Maxime: https://www.linkedin.com/in/maxime-daniel-29bb8055/ 
- Geert: https://www.linkedin.com/in/geert-machtelinckx-a72453b/
- Dylan: https://www.linkedin.com/in/dylan-verstraete-229539a4/
- Lee: https://www.linkedin.com/in/lee-smet-4a279a136/

## Development Status :open_book:

> TO DO: @Maxime 

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
