# Passport Embed FAQ

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

In certain cases, projects may require [minting your verification onchain](../using-passport/onchain-passport.md), which costs $3 per mint. It's sufficient to just int once - your score will then be available onchain for any partner using onchain passport feature. You may also encounter small, network-level gas fees when completing specific onchain actions.

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
