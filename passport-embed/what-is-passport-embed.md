# What is Passport Embed?

[**Passport Embed**](https://passport.human.tech/embed) lets websites verify that you are a real, unique person without sending you elsewhere. It is a React component that connects to the same trusted backend as the [Passport App](https://app.passport.xyz). When you click “Verify with Passport,” it checks your [Unique Humanity](../common-questions/what-is-unique-humanity.md) score using [Stamps](/broken/pages/4OxH7lj6TaW26Scbkib0) — privacy-preserving proofs from your web3 activity or selected web2 accounts or government documents — and confirms that you are human, all while staying on the same site. Verification per Stamps is optional and you can build your Humanity Score however you like.&#x20;

See [scoring-20-for-humans.md](../using-passport/scoring-20-for-humans.md "mention") for more information about available Stamps and [full announcement blog](https://passport.human.tech/blog/passport-embed-is-live-bring-privacy-preserving-proof-of-humanity-directly-into-your-dapp-or-website) for more high-level overview. See Loom video for the [Passport Embed walkthrough](https://app.gitbook.com/u/fnvMNUN77Sh8QlKhdti5dfPWCjj1).&#x20;

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

To summarize, Passport Embeds is like having a universal “humanity badge” you carry to different sites. For users, it means proving yourself once and reusing that proof everywhere. For sites, it means keeping bad actors out while welcoming good users in, with minimal friction. This also means you’ll likely see more and more sites using Passport Embeds, creating a network effect where your one Passport unlocks multiple doors across the web.

**See Passport Embed FAQ:** [passport-embed-faq.md](passport-embed-faq.md "mention")<br>
