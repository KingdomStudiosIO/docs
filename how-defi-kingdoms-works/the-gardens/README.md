# The Gardens

In each realm, the Gardens is a place to stake liquidity pool tokens to receive a share of power token emissions. In the JEWEL gardens of Serendale, players can stake to receive JEWEL emissions, while in the Ice Gardens of Crystalvale, CRYSTAL emissions are on offer for those who stake.

![](<../../.gitbook/assets/Cute Henry.gif>)

Additionally, players can assign their Hero NFTs to work in their gardens. Those Heroes earn additional rewards in JEWEL or CRYSTAL based on the skill of the Hero and the amount invested in the garden they're tending, so players who invest in the Gardens and in Heroes have synergistic utility for their NFTs right away.

### Epochs and Emissions

Each power token has its own emissions schedule. Generally speaking, emissions per minute are higher when the token launches, and decrease over time. This decrease in emissions is not linear, so it is important to review the emissions schedules for each token in its related Gardens subpage.

Emissions are governed by periods of time called Epochs. Each token starts in Epoch 1 on launch, which has the highest emission rate. With each Epoch, the rate may change or may remain consistent, as shown in each token's chart on its Gardens page.

Epochs on the Harmony chain are linked to block speed, so JEWEL emissions are tied to the speed of the Harmony chain and the length of each Epoch (ideally one week) may vary if the chain experiences slowdowns.

On Avalanche, the Epochs are based on timestamps and last exactly one week.

### Allocations and Rewards

The total amount of each token emitted per minute can be determined by Epoch, but those tokens have to go somewhere! Each individual garden (representing a specific LP pair) is assigned an allocation of the total tokens minted. The allocation for each pool can be viewed in the Seed Box. Based on the current Epoch, its emission rate, and the allocation for a specific pool, players can determine how many of a token will be given to that pool each second, minute, or day. From there, the pool divides those tokens among all of its investors proportional to their share of the total pool and distributes them as rewards. When making these calculations it is imperative to remember that players can enter or leave liquidity pools freely, so each player's share is constantly in flux as liquidity is added or removed.

### Locking Model

To balance the high emissions rates in earlier Epochs and to provide price stability, our tokenomics includes a locking model on Gardens rewards. A portion of the tokens grown, harvested, and distributed as Gardens rewards is unlocked. Once claimed, these unlocked reward tokens transfer directly into the players wallets and are immediately usable. However, a portion of Gardens rewards are also locked deep underground. These rewards are allocated to the player's wallet, but cannot be accessed or used in any way until they become unlocked.

For each token, starting in Epoch 1, 5% of claimed rewards are unlocked while 95% are locked. Each Epoch, the percentage of claimed rewards that are unlocked increases by 2%, so in Epoch 2, 7% are unlocked and 93% are locked, and so on. It is important to note that these percentages are based on the Epoch at the time that the player chooses to claim, not when the rewards were allocated. If a player chooses not to claim right away, the percentage that they _will_ be able to claim increases by 2% each Epoch. Once a player does claim, however, the remainder of the locked rewards cease their unlocking until Epoch 51, at which point they begin unlocking ratably over the next 52 Epochs. After Epoch 51, no further locking will occur and all newly generated rewards will be fully unlocked immediately.

### Locking Model - Early Unlocking with Hero NFTs

One of the most unique features of DeFi Kingdoms is our Hero NFTs that provide true in-game utility. The mining profession is one such use-case. Players who have locked rewards can send their Heroes on JEWEL or CRYSTAL mining quests to unlock some early, granting access to locked rewards before Epoch 51 and unlocking faster even once that threshold arrives.&#x20;

Not all Heroes will have the same level of proficiency in mining, so it is important to learn about the various stats that Heroes use and how each profession works when looking to buy and use them.

### **Garden Staking Deposit and Withdrawal Fees**

**There are no deposit fees for staking LP tokens in the Gardens.** To protect against flash loans and pump and dumps, we have implemented withdrawal fees for withdrawing staked LP tokens. Each withdrawal resets the fee timer. The withdrawal fees are listed below:

* **0.01%** fee if a user withdraws after **4 Epochs**
* **0.25%** fee if a user withdraws after **2 Epochs but before 4 Epochs**
* **0.5%** fee if a user withdraws after **5 days but before 2 Epochs**
* **1%** fee if a user withdraws under **5 days. \***
* **2%** fee if a user withdraws under **3 days. \***&#x20;
* **4%** fee if a user withdraws under **24 hours. \***&#x20;
* **8%** fee if a user withdraws under **1 hour. \***
* **25%** slashing fee if a user withdraws **during the same block.**

_\*In the case of JEWEL and Harmony, days/hours listed assume a 2 seconds per block speed during such period and will depend on blockchain speed._
