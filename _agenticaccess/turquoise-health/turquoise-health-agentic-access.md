---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 11
api_specs:
- filename: turquoise-health-consumer-pricing-openapi.yml
  format: yaml
  label: Turquoise Consumer Pricing API
  slug: turquoise-consumer-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/openapi/turquoise-health-consumer-pricing-openapi.yml
consequence_counts:
  read: 11
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Turquoise Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Turquoise Health exposes 15 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Turquoise Health
provider_slug: turquoise-health
slug: turquoise-health-agentic-access
source_filename: turquoise-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/turquoise-health-consumer-pricing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 11\n    acting: 4\n  by_consequence:\n    read: 11\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/providers/types\n  method: get\n  operationId: v3_get_provider_types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/providers\n  method: get\n  operationId: v3_list_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v3/providers/{provider_id}\n  method: get\n  operationId: v3_get_provider\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payers\n  method: get\n  operationId: v3_list_payers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/payers/{payer_id}\n  method: get\n  operationId: v3_get_payer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/networks\n  method: get\n  operationId: v3_list_networks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/networks/{network_id}\n  method: get\n  operationId: v3_get_network\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/packages\n  method: get\n  operationId: v3_list_packages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/packages/{package_id}\n  method: get\n  operationId: v3_get_package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/packages/{package_id}/line_items\n  method: get\n  operationId: v3_list_package_line_items\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/prices/query\n  method: post\n  operationId: v3_query_prices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/prices/compare\n  method: post\n  operationId: v3_compare_prices\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/prices/{price_id}\n  method: get\n  operationId: v3_get_price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/personalized-estimates\n  method: post\n  operationId: v3_list_personalized_estimates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/personalized-estimates/compare\n  method: post\n  operationId: v3_compare_personalized_estimates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turquoise-health/refs/heads/main/agentic-access/turquoise-health-agentic-access.yml
summary_line: 15 operations · 4 acting
tags:
- Healthcare
- Price Transparency
- Hospital Rates
- Payer Rates
- Machine-Readable Files
- FHIR
- Health Insurance
- Negotiated Rates
- Out-of-Pocket Costs
- MRF
- Consumer Pricing
- MCP
- Eligibility
- Standard Service Packages
- HIPAA
---
