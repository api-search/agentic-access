---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 23
api_specs:
- filename: kairossignal-com-brief-api-openapi.yml
  format: yaml
  label: kairossignal-com Brief API
  slug: kairossignal-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-brief-api-openapi.yml
- filename: kairossignal-com-credits-api-openapi.yml
  format: yaml
  label: kairossignal-com Credits API
  slug: kairossignal-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-credits-api-openapi.yml
- filename: kairossignal-com-export-api-openapi.yml
  format: yaml
  label: kairossignal-com Export API
  slug: kairossignal-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-export-api-openapi.yml
- filename: kairossignal-com-market-api-openapi.yml
  format: yaml
  label: kairossignal-com Market API
  slug: kairossignal-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-market-api-openapi.yml
- filename: kairossignal-com-mcp-api-openapi.yml
  format: yaml
  label: kairossignal-com MCP API
  slug: kairossignal-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-mcp-api-openapi.yml
- filename: kairossignal-com-network-api-openapi.yml
  format: yaml
  label: kairossignal-com Network API
  slug: kairossignal-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-network-api-openapi.yml
- filename: kairossignal-com-networks-api-openapi.yml
  format: yaml
  label: kairossignal-com Networks API
  slug: kairossignal-com-networks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-networks-api-openapi.yml
- filename: kairossignal-com-provenance-api-openapi.yml
  format: yaml
  label: kairossignal-com Provenance API
  slug: kairossignal-com-provenance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-provenance-api-openapi.yml
- filename: kairossignal-com-revenue-api-openapi.yml
  format: yaml
  label: kairossignal-com Revenue API
  slug: kairossignal-com-revenue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-revenue-api-openapi.yml
- filename: kairossignal-com-supply-api-openapi.yml
  format: yaml
  label: kairossignal-com Supply API
  slug: kairossignal-com-supply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-supply-api-openapi.yml
- filename: kairossignal-com-try-api-openapi.yml
  format: yaml
  label: kairossignal-com Try API
  slug: kairossignal-com-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-try-api-openapi.yml
- filename: kairossignal-com-x402-api-openapi.yml
  format: yaml
  label: kairossignal-com X402 API
  slug: kairossignal-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kairossignal-com/openapi/kairossignal-com-x402-api-openapi.yml
consequence_counts:
  physical: 1
  read: 23
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kairossignal Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/credits/purchase
operation_count: 26
overview: 'kairossignal-com exposes 26 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: kairossignal-com
provider_slug: kairossignal-com
slug: kairossignal-com-agentic-access
source_filename: kairossignal-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/kairossignal-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 3\n    connected: 23\n  by_consequence:\n    write: 2\n    read: 23\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /try\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/brief\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/pricing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/purchase\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/register\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/network/{symbol}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/networks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/provenance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/revenue\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/supply\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/purchases\n  method: get\n  operationId: listPurchases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/purchases/{purchase_id}\n  method: get\n  operationId: getPurchaseReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/depin_provenance\n  method: get\n  operationId: x402_depin_provenance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/depin_networks\n  method: get\n  operationId: x402_depin_networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/depin_revenue_snapshot\n  method: get\n  operationId: x402_depin_revenue_snapshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/node_quality_score\n  method: get\n  operationId: x402_node_quality_score\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /x402/v1/data/dilution_risk_map\n  method: get\n  operationId: x402_dilution_risk_map\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/gpu_supply_demand\n  method: get\n  operationId: x402_gpu_supply_demand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/sector_health_index\n  method: get\n  operationId: x402_sector_health_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/geo_concentration\n  method: get\n  operationId: x402_geo_concentration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/dev_velocity\n\
  \  method: get\n  operationId: x402_dev_velocity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /x402/v1/data/competitive_landscape\n  method: get\n  operationId: x402_competitive_landscape\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/kairossignal-com/agentic-access/kairossignal-com-agentic-access.yml
summary_line: 26 operations · 3 acting
tags:
- Company
- DePIN
- Data API
- Cryptocurrency
- Telemetry
- Analytics
---
