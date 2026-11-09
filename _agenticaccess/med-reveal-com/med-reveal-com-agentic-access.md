---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 13
api_specs:
- filename: med-reveal-com-benchmarking-api-api-openapi.yml
  format: yaml
  label: MedReveal Benchmarking API
  slug: med-reveal-com-benchmarking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-benchmarking-api-api-openapi.yml
- filename: med-reveal-com-health-api-openapi.yml
  format: yaml
  label: MedReveal Health API
  slug: med-reveal-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-health-api-openapi.yml
- filename: med-reveal-com-market-api-api-openapi.yml
  format: yaml
  label: MedReveal Market API
  slug: med-reveal-com-market-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-market-api-api-openapi.yml
- filename: med-reveal-com-npi-api-api-openapi.yml
  format: yaml
  label: MedReveal Npi API
  slug: med-reveal-com-npi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-npi-api-api-openapi.yml
- filename: med-reveal-com-provider-api-api-openapi.yml
  format: yaml
  label: MedReveal Provider API
  slug: med-reveal-com-provider-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-provider-api-api-openapi.yml
- filename: med-reveal-com-taxonomy-api-api-openapi.yml
  format: yaml
  label: MedReveal Taxonomy API
  slug: med-reveal-com-taxonomy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-taxonomy-api-api-openapi.yml
- filename: med-reveal-com-tin-api-api-openapi.yml
  format: yaml
  label: MedReveal Tin API
  slug: med-reveal-com-tin-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-tin-api-api-openapi.yml
- filename: med-reveal-com-usage-api-api-openapi.yml
  format: yaml
  label: MedReveal Usage API
  slug: med-reveal-com-usage-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-usage-api-api-openapi.yml
consequence_counts:
  read: 13
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Med Reveal Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'MedReveal exposes 16 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: MedReveal
provider_slug: med-reveal-com
slug: med-reveal-com-agentic-access
source_filename: med-reveal-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/med-reveal-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 13\n    acting: 3\n  by_consequence:\n    read: 13\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/search\n  method: post\n  operationId: market_search_api_v1_market_search_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/market/filters\n  method: get\n  operationId: get_market_filters_api_v1_market_filters_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/benchmarking\n  method: post\n  operationId: get_market_benchmarks_api_v1_market_benchmarking_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/market/benchmarking/info\n  method: get\n  operationId: get_benchmarking_info_api_v1_market_benchmarking_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/npis/{npi}\n  method: get\n  operationId: get_npi_api_v1_npis__npi__get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/npis\n  method: post\n  operationId: batch_lookup_npis_api_v1_npis_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tins/{tin}\n  method: get\n  operationId: get_tin_api_v1_tins__tin__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tins\n  method: post\n  operationId: batch_lookup_tins_api_v1_tins_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tins/{tin}/npis\n  method: get\n  operationId: get_tin_npis_api_v1_tins__tin__npis_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/npiSearch\n  method: post\n  operationId: search_npi_endpoint_api_v1_npiSearch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tinSearch\n  method: post\n  operationId: search_tin_endpoint_api_v1_tinSearch_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: get_usage_api_v1_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/taxonomy/{code}\n  method: get\n  operationId: get_taxonomy_api_v1_taxonomy__code__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provider/searchrates\n  method: post\n  operationId: search_provider_rates_api_v1_provider_searchrates_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/provider/searchrates/info\n  method: get\n  operationId: get_provider_search_info_api_v1_provider_searchrates_info_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/med-reveal-com/agentic-access/med-reveal-com-agentic-access.yml
summary_line: 16 operations · 3 acting
tags:
- Company
- Healthcare
- Pricing
- Data Analytics
- MCP
---
