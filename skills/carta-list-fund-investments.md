---
name: carta-list-fund-investments
description: Walk an investment firm's funds on Carta and list each fund's portfolio investments.
api: Carta API
operations:
  - get_v1alpha1_investors_firms
  - get_v1alpha1_investors_firms_firmid_funds
  - get_v1alpha1_investors_firms_firmid_funds_fundid_investments
---
Contract is GENERATED from docs.carta.com reference pages (x-generated-from: documentation).

1. `get_v1alpha1_investors_firms` (scope read_investor_firms) - page with `pageSize` (max 50) / `pageToken`, follow `nextPageToken`.
2. For each firm, `get_v1alpha1_investors_firms_firmid_funds`.
3. For each fund, `get_v1alpha1_investors_firms_firmid_funds_fundid_investments`.

Rules: OAuth 2.0 bearer token (1 hour lifetime); 10 req/s burst, 300 req/min - back off on 429; 403 INSUFFICIENT_SCOPE means the app lacks the scope.
