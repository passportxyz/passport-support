---
description: >-
  This guide describes what's changing, why it's changing, and addresses some
  frequently asked questions.
hidden: true
noIndex: true
icon: scale-unbalanced-flip
---

# Stamp Re-weight: December 2024

[_Skip to the FAQs_](stamp-re-weight-december-2024.md#frequently-asked-questions-faqs)

## Strengthening Passport Humanity Verification: Upcoming Stamp Updates

The red team versus blue team battle continues, and we have seen more and more sophisticated Sybil attackers working to earn passing Passport scores. It is time for us to disrupt their automated habits and to make it harder for them to infiltrate your ecosystem. Fret not real humans, these changes should not increase the time it takes for you to prove your unique humanity though! &#x20;

A few times each year, we adjust our Passport Stamps (verifiable credentials) in response to evolving Sybil tactics. These refinements ensure we maintain the highest levels of security and authenticity without creating undue friction for genuine users. Read on for more details on what’s happening, and how it will impact both the humans who are proving their humanity, and the communities we are working to protect.

### What’s Changing and **Why**

1. **A Gradual Rollout of Adjustments for existing Passport holders**\
   For users, some current scores will stay intact until the Stamps would naturally expire. This means Stamp values will reflect their updated scoring naturally as the old Stamps expire in users’ Passports. This gives everyone ample time to adapt without interruption. For new users, these new Stamp weights will be used by default.
2. **Consolidating Onchain Activity Signals**\
   We’re immediately removing the zkSync Stamp, and making some big changes to the ETH Activity Stamp. This new ETH Activity Stamp draws upon activity across [multiple Layer 2 (L2) networks](../model-based-detection/guide-to-model-based-detection.md), beyond just ETH Mainnet and zkSync activity, resulting in a stronger, more holistic measure of genuine user participation.
3. **Fine-Tuning Binance and Coinbase points**\
   Over the past year, Passport has added multiple KYC Stamps with high points. While adding optionality is important, this also enabled Sybils to build up a passing score with multiple accounts more easily. Because of this and other challenges that we’ve seen with KYC user experiences, we’re reducing the points for the Binance and Coinbase Stamps for the time being.&#x20;
4. **Introducing a New Phone Verification Stamp from Zeronym**\
   To offer a more accessible option—particularly for crypto newcomers—we’re adding a phone number verification Stamp powered by Zeronym. This user-friendly, privacy-focused option helps beginners build up their Passport scores quickly and safely, easing the early stages of their journey.
5. **Rebalancing Points Across all Stamps**\
   While we’re reducing points in a few areas, we’re simultaneously redistributing points to Stamps that have proven both Sybil-resistant and easy to complete. This ensures that users always have meaningful, straightforward ways to strengthen their Passports while giving partners confidence that participants are truly human.

### What This Means for You

These adjustments deliver a more reliable, secure, and user-friendly verification process. By refining our Stamps to better reflect real human behavior, we’re ensuring that Human Passport remains a trusted solution for our partners and a smooth, welcoming experience for real humans. As we continue to monitor emerging tactics and adapt accordingly, our guiding principle remains the same: make it simple for real people to prove their humanity and participate in the crypto ecosystem with confidence.



***

## Frequently Asked Questions (FAQs)

**Will my score decrease as part of this change?**

For this Stamp reweight, the Stamps that are being adjusted and that you have verified will not see any changes until they expire (90 days after verifying)&#x20;

Your score may fluctuate as part of this update, but not until the affected Stamps that you’ve verified expire. Once the zkSync, Trusta, Coinbase, Binance, and Eth Activity Stamps expire within your Passport, zkSync and Trusta will be fully retired, and you will be able to reverify the others with the updated score weights. \


#### What is the new criteria for the ETH Activity Stamp?

While we don’t plan to make the exact criteria public for the ETH activity Stamp, we can provide some key details:

* This Stamp uses several supervised machine learning models to review transaction history and identify if the activity more closely resembles Sybil or human behavior.
* As of this Stamp reweight, the ETH activity Stamp will look at transaction history across not only ETH L1 mainnet, but also Arbitrum, Optimism, Polygon, and zkSync (which is why the zkSync Stamp is being retired).
* Each network’s model comes with a different set of criteria that is customized to that network. Some models have as many as 50+ different features that they look for.&#x20;
* OpenBlock recently ranked our Sybil detection models as the best-in-class.&#x20;

There are no plans to release the exact criteria for the ETH activity Stamp. There are a couple of reasons for this:

1. Releasing the secret sauce will enable Sybils and other bad actors from being able to more quickly game the system.&#x20;
2. We might make some quick adjustments here and there to the features that make up these models based on changes to Sybil behavior.&#x20;

If you can’t verify this Stamp, don’t worry. We have plenty of other Stamps that you might be able to verify.&#x20;

#### Why is the Trusta Stamp being removed?

The new ETH Activity Stamp provides a very similar signal as the Trusta Stamp, so we decided to reduce complexity and rely on models that we can actively adjust as we see Sybil behavior change. \


**Why is the zkSync Stamp being removed?**

We are merging this Stamp into the ETH Activity Stamp. Previously, the ETH Activity Stamp only looked at ETH L1 transaction history. With the latest update, the ETH Activity Stamp now looks at the transaction history across ETH L1, zkSync, Arbitrum, Optimism, and Polygon, providing a much more complete picture of a user’s onchain activity.&#x20;

#### Why are the scores changing for the Binance/Coinbase Stamps?

Over the past year, Passport has added multiple KYC Stamps with high points, including Holonym, Coinbase, and Binance.&#x20;

While adding optionality is important, this also enabled Sybils to build up a passing score with multiple accounts more easily. Because of this and other challenges that we’ve seen with KYC user experiences, we’re reducing the points for the Binance and Coinbase Stamps for the time being.&#x20;

More specifically, Coinbase and Binance have been the cause of 80% of our support requests within the last several months, pointing towards challenges with the user flow between the Passport app and their ID verification systems. We hope to continue to partner with both parties to make further improvements to this flow in the future.

\
**What are the Coinbase and Binance “Retired” credentials?**

For those users who had Coinbase and/or Binance verified at the time of the score weight adjustment, you will see two different credentials within those Stamps.&#x20;

1. One will be labeled as “retired”. This is the credential that is grandfathered in. When it expires, it will retire and disappear.&#x20;
2. The other is the new credential with the new score weight.&#x20;

If you still have a retired Stamp, we recommend that you keep that Stamp until it expires, and then verify the new Stamp. \


#### Are you removing points entirely?

For any of the credentials that are being removed or reduced, we’ll be reapplying those points to other Stamps.&#x20;

You can review the new score weights at the following link:

[Passport's Stamp weights](../stamps/how-is-gitcoin-passports-score-calculated.md)\


**Is Passport pay-to-play?**

It is not.&#x20;

Passport is a public good that continues to provide an identity verification system that is easy and cheap for all users, while also providing a strong human/Sybil signal for our 100+ partners who have relied on Passport’s tools to protect rewards, governance, and other community programs. \


**How do I build up a score of 20?**

We created a guide that lists all of our free Stamps, Stamps that are great for crypto beginners, and other groupings of Stamps to help you out:

[Scoring 20, for humans](https://support.passport.xyz/passport-knowledge-base/using-passport/scoring-20-for-humans#building-up-a-score-with-free-stamps)\


**How can I request for a new Stamp to be added?**

We would love to learn more about Stamps that may be high quality signals to help real humans prove their humanity. We are exploring a number of other Stamps, and would love your ideas as well.&#x20;

Open a [support ticket](../need-support.md) and let us know.\
