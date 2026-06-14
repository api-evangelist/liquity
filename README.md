# Liquity

Liquity is a decentralized borrowing protocol on Ethereum allowing users to
draw interest-free (V1) or interest-rate-based (V2) loans collateralized by
ETH, wstETH, or rETH. V1 issues LUSD; V2 issues BOLD. The protocol is
non-custodial, immutable, and governance-free at the contract level.

The public API at api.liquity.org provides static JSON and plaintext data
files covering protocol metrics, token supplies, stability pool deposits,
yield opportunities, governance epochs, and a points leaderboard.

## API Endpoints

### V1 (LUSD / LQTY)

| Endpoint | Description |
|----------|-------------|
| `GET https://api.liquity.org/v1/lusd_total_supply.txt` | LUSD total supply (plaintext decimal) |
| `GET https://api.liquity.org/v1/lqty_circulating_supply.txt` | LQTY circulating supply (plaintext decimal) |
| `GET https://api.liquity.org/v1/lusd_cb_bamm_stats.json` | LUSD Chicken Bonds BAMM stats (debt + APRs) |

### V2 (BOLD / Multi-Collateral)

| Endpoint | Description |
|----------|-------------|
| `GET https://api.liquity.org/v2/ethereum.json` | Full V2 relaunch protocol stats (TVL, supply, per-branch data, prices) |
| `GET https://api.liquity.org/v2/mainnet.json` | V2 legacy deployment stats |
| `GET https://api.liquity.org/v2/testnet/sepolia.json` | Sepolia testnet protocol stats |

### V2 Website Data

| Endpoint | Description |
|----------|-------------|
| `GET https://api.liquity.org/v2/website/bold-venues.json` | BOLD yield venues (protocol, APR, TVL) |
| `GET https://api.liquity.org/v2/website/fork-venues.json` | Liquity fork protocol data |
| `GET https://api.liquity.org/v2/website/leaderboard.json` | Points leaderboard (1,900+ addresses) |
| `GET https://api.liquity.org/v2/website/borrow-rates.json` | Borrow rate comparison vs DeFi averages |

### V2 Governance

| Endpoint | Description |
|----------|-------------|
| `GET https://api.liquity.org/v2/governance/initiatives.json` | Active governance initiatives mapping |
| `GET https://api.liquity.org/v2/governance/latest_completed_epoch.json` | Latest completed governance epoch number |
| `GET https://api.liquity.org/v2/governance/allocation/` | Per-epoch LQTY allocation snapshots |

## Authentication

None required. All endpoints are publicly accessible without API keys.

## SDKs

- `@liquity/lib-base` — Common interfaces
- `@liquity/lib-ethers` — Ethers.js on-chain middleware
- `@liquity/lib-react` — React hooks and components
- `@liquity/lib-subgraph` — Apollo/The Graph middleware

## Links

- Website: https://www.liquity.org/
- V1 Docs: https://docs.liquity.org/liquity-v1
- V2 Docs: https://docs.liquity.org/
- GitHub: https://github.com/liquity
- API Repo: https://github.com/liquity/api.liquity.org
- Discord: https://discord.gg/2up5U32
- Twitter: https://twitter.com/LiquityProtocol
