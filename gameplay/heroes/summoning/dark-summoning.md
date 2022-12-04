---
description: >-
  Dark Summoning allows players to sacrifice two Heroes in order to summon a new
  one.
cover: ../../../.gitbook/assets/dark_summonoing_cover.png
coverY: 48.227360026226236
---

# Dark Summoning

**Dark Summoning** allows players to sacrifice two Heroes in order to summon a new one. There are reduced costs and restrictions on the summon, and in exchange, benefits to the new Hero.

> _"What do we have here? Hrrgh... A new face. Yesss... and there, behind the eyes, a darkness... deepening. Come, young one, stand with me and look into the void. There is pain there, yesss... but also great power."_

<figure><img src="https://defi-kingdoms.b-cdn.net/art-assets/items/dark-crystal.gif" alt=""><figcaption></figcaption></figure>

## Mechanics

Dark Summoning works the same as standard Summoning, where two Heroes can create a new Hero. Hero genetics and remaining summons are passed down in the same way. Players are allowed to use [Enhancement Stones](../../../learn/gameplay/heroes/enhancement-stones.md) and infuse the new summon with Gaia's Tears to receive stat bonuses.&#x20;

There a few key differences from standard Summoning, however:

### Hero Burning

{% hint style="warning" %}
Unlike standard Summoning, in Dark Summoning, the two summoning Heroes are **sacrificed (burned)**, and permanently sent to a Graveyard wallet. _This action cannot be undone._
{% endhint %}

### Reduced Summoning Costs

Dark Summoning costs 1/4 the amount of CRYSTAL of standard Summoning.

### Removed Restrictions

* Heroes with zero summons remaining are eligible to Dark Summon. Any resulting Hero will also have zero summons (even in the case of a Hero Class mutation).
* There are no restrictions on Dark Summoning with Heroes that share a common origin.
* The summoning cooldown on Heroes is ignored when Dark Summoning.

### Additional Restrictions

* Gen0 Heroes are ineligible for Dark Summoning.
* Heroes listed for hire in the [Tavern](../../../learn/gameplay/tavern.md) cannot be used in Dark Summoning. Players must own both summoning Heroes.

## Hero Benefits

In exchange for the sacrifice of the summoning Heroes, Dark Summoned Heroes receive the following benefits:

### Level Carryover

Dark Summoned Heroes are eligible to immediately [level up](../../../learn/gameplay/heroes/leveling.md) to the average level of the two summoning Heroes (rounded down). No XP is necessary for these level ups, and any XP earned will not carry over. Level ups are done individually, and players can choose stats for Gaia's Blessing and use [Attunement Crystals](../../../learn/gameplay/heroes/attunement-crystals/) during each one.

### Rarity

The base rarity chances for Dark Summoned Heroes are increased from regular Summoning as follows:

<figure><img src="../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption><p>Base Rarity chances for Dark Summoned Heroes</p></figcaption></figure>

#### Rarity Floor

The lowest rarity possible when Dark Summoning is based on the average rarity of the two sacrificed Heroes (rounded down). The floor rarity does not increase the chances of getting higher rarities, it simply guarantees that the summoned Hero will not be a lower rarity than the average of the two sacrificed Heroes.

{% hint style="info" %}
Example: a Common Hero paired with a Rare would have a floor rarity of Uncommon, and likewise for a Common paired with a Legendary.
{% endhint %}

#### Rarity Overcharging

Players may spend extra CRYSTAL and Gaia’s Tears to increase the chances of getting higher rarity Heroes. The amount extra allowed to be paid is based on the sum of the remaining summons of the two summoning Heroes. For each remaining summon, players may pay 0.625 CRYSTAL and 20 Gaia’s Tears to receive 1/5th of the bonus that is gained by summoning with a rarer Hero. So, for example, if they have 20 remaining summons, it would be as if both Heroes were two rarity levels higher than they actually are.

{% hint style="info" %}
Rarity overcharging does not affect the number of summons that the new Hero will have.
{% endhint %}

#### Rarity Calculations

The calculations for Dark Summoning rarity are as follows:

**`rareMod`** = the sum of the rarity values of the two Heroes. Common has a rarity value of 0, and each step up in rarity increases the value by 1, so Mythic has a rarity value of 4.

**`chargeValue`** = this value represents the number of remaining summons from the sacrificed Heroes that players pay extra to overcharge. This value can range from 0 to 20 depending on the two Heroes sacrificed.

* `Common = 527000 - 34250*rareMod - 6850*chargeValue`
* `Uncommon = 300000 + 10250*rareMod + 2050*chargeValue`
* `Rare = 140000 + 9375*rareMod + 1875*chargeValue`
* `Legendary = 30000 + 8500*rareMod + 1700*chargeValue`
* `Mythic = 3000 + 6125*rareMod + 1225*chargeValue`

Divide these values by `10000` to find the final percentage.

### Shiny

The chance of receiving a [Shiny](../../../learn/gameplay/heroes/rarity.md#shininess) Hero is increased by 5x over standard Summoning.

