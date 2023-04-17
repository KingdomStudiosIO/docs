# Leveling

Heroes can increase their stats by leveling up. To level up, a Hero must first have accumulated enough experience from their adventures. Once they have done that, they visit the **Meditation Circle**, and spend a certain number of runes and Power Tokens based on their level. They also have the option to use an [Attunement Crystal](attunement-crystals/) while leveling up, which will increase the success rate for certain stat increases.

<figure><img src="../../../.gitbook/assets/Screenshot 2023-04-11 at 11.41.24 PM.png" alt=""><figcaption><p>The Crystalvale Meditation Circle</p></figcaption></figure>

Each set of 10 levels has a focus rune associated with it. For levels 1 through 10, that rune is the **Shvās Rune**, and for levels 11-20, it is the **Moksha Rune**.

![Shvās Rune](https://dfk-hv.b-cdn.net/art-assets/rune.gif)

The rune cost for leveling increases each time a Hero moves to an odd-numbered level. So, a Level 1 Hero will pay one Shvās Rune to level up to Level 2, then two Shvās Runes to move from level 2 to 3 and again from 3 to 4, and so on. As a result, the maximum number of any single rune type needed in a single level-up is five. Leveling costs are summarized in a chart below.

After reaching level 10, the Hero will need an additional rune type (Moksha Rune) to level up further. However, as the Hero progresses from level 11 to 20, their Shvās Rune cost will decrease each time the Moksha Rune cost increases. The Shvās Rune cost will stop decreasing once it reaches 1 (meaning a Hero will always pay at least 1 rune of a type they have used before). This pattern continues with new rune types every ten levels.

![](../../../.gitbook/assets/Meditation\_Quest\_no\_pic-1.png)

The Power Token cost of leveling up is `0.1*currentLevel`.

The benefit of leveling up is an increase to a Hero’s stats. Excluding HP, MP, and Stamina, the game will roll twice for each stat to see if they increase. The first roll will be based on the Hero’s **Primary Stat Growth** percentage, which is primarily based on the Hero’s class. The second roll is based on the Hero’s **Secondary Stat Growth** percentage, which is primarily based on the Hero’s subclass. For each successful roll, the stat receives +1 to its value.

Primary Stat Growth and Secondary Stat Growth are important factors that the player can modify through the use of enhancement stones and summoner bonuses from spending additional Gaia’s Tears during the summoning process (more on this later).

See these [stat growth breakdown charts](https://docs.google.com/spreadsheets/d/1jfG6E6otW1V6ZLQycF5DumoBr\_LrpQaz7cTmDPpwV2s/edit#gid=655220330) for insight into the base growth rates of each class.

In addition to these two rolls per stat, the player will be given a choice of one stat to grant an extra +1 bonus. But that is not all, players also have a chance to seek Gaia’s blessing for two other stats. Gaia’s blessing has a 50% chance of increasing each of the selected stats.

<figure><img src="../../../.gitbook/assets/Screenshot 2023-04-11 at 11.49.02 PM.png" alt=""><figcaption><p>Stat Selection in Leveling</p></figcaption></figure>

In summary, when a Hero levels up the following will happen:&#x20;

1. The game will roll for each stat to increase based on the Hero's primary stat growth parameters and any bonuses provided by attunement crystals. Successful rolls receive +1 to that stat.&#x20;
2. The game will roll for each stat to increase based on the Hero's secondary stat growth parameters and any bonuses provided by attunement crystals. Successful rolls receive +1 to that stat.&#x20;
3. The game provides a +1 bonus to the stat selected by the player.&#x20;
4. The game will roll for the two stats selected to seek Gaia's blessing. Each has a 50% chance of success. Successful rolls receive +1 to that stat.

Stamina has a fixed growth rate for all Heroes. It increases by 1 every even level.

Lastly, HP and MP increases are calculated after other stat bonuses are applied. Each class has its own chances for small, regular, or large increases in HP and MP. For example, a Wizard has higher chances for large MP increases, but lower chances for large HP increases.
