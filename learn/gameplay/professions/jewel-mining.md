---
description: Information about Token Mining Quests
cover: ../../../.gitbook/assets/pickmankhudmire.gif
coverY: 0
---

# Token Mining

**Token Mining Quests** can be performed by up to six Heroes at a time in each realm. These quests unlock [**Power Tokens**](../../../how-defi-kingdoms-works/power-tokens/) from your locked balance, and can award other rare items.

> Ready to start doing some mining for some real treasure, are ye? Let's get ta diggin'! I'll treat ya to some ale if we come back alive!

Token Mining Quests are begun in the **Professions** zone by speaking to the **Miner** or **Pickman**, depending on the realm. Heroes may only begin Token Mining Quests if the player has a locked balance of the realm's Power Token. The token yield increases with the locked balance of the player—up to a specific limit—as well as the stats of the Heroes that are sent on the quest.

Token Mining Quests also have a chance to reward Heroes with **Gaia's Tears**, **Runes**, and **Yellow Pet Eggs**. All of these items may be swapped at the Trader for other tokens or items. Some items are also used as reagents in **Potions** and [Enhancement Stones](../heroes/enhancement-stones.md), for hatching [Pets](../heroes/pets.md), and for [leveling Heroes](../heroes/leveling.md).

### **Mining Basics**

#### Duration per Stamina

12 minutes (10 with **Mining profession gene**)

#### Stamina Required

1 Stamina minimum

#### Required Hero Range

1-6 Heroes

### **Token Rewards**

**Token Mining Quests** require the player to select a **Lead Miner** for each quest, whose stats determine the maximum amount of Power Tokens that can be unlocked during that quest. These stats include the Hero's **Strength** and **Endurance** scores, their **Mining** skill, and whether they have the **Mining profession gene**. Up to five additional Heroes can be added to assist the Lead Miner, whose stats all determine the final quest reward. If the group's total unlockable amount reaches the maximum unlockable amount, adding additional Heroes will not increase the token rewards further, although those Heroes can still receive **item rewards**.

#### Formula

The unlocked Power Token reward for Mining per stamina spent is equal to the **`maxUnlockRate`** or the sum of the **`heroUnlockRate`** for each Hero sent on the Quest, whichever value is smaller.&#x20;

These values are calculated from the following formulas and variables:

* **`maxUnlockRate`** - The maximum amount of Power Tokens that can be unlocked per stamina spent. This amount is set according to the stats of the **Lead Miner**:\
  `maxUnlockRate = (1000 * (0.25 + (`**`STR`**`+`**`END`**`) * 0.000625 + (`**`MinSkl`**`) * 0.0025)) /`` `**`lockedRatio`**
* **`heroUnlockRate` -** The amount of Power Tokens that are unlocked per stamina spent. This amount is calculated according to the stats of **each Miner**:\
  `heroUnlockRate = (1000 * (0.25 + (`**`STR`**`+`**`END`**`) * 0.000625 + (`**`MinSkl`**`) * 0.0025)) / (6 * (1000 - 166 *`` `**`geneBonus`**`))`
* **`lockedRatio`** - The ratio between **`minLocked`** and **`lockedPT`**:

```javascript
if lockedPT > minLocked {
    lockedRatio = (1000 - 166 * geneBonus)
else
    lockedRatio = ((1000 - 166 * geneBonus) * minLocked) / lockedPT
}
```

* **`lockedPT`** - The number of locked Power Tokens in the player's wallet.
* **`minLocked`** - The minimum amount of locked Power Tokens a player must have to get the maximum mining reward. Set to `5000` Power Tokens.
* **`STR`** / **`END`** - The value of the Hero's **Strength** and **Endurance** stats, respectively.
* **`MinSkill`** - The Hero's **Mining** skill, rounded down (e.g. use `15` for 15.9 Mining).&#x20;
* **`geneBonus`** - If a Hero has the **Mining profession gene**, it provides a 20% bonus to Power Token returns, increases the chances of finding Gaia's Tears and Runes, and decreases the amount of time spent Mining per stamina from 12 minutes to 10 minutes. If the Hero has this gene, **`geneBonus`**`= 1`, if not, **`geneBonus`**`= 0`.

#### Mining Jackpots

For every 15 Stamina spent by the **lead miner**, the player will receive a bonus roll with a 10% chance to unlock bonus Power Tokens. The maximum bonus is 10 Power Tokens if the wallet has at least 1,250 locked Power Tokens. This bonus scales down linearly if the wallet has less than 1,250 locked Power Tokens, and is halved if the **Lead Miner** does not have the **Mining profession gene**.

### **Item Rewards**

{% hint style="info" %}
The item drop rates below are increased by varying combinations of the Hero's **Strength** and **Endurance** stats, its **Mining skill,** and the presence of the **Mining profession gene**.
{% endhint %}

<table><thead><tr><th>Name</th><th>Base Drop Rate</th><th>XP Awarded</th><th>Stamina Usage</th><th data-hidden align="center"> </th></tr></thead><tbody><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/gaias-tear.png" alt="" data-size="original"> Gaia's Tear</td><td>7.5% / 11.25% *</td><td>10 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/shvas-rune.gif" alt=""> Shvās Rune</td><td>0.3% / 1.5% *</td><td>30 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/moksha-rune.gif" alt=""> Moksha Rune</td><td>0.009% / 0.045% *</td><td>100 XP</td><td>per <strong>5</strong> Stamina</td><td align="center"></td></tr><tr><td><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-yellow.png" alt="Green Pet Egg"> Yellow Pet Egg</td><td>0.02%</td><td>100 XP</td><td>per <strong>10</strong> Stamina</td><td align="center"><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/pet-egg-green.png" alt="Green Pet Egg"></td></tr></tbody></table>

\* The higher percentage applies to Heroes with the **Mining profession gene**.
