---
icon: hands
---

# Unlock Protocol – memberships and access control

[Unlock](https://unlock-protocol.com/) is a protocol for creating **onchain memberships, tickets, and subscriptions as NFTs.**&#x20;

Unlock integrates Human Passport to add Sybil-resistant identity checks to memberships and tickets. The check happens through a **Passport Hook** that compares a buyer’s Passport Score to a threshold before the purchase goes through.

This page explains the flow for members and for organizers, with clear steps and troubleshooting. The terms Stamp and Passport Score are product names and are capitalized.

***

### Live Demo

{% embed url="https://x.com/HumnPassport/status/1983957555417379328" %}

***

### Quick glossary

* **Lock:** an Unlock smart contract that issues memberships or tickets.
* **Key:** the NFT a user receives when they buy or claim access from a Lock.
* **Passport Score:** a score derived from a user’s Stamps in Human Passport.
* **Stamp:** a verified credential that contributes to the Passport Score.
* **Passport Hook:** an Unlock contract hook that checks a buyer’s Passport Score against a threshold at checkout.

***

### For members: how to get access

1.  **Connect your wallet**

    Go to the organizer’s site or the Unlock checkout and connect the wallet you plan to use for purchase or claim.
2.  **Attempt the purchase or claim**

    Start the checkout for the membership or ticket (the Key). The Lock will run the Passport Hook during checkout.
3. **Score check happens automatically**

* If your Passport Score meets the threshold set by the organizer, the transaction is approved, and you receive the Key.
* If your Score is below the threshold, the transaction is blocked. You may see an error or a message that verification did not meet requirements. The organizer controls the threshold.

4.  **If you were blocked, improve your Score and retry**

    Open your [Human Passport](https://app.passport.xyz/), add or re-verify relevant Stamps, and wait for your [Passport Score](../common-questions/how-is-my-score-calculated.md) to update. Return to the checkout with the same wallet and try again. The hook will recheck your Score at checkout.

#### Member FAQs

*   **Where do I see the required Score?**

    Organizers choose the threshold. It is often stated on the event or membership page. If it is not visible, ask for the organizer’s support.
*   **My Score shows 0. What does that mean?**

    Usually, no Stamps have been added, or a Stamp verification was not completed. Open Passport, add Stamps, and re-run any failed ones.
*   **Do I need to use the same wallet everywhere?**

    Yes. The hook checks the wallet you use at checkout. If you verified Stamps for a different wallet, either switch to that wallet or rebuild your Score for the wallet you are using.
*   **Does the organizer see my personal data?**

    The hook compares your Score to a threshold at checkout. It exists to approve or block a purchase based on the Score, not to expose personal data. Human Passport does not store or share any personally identifiable information (PII).&#x20;

***

### For organizers: how to require a Passport Score

You can require a minimum Passport Score before a buyer can purchase or claim a Key from your Lock. The check runs at checkout via an Unlock Passport Hook you enable in the dashboard.

#### Set up the Passport Hook

1.  **Open your Lock in the Unlock dashboard**

    Go to the Lock you want to protect.
2.  **Go to “Hooks”**

    Find the Hooks section for that Lock.
3.  **Add the Passport Hook**

    Select the hook that checks Gitcoin Passport / Passport Score. This is the integration that enforces a Score threshold at checkout.
4.  **Set the Score threshold**

    Choose the minimum Passport Score a buyer must have for the purchase to succeed. Save your changes.
5. **Test the flow**
   * Use a wallet with a known Score above the threshold to confirm success.
   *   Use a wallet with a low or zero Score to confirm the hook blocks checkout.

       Adjust the threshold if needed based on the expected audience.

{% embed url="https://www.youtube.com/watch?v=I19WtTbamZM" %}

#### UX tips

*   **Tell buyers the requirement**

    State your Passport Score threshold near the buy or claim button, and link to guidance on how to improve a Score. This reduces support load.
*   **Offer a retry path**

    If checkout is blocked, tell buyers they can improve their Stamps and try again with the same wallet.
*   **Keep the copy neutral**

    Explain that the requirement helps keep tickets and memberships in human hands. Avoid jargon in user-facing text.

#### Operational notes

* The check runs at checkout via a contract hook, so it is part of the purchase path for memberships, tickets, and subscriptions. There is no need for separate scripts or manual reviews.
* The threshold is set per Lock by you as the lock manager. You can change it later if your audience changes.
* This helps prevent bot purchases, mass sign-ups, and ticket or membership hoarding.

***

### Troubleshooting

*   **Buyers say they are blocked even after adding Stamps**

    Ask them to confirm they used the same wallet they verified in Passport, and to wait for the Passport Score to update before retrying.
*   **False negatives at checkout**

    Lower the threshold temporarily and test again. If issues persist, collect affected wallet addresses and test their Scores directly in Passport, then report findings to support.
*   **High support volume around verification**

    Add a short guide on your site: how to open Passport, which Stamps are most impactful, and how long Score changes usually take to reflect. You can use our guide: [scoring-20-for-humans.md](../using-passport/scoring-20-for-humans.md "mention")

***

### Where to get help

* Unlock resources on the Passport Hook:
  * [Feature announcement on Unlock Protocol blog](https://unlock-protocol.com/blog/unlock-labs-feature-announcement--gitcoin-passport-hook)
  * [Explainer post on Paragraph](https://paragraph.com/@unlockprotocol/gitcoin-passport-hook)
* Human Passport documentation:
  * [Docs: Stamps, Scores, and integration guides](https://docs.passport.xyz)
* Community channels:
  * [Unlock Protocol Discord](http://discord.com/invite/ueJDH2qwRs)
  * [Human Passport Discord](https://discord.gg/humantech)
