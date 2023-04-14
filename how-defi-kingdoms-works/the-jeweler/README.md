---
cover: ../../.gitbook/assets/jeweler.png
coverY: 229.10101946246527
---

# The Jeweler

## Jeweler 2.0

The **Jeweler 2.0** adopts the benefits gained from the **veToken** governance model developed by [Curve](https://curve.fi/), and combines that with a method for fee distribution, airdrop rewards, and in-game [Power-Ups](power-ups.md). **cJEWEL** is the name for the **Governance Token** in Crystalvale, and **sJEWEL** is the equivalent for Serendale (both are functionally the same, though these docs will use cJEWEL for convenience).

{% hint style="info" %}
The Jeweler 2.0 model was adopted by [community governance vote](https://vote.defikingdoms.com/#/proposal/0x8b74fefcfbd5b6751c190361577fd65ff79084b5250ed3265a14a16140d67fba) on 10/14/2022 and went into effect on 11/4/2022. It replaced the [Jeweler 1.0](./#jeweler-1.0) model that used xJEWEL and xCRYSTAL.
{% endhint %}

Players receive cJEWEL or sJEWEL tokens by **locking their JEWEL** in the Jeweler in the applicable realm for a duration of time of their choosing. This locking mechanism encourages staking into the protocol, and allows those who want to support the project for the long term to have more of a say and receive a larger share of the rewards. It also discourages third-parties from gaming votes and snapshots by buying large amounts of JEWEL right before, only to sell right after.

cJEWEL/sJEWEL tokens are **soulbound** to the wallet that generates them and cannot be transferred or traded. Players may hold their cJEWEL/sJEWEL after the locking period has expired and still receive rewards and governance power.&#x20;

### **Benefits to Holding**

The four main benefits to holding cJEWEL are: Governance, fee distribution, in-game enhancements and premium feature access (Power-Ups), and token locking.

* [Governance](./#governance-votes) will utilize the cJEWEL/sJEWEL balance of users for voting on proposals.&#x20;
* Rewards will come by way of [fee distribution](./#fee-sharing), but also regular airdrops can be implemented thanks to the safer timelock nature of cJEWEL/sJEWEL.
* In-game [Power-Ups](./#power-ups) will allow players to allocate a certain amount of their cJEWEL/sJEWEL in order to gain access to bonuses, enhancements, and premium features, all while still earning the normal rewards.
* Due to cJEWEL and sJEWEL requiring some period of **JEWEL** token locking in order to be created, the expected outcome of this system is an overall reduction of the available liquid supply of JEWEL (depending on user engagement with the system).

### Locking Mechanism

Players may lock their JEWEL in the Jeweler contract for any length of time between 7 days and 1095 days (3 years). In exchange, they will receive an amount of cJEWEL/sJEWEL relative to the amount locked and the duration of time locked, according to this formula, where `MAX DAYS` is equal to 1095 and `daysLocked` is a minimum of 7:

$$
cJEWEL_{earned} = (\frac{JEWEL_{deposited} *  days_{locked}}{MAX _{DAYS}})
$$

{% hint style="info" %}
#### **Example**

<img src="../../.gitbook/assets/keal.gif" alt="" data-size="original">Keal has 50,000 JEWEL and wants to deposit them in the Jeweler. He decides to deposit for the minimum locking period of 7 days and receives \~320 cJEWEL.



![](../../.gitbook/assets/gribbitz.gif) Rolando doesn’t have the same means as Keal, but he decides to make up for that by depositing his JEWEL for longer. Not willing to be outdone by Keal, he acquires 320 cJEWEL of his own by depositing \~960 JEWEL for one year.



**Takeaway**_**:** You don’t have to have the most JEWEL to have the most influence with this model._
{% endhint %}

Players can receive more cJEWEL without depositing more JEWEL by **extending the locking period**. They can also **add more JEWEL** to what is already locked (using the same remaining time locked) to receive more cJEWEL. Rewards may be claimed manually, but will also be automatically claimed when a player makes an additional deposit, extends their locking period, or withdraws their JEWEL balance.

#### Withdrawing

When players withdraw JEWEL from the cJEWEL contract, they may **only withdraw 100% of the balance**. This means that all cJEWEL will be burned whenever a player performs this action.

{% hint style="warning" %}
#### Emergency Withdraw

If the locking period has not expired, players can only withdraw using the **Emergency Withdraw** method, which will **return 50% of their locked balance and burn the remaining 50%**.
{% endhint %}

#### Jeweler Interactions

This model changes the way players will interact with the Jeweler, allowing them to call the following functions:&#x20;

* `createLock` - Takes a selected amount of JEWEL to deposit and days to lock and gives back cJEWEL based on the values chosen (only available if you have 0 cJEWEL)
* `increaseAmount` - Allows players to add more JEWEL to your deposited balance and receive more cJEWEL based on the remaining locking schedule for their existing balance
* `increaseUnlockTime` - Allows players to receive cJEWEL by extending the unlocking period of their existing JEWEL balance
* `claimReward` - Allows players to claim any pending fee-distribution rewards from the Jeweler
* `updatePool` - Will update the rewards available to everyone with cJEWEL by pulling in fees from the Fee Collector contract (this is also called whenever anyone deposits, extends unlocking periods, claims rewards, or withdraws)
* `withdraw` - Allows players to withdraw their entire JEWEL balance from the Jeweler if their locking period is expired
* `emergencyWithdraw` - Allows players to withdraw before their locking period is expired, but with a 50% penalty (which is burned)

### Governance Votes

Like many DeFi projects, the developers of DeFi Kingdoms may call for governance votes to empower token holders to make decisions about the direction of the project. Governance votes might determine the inclusion of a new token in incentivized pools, the retirement of a token from the pools, or a policy change that impacts token holders.

When this happens, the vote is announced on Discord and through the other DeFi Kingdoms social media accounts. cJEWEL and sJEWEL holders can visit the [Governance portal](https://vote.defikingdoms.com/), where they can connect their wallet and cast a number of votes equal to the number of tokens held.

Governance votes allow the holders of the token to have an active voice in decision-making, and the developers view this as a key component to a successful DeFi project.

{% hint style="info" %}
In addition to cJEWEL and sJEWEL holders being able to vote, holders of Hero NFTs and Land NFTs also have voting rights.&#x20;

Hero NFTs have the voting power of 10 cJEWEL/sJEWEL as the result of a [community governance vote](https://vote.defikingdoms.com/#/proposal/0xd74484526e93cd325e853aea1444d0c6d3019749beb31b65ee03f1a52e18e04f) held on 2/23/2022, and Land NFTs have the voting power of 100 cJEWEL/sJEWEL tokens.
{% endhint %}

### Fee Distribution

A portion of the transaction fees collected in-game are sent to the Jeweler as rewards for depositors. This includes 1/6 of collected fees from the DEX and [15% of Power Token fees](../power-tokens/#transactions-and-fee-distribution) from in-game transactions, including Hero summons, Pet incubations, Hero, Pet, and Land sales, and Hero meditations.&#x20;

These fees are sold for JEWEL and will accrue for the player according to their share of the total cJEWEL/sJEWEL in circulation, and will be claimable at any time, similar to how the [Gardens](../the-gardens/) work.  Because the amount of tokens coming into this reward pool fluctuates based on transaction volume, and because each player's share fluctuates with deposits and withdrawals, the Jeweler does not have a fixed APR.

{% hint style="info" %}
Since fees accrue and are distributed separately on each realm, cJEWEL and sJEWEL rewards will differ depending on the transaction volume in Crystalvale and Serendale. Players should choose carefully where and for how long they stake their JEWEL.
{% endhint %}

Claiming rewards can be done manually at any time, and will also happen automatically whenever the player deposits more JEWEL, extends their locking time, or withdraws their JEWEL balance.

For more technical detail on how these fees are apportioned to token holders, see [this article](https://dev.to/heymarkkop/understanding-sushiswaps-masterchef-staking-rewards-1m6f).

### Power-Ups

Holders of cJEWEL/sJEWEL will be able to activate **in-game enhancements and rewards** by allocating a portion of their holdings toward activating them. Power-Ups use your “available Power-Up balance,” which is the total amount of cJEWEL you hold minus the cJEWEL requirements of each of your active Power-Ups. Activating Power-Ups does not consume cJEWEL or the JEWEL used to produce it. Power-Ups can be deactivated at any time, or automatically, if the player's cJEWEL balance drops below the minimum necessary to keep them active.

Power-Up rewards may include bonuses to Hero experience, reduced in-game fees, and access to premium features. These Power-Ups are being continuously implemented over time.

Learn more about [Power-Ups](./#power-ups).

### Contract Addresses

* cJEWEL (DFK Chain): [`0x9ed2c155632C042CB8bC20634571fF1CA26f5742`](https://subnets.avax.network/defi-kingdoms/address/0x9ed2c155632C042CB8bC20634571fF1CA26f5742)
* sJEWEL (Klaytn): [`0xaA8548665bCC12C202d5d0C700093123F2463EA6`](https://scope.klaytn.com/token/0xaa8548665bcc12c202d5d0c700093123f2463ea6)

## Jeweler 1.0

The **Jeweler 1.0** was adapted from [SushiSwap](https://www.sushi.com/)'s [SushiBar](https://docs.sushi.com/docs/Products/Yield%20Farming/The%20SushiBar) contract, which allowed players to stake JEWEL and CRYSTAL for xJEWEL and xCRYSTAL, respectively. A portion of collected in-game fees were swapped for the Power Token, increasing the ratio between the Power Token and the xToken. &#x20;

When the player withdrew, they exchanged their xToken for the Power Token. The longer they had held the xToken, the more the ratio would have increased, and therefore the more of the Power Token they received back relative to their deposits.

### Contract Addresses

#### Harmony

* xJEWEL: [`0xA9cE83507D872C5e1273E745aBcfDa849DAA654F`](https://explorer.harmony.one/address/0xA9cE83507D872C5e1273E745aBcfDa849DAA654F)

#### DFK Chain&#x20;

* xCRYSTAL: [`0x6e7185872bcdf3f7a6cbbe81356e50daffb002d2`](https://subnets.avax.network/defi-kingdoms/address/0x6e7185872bcdf3f7a6cbbe81356e50daffb002d2)
* xJEWEL: [`0x77f2656d04E158f915bC22f07B779D94c1DC47Ff`](https://subnets.avax.network/defi-kingdoms/token/0x77f2656d04E158f915bC22f07B779D94c1DC47Ff)
