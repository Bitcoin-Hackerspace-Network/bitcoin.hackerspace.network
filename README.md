# Bitcoin Hackerspace Network
[![bitcoin-hackerspace-network-header-img](./graph-0000/header.png)](https://bitcoin.hackerspace.network)

## What is Bitcoin Hackerspace Network (BitHackNet)?
Bitcoin Hackerspace Network (BitHackNet) is a self-sovereign movement connecting bitcoin-focused hackerspaces across the globe to form a decentralized network 
of physical bitcoin-focused spaces. The specific goals of these hackerspaces vary, but the first principle that all are built upon is the idea of building builders.

BitHackNet strives to achieve this goal by providing its members and member hackerspaces with the technology to easily onboard new members in a cryptographically verifiable way. Self-sovereign identity verifiable credentials is part of the solution while a communications protocol provides the other part. Together, these two technology primitives can be used to issue credentials to bitcoiners wanting to join their local hackerspace and gain access to the entirty of BitHackNet. To become a member of BitHackNet, contact a hackerspace participating in the network (typically one that is closest to you) and ask about onboarding.

Generally speaking, "onboarding" requires selecting a memebership, paying an invoice and acquiring a BitHackNet credential from an issuer. In ideal case, the onboarding hackerspace is also the issuer running their own ssi-service server; however, an alternative is to have another hackerspace in network do the issuing on their behalf and either store it with the proxy issuer or with the onboarder. The idea is that people with a BitHackNet credential will be able to enjoy various benefits at any of the participating hackerspaces. The exact details of those benefits may vary pending on location and must be designed collaboratively by the network members. That is one of the goals of this repository. Additionally, hackerspace organizers can rest assured that the out-of-towner standing in front of them has been onboarded by a network hackerspace they trust. In this way, we can provide easier access to hackerspaces for bitcoiners, provide more members and more revenue for hackerspaces, and provide the industry and world with more builders.

## Goals
1. Connect bitcoin hackerspaces into a global network
2. Provide value to hackerspace members
3. Provide support to hackerspaces
4. Build builders
5. Change the world, together

## Development Process
The main purpose of this repo is to provide an easy and efficient way for the community to collaborate on the business and technical parts of the hackerspace network. Below is a list requirements that need to be completed that will help define the framework of the Bitcoin Hackerspace Network. These requirements will be completed collaboratively, in the open-source by way of the [GRAPH process](./graph-0000.md).

### Business Requirements
- [ ] Define best practices for onboarding new hackerspaces to network and members to hackerspaces (operations)
- [ ] Define best practices for sustainable business models between the hackerspaces aiming at maintaining profitability, scalability, collaboration and/or any other success metric for a respective space (business)
- [ ] Define intra-network memebership benefits that works between various hackerspaces on a space-by-space basis
- [ ] Determine how that is represented in a credential and attached to a member credential
- [ ] Define cost structure and rev share / split on a space-by-space basis

### Technical Requirements
- [ ] Define best practices for implementing and improving the technical specification.
- [ ] Design and document technical parts (schemas, protocols, etc.)
    - [ ] JSON schema to represent hackerspaces and their membership to BitHackNet
    - [ ] JSON schema to represent members and their membership to their onboarding / issuing hackerspace
    - [ ] JSON schema to represent memberships and the specific benefits available to the holding members
    - [ ] Protocol for issuing valid credentials to hackerspaces and memebers
    - [ ] Protocol for storing and retrieving JSON schemas and credentials
    - [ ] Protocol for presentation (by the holder) and verification of credentials
- [ ] Produce documents to explain technical design and implementation
- [ ] Implement technical design as an open source repo functioning like a hackerspace "toolbox"
    - [ ] SSI stack: implement SSI primitives building a "one-click" solution using DIDs, VCs and DWNs
    - [ ] Alt stack: design and implement the system with alternative protocols (e.g. nostr)
    - [ ] Interoperability: design and implement ways to interoperate these tech stacks
- [ ] Publish implementation documentation to allow for a self-sovereign onbaording process
- [ ] Help onboard any bitcoin spaces that want to participate

## Guidelines and Resources to Advance Protocols for Hackerspaces (GRAPH)
_*GRAPH is a temp working name, looking for feedback on good names for submitting improvements. Check out possible alternatives to GRAPHs [here](./graph-0000.md)_

Below are guidelines and resources for the various protocols (business and technical) for the Bitcoin Hackerspace Network.
If you have improvements or suggestions, please feel fork, follow the spec in [graph-0000](./graph-0000.md) and submit a PR with a new GRAPH.

|           Number            |           Title             |           Author            |           Type              |           Status            |
|-----------------------------|-----------------------------|-----------------------------|-----------------------------|-----------------------------|
|     [0](./graph-0000.md)    |        GRAPH Process        |         Bryan Nonni         |          Process            |            Draft            |
|     [1](./graph-0001.md)    |      Temp Cred Schema       |         Bryan Nonni         |          Standard           |            Active           |
|     [2](./graph-0002.md)    |    Upgraded Cred Schemas    |         Bryan Nonni         |          Standard           |            Draft            |
