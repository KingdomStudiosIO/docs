# Summoning

![Summoning Portal (work in progress)](https://dfk-hv.b-cdn.net/art-assets/portal.gif)

To summon, two heroes must visit the **Arch Druid** and infuse a summoning crystal with their combined essence. **Infused crystals** are then used at the portal to seek heroes from far away lands that are in tune with the heroes that infused the crystal. 

![Infused Crystal](https://dfk-hv.b-cdn.net/art-assets/crystal-yellow.gif)

To infuse a crystal, heroes pour their energy into **Gaia’s Tears** and **JEWELs**, which are then fed into a summoning crystal. Stronger heroes may use additional Gaia’s Tears to cause the portal to seek stronger heroes more like the summoner. 

NOTE: Summoned heroes are too similar to the heroes that summoned them to be able to properly attune a new summoning crystal. This is also true for pairs of heroes that were summoned by one or two of the the same heroes. All other combinations of heroes will not encounter any trouble attuning a summoning crystal so long as they have remaining attunement energy.

For every 5 levels a summoning hero has reached, they may increase the tear cost by 10 to provide bonuses to the summoned hero. Those bonuses are applied to the summoned hero’s stats, Primary Stat Growth, and Secondary Stat Growth. The bonuses are based on the summoning hero’s top three stats, and each summoning hero may provide their own bonuses if they use extra tears.

The bonuses loop through the following pattern with each increased step in +10 tears paid per summoning hero:

1. +(1 + loopCount) to stat matching highest stat of summoning hero
2. +(1 + loopCount)% to primary stat growth rate of stat matching the highest stat of summoning hero
3. +(2 + loopCount)% to secondary stat growth rate of stat matching the highest stat of summoning hero
4. +(1 + loopCount) to stat matching second highest stat of summoning hero
5. +(1 + loopCount)% to primary stat growth rate of stat matching the second highest stat of summoning hero
6. +(2 + loopCount)% to secondary stat growth rate of stat matching the second highest stat of summoning hero
7. +(1 + loopCount) to stat matching third highest stat of summoning hero
8. +(1 + loopCount)% to primary stat growth rate of stat matching the third highest stat of summoning hero
9. +(2 + loopCount)% to secondary stat growth rate of stat matching the third highest stat of summoning hero

In these formulas, loopCount indicates the number of times the bonuses have looped back to step 1 (this happens at +100 and +190 tears added). So the second time around, on step 1 the bonus would be +2 added to the stat matching the highest stat of the summoning hero, and so on.

Examples: 
LVL30 Wizard (highest stats INT, WIS, and LCK) pays 70 Gaia’s Tears (base 10 + 60 for 6 steps of 5 levels)
Summoned hero receives +1 to INT and WIS, +1% primary stat growth to INT and WIS, and +2% secondary stat growth to INT and WIS

LVL100 Wizard (highest stats INT, WIS, and LCK) pays 210 Gaia’s Tears (base 10 + 200 for 20 steps of 5 levels)
Summoned hero receives +6 to INT, +3 WIS, and +3 LCK, +6% primary stat growth to INT, +3% to WIS, and 3% to LCK, and +5% secondary stat growth to INT, WIS, and LCK

These bonuses are **per** summoning hero, so the maximum possible for two LVL100 heroes to spend would be 420 Gaia's Tears (base 10\*2 + 200\*2 extra)

![TearsBonus](https://user-images.githubusercontent.com/91647016/136145171-dc6d4256-c1f5-40f6-b8a7-de6d8d46c593.png)

**Enhancement stones** can also be used during this process to further improve the starting parameters of the summoned hero!

The act of summoning is an exhausting process, and that exhaustion compounds with each act of summoning. For each summon a hero performs, they must wait for a **cooldown period** before they can summon again. The cooldown period increases by four hours with each summon, up to a maximum limit. The base cooldown period is 4\*summonerGeneration hours. In addition, with the exception of Gen0 heroes, all new summoned heroes have a 24 hour cooldown period before they can summon. 

The exhaustion of summoning doesn’t end at just a cooldown. The amount of JEWELs needed to for each hero to infuse the next summoning crystal also increases by 2 JEWELs after each summon. Gen0 heroes have the lowest starting cost for summoning (6 JEWELs), and each generation above 0 will see an increase of 10 JEWEL per generation in cost for their summons compared to lower generations. The gen0 increase in cost per summon will eventually cap at a price that is lower than what later generations will pay to perform their final summon.

What’s this? Yes, unfortunately only Gen0 heroes are able to maintain their attunement to Gaia summon after summon. All later generations simply have a limit to how many times they can focus their energies into Gaia’s Tears. Once they have expended the last of their attunement energies, they can no longer summon. Another quirk of the summoning process is that the portal seeks those who have similar Gaia attunement strength as the weakest summoner. So if a gen0 summoner hero infuses a crystal with a gen1 summoner hero with only four remaining summons worth of attunement, then the summoned gen2 will only be able to summon three times (the same number of remaining summons as the weakest summoner after summoning this new hero). Two gen0 summoners will summon a gen1 with ten summons worth of attunement. 

Higher ranked heroes have begun to arrive at the kingdom!!!

![Summoner](https://user-images.githubusercontent.com/91647016/136327660-f398e0a4-cb99-4be5-b102-8a20b9366053.png)

Heroes of higher rank have better starting stats and stat growth parameters than those of ranks below them. However, a side effect of their advanced abilities is that they require more Gaia's Tears to perform a summon than heroes of lower ranks. For example, the summoner depicted above must pay 40 tears to be able to summon. In addition, higher ranked heroes are more difficult for the portal to have a chance to locate, so higher rank heroes have lower maximum summons than lower ranked ones. This can be seen in the image of the Summoner above. 

**Ranks**
Basic - Warrior, Knight, Thief, Archer, Priest, Wizard, Monk, Pirate
Advanced - Paladin, Dark Knight, Summoner, Ninja

