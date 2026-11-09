---
acting_count: 0
action_class_counts:
  connected: 40
api_specs:
- filename: loopholetape-com-discovery-api-openapi.yml
  format: yaml
  label: loopholetape-com Discovery API
  slug: loopholetape-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopholetape-com/openapi/loopholetape-com-discovery-api-openapi.yml
- filename: loopholetape-com-free-api-openapi.yml
  format: yaml
  label: loopholetape-com Free API
  slug: loopholetape-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopholetape-com/openapi/loopholetape-com-free-api-openapi.yml
- filename: loopholetape-com-paid-api-openapi.yml
  format: yaml
  label: loopholetape-com Paid API
  slug: loopholetape-com-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/loopholetape-com/openapi/loopholetape-com-paid-api-openapi.yml
consequence_counts:
  read: 40
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Loopholetape Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 40
overview: 'loopholetape-com exposes 40 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: loopholetape-com
provider_slug: loopholetape-com
slug: loopholetape-com-agentic-access
source_filename: loopholetape-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/loopholetape-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 40\n  by_consequence:\n    read: 40\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: index__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calibration\n  method: get\n  operationId: calibration_v1_calibration_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/x402\n  method: get\n  operationId: well_known_x402__well_known_x402_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/labels\n  method: get\n  operationId: labels_v1_labels_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/market/regime\n  method: get\n  operationId: market_regime_v1_market_regime_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sample/launches\n  method: get\n  operationId: sample_launches_v1_sample_launches_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sample/rugs\n  method: get\n  operationId: sample_rugs_v1_sample_rugs_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sample/mint\n  method: get\n  operationId: sample_mint_v1_sample_mint_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets\n  method: get\n  operationId: datasets_index_v1_datasets_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/datasets/pumpfun_launches/{day}\n  method: get\n  operationId: dataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/track-record\n\
  \  method: get\n  operationId: track_record_view_v1_track_record_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/new\n  method: get\n  operationId: keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/trial\n  method: get\n  operationId: keys_trial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/balance\n  method: get\n  operationId: keys_balance_v1_keys_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/radar\n  method: get\n  operationId: radar_view_v1_radar_get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mint/{mint}\n  method: get\n  operationId: mint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mint/{mint}/holders\n  method: get\n  operationId: mint_holders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/mint/{mint}/flow\n  method: get\n  operationId: mint_flow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outcome/batch\n  method: get\n  operationId: outcome_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/outcome/{mint}\n  method: get\n  operationId:\
  \ outcome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/launches/since\n  method: get\n  operationId: launches_since\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/launches/screened\n  method: get\n  operationId: launches_screened\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/launches/recent\n  method: get\n  operationId: launches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rugs/recent\n  method: get\n  operationId: rugs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/graduations/recent\n  method: get\n  operationId: graduations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/creator/{address}\n  method: get\n  operationId: creator\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/wallet/{address}\n  method: get\n  operationId: wallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rhc/regime\n  method: get\n  operationId: rhc_regime_v1_rhc_regime_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/coverage\n  method: get\n  operationId: check_coverage_v1_check_coverage_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/watch\n  method: get\n  operationId: watchlist_updates_v1_check_watch_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/mint/{mint}\n  method: get\n  operationId: risk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/watchlist\n  method: get\n  operationId: risk_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/check/batch\n  method: get\n  operationId: check_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/verdict/{mint}\n  method: get\n  operationId: verdict\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rhc/launches/recent\n  method: get\n  operationId: rhc_launches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rhc/curve/{address}\n  method: get\n  operationId: rhc_curve\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rhc/curve/{address}/trades\n  method: get\n  operationId: rhc_trades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/token_check/{mint}\n  method: get\n  operationId: token_check\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/webhook\n  method: get\n  operationId: alerts_subscribe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/loopholetape-com/agentic-access/loopholetape-com-agentic-access.yml
summary_line: 40 operations
tags:
- Company
- Cryptocurrency
- Solana
- Risk Management
---
