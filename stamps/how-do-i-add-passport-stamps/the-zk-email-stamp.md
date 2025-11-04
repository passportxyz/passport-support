# ☑️ The ZK Email Stamp

Verify your Amazon and Uber activity using zero-knowledge email analysis provided by ZK Email. Earn up to 6 different credentials based on your Amazon shipping and Uber rides, all while keeping your email data completely private.&#x20;

{% hint style="info" %}
**Note:** Only Google Gmail accounts are currently supported.
{% endhint %}

* **Time Required:** 5-10 minutes
* **Cost:** Free
* **Difficulty:** Beginner-friendly
* **Privacy Level:** High (zero-knowledge proofs)

## Prerequisites:

* Active **Google Gmail account** with email history
* Amazon shipping confirmations in your email inbox or archive
* Uber ride receipts in your email’s inbox or archive
* Web browser (Chrome, Firefox, Safari, or Edge)
* Stable internet connection

{% hint style="info" %}
**Note:** You can earn credentials from both the Amazon and Uber categories simultaneously. Each credential contributes points to your Passport score.
{% endhint %}

## Step-by-Step Guide:

{% stepper %}
{% step %}
### Start the Verification Process

1. Click the _"Check Eligibility"_ button in your Human Passport dashboard
2. You'll be redirected to the ZK Email verification interface
3. Review the privacy notice explaining how your data is protected

**What's happening:** ZK Email prepares to analyze your email patterns without accessing your actual email content
{% endstep %}

{% step %}
### Connect Your Google Account

1. Click _"Connect Google Account"_ on the ZK Email interface
2. Sign in to your Google account when prompted
3. Review the permissions requested by ZK Email:
   1. Read-only access to email metadata
   2. Permission to scan for purchase patterns
4. Click _"Allow"_ to grant permissions

{% hint style="info" %}
**Privacy Note:** ZK Email uses zero-knowledge proofs to verify your purchase patterns without ever seeing your actual emails or personal information.
{% endhint %}
{% endstep %}

{% step %}
### Email Analysis & Credential Assignment

1. ZK Email scans your inbox for Amazon and Uber patterns:
   * Looks for purchase confirmations from Amazon in your inbox and archive
   * Searches for ride receipts from Uber in your inbox or archive
2. Analysis typically takes anywhere from 15 seconds to a couple of minutes
3. View your results:
   * Amazon credentials earned (if any)
   * Uber credentials earned (if any)
   * Total points added to your Passport score
{% endstep %}

{% step %}
### Verify the additions in your Human Passport dashboard

Congratulations! Your ZK Email credentials are now active in your Passport.
{% endstep %}
{% endstepper %}

## Technical Details

### Supported Email Providers

* Primary: Gmail (Google Workspace accounts)
* Coming Soon: Outlook

### Emails that are scanned

* All emails in the Inbox
* All emails that are archived
* No deleted emails

## Understanding Your Credentials

### Amazon Credentials

| Credential       | Credential    | Points Value\* | Typical Use Cases              |
| ---------------- | ------------- | -------------- | ------------------------------ |
| Casual Purchaser | 1+ purchases  | 1              | Basic e-commerce engagement    |
| Regular Customer | 10+ purchases | 0.6            | Consistent shopping activity   |
| Heavy User       | 50+ purchases | 0.4            | Substantial e-commerce history |

### Uber Credentials

| Credential       | Requirement | Points Value\* | Typical Use Cases             |
| ---------------- | ----------- | -------------- | ----------------------------- |
| Occasional Rider | 3+ rides    | 1              | Basic mobility service usage  |
| Regular Rider    | 25+ rides   | 0.6            | Frequent transportation usage |
| Power User       | 75+ rides   | 0.4            | Extensive mobility engagement |

## Privacy & Security

### How ZK Email Protects Your Data

Zero-Knowledge Proofs: ZK Email can verify your purchase patterns without ever seeing your actual emails, personal information, or purchase details.

Zero-knowledge means that it’s mathematically impossible to read the contents of your inbox, not just 'we promise we won't look.' The proof verifies you received an email without revealing its contents—not to Passport, not to anyone.

Similar to how Face ID proves you're you without Apple storing your face, ZK Email proves you received an email without anyone accessing the content.

The Stamp scans for Amazon/Uber emails, generates a cryptographic proof, and that's all ZK Email or Passport receives. The emails themselves never leave your inbox.

As with any Passport Stamp, the ZK Email Stamp is optional, so if you’re still not comfortable with the concept, feel free to prove your humanity with any of our other Stamps.

### Data Storage & Retention

* **No email content stored:** Only cryptographic proofs are generated
* **No personal data retained:** Verification results are anonymous
* **Temporary access only:** Permissions can be revoked in your Google account settings
* **Transparent process:** All verification logic is publicly auditable

#### **What ZK Email CAN verify:**

* That you have Amazon purchase confirmations
* That you have Uber ride receipts
* The frequency of your activity

#### **What ZK Email CANNOT see:**

* Your email content or subject lines
* Your personal information or addresses
* Your purchase amounts or payment details
* Your trip destinations or personal data

#### Full zk proof generation process:

1.  **User authorization**

    The user connects their email account (e.g., Gmail) through OAuth and grants zk.email permission to read specific metadata — not full email contents.
2.  **Email retrieval & parsing**

    zk.email’s off-chain service fetches the relevant email data (headers or structured metadata) and encodes it into a machine-readable format suitable for proving.
3.  **Proof generation**&#x20;

    A zero-knowledge circuit runs to prove that a valid email meeting predefined conditions exists (e.g., from a specific sender or containing a certain field). The proof hides all personal or message details.
4.  **Proof verification**

    The proof is submitted to a verifier smart contract, which checks its validity. The contract does not learn anything about the underlying email — only that the proof is mathematically sound.
5.  **Result anchoring & linking**

    The verification outcome (a success flag or credential) is anchored on-chain and associated with the user’s wallet. Applications like Human Passport can then read this status to confirm that the user passed verification, without any access to their email or private data.

Learn more: [https://docs.zk.email/architecture/zk-proofs](https://docs.zk.email/architecture/zk-proofs)

## FAQ

#### **Can I revoke email reading permissions given to ZK Email?**

Yes. Users can revoke reading permission in their Gmail settings once the proof is generated.

#### **Is this privacy-preserving? Nobody shares my email content?**&#x20;

Yes, fully. No personal data is stored or shared, and there is no link between email and the wallet. Here’s the full ZK Email zk tech explainer: [ZK Email Documentation](https://docs.zk.email/architecture/zk-proofs)

#### Which international Amazon domains are supported other than amazon.com?

India, Japan, Spain, USA, Germany, Canada, UK, Poland, Sweden, Netherlands, Italy, France, Mexico, UAE.&#x20;

#### Can I verify with Outlook or Protonmail?

No, currently only Gmail is supported.&#x20;

#### Is there any fee for verifying this Stamp?

There is no fee. Verification is fully free of charge.&#x20;

#### What exact type of emails are you looking for with this Stamp?

Zk Email scans for Uber receipts and Amazon shipping notifications.&#x20;

#### Do emails have to be stored in a specific place to be counted?

Yes, they have to be in the main Inbox or in the Archive.&#x20;

#### What if I keep my email inbox clean?

Unfortunately, we won't be able to confirm your Amazon and Uber history, so you won't be assigned points for this Stamp.&#x20;

## Need Help?

### Troubleshooting Steps

* See if your Uber/Amazon emails are not in the spam or promotional folder&#x20;
  * If yes, move them to the main inbox&#x20;
* Clear the cache and cookies of your browser
* Try using another browser

### Quick Support Options

Click on the icon in the **bottom right corner** of this page to reach out to support ↘

{% hint style="info" %}
### When contacting support, include:

* Your browser type and version
* Error messages or screenshots
* Whether you've tried any troubleshooting steps
* Your approximate email volume (helps with optimization)
{% endhint %}



### Recommended Next Steps

Complete guide to reaching verification thresholds:

{% content-ref url="../../using-passport/scoring-20-for-humans.md" %}
[scoring-20-for-humans.md](../../using-passport/scoring-20-for-humans.md)
{% endcontent-ref %}
