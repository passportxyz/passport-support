# Passport Embed

## What is Passport Embed?

[**Passport Embed**](https://passport.human.tech/embed) lets websites verify that you are a real, unique person without sending you elsewhere. It is a React component that connects to the same trusted backend as the [Passport App](https://app.passport.xyz). When you click “Verify with Passport,” it checks your [Unique Humanity](../common-questions/what-is-unique-humanity.md) score using [Stamps](broken-reference) — privacy-preserving proofs from your web3 activity or selected web2 accounts or government documents — and confirms that you are human, all while staying on the same site. Verification per Stamps is optional and you can build your Humanity Score however you like.&#x20;

See [scoring-20-for-humans.md](scoring-20-for-humans.md "mention") for more information about available Stamps and [full announcement blog](https://passport.human.tech/blog/passport-embed-is-live-bring-privacy-preserving-proof-of-humanity-directly-into-your-dapp-or-website) for more high-level overview. See Loom video for the [Passport Embed walkthrough](https://app.gitbook.com/u/fnvMNUN77Sh8QlKhdti5dfPWCjj1).&#x20;

{% embed url="https://www.loom.com/share/bb23acaaffec464e83ef36d6d70c10bc" %}

### How it works&#x20;

Passport is built on the idea of scores and Stamps. Think of a Passport as an aggregate score for your online identity. If you can build up a score over 20, it represents to the world that you are unique and human. You increase your score by collecting Stamps, which are verifications of different online activities – for example, verifying you have a unique phone number, a valid social media account, maybe an email, or even doing a liveness check. Each Stamp adds extra points.&#x20;

When a site uses Passport Embeds, it typically sets a score threshold (for example, >20) that it considers “good enough” to trust you​r unique humanity. The Passport Embed component will check your score and simply tell the site whether you meet that threshold or not. This happens by connecting your crypto wallet (which holds your Passport onchain history) and possibly verifying a few additional Stamps – all done in a couple of clicks. You don't have to navigate away; everything shows up right on the site.

### Why it’s useful (for users)

From a user perspective, Passport Embed means less hassle and more privacy. Many users will be able to verify their Passport without needing to add any Stamps since their onchain history is enough to prove they’re human. Others might need to verify a Stamp or two to build up enough evidence of their humanity.&#x20;

Good news: your humanity score on Human. Passport is totally composable, so once the score is high enough, you can take it with you to use for any of the campaigns that are protected by us.&#x20;

Human Passport is also completely privacy-preserving, so there’s no need to worry about personally identifying information being attached to your wallet or email through the process. Only a yes/no or a score is shared with the site, never your personal details. This way, you can unlock special features or rewards (like access to exclusive chat groups, the ability to vote in a DAO, or matching donations in a grants round) simply by having built up your Passport beforehand.

### Why it’s useful (for Passport partners)

For websites and apps, Passport Embed provides proofs that the users interacting with their programs are **unique humans**. Dealing with bots, Sybil attacks, fake sign-ups, and duplicate accounts isn’t fun. It wastes time, dilutes metrics, breaks trust, and drains rewards meant for real participants. Passport Embeds helps solve that by giving a reliable signal of “this user is likely a unique human with verified credentials.”&#x20;

Site owners can integrate Embed easily as a React component. Integration is free and does not even require contacting the Passport team (although we recommend doing so anyways).&#x20;

While integrating, they can set their desired score requirement. We recommend using **20** as our system is optimized around that number. If a user passes, the site can confidently allow them through (to register, to participate in an event, to claim a reward, etc.). If not, the site can gently ask them to verify more and try again. This keeps communities and platforms fair – for instance, only one account per person in a voting scenario – and it does so without the site collecting sensitive data. It’s a win-win: users’ privacy is not invaded, and projects get fewer bots and more real engagement.

### Key benefits summary

* **Seamless experience:** All verification happens in-line on the site. No more jumping out to external identity portals. This keeps users engaged and significantly reduces drop-off rates.
* **Privacy-preserving:** Passport uses cryptographic proofs. That means the site never sees how you verified yourself (it doesn’t see your phone number or Discord handle, for example), only that your overall identity score is high enough. Your personal data remains with you - Passport doesn't store it.
* **Community trust:** When everyone accessing a certain feature has a passing Unique Humanity score, the community can trust that those participants are genuine. This leads to better discussions, fairer token distributions, more reliable poll results, etc.&#x20;
* **Ease of integration:** (For partners) It’s very easy to add Embed to a site. No need to build a verification system from scratch. You can[ learn more in our docs](https://docs.passport.xyz/building-with-passport/embed/introduction).

To summarize, Passport Embeds is like having a universal “humanity badge” you carry to different sites. For users, it means proving yourself once and reusing that proof everywhere. For sites, it means keeping bad actors out while welcoming good users in, with minimal friction. This also means you’ll likely see more and more sites using Passport Embeds, creating a network effect where your one Passport unlocks multiple doors across the web.\


## FAQ – Passport Embed

### **Q: What is Passport Embeds, in simple terms?**

Passport Embed is an embeddable component that websites and apps can use to verify that you’re a real, unique human — without leaving their site. Think of it as a privacy-preserving “Captcha for web3,” powered by your Human Passport.

When you interact with it, it checks your Unique Humanity Score (sometimes called a Passport score) — a score built from verified Stamps linked to your wallet. If your score meets the site’s threshold, it confirms: “✓ Verified human.” If not, you can complete more verifications to raise your score.

Everything happens through your wallet, not through forms or ID uploads. It’s an easy, on-site way for apps to ask: “Are you uniquely human?” — and for you to prove it securely and privately.

### **Q: How do Passport scores work?**

Your Unique Humanity Score (sometimes called a Passport score) is essentially a number that measures how many verification “stamps” you’ve collected. Each Stamp is a proof of some online activity – for example, that you have a unique phone number, a government ID verified (if you chose to do that), a social media account, or transaction history that appears to be coming from a human. The more Stamps you add, and the more valuable they are, the higher your score.&#x20;

Passport optimizes its score around a score of 20. If you are able to build up a score greater than 20, you have effectively proven that you are a unique human. Since 20 is the threshold number, there is no need to build up a score higher than this.&#x20;

The scores are calculated automatically by adding up the weights of your Stamps (each Stamp type might contribute a certain number of points). It’s important to note that this is privacy-preserving – the site sees the score or a yes/no, but doesn’t get the details of your Stamps or personal info.

### **Q: What happens if someone doesn’t qualify or has a low score?**

If you don’t meet the required score, Passport Embed will let you know and guide you on what to do next. You’ll see a prompt explaining that your Unique Humanity Score needs to improve before you can continue.

You can increase your score by verifying additional Stamps directly within the Embed. The interface walks you through available verification options — such as Government ID, Biometrics, or social (web2) activity. Some partners may customize which Stamps are shown, but the process always follows the same flow.

Your score updates automatically as you verify more Stamps. Once you reach the partner’s threshold (typically 20), the protected feature or program will unlock. You can then take your verified Passport to other programs using the same protocol — your proof of unique humanity travels with you.

**Keep in mind that some partners may combine Passport verification with their own requirements, such as completing certain in-app actions or eligibility checks before full access is granted.**

### **Q: How do I get verified or increase my Unique Humanity score on Human Passport?**

To raise your Unique Humanity Score and get verified, you’ll need to collect more Stamps — each one is a different way to prove you’re a real, unique human. Here’s how it works:

1.  **Create your Passport**

    Go to [app.passport.xyz](https://app.passport.xyz) (or use a partner’s Passport Embed) and connect your crypto wallet. If you’re interacting through a partner site using Embed, your Passport account is created automatically.
2.  **Automatic verification**

    When you first connect, Passport automatically checks for existing onchain Stamps based on your wallet’s activity. This gives you an initial score derived from credible web3 signals. If you're a crypto OG, you might already score 20 and be done at this stage.&#x20;
3.  **Add more Stamps**

    If your score isn’t yet above the threshold (typically 20), you’ll see a list of available verification options. These can include verifying:

    * Google or GitHub account
    * Phone number
    * Discord or LinkedIn account
    * ENS domain
    * zk KYC or liveness proof&#x20;

    You can choose which verifications you’re comfortable completing - tehre's no need to complete all. Each one adds a new Stamp to your Passport.
4.  **Watch your score increase**

    Your score updates automatically as you verify new Stamps. Some carry more weight than others — for example, government or biometric verifications add a bigger boost than basic social accounts. That's becouse they are harder to forge for attackers.&#x20;
5.  **Reach the threshold**

    Once your score reaches 20 or higher, you’re considered verified. In most cases, the partner program will unlock automatically. If you’re using the Passport App, you might need to refresh the partner page to sync your new score.

The whole process usually takes 5–10 minutes. You remain pseudonymous throughout — proving that you’re a unique human, not revealing personal details. You can always add new Stamps later to strengthen your proof and access more programs across the ecosystem.

### Q: Is my data safe? How is the information handled?

Yes — your data is safe. Privacy is at the core of Human Passport’s design. When you use Passport Embed, the site you’re on never receives your personal data — only the verification result (your score, or a simple pass/fail).

Here’s how it works behind the scenes:

*   **No personal data collected**

    Passport is fully privacy-preserving. We don’t collect or store any personally identifying information (PII) when you verify Stamps.
*   **Minimal data exchange**

    When a site checks your Passport via the Embed, it sends your wallet address (your Passport identifier) to the Passport API. The API responds with only what’s required for verification — typically your score, whether it meets the threshold, and a list of Stamp types you’ve verified.

    Example response:

`Address 0xABC... → Score: 42 | Threshold: 20 | passingScore: true ✅`

*   **No exposure of personal details**

    No names, emails, phone numbers, or social handles are ever shared. The site never sees your private data — only that your Passport meets the verification criteria.\


In short, Passport Embed shares the minimum information needed to confirm you’re a unique human, nothing more. You stay pseudonymous, private, and in control of your data.

Learn more about Passport’s privacy approach here: [passport.human.tech/privacy](https://passport.human.tech/privacy)

### Q: Do I need cryptocurrency or have to pay for using Passport?

Passport itself, Passport Embed included, is free to use, and you don’t need to pay for many Stamps (some Stamps require a fee). However, since it’s based on a crypto wallet, you do need a wallet (like MetaMask, Coinbase Wallet, etc.) to serve as your identity.&#x20;

Stamps issued by human.tech (the high-value, high-weight ones such Government ID/Biometric) are paid. They typically cost about $5 per Stamp because they rely on external verification providers and stronger checks. These Stamps help you reach the Unique Humanity threshold faster. You'll need to have sufficient amount to be able to verify those.&#x20;

In certain cases, projects may require [minting your verification onchain](onchain-passport.md), which costs $3 per mint. It's sufficient to just int once - your score will then be available onchain for any partner using onchain passport feature. You may also encounter small, network-level gas fees when completing specific onchain actions.

Always make sure you’re interacting with official Passport partners, and never sign transactions you don’t understand.

### Q: Where can I see or manage my Passport?

You can manage your Passport on the main Passport app (app.passport.xyz). When you go there, connect your wallet and you’ll be able to see:

* Your current Unique Humanity score.
* All the stamps you’ve collected, often with details or statuses.
* Available Stamp options to add new verifications.

### Q: What kinds of sites or applications use Passport Embeds?

A variety of web3 and even web2 platforms are starting to use Passport Embeds. Examples include:

* **Crypto airdrops and token sales:** Projects that want to ensure each person only claims once, or only real humans (not bots) participate.
* **DAO membership or voting:** Communities that give voting rights or membership roles only to verified humans to prevent one person from having multiple votes.
* **Grant programs or donation matching (like Gitcoin grants):** Where they match funds only for verified users to avoid Sybil attacks on funding pools ​[support.gitcoin.co](https://support.gitcoin.co/gitcoin-knowledge-base/misc/explorer-passport-guide)​[support.gitcoin.co](https://support.gitcoin.co/gitcoin-knowledge-base/misc/explorer-passport-guide).
* **Online forums or social platforms:** To reduce spam and bot accounts – e.g., requiring new users to have a Passport score before posting or accessing certain channels.
* **NFT drops or raffles:** Ensuring fair distribution by limiting to one per person (Passport can help enforce that).
* **DApps with rewards or referral systems:** So that one person can’t just create 100 accounts to farm rewards.

As Passport Embeds becomes more popular, you may see its “Verify with Passport” button in many places, similar to how you see “Login with Google” or “Login with Facebook” on websites. The difference is that Human Passport is decentralized and privacy-centric. It’s a sign that the site values unique human users and is protecting its community from bots/abuse.&#x20;

For users, it’s usually optional but beneficial to participate fully. If you don’t have a Passport, you might still use some sites, but you’ll miss out on certain perks or access levels.

We hope this gives you a clear overview of Passport Embeds. It’s all about making the web a more human place by allowing people to prove personhood in a user-friendly way.&#x20;

If you have more questions or need help with a specific site’s implementation, check that site’s support page or the [Passport documentation](https://docs.passport.xyz/).&#x20;

Happy verifying, and welcome to the HUMN club!&#x20;
