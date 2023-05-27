# JEWEL Gardens

{% hint style="danger" %}
In accordance with the [community governance vote](https://vote.defikingdoms.com/#/proposal/0x2a83ec79bf88a5d8170b831b4c941a934e47ca0c569a40bb8d240666978b73e6) adopted on 9/1/2022, **JEWEL emissions on Harmony have ended and locked JEWEL will never unlock.**

For details on these changes, please read about the project's [updated tokenomics](../power-tokens/jewel-token.md#updated-tokenomics).
{% endhint %}

{% hint style="info" %}
On account of the above, the information below about the original Serendale JEWEL Gardens is no longer applicable, but has been left here for reference.
{% endhint %}

### Issuance Schedule

The issuance of JEWEL as rewards for staking LP tokens in the Garden is scheduled to change during each consecutive period of time, which we refer to as an Epoch. Each Epoch is 302,400 blocks on the Harmony Blockchain, and the length of each Epoch depends on the average block speed on Harmony. Epochs were calculated to 302,400 blocks so that each Epoch would equal one week assuming a speed of 2 seconds per block on the Harmony Blockchain. However, if block speeds are longer than 2 seconds per block on average, an Epoch will last longer than a week.

<table><thead><tr><th width="150" align="center">Epoch</th><th width="150" align="center">Block</th><th width="150" align="center">JEWEL/block</th><th align="center">JEWEL/minute</th></tr></thead><tbody><tr><td align="center">1</td><td align="center">16,350,367</td><td align="center">256</td><td align="center">7680</td></tr><tr><td align="center">2</td><td align="center">16,652,767</td><td align="center">128</td><td align="center">3840</td></tr><tr><td align="center">3</td><td align="center">16,955,167</td><td align="center">96</td><td align="center">2880</td></tr><tr><td align="center">4</td><td align="center">17,257,567</td><td align="center">64</td><td align="center">1920</td></tr><tr><td align="center">5</td><td align="center">17,559,967</td><td align="center">56</td><td align="center">1680</td></tr><tr><td align="center">6</td><td align="center">17,862,367</td><td align="center">48</td><td align="center">1440</td></tr><tr><td align="center">7</td><td align="center">18,164,767</td><td align="center">40</td><td align="center">1200</td></tr><tr><td align="center">8</td><td align="center">18,467,167</td><td align="center">32</td><td align="center">960</td></tr><tr><td align="center">9</td><td align="center">18,769,567</td><td align="center">28</td><td align="center">840</td></tr><tr><td align="center">10</td><td align="center">19,071,967</td><td align="center">24</td><td align="center">720</td></tr><tr><td align="center">11</td><td align="center">19,374,367</td><td align="center">20</td><td align="center">600</td></tr><tr><td align="center">12</td><td align="center">19,676,767</td><td align="center">16</td><td align="center">480</td></tr><tr><td align="center">13</td><td align="center">19,979,167</td><td align="center">15</td><td align="center">450</td></tr><tr><td align="center">14</td><td align="center">20,281,567</td><td align="center">14</td><td align="center">420</td></tr><tr><td align="center">15</td><td align="center">20,583,967</td><td align="center">13</td><td align="center">390</td></tr><tr><td align="center">16</td><td align="center">20,886,367</td><td align="center">12</td><td align="center">360</td></tr><tr><td align="center">17</td><td align="center">21,188,767</td><td align="center">11</td><td align="center">330</td></tr><tr><td align="center">18</td><td align="center">21,491,167</td><td align="center">10</td><td align="center">300</td></tr><tr><td align="center">19</td><td align="center">21,793,567</td><td align="center">9</td><td align="center">270</td></tr><tr><td align="center">20-35</td><td align="center">22,095,967</td><td align="center">8</td><td align="center">240</td></tr><tr><td align="center">36+</td><td align="center">26,934,367</td><td align="center">4</td><td align="center">120</td></tr></tbody></table>

_\*Listed emissions are spread out across all gardens. See the Seed Box for pool-specific emission rates._

The current block number is shown in the bottom right of the game screen, or players may visit the[ Harmony Blockchain Explorer](https://explorer.harmony.one/) to see the current Harmony block. Please note that Harmony block speeds fluctuate and should be viewed on an average (i.e. daily or weekly basis) when trying to plan your Garden farming strategies.

### Locking

Claimed locked JEWEL will remain **locked until block 31,772,767,** which marks the end of Epoch 51. Locked rewards will begin unlocking ratably at that time over the following 52 Epochs. At the time of writing, unlocking is estimated to begin in Q3 2022; however, network latency has already extended the duration of most Epochs and it is not possible to determine a specific date when this block will be reached.

The percentage of JEWEL that is unlocked when claimed began at 5% in Epoch 1 and increases by 2% each Epoch. Unclaimed rewards continue to unlock on this schedule until claiming, at which time unlocked rewards go directly into the player's wallet and locked rewards become fully locked until the end of Epoch 51.

### Locking Model - Simplified Examples

Below are two simplified examples that show how the locking model works. For the sake of simplicity, **the examples assume no compounding** of unlocked claimed rewards into additional LP positions and that a player earned 100 JEWEL in Garden rewards during Epoch 1, 50 JEWEL in Epoch 2 and so on to reflect the reduced JEWEL emission per Epoch. In both scenarios, 301.6 JEWEL is earned, but the amount unlocked versus locked is different. This locking model provides players the opportunity to choose a strategy that suits their style and risk appetite.

**Illustrative Example A**: Rewards earned during each Epoch are claimed during each Epoch (and not compounded).

* _10 Epoch Summary_:
  * Total unlocked JEWEL: **29.8** JEWEL
  * Total locked JEWEL: **271.8** JEWEL (inaccessible until after Epoch 51 unless unlocked earlier via Heroes)
  * Total rewards: **301.6** JEWEL
  * _Lower unlocked JEWEL over the sample period, but allows for use of and potential compounding of unlocked JEWEL during sample period, which could result in more unlocked JEWEL than not claiming over the same period depending on what you choose to do with such unlocked claimed rewards. The choice is yours!_

|   Epoch  | Unlocked at time of claiming | Locked at time of claiming | Example JEWEL Earned during Epoch | Unlocked Claimed during Epoch | Locked Claimed During Epoch | Unlocked Cumulative | Locked Cumulative |
| :------: | :--------------------------: | :------------------------: | :-------------------------------: | :---------------------------: | :-------------------------: | :-----------------: | :---------------: |
|  Epoch 1 |              5%              |             95%            |               100.0               |              5.0              |             95.0            |         5.0         |        95.0       |
|  Epoch 2 |              7%              |             93%            |                50.0               |              3.5              |             46.5            |         8.5         |       141.5       |
|  Epoch 3 |              9%              |             91%            |                37.5               |              3.4              |             34.1            |         11.9        |       175.6       |
|  Epoch 4 |              11%             |             89%            |                25.0               |              2.8              |             22.3            |         14.6        |       197.9       |
|  Epoch 5 |              13%             |             87%            |                21.9               |              2.8              |             19.0            |         17.5        |       216.9       |
|  Epoch 6 |              15%             |             85%            |                18.8               |              2.8              |             15.9            |         20.3        |       232.8       |
|  Epoch 7 |              17%             |             83%            |                15.6               |              2.7              |             13.0            |         22.9        |       245.8       |
|  Epoch 8 |              19%             |             81%            |                12.5               |              2.4              |             10.1            |         25.3        |       255.9       |
|  Epoch 9 |              21%             |             79%            |                10.9               |              2.3              |             8.6             |         27.6        |       264.6       |
| Epoch 10 |              23%             |             77%            |                9.4                |              2.2              |             7.2             |         29.8        |       271.8       |

**Illustrative Example B**: Rewards are not claimed until the end of Epoch 10.

* 10 Epoch Summary:
  * Total unlocked JEWEL: **69.4** JEWEL
  * Total locked JEWEL: **232.2** JEWEL (inaccessible until after Epoch 51 unless unlocked earlier via Heroes)
  * Total rewards: **301.6** JEWEL
  * _Higher unlocked JEWEL count by the end of sample period, but unable to use or compound unlocked Jewel during sample period._

|   Epoch  | Unlocked at time of claiming | Locked at time of claiming | Example JEWEL Earned during Epoch | Cumulative UNCLAIMED Unlocked | Cumulative UNCLAIMED Locked | Cumulative CLAIMED Unlocked | Cumulative CLAIMED Locked |
| :------: | :--------------------------: | :------------------------: | :-------------------------------: | :---------------------------: | :-------------------------: | :-------------------------: | :-----------------------: |
|  Epoch 1 |              5%              |             95%            |               100.0               |              5.0              |             95.0            |             0.0             |            0.0            |
|  Epoch 2 |              7%              |             93%            |                50.0               |              10.5             |            139.5            |             0.0             |            0.0            |
|  Epoch 3 |              9%              |             91%            |                37.5               |              16.9             |            170.6            |             0.0             |            0.0            |
|  Epoch 4 |              11%             |             89%            |                25.0               |              23.4             |            189.1            |             0.0             |            0.0            |
|  Epoch 5 |              13%             |             87%            |                21.9               |              30.5             |            203.9            |             0.0             |            0.0            |
|  Epoch 6 |              15%             |             85%            |                18.8               |              38.0             |            215.2            |             0.0             |            0.0            |
|  Epoch 7 |              17%             |             83%            |                15.6               |              45.7             |            223.1            |             0.0             |            0.0            |
|  Epoch 8 |              19%             |             81%            |                12.5               |              53.4             |            227.8            |             0.0             |            0.0            |
|  Epoch 9 |              21%             |             79%            |                10.9               |              61.4             |            230.8            |             0.0             |            0.0            |
| Epoch 10 |              23%             |             77%            |                9.4                |              69.4             |            232.2            |             69.4            |           232.2           |

