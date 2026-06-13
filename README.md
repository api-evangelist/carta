# Carta

Carta is an equity management platform offering a REST API for cap table management, 409A valuations, fund administration, employee equity plans, and investor portfolio management. Carta's Developer Platform exposes five API suites — Launch, Investor, Issuer, Portfolio, and CRM — authenticated via OAuth 2.0.

## API Suites

| API | Purpose |
|-----|---------|
| Launch | Incorporation partners and law firms onboard new companies programmatically |
| Investor | Fund operators retrieve cap table summaries and portfolio position data |
| Issuer | Law firms and tech partners access cap table data on behalf of companies |
| Portfolio | Personal finance platforms aggregate individual equity holdings |
| CRM | Deal and fundraising relationship management for fund operators |

## Authentication

OAuth 2.0 is the primary authentication method, supporting:
- Authorization Code Flow (user-delegated access)
- Client Credentials Flow (service-to-service)
- OpenID Connect

## Access Model

Partner API access is invite-only and requires a valid SOC 2 Type 2 certification. Carta customers (companies and investment firms) may request access to their own data on demand.

A sandbox/mock environment is available at `https://mock-api.carta.com` without production credentials.

## Rate Limits

| Environment | Burst | Sustained |
|-------------|-------|-----------|
| Sandbox | 5 req/s | 150 req/min |
| Production | Per partner agreement | Per partner agreement |

## Links

- Website: https://carta.com
- Developer Platform: https://carta.com/api/
- Documentation: https://docs.carta.com/api-platform/docs/introduction
- GitHub: https://github.com/carta
- LinkedIn: https://www.linkedin.com/company/carta--
- Blog: https://carta.com/blog/
- Status Page: https://status.carta.com
- Pricing: https://carta.com/plans/pricing-for-investors/

## APIs.json

This repository contains an [APIs.json](apis.yml) index conforming to specification version 0.19.
