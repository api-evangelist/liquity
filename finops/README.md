# Liquity API FinOps

## Cost Model

The Liquity API is entirely free and open. There are no usage fees, subscription
costs, or metered billing for accessing api.liquity.org endpoints.

## Cost Drivers for Integrators

While Liquity's static API has no direct cost, integrators may incur costs from
adjacent services:

| Service | Cost Driver | Typical Cost |
|---------|-------------|--------------|
| Ethereum RPC (Alchemy/Infura) | Required for SDK / direct on-chain calls | Free tier available; paid from ~$49/mo for high volume |
| The Graph (subgraph queries) | Querying Liquity subgraph for historical data | Free on hosted service; GRT fees on decentralized network |
| Dune Analytics | Accessing Liquity's published Dune queries | Free tier available; paid plans for API access from $349/mo |
| CoinGecko API | Price data (used internally by Liquity) | Free Demo key available; paid from $129/mo |

## Protocol Economics (Not API Costs)

Liquity itself is a protocol with economic parameters relevant to integrators
building borrowing/lending products:

| Parameter | V1 | V2 |
|-----------|----|----|
| Borrowing fee | 0.5% one-time | Interest-rate based (variable) |
| Redemption fee | 0.5% minimum | Calculated dynamically |
| Collateral ratio | 110% minimum | Depends on collateral type |
| Stability pool token | LUSD | BOLD |
| Governance token | LQTY | LQTY |

## Summary

For API consumers, the total cost of using Liquity's public API is $0. The only
costs arise if you choose to use premium RPC providers, Dune API access, or
CoinGecko paid plans for supplementary data — all of which are optional.
