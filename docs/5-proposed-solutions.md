# Proposed Solutions
**A. Solution to Layer 1 Gas Fee and Scalability**

One solution Ethereum has adopted is The Merge, which transitioned Ethereum from a Proof of Work (PoW) to a Proof of Stake (PoS) consensus mechanism in 2022. Uniswap, being a decentralized exchange (DEX), relies heavily on Ethereum's network for processing trades and liquidity provision. High gas fees and network congestion under PoW often made small trades expensive. With PoS, Ethereum aims to reduce congestion and transaction fees by increasing network efficiency. This could lead to more cost-effective trades and improved user experience on Uniswap. The Merge also stated that the scalability will be enhanced after the event [1]; however, the number of TPS now is still around 15-20 [2], much lower than in Layer 2. Other solutions is to derived proof mechanism from other chains e.g. Solana with Proof of History and TPS of 3000 or Fantom with trade-off security, only single confirmation needed.

**B. Solution to Layer 2 Security**

Layer 2 inherits the security from layer 1 and trades off the number of validators to increase scalability. Arbitrum One and Optimiusm, the most 2 popular L2 chains in Uniswap, use Optimistic Rollup Fault Proofs. However, Optimistic Rollup is not really good at security compared to others. Optimistic Rollups "optimistically" assume that all transactions are valid with only proof from 1 honest validator until proven otherwise [3]. Optimistic Rollups need to increase the number of honest validators to enhance security and more decentralize. Another solution is to switch to a more security-proof mechanism, ZK-Rollups. ZK-Rollups assume all transactions are false until proven valid through ZKPs. ZK rollup nodes must provide proof of validity to verify all transactions.


**C. Solution to AMM Liquidity Pool Security**

Traders can exploit price differences between the AMM pool and external markets, making the exchanges vulnerable. If the pool’s price deviates from the market price, arbitrage traders conduct trades to bring the pool’s price back in line with the market. One solution for this is to use price oracles to set the measured price to one that is out of sync with the global market price, an attacker has to make a bad trade at the end of a previous block [4]. Uniswap also introduced gas-adjusted execution on some chains, liquidity providers are more capital efficient, and liquidity providers have increased fee returns from more arbitrage [5].

# References
[1] https://ethereum.org/en/roadmap/merge/#merge-and-scaling

[2] https://chainspect.app/chain/ethereum

[3] https://chain.link/education-hub/what-is-layer-2

[4] Aigner, Andreas A., and Gurvinder Dhaliwal. "Uniswap: Impermanent loss and risk profile of a liquidity provider." arXiv preprint arXiv:2106.14404 (2021).

[5] Adams, Austin. "Layer 2 be or Layer not 2 be: Scaling on Uniswap v3." arXiv preprint arXiv:2403.09494 (2024).
