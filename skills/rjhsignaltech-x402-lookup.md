---
name: rjhsignaltech-x402-lookup
description: Perform a paid x402 lookup using the provider's API.
api: openapi/whorepresents.openapi.json
operations:
- x402Lookup
- x402LookupPost
generated: '2026-09-25'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/whorepresents.openapi.json ; every operationId checked against the contract
---

# rjhsignaltech-x402-lookup

Perform a paid x402 lookup using the provider's API.

## Steps

1. 1. Call `x402Lookup` with the required query parameters (if any) and include the `X-API-Key` header for authentication.
2. 2. If the caller prefers a POST request, call `x402LookupPost` with a JSON body containing the lookup data and include the `X-API-Key` header.

## Rules

- Authentication: Provide the API key in the `X-API-Key` request header.
- Error handling: The endpoint always returns HTTP 402 with x402 requirements and a cost of 0.003 USDC.
