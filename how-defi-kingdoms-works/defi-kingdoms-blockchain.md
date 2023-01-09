---
description: Information about DFK Chain, an Avalanche Subnet
cover: ../.gitbook/assets/DFK Chain Announcement Twitter.png
coverY: 0
---

# DeFi Kingdoms Blockchain

With the DeFi Kingdoms: Crystalvale expansion, DeFi Kingdoms introduced its own blockchain, which handles gameplay transactions in Crystalvale and hosts the Crystalvale DEX. The DeFi Kingdoms Blockchain, or **DFK Chain**, is being built in partnership with Avalanche using their [Subnet technology](https://docs.avax.network/subnets).

### DFK Chain Advantages

DFK Chain uses [JEWEL](power-tokens/jewel-token.md) for gas. This adds additional utility to the JEWEL power token and simplifies life for players so that they don't have to hold a second token just to use for gas fees.&#x20;

Using JEWEL for gas means that we can better control gas prices. This mechanism will allow us to ensure greater stability in the network and keep fees as low as possible for our users.&#x20;

In addition, the DFK Chain will only handle transactions for DeFi Kingdoms and our partners, on RPCs managed by Ava Labs and POKT, with more nodes to come. That means that block speed and transaction finality are not placed at the whim of the blockchain as a whole, giving us more control over user experience.

### Gas Fee Distribution

Gas fees are collected by a smart contract and then distributed as follows:

* 25% is given to the designated wallets of the validators. This allows us to attract more validators and further decentralize the chain.
* 50% is burned. This will continuously increase the value of JEWEL by implementing a consistent burn mechanic and deflating the supply.
* 25% will be sent to the [Quest Reward Fund](https://subnets.avax.network/defi-kingdoms/address/0x1137643FE14b032966a59Acd68EBf3c1271Df316) to reward our community and players.

### Bridged JEWEL and Gas

A protocol is in place to automatically exchange JEWEL bridged onto the DFK Chain for the native gas token. No special action is needed on the part of players to handle this. The implementation of DFK Chain does not impact the total cap of JEWEL. There is also an option to wrap JEWEL into wJEWEL, as needed, in Crystalvale. This process is handled automatically when trading on the Crystalvale DEX.

### DFK Chain Technical Specs

The DFK Chain is built on Avalanche's Subnet platform. More information about Avalanche Subnets can be found on their [website](https://docs.avax.network/build/tutorials/platform/subnets/).

Additional specific technical information about DFK Chain can be found in the DeFi Kingdoms Developer Docs at: [https://devs.defikingdoms.com/dfk-chain](https://devs.defikingdoms.com/dfk-chain).

### DFK Chain RPC Information

Please visit [Chainlist](https://chainlist.org/?search=dfk) for information on available RPCs. Chainlist will also configure these RPCs for you automatically if you choose.

### DFK Validator Fees

Validator fees that are received for the DFK-owned validators being used on DFK Chain are held in the following smart contract: [`0xED6dC9FD092190C08e4afF8611496774Ded19D54`](https://subnets.avax.network/defi-kingdoms/address/0xED6dC9FD092190C08e4afF8611496774Ded19D54).
