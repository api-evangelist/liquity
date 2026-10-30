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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Liquity is a decentralized borrowing protocol that allows users to draw interest-free loans against Ether and liquid staking tokens as collateral. The protocol (V1) issues LUSD stablecoin backed by ETH, while V2 (BOLD) supports multi-collateral borrowing with WETH, wstETH, and rETH. Liquity exposes a static JSON API at api.liquity.org covering circulating supplies, protocol stats, stability pool data, prices, governance epochs, yield opportunities, borrow rates, and a points leaderboard — all generated on-chain and published as flat files to GitHub Pages.

**Areas:** DeFi · Decentralized Finance · Lending · Stablecoins · Ethereum · LUSD · BOLD · Liquidity Protocol

## Liquity on APIs.io

Everything profiled for Liquity is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/liquity/](https://apis.io/providers/liquity/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Liquity V2 Protocol Stats API](https://apis.io/apis/liquity/liquity-v2-protocol-stats-api/) — Provides JSON snapshots of Liquity V2 (BOLD) protocol state including total BOLD supply, collateral values, stability pool deposits, TVL, per-branch…
- [Liquity V2 Website Data API](https://apis.io/apis/liquity/liquity-v2-website-data-api/) — Provides JSON data feeds used by the Liquity website including yield venue listings for BOLD, protocol fork venues, points leaderboard rankings, and…
- [Liquity V2 Governance API](https://apis.io/apis/liquity/liquity-v2-governance-api/) — Provides JSON snapshots of Liquity V2 governance state including active initiatives, epoch allocation data, and the latest completed governance epoch…
- [Liquity V1 Supply API](https://apis.io/apis/liquity/liquity-v1-supply-api/) — Liquity V1 circulating supply and BAMM stats endpoints.
- [Liquity V2 Governance API](https://apis.io/apis/liquity/liquity-v2-governance-api/) — Liquity V2 governance state including initiatives and epoch data.
- [Liquity V2 Protocol Stats API](https://apis.io/apis/liquity/liquity-v2-protocol-stats-api/) — Liquity V2 (BOLD) protocol state snapshots for mainnet and testnet.
- [Liquity V2 Website Data API](https://apis.io/apis/liquity/liquity-v2-website-data-api/) — Data feeds for the Liquity website including yield venues, leaderboard, and borrow rates.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Liquity Agentic Access](https://apis.io/agentic-access/liquity/liquity-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [GovernanceSchemas](https://apis.io/schemas/liquity/governance/)
- [Leaderboard](https://apis.io/schemas/liquity/leaderboard/)
- [ProtocolStats](https://apis.io/schemas/liquity/protocol-stats/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Liquity Context](https://apis.io/jsonld/liquity/liquity-context/)

#### Examples (3)

Example requests and responses.

- [Ethereum Protocol Stats](https://apis.io/examples/liquity/ethereum-protocol-stats/)
- [Governance Initiatives](https://apis.io/examples/liquity/governance-initiatives/)
- [Leaderboard](https://apis.io/examples/liquity/leaderboard/)

#### Collections (4)

Postman and Open Collection request collections.

- [Liquity Protocol V1 Supply API](https://apis.io/collections/liquity/open-liquity-v1-supply-api/)
- [Liquity Protocol V1 Supply V2 Governance API](https://apis.io/collections/liquity/open-liquity-v2-governance-api/)
- [Liquity Protocol V1 Supply V2 Protocol Stats API](https://apis.io/collections/liquity/open-liquity-v2-protocol-stats-api/)
- [Liquity Protocol V1 Supply V2 Website Data API](https://apis.io/collections/liquity/open-liquity-v2-website-data-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Liquity — jsonschema rules](https://apis.io/rules/liquity/liquity-jsonschema-spectral-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Liquity Domain Security](https://apis.io/security/liquity/liquity-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.liquity.org/)
- [Documentation](https://docs.liquity.org/)
- [Blog](https://www.liquity.org/blog)
- [Terms of service](https://www.liquity.org/terms)
- [Privacy policy](https://www.liquity.org/privacy)
- [GitHub](https://github.com/liquity)
- [Status](https://api.liquity.org/)

## API Evangelist rating

**Kin Score 29.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 53.9 |
| Contract governance | 9.8 |
| Operational transparency | 10.5 |
| Developer ergonomics | 21.4 |
| Access clarity | 10.5 |

**Agent readiness 22.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 14.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/liquity/](https://apis.io/providers/liquity/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Liquity: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/liquity/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
