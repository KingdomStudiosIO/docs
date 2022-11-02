---
description: Information about the Level 0 Gardening quest.
---

# Gardening

**Gardening Quests** can be performed by one Hero at a time in each of the incentivized pools listed in the **Seed Box** in the Gardens. The quest is begun in the **Professions** area by speaking to the **Gardener**, Druid Lam. Heroes may Garden in any of the available Gardens, but the JEWEL yield increases with the number of seeds planted by that player in that particular garden. However, there is a minimum JEWEL yield from all gardens, a potential jackpot available for every 15 Stamina spent, and chance for Heroes to be rewarded with **plants**, **Gaia's Tears**, **Shvās runes**, and **Green Eggs** whether the player has seeds in the garden or not. All plants may be sold in the [Marketplace](../../locations/marketplace.md) to Vendor Zada for **gold** or swapped with Trader Matoya for **JEWEL**. Some plants are ingredients in **potions**, which can be crafted with Alchemist Herbert. All plants may have uses that are unknown as yet.

**The Level 0 Gardening quest is being launched with a special multiplier to increase its rewards yield for a limited time.** The quest launch occurred on 12/22/21. This multiplier will decrease over a period of 16 weeks until the quest settles at the intended yield formula. Gardening yields rely heavily on both the player's share of the liquidity pools that their Heroes will work in and on the overall balance of the Quest Rewards wallet, so there will be both a large variance in yields between players and pools and a variance in yields over time as the Quest Rewards pool grows or shrinks.

### **Level 0 rewards formula:**

earnRate (per tick) = **launchBonus**\*(**rewardPool**\***poolAllocation**_\*_**LPowned**\*(0.1+ (**WIS**+**VIT**)/1222.22+(**GrdSkl**)/244.44))/(43,200-(7200\***geneBonus**)) \*\*&#x20;

**rewardPool** - This is the balance of the quest pool wallet.&#x20;

**poolAllocation** - This is the percent of allocation a specific garden has (the allocation for JEWEL distribution).&#x20;

**LPowned** - The percent of the liquidity pool that the player owns in the selected Garden.&#x20;

**GrdSkl** - A hero's Gardening skill (only counts integer value (1.9 GrdSkl will have same result as 1.0 GrdSkl).&#x20;

**geneBonus** - Provides a 20% bonus to JEWEL returns, increases the chances of finding tears and runes, and decreases the amount of time per tick from 12 minutes to 10 minutes. These bonuses are only present if the hero has the gardening gene. If they have the gene, geneBonus = 1, if not, geneBonus = 0.&#x20;

**launchBonus** - A special multiplier applied at launch that will start at 5 at launch, and decrease by 0.5 every two weeks until the value is 1.

\*\*The minimum JEWEL earned per Stamina spent is .0002 JEWEL.

Additionally, for every 15 Stamina spent, there is a 9.9% chance to receive .1 bonus JEWEL and a .1% chance to receive 1 bonus JEWEL. This bonus is halved if the Hero does not have **gardening** as their main skill and the bonus is calculated in one roll, so a Hero cannot receive both bonuses. This bonus was implemented in Beta on February 2, 2022.

### **Level 0 item drop rates:**

**Spiderfruit** - 6% (per 5 Stamina spent)

**Milkweed** - 4% (per 5 Stamina spent)

**Bluestem** - 9% (per 5 Stamina spent)

**Green Egg** - .02% (per 10 Stamina spent)

**Item drop rates are increased by varying combinations WIS, VIT, and, the gardening stat, and the gardening gene.**
