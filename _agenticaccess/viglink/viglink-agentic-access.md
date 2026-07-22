---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 14
api_specs:
- filename: viglink-link-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Link Check API
  slug: link-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-link-check-openapi.yml
- filename: viglink-bid-check-openapi.yml
  format: yaml
  label: Sovrn Commerce Bid Check API
  slug: bid-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-bid-check-openapi.yml
- filename: viglink-campaigns-openapi.yml
  format: yaml
  label: Sovrn Commerce Campaigns API
  slug: campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-campaigns-openapi.yml
- filename: viglink-reports-openapi.yml
  format: yaml
  label: Sovrn Commerce Real-Time Reports API
  slug: real-time-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-reports-openapi.yml
- filename: viglink-merchant-summaries-openapi.yml
  format: yaml
  label: Sovrn Commerce Merchant Group Summaries API
  slug: merchant-summaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-merchant-summaries-openapi.yml
- filename: viglink-product-recommendations-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Recommendations API
  slug: product-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-recommendations-openapi.yml
- filename: viglink-product-promo-codes-openapi.yml
  format: yaml
  label: Sovrn Commerce Product Promo Codes API
  slug: product-promo-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-product-promo-codes-openapi.yml
- filename: viglink-price-comparisons-openapi.yml
  format: yaml
  label: Sovrn Commerce Price Comparisons API
  slug: price-comparisons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/openapi/viglink-price-comparisons-openapi.yml
consequence_counts:
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Viglink Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'VigLink (Sovrn Commerce) exposes 16 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VigLink (Sovrn Commerce)
provider_slug: viglink
slug: viglink-agentic-access
source_filename: viglink-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/viglink-bid-check-openapi.yml, openapi/viglink-campaigns-openapi.yml, openapi/viglink-link-check-openapi.yml,\n  openapi/viglink-merchant-summaries-openapi.yml, openapi/viglink-price-comparisons-openapi.yml,\n  openapi/viglink-product-promo-codes-openapi.yml, openapi/viglink-product-recommendations-openapi.yml,\n  openapi/viglink-reports-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 14\n    acting: 2\n  by_consequence:\n    read: 14\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/bid\n  method: get\n  operationId: getBid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/campaigns/{search}\n  method: get\n  operationId: campaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/\n  method: get\n  operationId: link\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /summaries\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /summaries/delta\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{site-api-key}/compare/prices/{market}/by/accuracy\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /product\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-orchestration/products\n  method: post\n  operationId: get_product_recommendations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reports/transactions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchants\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchantsbydate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/links\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/pages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/merchandise\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reports/networks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /reports/cuids\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viglink/refs/heads/main/agentic-access/viglink-agentic-access.yml
summary_line: 16 operations · 2 acting
tags:
- Affiliate Marketing
- Commerce
- Monetization
- Publishers
- Links
- Advertising
- Reporting
---
