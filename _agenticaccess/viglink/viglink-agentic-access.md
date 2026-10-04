---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 15
api_specs:
- filename: viglink-account-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Account API
  slug: viglink-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-account-api-openapi.yml
- filename: viglink-ai-orchestration-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Ai Orchestration API
  slug: viglink-ai-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-ai-orchestration-api-openapi.yml
- filename: viglink-bid-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Bid API
  slug: viglink-bid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-api-openapi.yml
- filename: viglink-link-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Link API
  slug: viglink-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-api-openapi.yml
- filename: viglink-merchant-group-summaries-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Merchant Group Summaries API
  slug: viglink-merchant-group-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-group-summaries-api-openapi.yml
- filename: viglink-product-coupons-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Product Coupons API
  slug: viglink-product-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-coupons-api-openapi.yml
- filename: viglink-reports-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) reports API
  slug: viglink-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-api-openapi.yml
- filename: viglink-sites-api-openapi.yml
  format: yaml
  label: VigLink (Sovrn Commerce) Sites API
  slug: viglink-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-sites-api-openapi.yml
consequence_counts:
  read: 15
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Viglink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'VigLink (Sovrn Commerce) exposes 16 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VigLink (Sovrn Commerce)
provider_slug: viglink
slug: viglink-agentic-access
source_filename: viglink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/viglink-account-api-openapi.yml, openapi/viglink-ai-orchestration-api-openapi.yml,\n  openapi/viglink-bid-api-openapi.yml, openapi/viglink-link-api-openapi.yml, openapi/viglink-merchant-group-summaries-api-openapi.yml,\n  openapi/viglink-product-coupons-api-openapi.yml, openapi/viglink-reports-api-openapi.yml,\n  openapi/viglink-sites-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 15\n    acting: 1\n  by_consequence:\n    read: 15\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /account/campaigns/{search}\n  method: get\n  operationId: campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-orchestration/products\n  method: post\n  operationId: get_product_recommendations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/bid\n  method: get\n  operationId: getBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/\n  method: get\n  operationId: link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summaries\n  method: post\n  operationId: postSummaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /summaries/delta\n  method: get\n  operationId: getSummariesDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/transactions\n  method: get\n  operationId: getReportsTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchants\n  method: get\n  operationId: getReportsMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchantsbydate\n  method: get\n  operationId:\
  \ getReportsMerchantsbydate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/links\n  method: get\n  operationId: getReportsLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/pages\n  method: get\n  operationId: getReportsPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchandise\n  method: get\n  operationId: getReportsMerchandise\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/networks\n  method: get\n  operationId: getReportsNetworks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/cuids\n  method: get\n  operationId: getReportsCuids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site-api-key}/compare/prices/{market}/by/accuracy\n  method: get\n  operationId: getSitesBySiteApiKeyComparePricesByMarketByAccuracy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/agentic-access/viglink-agentic-access.yml
summary_line: 16 operations · 1 acting
tags:
- Affiliate Marketing
- Commerce
- Monetization
- Publishers
- Links
- Advertising
- Reporting
---
