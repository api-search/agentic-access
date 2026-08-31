---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: landcor-avm-summary-api-openapi.yml
  format: yaml
  label: Landcor Data AVM Summary API
  slug: landcor-avm-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-avm-summary-api-openapi.yml
- filename: landcor-comparables-api-openapi.yml
  format: yaml
  label: Landcor Data Comparables API
  slug: landcor-comparables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-comparables-api-openapi.yml
- filename: landcor-health-api-openapi.yml
  format: yaml
  label: Landcor Data Health API
  slug: landcor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-health-api-openapi.yml
- filename: landcor-property-api-openapi.yml
  format: yaml
  label: Landcor Data Property API
  slug: landcor-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-property-api-openapi.yml
- filename: landcor-valuation-api-openapi.yml
  format: yaml
  label: Landcor Data Valuation API
  slug: landcor-valuation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/openapi/landcor-valuation-api-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Landcor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Landcor Data exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Landcor Data
provider_slug: landcor
slug: landcor-agentic-access
source_filename: landcor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/landcor-property-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/search\n  method: get\n  operationId: search_property_property_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /property/{pid}\n  method: get\n  operationId: read_property_property__pid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/{pid}/report/pdf\n  method: get\n  operationId: read_property_pdf_property__pid__report_pdf_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuationRange/{pid}\n  method: get\n  operationId: read_valuation_range_valuationRange__pid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuationRange/{pid}/updates\n  method: get\n  operationId: read_property_monthly_update_valuationRange__pid__updates_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /valuationRange/{pid}/history\n  method: get\n  operationId: read_valuation_history_valuationRange__pid__history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valuation/ltv-check\n  method: post\n  operationId: run_ltv_check_valuation_ltv_check_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valuation/neighbourhood/{neighbourhood_code}/{unit_type_code}/sales\n  method: get\n  operationId: read_neighbourhood_sales_series_valuation_neighbourhood__neighbourhood_code___unit_type_code__sales_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /comparables/{pid}\n  method: get\n  operationId: read_comparables_comparables__pid__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /address/autocomplete\n  method: get\n  operationId: autocomplete_address_address_autocomplete_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /generate-avm-summary\n  method: post\n  operationId: generate_avm_summary_generate_avm_summary_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landcor/refs/heads/main/agentic-access/landcor-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Real-Estate
- Canada
- Valuation
- AVM
- Property Records
- Title
- Land Registry
- Mortgage
- PropTech
- Property Data
---
