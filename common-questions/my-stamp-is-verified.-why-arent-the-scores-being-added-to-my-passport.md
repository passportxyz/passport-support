# My Stamp is verified. Why aren't the scores being added to my Passport?

It’s likely that the account, token, or NFT you’re trying to link has already been connected to another Passport. By default, the Passport API uses a Last In, First Out (LIFO) Stamp deduplication method. This means that if a Passport holder submits a Stamp that has already been used by another Passport, the duplicate Stamp is ignored and doesn’t count toward the score.

Although the Stamp on subsequent Passports can be verified, it won’t contribute to your score until the Stamp on the first Passport expires, which occurs after 90 days. Once it expires, points will be added from the next verified Passport in line.

Stamp deduplication is essential to prevent users from increasing their influence by submitting the same Stamps across multiple Passports. This process ensures that a user can associate an individual Stamp with only one identity within a specific context.

For more information on Stamp Deduplication, please check [here](https://docs.passport.xyz/building-with-passport/major-concepts/deduplicating-stamps).

\
