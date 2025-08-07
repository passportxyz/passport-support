# Why is my score on the Passport app different than my score on a partner site?

At times, you may encounter a situation where your score on a partner site differs from the one that you have within the Passport app.&#x20;

## Stamp Deduplication

**The primary reason for this discrepancy is typically the claiming of the same Stamp using multiple wallet addresses.**

Passport serves as an identity verification application designed to mitigate [Sybil](what-is-a-sybil.md) attacks. Therefore, we've implemented some protective functionality into our system to prevent multiple accounts from being able to verify the same Stamp.

Here are the details:

* _**When attempting to claim a Stamp using more than one wallet address,**_ the score associated with second, third, etc wallet addresses will display a zero (0) score for duplicate Stamps in the Passport app.&#x20;
* _**When participating in partner programs,**_ you can ignore the 0 score for these Stamps. The first wallet containing a duplicate Stamp that is submitted to a partner program will count the duplicate Stamp score. Any other addresses submitted to that same partner program will not count the duplicate Stamp score.&#x20;
* If you'd like the duplicate Stamp to permanently move to another address and display properly in the Passport app, you will need to wait until that Stamp expires within the first wallet after the 90 day expiration period, then reverify that Stamp in the new wallet.



**To simplify:** For wallets with duplicate Stamps, it all depends on which wallet is submitted to a partner first. All others that are trying to claim the same Stamp and are submitted to the same partner will receive zero points for the duplicate Stamps.&#x20;



## Custom Dashboards and Scores

Passport offers partners the ability to create [custom dashboards and scores](../using-passport/custom-passport-dashboards-and-scores.md), which weigh Stamps differently. If a user is on a custom dashboard, they might see a different score than the score on the standard Passport app, or the score that is available via a partner site.&#x20;

You can tell if you’re accessing a custom dashboard by looking at the URL. If it has an element after `/#/` and before `/dashboard`, then the dashboard that you are on could have a custom set of Stamp weights.&#x20;

[`https://app.passport.xyz/#/shape/dashboard`](https://app.passport.xyz/#/shape/dashboard)
