---
description: 5-minute process
---

# ☑️ The Proof of Clean Hands Stamp

Proof of Clean Hands (PoCH) is a privacy-preserving way to prove you are not present on any sanction lists and are not a politically exposed person. This guide will walk you step by step through the Proof of Clean Hands Stamp issuance process.&#x20;

**Cost:** \~$5&#x20;

**Time:** \~5 minutes

**Validity**: 90 days Stamp / 1 year PoCH<br>

## Prerequisites

* A smartphone with a camera and the internet
* A current and valid government ID
* An Ethereum wallet with at least \~$5 on the desired network to cover both payment and gas fees
* A Human Passport account

## Available Networks

* Ethereum
* Optimism
* Avalanche
* Base

## Step-by-Step Guide

#### **Step 1: Visit the issuance page**

Go to the [credential issuance page](https://silksecure.net/holonym/diff-wallet/clean-hands).

**Note:** This attestation requires you to prove your identity first. If you’ve verified your identity with Holonym before, you will be redirected straight to **step 5**.&#x20;

#### **Step 2: Connect your wallet**

Connect your wallet to a supported network (Ethereum, Optimism, Avalanche, or Base). Make sure your balance is greater than $5 to cover both the payment and gas fees, which vary by network.&#x20;

#### **Step 3: Scan QR code (desktop users)**&#x20;

Click "Verify now." If you’re on a desktop, scan the QR code displayed on your screen to use your mobile device’s camera. If you’re using a mobile device, continue directly with the camera.

#### **Step 4: Verify your identity with your government ID**

Follow the verification flow that includes uploading document photos and performing a liveness check. Some countries are excluded from verification - see details [here](https://documentation.onfido.com/guide/supported-applicant-countries/).&#x20;

#### **Step 5: Generate Proof of Clean Hands**

Click “Verify Now”, then “Continue”. Human ID will verify that you are not on any sanctions lists and are not a politically exposed person. Wait a few seconds until verification is complete.&#x20;

#### **Step 6: Mint the Soulbound Token (SBT)**&#x20;

After a successful sanctions check, mint the SBT to the wallet linked to your Passport. Click “Continue”, pay the $5 fee plus gas, and confirm the payment in your wallet. The fee is to be paid in the native currency of the chain on which you decided to mint.&#x20;

**Note:** Once the SBT has been issued, it cannot be transferred.

#### **Step 7: Verify the Stamp in the Passport app**

Return to the Passport app, connect your wallet, and click “Check Eligibility” to add the Proof of Clean Hands Stamp.

After 90 days, your Stamp will be automatically reissued without extra payment. After one year, when the Proof of Clean Hands expires, you will have to redo the verification process. &#x20;

## FAQs

#### What is Proof of Clean Hands (PoCH)?

Proof of Clean Hands (PoCH) is a verification flow that allows a user to prove they passed identity and sanctions checks without disclosing their personal information to applications.

It is designed for use cases that require both:

* strong privacy guarantees for users, and
* the ability to meet compliance or accountability requirements when necessary.

***

#### What does a PoCH Stamp represent?

A PoCH Stamp represents that:

* The user completed an identity verification process.
* The user was screened against supported sanctions and watchlists at the time of verification.
* A valid cryptographic proof of this verification was presented and accepted.
* The result is bound to a specific wallet address.<br>

The PoCH Stamp does not contain personal data and does not encode identity attributes such as name or date of birth.

***

#### What information do applications see?

Applications that integrate PoCH can verify:

* That a wallet holds a valid PoCH attestation.
* That the attestation is not expired or revoked.
* Optional public metadata, such as expiry timestamps or uniqueness signals.

Applications do not receive:

* Name, date of birth, or document details.
* Government ID numbers.
* Raw KYC data.
* Encrypted identity fields.
* Any ability to decrypt or request disclosure.

***

#### What information is never shared with applications?

Applications never see:

* Personal identity data.
* Sanctions screening inputs.
* Biometric data.
* OAuth login credentials.
* Any plaintext or encrypted identity fields.

All personal data remains outside the application’s control.

***

#### How does PoCH preserve privacy?

PoCH relies on a combination of architectural and cryptographic measures:

* Zero-knowledge proofs are used so verification results can be proven without revealing underlying data.
* Cryptographic hashing is used to avoid storing raw identifiers and to support uniqueness checks.
* Separation of roles ensures that verification, storage, and disclosure control are handled by different components.
* No central identity database is created for applications to query or access.

As a result, applications can verify eligibility without collecting or storing personal data.

***

#### What role do zero-knowledge proofs play?

Zero-knowledge proofs allow the user to prove statements such as:

* “I completed the required identity and sanctions checks.”
* “The verification was issued by an authorised issuer.”
* “This proof is correctly bound to my wallet address.”

These proofs reveal only the validity of the statement, not the underlying identity data used to generate it.

***

#### Is personal data stored as part of PoCH?

PoCH is designed so that verification does not require applications to store personal data.

In the PoCH flow, identity attributes may be:

* processed transiently for verification, and
* represented cryptographically (for example via proofs or encrypted representations) as required for the protocol to function.

Plaintext personal data is not made available to applications and is not stored in a way that allows routine access.

***

#### Can identity data ever be disclosed?

Disclosure is not the default and does not occur during normal use.

In PoCH, disclosure is only possible if:

* the user explicitly agreed to predefined terms covering such disclosure, and
* specific contractual and on-chain conditions are met.

Any potential disclosure is:

* conditional,
* rate-limited,
* and governed by predefined rules.

Disclosure is never initiated by applications.

***

#### Who controls disclosure or decryption?

No single party has unilateral control.

Disclosure requires coordination between:

* authorised roles defined by the protocol,
* and cryptographic enforcement mechanisms that prevent unilateral access.

This design ensures that no single component or operator can independently access identity information.

***

#### What is the PoCH SBT?

The PoCH SBT is an on-chain attestation issued to a wallet after a valid PoCH proof is verified.

The SBT:

* Contains no personal data.
* Is untransferable.
* Is what applications check to verify PoCH status.
* Is time-bound (it can expire).
* May be revoked under defined conditions.

***

#### What happens when a PoCH SBT expires or is revoked?

When a PoCH SBT expires or is revoked:

* Applications will no longer treat the wallet as PoCH-verified.
* No personal data is exposed as a result.
* The user may re-verify to obtain a new attestation if they wish to continue using PoCH-gated services.

This mechanism helps ensure verification remains current over time.

***

#### Is PoCH the same as traditional KYC?

No.

Traditional KYC typically requires each application to collect and store personal data.

PoCH allows applications to:

* verify eligibility,
* enforce access controls,
* and meet certain compliance requirements,

without collecting or storing user identity data themselves.

***

#### Where is PoCH typically used?

PoCH is commonly used in scenarios such as:

* privacy-preserving bridges,
* DeFi protocols with compliance constraints,
* real-world asset platforms,
* large airdrop or reward distributions,
* on-ramps and off-ramps that require eligibility checks.

***

#### What is the primary benefit of PoCH for users?

PoCH allows users to access high-trust or regulated applications without repeatedly sharing their identity and without enabling applications to build identity profiles or centralised user databases.

***

## Troubleshooting

If you run into any issues, please[ reach out to support](https://support.passport.xyz/passport-knowledge-base/need-support).&#x20;



## Learn more

{% embed url="https://passport.human.tech/blog/proof-of-clean-hands-introduction" %}

