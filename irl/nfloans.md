---
description: liquidity pools backed by an NFT and used as a basis for a loan
---

# NFLoans

First a user mints their respective [NFTitle & Liquid RWA Tokens](../rwa.md).  Then they propose a pool to be made according to a certain valuation.  This looks like them staking their NFT along with the tokens they want to make the liquidity pool up with. &#x20;

When the DAO approves this valuation a pool is created with their asset token and what they want to pool it with, thus creating their self assessed valuation.  Say you've minted 100 Asset Tokens for your house and created a liquidity pool where you deposit 10 Asset Tokens and $10,000.  This pegs the price to a $100,000 valuation.  This is the basic mechanism involved, however it sets the foundation for varying models and add-ons. &#x20;

### Interest Bearing Loan

This type of loan is a carry over from our current common loan.  A monthly payment must be made into a smart contract.  Late fees are automatically applied and profits automatically distributed to token holders following the yield bearing [ERC4626 Vault](https://erc4626.info/) so that it is modular and can plug into other yield bearing token ecosystems.

### Self Funded 0% Interest Loans

This model takes inspiration from a mashup of [Liquity](https://www.liquity.org/) and [Splitero](https://www.splitero.com/) in which a pre-defined fee is determined to be paid in the underlying equity of the asset rather than an ongoing monthly payment.  For example a user wants to get a $50,000 loan for a $100,000 asset.  The DAO determines we will take 1% each month in exchange for providing the $50,000.\
\
The % determines the length of the loan, which in this case means the loan has a life of 100 months before the DAO fully owns the asset and can withdraw it. The loan can be paid back at anytime, however the NFT stays locked in escrow until either a Buy Back price is paid or the DAO and asset owner come to another arrangement.

### Buy Back & Buy Now

A user can at anytime determine that they want to buy back their NFT completely and close the loan.  Typically one would need to re-purchase all the outstanding tokens in order to redeem them and close the escrow.  Our model allows a price to be paid and later each token holder can redeem their share of the profits.\
\
In practice this would look like a user borrowing $50,000 on a $100,000 asset with a buy back price of $60,000.  If the price is falling and are concerned with having a liquidation or the owner decides they want to close out the loan our design allows for a base "buy back" price to be set.  They deposit the $60,000 into an escrow account and the holders of the asset token can redeem their liquidity pool tokens in exchange for the asset price.  This allows for a loan to be repaid early and investors will still have a certain base APY.

### Devaluation Protection

If an asset is being devalued and it's token price is plummeting, either the owner of the asset needs to rebalance their pool so that it meets the criteria defined by the agreement with the DAO or it's underlying NFT will be susceptible to being claimed by the DAO. The "buy back" price would still valid until the asset is liquidated.

