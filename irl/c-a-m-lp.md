---
description: cross-chain cross-asset automated market maker liquidity pools
---

# C³A²M² LP

Cross-chain cross-asset liquidity pools help prevent the price from becoming “de-pegged” or attacked in a low liquidity situation that may occur if tokens get spread out on various different L2s.  In order to understand what we are proposing it is important to understand what a typical [Automated Market Maker](https://academy.binance.com/en/articles/what-is-an-automated-market-maker-amm) is first, but essentially we will mint a single liquidity pool on our home chain and using something like [Wormhole](https://wormhole.com/) or [LIFI](https://li.fi/) to enable on and off ramps to any chain and any popular token.  The flow looks roughly like this:

> Any Chain => Bridge => $TBL => Asset Pool

This allows us to diversify the underlying trade assets so it is not tied to one token, but rather the currency of asset's original valuation and also prevents the need to manage arbitrage opportunities between chains.
