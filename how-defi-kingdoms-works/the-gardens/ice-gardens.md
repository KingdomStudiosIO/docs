# Ice Gardens

### Issuance Schedule

The issuance of CRYSTAL is scheduled to change during each consecutive period of time, which we refer to as an Epoch. Each Epoch is exactly one week long and begins at 20:00 EST on the date listed in the table below:

|  Epoch |     Date     | CRYSTAL/block | CRYSTAL/minute |
| :----: | :----------: | :-----------: | :------------: |
|    1   | Mar 30, 2022 |       32      |       960      |
|    2   |  Apr 6, 2022 |       24      |       720      |
|    3   | Apr 13, 2022 |       20      |       600      |
|    4   | Apr 20, 2022 |       16      |       480      |
|    5   | Apr 27, 2022 |       14      |       420      |
|    6   |  May 4, 2022 |       12      |       360      |
|    7   | May 11, 2022 |       10      |       300      |
|    8   | May 18, 2022 |       10      |       300      |
|    9   | May 25, 2022 |       8       |       240      |
|   10   |  Jun 1, 2022 |       8       |       240      |
|   11   |  Jun 8, 2022 |       6       |       180      |
|   12   | Jun 15, 2022 |       6       |       180      |
|   13   | Jun 22, 2022 |       4       |       120      |
|   14   | Jun 29, 2022 |       4       |       120      |
|   15   |  Jul 6, 2022 |       4       |       120      |
|   16   | Jul 13, 2022 |       4       |       120      |
|   17   | Jul 20, 2022 |       3       |       90       |
|   18   | Jul 27, 2022 |       3       |       90       |
|   19   |  Aug 3, 2022 |       3       |       90       |
|   20   | Aug 10, 2022 |       3       |       90       |
| 21-100 | Aug 17, 2022 |       2       |       60       |
|  101+  | Feb 28, 2024 |       1       |       30       |

### Locking

Claimed locked CRYSTAL will remain March 22, 2023**,** which marks the end of Epoch 51. Locked rewards will begin unlocking ratably at that time over the following 52 Epochs.&#x20;

The percentage of CRYSTAL that is unlocked began at 5% in Epoch 1 and increases by 2% each Epoch. Unclaimed rewards continue to unlock on this schedule until claiming, at which time unlocked rewards go directly into the player's wallet and locked rewards become fully locked until the end of Epoch 51.

### **Garden Staking Deposit and Withdrawal Fees**

**There are no deposit fees for staking LP tokens in the Gardens.** To protect against flash loans and pump and dumps, we do implement withdrawal fees for withdrawing staked LP tokens. Each withdrawal resets the fee timer. The withdrawal fees are listed below:

* **0.01%** fee if a user withdraws after **4 Epochs**
* **0.25%** fee if a user withdraws after **2 Epochs but before 4 Epochs**
* **0.5%** fee if a user withdraws after **5 days but before 2 Epochs**
* **1%** fee if a user withdraws under **5 days.**&#x20;
* **2%** fee if a user withdraws under **3 days.**&#x20;
* **4%** fee if a user withdraws under **24 hours.**&#x20;
* **8%** fee if a user withdraws under **1 hour.**&#x20;
* **25%** slashing fee if a user withdraws **during the same block.**
