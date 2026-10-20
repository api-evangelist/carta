---
name: carta-book-capital-call
description: Book a capital call for a fund on Carta and read it back.
api: Carta API
operations:
  - get_v1alpha1_investors_firms_firmid_funds
  - post_v1alpha1_investors_firms_firmid_funds_fundid_capitalCalls
  - get_v1alpha1_investors_firms_firmid_funds_fundid_capitalCalls_capitalcallid
---
Contract is GENERATED from docs.carta.com reference pages. Guide: https://docs.carta.com/api-platform/guides/guides/booking-capital-calls

1. Resolve the fund with `get_v1alpha1_investors_firms_firmid_funds`.
2. Create with `post_v1alpha1_investors_firms_firmid_funds_fundid_capitalCalls`.
3. Confirm with `get_v1alpha1_investors_firms_firmid_funds_fundid_capitalCalls_capitalcallid`.

No idempotency key is documented: do not blindly retry a POST after a timeout; read back first. No documented reversal operation.
