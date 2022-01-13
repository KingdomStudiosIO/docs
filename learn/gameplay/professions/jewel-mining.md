---
description: Information about the Level 0 JEWEL Mining quest.
---

# JEWEL Mining

**The following information is accurate for the version of the quest that is released on the Beta site. Any information in this document is subject to change.**

**JEWEL Mining Quests** can be performed by a party of anywhere between 1 and 6 Heroes at a time.  Heroes can be queued to begin questing as soon as the Stamina of the currently questing Heroes is expended; however, the party of Heroes will all stop mining as soon as any Hero's Stamina reaches zero. Additionally, once a party of any size enters the mine, additional miners cannot be added to the party. Those Heroes will be queued and will not commence their quest until one Hero in the previous party reaches 0 Stamina, causing the entire party to stop mining, or until the player ends the mining quest early.

**JEWEL mining** quests require the player to select a **lead miner**. The maximum amount of JEWEL that can be unlocked in the quest is determined by the stats of the **lead miner**: the Hero's **STR** and **END** scores, **mining** skill, and whether they have **mining** as their main profession all impact the max amount that can be unlocked. When a **lead miner** is selected, the maximum unlockable JEWEL for the party and the amount of JEWEL that can be unlocked by the **lead miner** alone will be displayed.

Up to five further Heroes can be added to the mining party to assist the **lead miner**. Their contribution to the party will be based on their **STR** and **END** scores, **mining** score and on whether the Hero has **mining** as their main profession. As individual Heroes are added to the party, the total amount of JEWEL that the party can unlock will update. Once the group's total unlockable amount reaches the maximum unlockable amount, adding further Heroes will not increase JEWEL rewards further, although those Heroes can still receive **Gaia's Tears**, **Shvās runes**, and **Yellow Eggs**.

Heroes with **mining** as their main profession expend 1 Stamina every 10 minutes, and all other Heroes expend 1 Stamina per 12 minutes. However, if a party of Miners contains Heroes that do _not_ have **mining** as their main profession, all Heroes in that party will expend at the 1 Stamina per 12 minutes rate. It is important to strategically group miners to achieve maximum rewards.

Mining quests also have a chance to reward Heroes with **Gaia's Tears**, **Shvās runes**, and **Yellow Eggs**. Item drop rates are increased by varying combinations of **STR**, **END**, the **mining** stat, and the **mining** gene.

### **Level 0 rewards formula:**

&#x20;    **Max unlock rate formula:**\
&#x20;       maxUnlockRate = (1000 \* (0.25 + (**STR** + **END**) \* 0.000625 + (**MinSkl**) \* 0.0025)) / lockedRatio

&#x20;    **LockedRatio formula:**\
&#x20;        if lockedJWL > minLocked {\
&#x20;            lockedRatio = (1000 - 166 \* geneBonus)\
&#x20;        else \
&#x20;            lockedRatio = ((1000-166 \* geneBonus) \* minLocked) / lockedJWL

&#x20;    **Hero unlock rate formula:**\
&#x20;        heroUnlockRate = (1000 \* (0.25 + (**STR** + **END**) \*0.000625 +(**MinSkl**) \* 0.0025)) / (6 \* (1000 -            \
&#x20;        166 \* geneBonus))

&#x20;   **minLocked** = 20,000 JEWEL (scales down linearly if wallet has less than 20k locked JEWEL)

&#x20;    **minSkill** = the integer value of the Hero's **mining** skill

&#x20;    **geneBonus** = 1 if character has **mining** as their main skill, else 0

Additionally, for every 15 Stamina spent by the **lead miner**, there is a 10% chance to receive bonus JEWEL. The maximum bonus is 10 JEWEL, if the wallet has at least 5,000 locked JEWEL. The bonus scales down linearly if the wallet has less than 5,000 locked JEWEL. This bonus is halved if the **lead miner** does not having **mining** as their main skill.

### Level 0 base item drop rates:

**Shvās rune** - 0.3% per 5 Stamina expended, boosted to 1.5% with **mining** main skill&#x20;

**Gaia's Tears** - 7%  per 5 Stamina expended, boosted to 10.75% with **mining** main skill

**Yellow Egg** - 0.02% (per 10 Stamina spent)
