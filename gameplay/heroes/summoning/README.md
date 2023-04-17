# Summoning

<figure><img src="../../../.gitbook/assets/Screenshot 2023-04-11 at 11.20.14 PM.png" alt=""><figcaption><p>The Crystalvale Summoning Portal</p></figcaption></figure>

To summon, two Heroes must visit the **Arch Druid** and infuse a Summoning Crystal with their combined essence. **Infused Crystals** are then used at the [Portal](../../../learn/gameplay/portal.md) to seek Heroes from far away lands that are in tune with the Heroes that infused the crystal.

![Infused Crystal](https://dfk-hv.b-cdn.net/art-assets/crystal-yellow.gif)

To infuse a crystal, Heroes pour their energy into **Gaia’s Tears** and the **Power Token** of that realm, which are then fed into a Summoning Crystal. Stronger Heroes may use additional Gaia’s Tears to cause the portal to seek stronger Heroes more like the summoner.

{% hint style="info" %}
Note: Summoned Heroes are too similar to the Heroes that summoned them to be able to properly attune a new Summoning Crystal. This is also true for pairs of Heroes that were Summoned by one or two of the the same Heroes. All other combinations of Heroes will not encounter any trouble attuning a Summoning Crystal so long as they have remaining attunement energy.
{% endhint %}

For every 5 levels a summoning Hero has reached, they may increase the Tear cost by 10 to provide bonuses to the Summoned Hero. Those bonuses are applied to the Summoned Hero’s stats, Primary Stat Growth, and Secondary Stat Growth. The bonuses are based on the summoning Hero’s top three stats, and each summoning Hero may provide their own bonuses if they use extra tears.

The bonuses loop through the following pattern with each increased step in +10 tears paid per summoning Hero:

1. \+(1 + loopCount) to stat matching highest stat of summoning Hero
2. \+(1 + loopCount)% to primary stat growth rate of stat matching the highest stat of summoning Hero
3. \+(2 + loopCount)% to secondary stat growth rate of stat matching the highest stat of summoning Hero
4. \+(1 + loopCount) to stat matching second highest stat of summoning Hero
5. \+(1 + loopCount)% to primary stat growth rate of stat matching the second highest stat of summoning Hero
6. \+(2 + loopCount)% to secondary stat growth rate of stat matching the second highest stat of summoning Hero
7. \+(1 + loopCount) to stat matching third highest stat of summoning Hero
8. \+(1 + loopCount)% to primary stat growth rate of stat matching the third highest stat of summoning Hero
9. \+(2 + loopCount)% to secondary stat growth rate of stat matching the third highest stat of summoning Hero

In these formulas, loopCount indicates the number of times the bonuses have looped back to step 1 (this happens at +100 and +190 tears added). So the second time around, on step 1 the bonus would be +2 added to the stat matching the highest stat of the summoning Hero, and so on.

Examples: LVL30 Wizard (highest stats INT, WIS, and LCK) pays 70 Gaia’s Tears (base 10 + 60 for 6 steps of 5 levels) Summoned Hero receives +1 to INT and WIS, +1% primary stat growth to INT and WIS, and +2% secondary stat growth to INT and WIS

LVL100 Wizard (highest stats INT, WIS, and LCK) pays 210 Gaia’s Tears (base 10 + 200 for 20 steps of 5 levels) Summoned Hero receives +6 to INT, +3 WIS, and +3 LCK, +6% primary stat growth to INT, +3% to WIS, and 3% to LCK, and +5% secondary stat growth to INT, WIS, and LCK

<figure><img src="../../../.gitbook/assets/Screenshot 2023-04-11 at 11.26.19 PM.png" alt=""><figcaption><p>Tears Bonus</p></figcaption></figure>

These bonuses are **per** summoning Hero, so the maximum possible for two LVL100 Heroes to spend would be 420 Gaia's Tears (base 10\*2 + 200\*2 extra)

**Enhancement stones** can also be used during this process to further improve the starting parameters of the summoned Hero!

The act of Summoning is an exhausting process, and that exhaustion compounds with each act of Summoning. For each Summon a Hero performs, they must wait for a **cooldown period** before they can Summon again. The cooldown period = ((heroGen \* 4 hours) + 4 hours) \* summonsUsed. The max cooldown for Gen0 Heroes is 72 hours. In addition, with the exception of Gen0 Heroes, all new Summoned Heroes have a 24 hour cooldown period before they can Summon.

The exhaustion of Summoning doesn’t end at just a cooldown. The amount of Power Tokens needed to for each Hero to infuse the next Summoning Crystal also increases by 2 Power Tokens after each Summon. Gen0 Heroes have the lowest starting cost for Summoning (6 Power Tokens), and each generation above 0 will see an increase of 10 Power Tokens per generation in cost for their Summons compared to lower generations. The Gen0 increase in cost per Summon will eventually cap at a price that is lower than what later generations will pay to perform their final summon.

What’s this? Yes, unfortunately only Gen0 Heroes are able to maintain their attunement to Gaia Summon after Summon. All later generations simply have a limit to how many times they can focus their energies into Gaia’s Tears. Once they have expended the last of their attunement energies, they can no longer Summon. Another quirk of the Summoning process is that the portal seeks those who have similar Gaia attunement strength as the weakest Summoner. So if a Gen0 summoner Hero infuses a crystal with a Gen1 summoner Hero with only four remaining summons worth of attunement, then the summoned Gen2 will only be able to summon three times (the same number of remaining summons as the weakest summoner after summoning this new hero). Two Gen0 summoners will Summon a Gen1 with ten Summons worth of attunement.

## Hero Ranks

Higher ranked Heroes have begun to arrive in the kingdom!!!

<figure><img src="../../../.gitbook/assets/1_Hero_Class_Summoning_Tree_Updated_2-2023.png" alt=""><figcaption></figcaption></figure>

Summoning with Heroes that have the appropriate genes can result in genetic mutation that results in a higher ranked Hero being Summoned from the Portal. The chart above displays the genetic combinations needed to Summon each possible Hero class.

Heroes of higher rank have better starting stats and stat growth parameters than those of ranks below them. However, a side effect of their advanced abilities is that they require more Gaia's Tears to perform a Summon than Heroes of lower ranks. In addition, higher-ranked Heroes are more difficult for the Portal to have a chance to locate, so higher-ranked Heroes have lower maximum summons than lower-ranked ones. The chart above displays the Gaia's Tears requirements for higher-ranked and the maximum number of Summons that higher-ranked classes can receive on Summoning.

Basic - Warrior, Knight, Thief, Archer, Priest, Wizard, Monk, Pirate, Berserker, Seer, Legionnaire, Scholar

Advanced - Paladin, Dark Knight, Summoner, Ninja, Shapeshifter, Bard

Elite - Dragoon, Sage, Spellbow

Exalted - DreadKnight

## Hero Rarity

The rarity level of a Summoned Hero is impacted by the rarity of the two Heroes used to infuse the Summoning Crystal.

![Summoning Rarity](<../../../.gitbook/assets/Summoner Combo.png>)

The chart above illustrates the likelihood that pairing Heroes of given rarities will result in a Summoned Hero of a given rarity. For further information on this topic, visit the [Rarity](../../../learn/gameplay/heroes/rarity.md) topic page.
