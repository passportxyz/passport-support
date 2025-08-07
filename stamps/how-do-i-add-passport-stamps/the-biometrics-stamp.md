---
description: Verify your uniqueness using facial biometrics, powered by human.tech.
---

# ☑️ The Biometrics Stamp



The Biometric Stamp by human.tech enables secure facial verification, including 3D liveness and duplicate checks, as part of Human Passport’s Proof of Humanity system. Upon successful verification, users mint a Soulbound Token (SBT) as proof of completing the biometric check.

**Cost:** \~$5&#x20;

**Time:** \~5 minutes

**Stamp validity:** 90 days (free renewal) / 1 year SBT (paid renewal)

**Device recommendation:** Use a mobile device for a smoother scan

## Prerequisites

* A smartphone or desktop device with a front-facing camera and internet access
* A unique human face (yours)
* An EVM-compatible wallet with at least $6 to cover payment and gas fees
* A Human Passport account

## Networks available for payment

* Ethereum
* Optimism
* Avalanche
* Base

## Important considerations:

* Uses 3D liveness detection by FaceTec to prevent spoofing attempts
* Biometric data is processed securely and not stored in raw form



## Step-by-Step Guide

{% embed url="https://www.youtube.com/watch?v=UyE5Nv81l8g" %}

{% stepper %}
{% step %}
### Visit the Issuance Page

Go to the [credential issuance page](https://silksecure.net/holonym/diff-wallet/biometrics).

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Connect Your Wallet

Connect your wallet on one of the supported networks: Ethereum, Optimism, Avalanche, or Base. Make sure you have at least \~$6 in your wallet to cover the payment and gas fees later (amount may vary by network).&#x20;
{% endstep %}

{% step %}
### Start Verification

There are three ways to complete the scan, depending on your device:

* **Option 1 (Desktop):**&#x20;
  * Click “Start Biometric Scan” to verify directly on desktop.
  * **Note:** Desktop verification may fail more often. If you run into issues, use Option 2.
* **Option 2 (Desktop + Mobile - Recommended):**&#x20;
  * Scan the QR code shown on your screen using your phone. Continue the scan on your mobile device.
* **Option 3 (Mobile):**&#x20;
  * Tap “Start Biometric Scan” and follow the prompts.

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Face Scan & Liveness Detection

Follow the instructions:\
– Fit your face into the oval frame\
– Move closer\
– Stay still for a few seconds

<figure><img src="../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

Wait till the system performs a deduplication check to ensure your biometric signature is unique in the database.

<figure><img src="../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Complete Payment**

After successful verification, click “Mint SBT.”

Select your network and confirm the payment in your wallet. Fees are paid in the native token of the selected chain.

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Mint the Soulbound Token on Optimism (SBT)**

Once payment is complete, you’ll be prompted to mint the SBT.&#x20;

We support minting on **Optimism** – it’s EVM-compatible and natively supported by the Passport app. Minting on other chains like Sui or Stellar is possible, but not currently usable with Human Passport.

{% hint style="info" %}
**Note:** Choose the wallet linked to your Passport as your minting wallet! Once the SBT has been issued, it cannot be transferred.
{% endhint %}
{% endstep %}

{% step %}
<figure><img src="../../.gitbook/assets/image (43).png" alt=""><figcaption></figcaption></figure>

### **Claim the Stamp in the Passport App**

Return to the [Passport app](https://app.passport.xyz/), connect your wallet, and click “Check Eligibility” to claim the Biometrics Stamp.

{% hint style="info" %}
**Note:** Every 90 days, your Stamp will be automatically reissued without extra payment. After one year, when the Biometric proof expires, you'll be asked to redo the verification process. &#x20;
{% endhint %}

<figure><img src="../../.gitbook/assets/image (44).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Troubleshooting

If you run into any issues, please[ reach out to support](https://support.passport.xyz/passport-knowledge-base/need-support).&#x20;

##

## FAQ

<details>

<summary>What's the difference between a 90-day expiry (Stamp) and a 1-year expiry (SBT)?</summary>

All Passport Stamps have an expiry time set up. Typically, it's 90 days. That's to allow users to change wallets, in case they lose access to old ones.\
**Renewal after 90 days:** The renewal process is simple and free - you just need to click one button. \
\
The SBT (underlying proof for this Stamp) has a validity of 1 year on the provider's side (human.tech). The limit is set up for similar reasons - to prevent identity fraud and to allow for changing the wallet in the future. \
**Renewal process after 1 year:** Once the SBT expires, you will have to go through the full verification process again.&#x20;

</details>

<details>

<summary>Why does the Stamp expire after 90 days?</summary>

This helps keep the credential fresh and defensible, while not making users verify too often.\
\
Renewal happens with one click — no extra steps or fees unless your proof expires.

</details>

<details>

<summary>Why does SBT expire after 1 year?</summary>

The 1-year expiry helps prevent abuse. It ensures no one can indefinitely reuse someone else’s biometric data, keeping your identity safer and the system more trustworthy for everyone.

It’s a tradeoff: short enough to reduce the risk if someone is ever forced to verify, but still long enough that real users don’t have to repeat it too often.

</details>

<details>

<summary>Should I complete the face scan on desktop or mobile?</summary>

Even if you start your verification on desktop, we recommend using a mobile device to complete the liveness check. For various reasons, mobile verification has a higher rate of success compared to desktop verification.&#x20;

</details>

<details>

<summary>Can I use a different wallet to mint and another to claim the Stamp?</summary>

No. The wallet you mint the SBT with must be the same one you connect to Passport to claim the Stamp.

</details>

<details>

<summary>Can I transfer the SBT to another wallet?</summary>

Nope. The SBT is soulbound — it’s non-transferable by design. You’ll need to mint it from the wallet you want to use with Passport.

However, after the SBT expires in 1 year, you can verify again using a different wallet to mint SBT.&#x20;

</details>

<details>

<summary>Why do I have to pay?</summary>

The fee covers the cost of running secure, privacy-preserving biometric verification and minting onchain. It helps ensure the system stays fair and bot-resistant.

</details>

<details>

<summary>What happens if I fail the face scan? Can I try again?</summary>

Yes, you can retry. If you’re consistently having trouble, try switching from desktop to mobile, or contact support.

</details>

<details>

<summary>Why do I need to scan my face at all?</summary>

Facial biometrics are a strong and accessible way to confirm you’re a unique human. The process by human.tech is privacy-first, thanks to zero-knowledge proofs.

However, it's totally fine to opt out!&#x20;

Human Passport offers many other Stamps that can help you pass the Humanity threshold (typically the score of 20). You are free to use only the Stamps you want.&#x20;

</details>

<details>

<summary>What chains can I pay on? Which one should I choose?</summary>

Supported networks: Ethereum, Optimism, Avalanche, and Base. All are equally fine.&#x20;

</details>

<details>

<summary>Do I need to keep my SBT forever? What if I change wallet?</summary>

The SBT lasts 1 year. After that, you’ll need to re-verify to keep your Biometric Stamp active. You can re-verify with another wallet.&#x20;

</details>

<details>

<summary>What if I don’t have $5 in my wallet? Can I still verify?</summary>

Unfortunately, no — you’ll need funds to cover the biometric verification fee and network gas.

</details>

<details>

<summary>What chains can I mint on? Which one should I choose?</summary>

To use SBT with Human Passport, you’ll need to mint on **Optimism** — it’s the only EVM-compatible option supported by the Passport app.

</details>

<details>

<summary>My wallet got hacked, can I move my Stamps to a new wallet?</summary>

First of all, we're sorry about your situation. You will be able to claim your Stamps from your new wallet after the proofs expire. For the Biometrics Stamps, the proof expiry is set to 1 year due to the SBT expiry date. For many other Stamps, you will be able to reclaim them after the 90-day expiry period.&#x20;

</details>



