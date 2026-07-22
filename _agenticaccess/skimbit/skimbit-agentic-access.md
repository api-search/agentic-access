---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 18
api_specs:
- filename: skimbit-merchant-openapi.yml
  format: yaml
  label: Skimlinks Merchant API
  slug: skimlinks-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-merchant-openapi.yml
- filename: skimbit-reporting-openapi.yml
  format: yaml
  label: Skimlinks Reporting API
  slug: skimlinks-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-reporting-openapi.yml
- filename: skimbit-product-key-openapi.yml
  format: yaml
  label: Skimlinks Product Key API
  slug: skimlinks-product-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-product-key-openapi.yml
consequence_counts:
  read: 18
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Skimbit Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'SkimBit exposes 19 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SkimBit
provider_slug: skimbit
slug: skimbit-agentic-access
source_filename: skimbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/skimbit-merchant-openapi.yml, openapi/skimbit-product-key-openapi.yml, openapi/skimbit-reporting-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 18\n    acting: 1\n  by_consequence:\n    read: 18\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v4/publisher/{publisher_id}/merchants\n  method: get\n  operationId: listMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/publisher/{publisher_id}/domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/verticals\n  method: get\n  operationId: listVerticals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/alternative_verticals\n  method: get\n  operationId: listAlternativeVerticals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/publisher/{publisher_id}/offers\n  method: get\n  operationId: listOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/product\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/publisher/{publisher_id}/products\n  method: post\n  operationId: getMultiProducts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /publisher/{publisher_id}/commission-report\n  method: get\n  operationId: searchCommissions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/reports\n  method: get\n  operationId: getAggregatedReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/link-report\n  method: get\n  operationId: getLinkReport\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/link-report/dimensions\n  method: get\n  operationId: getLinkReportDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/link-report/metrics\n  method: get\n  operationId: getLinkReportMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/page-report\n  method: get\n  operationId: getPageReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/page-report/dimensions\n  method: get\n  operationId:\
  \ getPageReportDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/aggregation/v1/page-report/metrics\n  method: get\n  operationId: getPageReportMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/trending-products\n  method: get\n  operationId: getTrendingProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/product-report\n  method: get\n  operationId: getProductBoughtReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/payment-status\n  method:\
  \ get\n  operationId: getPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /publisher/{publisher_id}/deactivated-merchants\n  method: get\n  operationId: getDeactivatedMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/agentic-access/skimbit-agentic-access.yml
summary_line: 19 operations · 1 acting
tags:
- Company
- Affiliate Marketing
- Content Monetization
- Commerce
- Publishers
- Advertising
- Retail
- Reporting
- Products
- eCommerce
---
