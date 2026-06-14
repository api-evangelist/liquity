# Liquity API Plans

Liquity is a fully decentralized, governance-free protocol. The public API
at api.liquity.org is an open, static JSON/text file service with no
authentication, no rate limits, and no paid tiers. All endpoints are freely
accessible without an API key.

## Access Model

| Tier | Cost | Auth Required | Rate Limits |
|------|------|---------------|-------------|
| Public | Free | None | None (GitHub Pages) |

## Notes

- All data files are served from GitHub Pages (api.liquity.org), which is
  backed by GitHub's CDN. There are no explicit rate limits beyond GitHub's
  standard CDN policies.
- On-chain data is fetched via Alchemy or Infura RPC providers by the Liquity
  team's cron jobs and published as static files. Consumers read static files,
  not a live API server.
- The Liquity SDK packages (`@liquity/lib-ethers`, `@liquity/lib-base`, etc.)
  provide direct on-chain access via Ethereum JSON-RPC — those require a
  personal Alchemy, Infura, or similar RPC endpoint.
- No SLA, uptime commitment, or commercial support tier is offered for the
  API. Developers requiring guarantees should query on-chain directly.

## Developer Resources

- GitHub: https://github.com/liquity/api.liquity.org
- V1 Docs: https://docs.liquity.org/liquity-v1
- V2 Docs: https://docs.liquity.org/
- Discord: https://discord.gg/2up5U32
