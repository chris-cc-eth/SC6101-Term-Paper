# Proposed Solutions
**A. Solution to Impermanent Loss**

*1) Concentrated LPs:* Uniswap V3 offers concentrated liquidity pools where LPs can specify a price range for their assets. By setting a narrower price range, LPs can limit their exposure to impermanent loss [1]. Moreover, a Hooks feature introduced in Uniswap V4 allows integrators to create a concentrated liquidity pool with flexible and customizable execution [2]. However, the impermanent loss increases at a faster pace with concentrated liquidity [5]; smaller intervals result in a higher concentration of liquidity and correspondingly larger fees when the price remains in the interval, but with higher risk as prices may exit the interval, leaving the LP with no fee rewards [6]. There is also evidence that users are rebalancing more frequently, resulting in more efficiently used concentrated liquidity [10]. 


*2) Less volatile pairs:* LPs benefit from fees, which are a function of volatility, but suffer from price change volatility [3]. The less volatile relative price makes it easier to determine the price range of a liquidity position and makes it less likely for the price to fall out of the liquidity position’s price range. Conversely, while higher volatility may lead to higher trading volume and more fees collected, the probability that the price drops out of the liquidity position increases with volatility [5]. Higher volatility of the AMM pool assets also implies higher uncertainty in yield [8]. Uniswap V3 introduced a dynamic fee tier to overcome the problem of some stablecoins. The fee is likely too high but too low for other highly volatile pairs [1].

*3) Market strategy:* Liquidity provision strategies provide significant gains for LPs relative to baseline uniform allocation strategies (similar to liquidity allocation in Uniswap v2) in multiple economic environments for decentralized exchanges [6]. Moreover, investment strategies with the potential to generate remarkably high yields also bear high risks [8]. Also, some medium-term LP strategies research is available that consistently outperforms HODLing (holding assets)[9]. 

*4) Risk management:* Obtaining high returns as a liquidity provider on Uniswap V3 is a complicated undertaking requiring active management and good know-how. Therefore, retail traders, unwilling to risk these losses and unable to perform resource-intensive active management, should restrict themselves to simple strategies that yield only small returns [5]. Risk management also affects your strategy; risk aversion mainly impacts the allocations in ODRA and OIRA LP strategies. LPs spread their liquidity more as they become more risk-averse. A more extensive spread of liquidity allocation typically implies lower expected earnings for an LP as they have less proportional liquidity at traded prices. Still, at the same time, there is less risk of missing out on fees due to prices escaping their position or suffering impermanent loss due to prices deviating from the initial price [6].



**B. Solution to Arbitrageurs**

In fact, decentralized exchanges such as Uniswap can represent a ‘fair’ price of assets since they will have been armed already. These are called price oracles, and Uniswap is regarded as such to prevent arbitrage tools from advantaging a trio of currency pairs that end up quoting different cross-exchange rates [4]. Uniswap also introduced gas-adjusted execution on some chains, liquidity providers are more capital efficient, and liquidity providers have increased fee returns from more arbitrage. Additionally, cheaper arbitrage transactions and the related increase in fees paid by arbitrageurs make LPs more profitable. Users (or likely arbitrageurs) may also be more inelastic to gas costs during times of volatility, making them more likely to swap at high gas costs due to profitable arbitrage opportunities resulting from volatility.  As a result, arbitrage transactions are likely lower bound by gas costs, as arbitrageurs will only execute if they can pay off their fixed costs for transacting (gas) [10].

# References
[1] Hayden Adams, Noah Zinsmeister, Moody Salem, River Keefer, and Dan Robinson. Uniswap v3 core, 2021. URL: https://uniswap.org/whitepaper-v3.pdf.

[2] Adams et al., Uniswap v4 Core Draft, 2023. URL: https://github.com/Uniswap/v4-core/blob/main/docs/whitepaper-v4.pdf.

[3] Lo, Yuen & Medda, Francesca, 2020. "Uniswap and the rise of the decentralized exchange," MPRA Paper 103925, University Library of Munich, Germany.

[4] Aigner, Andreas A., and Gurvinder Dhaliwal. "Uniswap: Impermanent loss and risk profile of a liquidity provider." arXiv preprint arXiv:2106.14404 (2021).

[5] Heimbach, Lioba, Eric Schertenleib, and Roger Wattenhofer. "Risks and returns of uniswap v3 liquidity providers." Proceedings of the 4th ACM Conference on Advances in Financial Technologies. 2022.

[6] Fan, Zhou, et al. "Strategic liquidity provision in uniswap v3." arXiv preprint arXiv:2106.12033 (2021).

[7] N. Koroļkovs and S. Kodors, “UNISWAP - A CASE STUDY OF DECENTRALIZED EXCHANGES ON THE BLOCKCHAIN”, HET, no. 26, pp. 25–30, Jan. 2023, doi: 10.17770/het2022.26.6950.

[8] Xu, Jiahua, and Yebo Feng. "Reap the harvest on blockchain: A survey of yield farming protocols." IEEE Transactions on Network and Service Management 20.1 (2022): 858-869.

[9] Loesch, Stefan, et al. "Impermanent loss in uniswap v3." arXiv preprint arXiv:2111.09192 (2021).

[10] Adams, Austin. "Layer 2 be or Layer not 2 be: Scaling on Uniswap v3." arXiv preprint arXiv:2403.09494 (2024).
