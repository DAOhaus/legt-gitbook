---
description: real world asset tokens
---

# rwā

In order to allow DAOs to own and manage assets, they must have their assets turned into blockchain tokens. This is the primary focus of the software we develop: **make it easy for a physical asset to be represented and managed via blockchain tokens.**  Currently we use NFTs and ERC20 Tokens instead of joint token standards such as ERC1155/1400 because of the large amount of tools that exist to support them both in creating [Instant Real Liquidity](irl/).\
\
Let's clear up any confusion between NFT & Token terminology.  A **Non Fungible Token** represents anything that is a 1 of 1.  Things with a unique identifier such as a serial or VIN number would fall into this category.  We will often refer to them as **NFTitles** and in our use cases are often just that , titles or legal documents that define ownership rights such an operating agreement.\
\
A **Fungible ERC20 Token** is anything that you lump together in a defined quantity and not it's individual pieces.  Often these will be referred to as **Fractional** / **Asset** / **Liquid Tokens** or even as "shares" and pertain to things like voting rights, utility allotments or currency amounts and are being designed with DeFi integrations in mind such as new [debt / lending tools](irl/nfloans.md), [liquidity pools](irl/c-a-m-lp.md), and [overall protocol governance](irl/stake-to-own.md).

We will in essence be linking together a legal contracts and smart contracts.  Each jurisdiction will require it's own kind of legal contracts, however for smart contracts we will be using our [RWA Token Standard](https://github.com/DAOhaus/CAIPs/blob/master/CAIPs/caip-legally-empowered-governance-tokens.md) which consists of both a NFT Factory and ERC20 Factory.  This combination allows for both a NFT and ERC20 Token to be minted in the same transaction, like token twins, that represent each other.  The NFT is the title and the ERC20 is it's fractional shares and includes attributes such as:

* functions for a DAO/Multisig/Admin to call for updating metadata
* whitelists, pause, lock & burn functionality
* linking variables that point to URLs and Token Addresses that pertain to its governance and ownership such as the linked erc20, nft, legal document, liquidity pool allowing for on-chain automated controls and hooks.
* chain agnostic & meta-standard compliant in order to be combined with many other chains, processes and standards outside of our protocol. &#x20;

We are not creating a walled garden, take your tokens where you'd like. The protocol will work regardless of a frontend and so the ability for a central actor to freeze or restrict your access is mitigated.

