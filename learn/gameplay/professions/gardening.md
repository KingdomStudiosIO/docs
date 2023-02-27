---
description: Information about Gardening Quests
cover: ../../../.gitbook/assets/gardener-splash.428a0e2f.gif
coverY: 17.238183503243746
---

# Gardening

**Gardening Quests** can be performed by up to two Heroes at a time in each of the incentivized liquidity pools listed in the **Seed Box** in the Gardens. These quests award **Power Tokens** and **JEWEL**, as well as **Plants** and other rare items.

> _A friend of the gardens is a friend of mine. Please, let me show you our ways. Together, we can grow a beautiful field._

Gardening Quests are begun in the **Professions** area by speaking to the **Gardener**. Heroes may Garden in any of the available Gardens, but increased **Token Rewards** are only available from those in which the player has planted seeds, and the Token _****_ yield increases with the number of seeds planted by the player in that particular garden.

The Gardening Quest also has a chance to reward Heroes with **Plants**, **Gaia's Tears**, **Runes**, and **Green Pet Eggs** whether the player has seeds in the garden or not. All plants may be sold to the Vendor in the [Marketplace](../marketplace.md) for **Gold** or swapped at the Trader for other tokens or items. Some items are also used as reagents in **Potions** and [Enhancement Stones](../heroes/enhancement-stones.md), for hatching [Pets](../heroes/pets.md), and for [leveling Heroes](../heroes/leveling.md).

### **Gardening Basics**

#### Duration per Stamina

12 minutes (10 with **Gardening profession gene**)

#### Stamina Required

1 Stamina minimum

#### Required Hero Range

1-2 Heroes per Garden

### **Token Rewards**

The first Hero sent to quest in each Garden will be rewarded in the realm's **Power Token**, while the second Hero will earn **JEWEL**. These rewards are funded by the [Quest Reward Fund](https://subnets.avax.network/defi-kingdoms/address/0x1137643FE14b032966a59Acd68EBf3c1271Df316) wallet on each realm. Gardening yields rely heavily on the player's share of the **Liquidity Pools** that their Heroes will work in, the overall balance of the Quest Fund, and the stats of the questing Heroes. Consequently, there will be a large variance in yields between players and pools as well as a variance in yields over time as the Quest Fund grows or shrinks.

#### Formula

Gardening Token Rewards use the following formula, which applies to both Power Token and JEWEL rewards, when applicable.

`earnRate (per stamina spent) =`**`annealingFactor`**`* (`**`rewardPool`**`*`**`poolAllocation`**` `_`*`_**`LPowned`**`* (0.1 + (`**`WIS`**`+`**`VIT`**`) / 1222.22 +`**`GrdSkl`**`/ 244.44)) / (43,200 - (7200 *`**`geneBonus`**`))`

Calculated from these variables:

* **`annealingFactor` ** - A multiplier applied at launch that gradually decreases over time, letting the Quest Fund continue to grow. **`annealingFactor`** begins at `50` and decreases every two weeks to a minimum of `1` after 26 weeks.
  * **`annealingFactor`**` ``= (9100 - 49 * (`**`daysSinceLaunch`**`/ 14) * 14) / 182`
  * For the purposes of calculating **`daysSinceLaunch`**, Gardening Quests on Crystalvale and Serendale launched on 9/15/2022.
* **`rewardPool` ** - The relevant token balance in the [Quest Reward Fund](https://subnets.avax.network/defi-kingdoms/address/0x1137643FE14b032966a59Acd68EBf3c1271Df316).&#x20;
* **`poolAllocation` ** - The percent of token emissions allocated to the specific garden (in decimals, e.g. `0.1` for 10%).&#x20;
* **`LPowned` ** - The percent of the Liquidity Pool that the player owns in the selected Garden (in decimals, e.g. `0.0015` for 0.15%).&#x20;
* **`WIS`** / **`VIT`** - The value of the Hero's **Wisdom** and **Vitality** stats, respectively.
* **`GrdSkl` ** - The Hero's **Gardening** skill, rounded down (e.g. use `15` for 15.9 Gardening).&#x20;
* **`geneBonus` ** - If a Hero has the **Gardening profession gene**, it provides a 20% bonus to Token returns, increases the chances of finding Gaia's Tears and Runes, and decreases the amount of time spent Gardening per stamina from 12 minutes to 10 minutes. If the Hero has this gene, **`geneBonus`**`= 1`, if not, **`geneBonus`**`= 0`.&#x20;

#### Minimum Reward

The minimum Token Reward earned per Stamina spent is .0002. If **`earnRate` ** is below this threshold, it will be raised to .0002.

Minimum rewards are only active when there is at least 420,000 of the appropriate token available in the Quest Reward Fund.

#### Gardening Jackpots

For every 15 Stamina spent during the quest, the player will receive a bonus roll with a 9.9% chance to receive .1 bonus Token and a .1% chance to receive an additional 1 bonus Token. This bonus is halved if the Hero does not have the **Gardening profession gene**. Players cannot receive both bonuses at once.

Jackpot rewards are only active when there is at least 950,000 of the appropriate token available in the Quest Reward Fund.

### **Item Rewards**

{% hint style="info" %}
The item drop rates below are increased by varying combinations of the Hero's **Wisdom** and **Vitality** stats, its **Gardening skill,** and the presence of the **Gardening profession gene**.
{% endhint %}

<table><thead><tr><th>Name</th><th>Base Drop Rate</th><th>XP Awarded</th><th>Stamina Usage</th><th data-hidden align="center"> </th></tr></thead><tbody><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/bluestem.png" alt="Bluestem"> Bluestem</td><td>9%</td><td>10 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/bluestem.png" alt="Bluestem"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/spider-fruit.png" alt="Spiderfruit"> Spiderfruit</td><td>6%</td><td>10 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/spider-fruit.png" alt="Spiderfruit"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/milkweed.png" alt="Milkweed"> Milkweed</td><td>4%</td><td>10 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/gaias-tear.png" alt="" data-size="original"> Gaia's Tear</td><td>7.5% / 11.25% *</td><td>10 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/shvas-rune.gif" alt=""> Shvās Rune</td><td>0.3% / 1.5% *</td><td>30 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/moksha-rune.gif" alt=""> Moksha Rune</td><td>0.009% / 0.045% *</td><td>100 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-green.png" alt="Green Pet Egg"> Green Pet Egg</td><td>0.02%</td><td>100 XP</td><td>per <strong>10</strong> Stamina</td><td align="center"><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-green.png" alt="Green Pet Egg"></td></tr></tbody></table>

\* The higher percentage applies to Heroes with the **Gardening profession gene**.

