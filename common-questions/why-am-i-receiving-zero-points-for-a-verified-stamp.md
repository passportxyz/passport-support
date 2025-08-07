# Why am I receiving zero points for a verified Stamp?

At times, you may encounter a situation where a newly verified Stamp appears to be verified, but it gives you zero (0) points.\


_**The primary reason for this discrepancy is typically the claiming of the same Stamp using multiple wallet addresses.**_

Passport serves as an identity verification application designed to mitigate [Sybil](what-is-a-sybil.md) attacks. Therefore, we've implemented some protective functionality into our system to prevent multiple accounts from being able to verify the same Stamp.&#x20;

Here are the details.

* _**When attempting to claim a Stamp using more than one wallet address,**_ the score associated with second, third, etc wallet addresses will display a zero (0) score for duplicate Stamps in the Passport app.&#x20;
* _**When participating in partner programs,**_ you can ignore the 0 score for these Stamps. The first wallet containing a duplicate Stamp that is submitted to a partner program will count the duplicate Stamp score. Any other addresses submitted to that same partner program will not count the duplicate Stamp score.&#x20;
* If you'd like the duplicate Stamp to permanently move to another address and display properly in the Passport app, you will need to wait until that Stamp expires within the first wallet after the 90 day expiration period, then reverify that Stamp in the new wallet.\


We also discuss this concept in our hacked (compromised) wallet FAQ:

[My wallet was hacked. Can I move my scores to a new Passport?](my-wallet-was-hacked-or-compromised-.-can-i-move-my-scores-to-a-new-passport.md)

\
Note that there are some side cases around how Partners can calculate your score, that are described in the following guide:

[Why is my score on the Passport app different then my score on a partner site?](why-is-my-score-on-the-passport-app-different-than-my-score-on-a-partner-site.md)

***

\
If you encounter any difficulties in resolving this issue, please feel free to [**contact us**](../need-support.md) without hesitation.



**For developers** — we have a detailed description of how we deduplicate Stamps across addresses via the following guide: \
[Deduplicating Stamps, for developers](https://docs.passport.xyz/building-with-passport/major-concepts/deduplicating-stamps)
