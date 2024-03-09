---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Power-Ups

## **What are Power-Ups?**

**Power-Ups** are a collection of **in-game enhancements** that are available to players that hold [governance tokens](./). Each Power-Up has a specific c/sJEWEL amount that must be allocated to it in order to activate its benefits. Some **premium features** will also require Power-Up allocations prior to access. Power-Ups do not consume c/sJEWEL nor the JEWEL used to produce the c/sJEWEL, but will only remain active if you continue to hold the necessary balance required to activate them.

### **Power-Up Types**

There are currently three primary Power-Up types:

* **Type 1 Power-Ups:** These Power-Ups are the simplest type, as they provide a single tier of benefits that is activated by allocating the required amount of c/sJEWEL. Cancelling this power-up will remove its benefits until it is re-activated, after waiting the necessary hold time.
* **Type 2 Power-Ups:** These Power-Ups present the player with multiple tier options with varying c/sJEWEL allocation requirements for each tier. Once a tier is selected, the player can increase to a higher tier at any time but not decrease tiers without cancelling the Power-Up first.
* **Type 3 Power-Ups:** These Power-Ups provide a variable number of charges based on the number of Heroes a player owns. Each charge contains multiple Hero slots. There is a fixed c/sJEWEL allocation required for every charge of these Power-Ups. Once activated, the player will assign their Heroes up to the maximum charges and total allotted Hero slots. The player may remove Heroes from the Power-Up, but will have to wait until after the specified slot hold time before assigning another. All Heroes must be unassigned from the Power-Up before it can be cancelled. Additional charges can be added but not removed without first cancelling the Power-Up.

### **Power-Up Requirements**

Each Power-Up has a **Minimum Lock Time** associated with it. In order to activate a Power-Up, players must have a c/sJEWEL lock time higher than the minimum lock time specified by each Power-Up, as well as ensure that it remains above that minimum time. If the player's c/sJEWEL lock time drops below the minimum lock time of a Power-Up, the Power-Up will be cancelled.

Players must also maintain an amount of c/sJEWEL equal to the amount they have allocated to Power-Ups. Calling the [Emergency Withdraw](./#withdrawing) function will cancel all Power-Ups.&#x20;

### Cancelling Power-Ups

When a Power-Up is cancelled, the c/sJEWEL allocated to it will not be immediately available for use elsewhere. Instead, each Power-Up has a **Cancellation Hold Time** that indicates how long after cancelling the Power-Up the c/sJEWEL will be available again for use elsewhere.

A **Hero Slot Hold Time** of the same duration as the Cancellation Hold Time also goes into effect when removing Heroes from a Type 3 Power-Up. Players must wait this amount of time before re-assigning those slots to other Heroes.

## Available Power-Ups

<table data-view="cards" data-full-width="true"><thead><tr><th>Name</th><th>Cost</th><th>Description</th><th>Minimum Lock Time</th><th>Cancellation Hold Time</th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td><strong>Quick Study</strong></td><td>30 per 6 Heroes</td><td>Grants a 15% bonus to experience gained from questing to each assigned Hero.</td><td>7 days</td><td>1 day</td><td><a href="../../.gitbook/assets/quick-study.png">quick-study.png</a></td></tr><tr><td><strong>Rapid Renewal</strong></td><td>20 per 6 Heroes</td><td>Reduces the stamina recharge rate of assigned Heroes by an additional 3 seconds per Hero level.</td><td>7 days</td><td>1 day</td><td><a href="../../.gitbook/assets/rapid-renewal.png">rapid-renewal.png</a></td></tr><tr><td><strong>Backstage Pass</strong></td><td>50</td><td>Grants access to the Combat Testing Grounds.</td><td>7 days</td><td>1 day</td><td><a href="../../.gitbook/assets/backstage_pass.png">backstage_pass.png</a></td></tr><tr><td><strong>Premium Provisions</strong></td><td>500</td><td>Increases the duration of well-fed time gained from Regular Pet Treats by 1 day and Premium Pet Treats by 4 days</td><td>14 days</td><td>14 days</td><td><a href="../../.gitbook/assets/premium-provisions.png">premium-provisions.png</a></td></tr><tr><td><strong>Master Merchant</strong></td><td>500 / 5000</td><td>Provides a 0.1% / 0.5% discount on Bazaar Trading Fees</td><td>7 days</td><td>1 day</td><td><a href="../../.gitbook/assets/master-merchant.png">master-merchant.png</a></td></tr><tr><td><strong>Thrifty</strong></td><td>500 / 1500</td><td>Provides a chance to randomly recover used items after combat</td><td>7 days</td><td>1 day</td><td><a href="../../.gitbook/assets/thrifty.png">thrifty.png</a></td></tr></tbody></table>

