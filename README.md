# awesome-tiktok-ads-api

> Curated list of resources for working with the TikTok for Business
> Marketing API: official docs, SDKs, tutorials, and tooling.
> Maintained by [Julian Reiter](https://github.com/ArtificialIntelligentGeneration).


[![License: CC0](https://img.shields.io/badge/license-CC0-blue.svg)](LICENSE)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#contributing)

## Contents

- [Official](#official)
- [Official SDKs](#official-sdks)
- [Reporting permission category](#reporting-permission-category)
- [Tutorials & write-ups](#tutorials--write-ups)
- [Open-source tools](#open-source-tools)
- [Community / forums](#community--forums)
- [Compliance / policy reading](#compliance--policy-reading)
- [Contributing](#contributing)

## Official

- [TikTok for Business Marketing API portal](https://business-api.tiktok.com/portal/) — where you create apps and request permission categories.
- [Marketing API documentation](https://business-api.tiktok.com/portal/docs?id=1738373164380162) — endpoint reference.
- [Permission categories overview](https://business-api.tiktok.com/portal/docs?id=1738373164380162) — Reporting, Ads Management, Creative Management, Account Management.
- [OAuth 2.0 authorization flow](https://business-api.tiktok.com/portal/docs?id=1738373164380162) — `auth/?app_id=...` → `oauth2/access_token/`.
- [Rate limits & quotas](https://business-api.tiktok.com/portal/docs?id=1738373164380162) — by app, by endpoint, by advertiser.
- [Status & changelog](https://business-api.tiktok.com/portal/docs?id=1738373164380162) — version-controlled API changes.

## Official SDKs

- [Python SDK](https://github.com/tiktok/tiktok-business-api-sdk) — `business_api_client` package.
- [Node.js / TypeScript SDK](https://github.com/tiktok/tiktok-business-api-sdk) — same monorepo.
- [PHP SDK](https://github.com/tiktok/tiktok-business-api-sdk) — same monorepo.
- [Java SDK](https://github.com/tiktok/tiktok-business-api-sdk) — same monorepo.

## Reporting permission category

- [Report endpoint reference](https://business-api.tiktok.com/portal/docs?id=1738864928947202) — `/report/integrated/get/`.
- [Available metrics](https://business-api.tiktok.com/portal/docs?id=1738864928947202) — spend, clicks, impressions, conversions, derived ratios.
- [Dimensions](https://business-api.tiktok.com/portal/docs?id=1738864928947202) — campaign, ad group, ad, country, placement.

> **Rate-limit cheatsheet (Reporting category):** ~1 request/sec per advertiser, ~600/hr per app. Async report endpoint exempts the synchronous size cap (~30 days × 100 dimensions).

- [Async report endpoint](https://business-api.tiktok.com/portal/docs?id=1738864928947202) — for queries above the synchronous size cap.

## Tutorials & write-ups

- [How to pull TikTok Ads reports to Google Sheets](https://aigen-agency.com/blog/tiktok-ads-google-sheets) — step-by-step, uses [aigen-reports](https://github.com/ArtificialIntelligentGeneration/aigen-reports).
- Add a tutorial here? Open a PR.

## Open-source tools

- [aigen-reports](https://github.com/ArtificialIntelligentGeneration/aigen-reports) — read-only CLI to pull reports to CSV / Sheets / webhook. MIT.
- Add yours here.

## Community / forums

- [TikTok for Business Help Center](https://business.tiktok.com/help/) — non-developer support.
- [TikTok Developer Community on Discord](https://discord.gg/tiktok-developers) — unofficial, but most useful real-time channel.


## Data protection

- TikTok Marketing API returns aggregated metrics (no end-user PII); no DSR (data-subject-request) handling required for Reporting category.
- Tokens are advertiser-scoped — one OAuth grant per advertiser, store encrypted at rest.
- TikTok's [API privacy supplement](https://business-api.tiktok.com/portal/docs?id=1738864928947202) is the source of truth for retention rules.

## Compliance / policy reading

- [TikTok Developer Terms of Service](https://developers.tiktok.com/doc/tiktok-api-terms-of-service/).
- [TikTok Marketing API privacy policy supplement](https://business-api.tiktok.com/portal/docs?id=1738864928947202).
- [App review guidelines](https://business-api.tiktok.com/portal/docs?id=1738864928947202) — what reviewers check before approving an app.

## License

[CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/) — public domain.

## Contributing

Open an issue or PR. Keep entries one line. No commercial spam, no
"awesome lists" inception.
