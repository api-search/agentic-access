---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 26
api_specs:
- filename: anansidata-xyz-admin-api-openapi.yml
  format: yaml
  label: Anansi Data Admin API
  slug: anansidata-xyz-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-admin-api-openapi.yml
- filename: anansidata-xyz-anansi-data-api-openapi.yml
  format: yaml
  label: Anansi Data Anansi Data API
  slug: anansidata-xyz-anansi-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-anansi-data-api-openapi.yml
- filename: anansidata-xyz-catalog-api-openapi.yml
  format: yaml
  label: Anansi Data Catalog API
  slug: anansidata-xyz-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-catalog-api-openapi.yml
- filename: anansidata-xyz-datasets-api-openapi.yml
  format: yaml
  label: Anansi Data Datasets API
  slug: anansidata-xyz-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-datasets-api-openapi.yml
- filename: anansidata-xyz-free-api-openapi.yml
  format: yaml
  label: Anansi Data Free API
  slug: anansidata-xyz-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-free-api-openapi.yml
- filename: anansidata-xyz-holder-api-openapi.yml
  format: yaml
  label: Anansi Data Holder API
  slug: anansidata-xyz-holder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-holder-api-openapi.yml
- filename: anansidata-xyz-launchpad-api-openapi.yml
  format: yaml
  label: Anansi Data Launchpad API
  slug: anansidata-xyz-launchpad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-launchpad-api-openapi.yml
- filename: anansidata-xyz-llms-txt-api-openapi.yml
  format: yaml
  label: Anansi Data Llms.txt API
  slug: anansidata-xyz-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-llms-txt-api-openapi.yml
- filename: anansidata-xyz-paid-api-openapi.yml
  format: yaml
  label: Anansi Data Paid API
  slug: anansidata-xyz-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-paid-api-openapi.yml
- filename: anansidata-xyz-stats-api-openapi.yml
  format: yaml
  label: Anansi Data Stats API
  slug: anansidata-xyz-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-stats-api-openapi.yml
- filename: anansidata-xyz-well-known-api-openapi.yml
  format: yaml
  label: Anansi Data .well Known API
  slug: anansidata-xyz-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anansidata-xyz/openapi/anansidata-xyz-well-known-api-openapi.yml
consequence_counts:
  read: 26
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anansidata Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 29
overview: 'Anansi Data exposes 29 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anansi Data
provider_slug: anansidata-xyz
slug: anansidata-xyz-agentic-access
source_filename: anansidata-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anansidata-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 26\n    acting: 3\n  by_consequence:\n    read: 26\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /admin/settlements\n  method: get\n  operationId: settlements_admin_settlements_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog\n  method:\
  \ get\n  operationId: index_catalog_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/search\n  method: get\n  operationId: free_search_free_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/sample\n  method: get\n  operationId: free_sample_free_sample_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/price/current\n  method: get\n  operationId: free_price_current_free_price_current_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /free/price/changes\n  method: get\n  operationId: free_price_changes_free_price_changes_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /holder/tiers\n  method: get\n  operationId: holder_tiers_holder_tiers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /holder/challenge\n  method: get\n  operationId: holder_challenge_holder_challenge_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /holder/session\n  method: post\n  operationId: holder_session_holder_session_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/x402.json\n  method: get\n  operationId: well_known_x402__well_known_x402_json_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: well_known_x402__well_known_x402_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets\n  method: get\n  operationId: list_datasets_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: stats_stats_get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/search/web\n  method: get\n  operationId: paid_search_web_paid_search_web_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/data/all\n  method: get\n  operationId: paid_data_all_paid_data_all_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/quote\n  method: get\n  operationId: paid_quote_paid_quote_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/data/latest\n  method: get\n  operationId: paid_latest_paid_data_latest_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /paid/intel/verdict\n  method: get\n  operationId: paid_verdict_paid_intel_verdict_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/data/search\n  method: get\n  operationId: paid_search_paid_data_search_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/intel/movers\n  method: get\n  operationId: paid_movers_paid_intel_movers_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/intel/anomalies\n  method: get\n  operationId: paid_anomalies_paid_intel_anomalies_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /paid/data/history\n  method: get\n  operationId: paid_history_paid_data_history_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/data/changes\n  method: get\n  operationId: paid_changes_paid_data_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/intel/model-advisor\n  method: get\n  operationId: paid_model_advisor_paid_intel_model_advisor_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paid/intel/model-changes\n  method: get\n  operationId: paid_model_changes_paid_intel_model_changes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /paid/extract\n  method: post\n  operationId: paid_extract_paid_extract_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /launchpad/reserve\n  method: post\n  operationId: launchpad_reserve_launchpad_reserve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/anansidata-xyz/agentic-access/anansidata-xyz-agentic-access.yml
summary_line: 29 operations · 3 acting
tags:
- Data
- Blockchain
- Payments
- Marketplace
---
