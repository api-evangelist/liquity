# Liquity

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
