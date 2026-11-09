---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 18
api_specs:
- filename: canlicapital-com-chain-api-openapi.yml
  format: yaml
  label: canlicapital-com Chain API
  slug: canlicapital-com-chain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-chain-api-openapi.yml
- filename: canlicapital-com-keys-api-openapi.yml
  format: yaml
  label: canlicapital-com Keys API
  slug: canlicapital-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-keys-api-openapi.yml
- filename: canlicapital-com-receipts-api-openapi.yml
  format: yaml
  label: canlicapital-com Receipts API
  slug: canlicapital-com-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-receipts-api-openapi.yml
- filename: canlicapital-com-record-api-openapi.yml
  format: yaml
  label: canlicapital-com Record API
  slug: canlicapital-com-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-record-api-openapi.yml
- filename: canlicapital-com-research-api-openapi.yml
  format: yaml
  label: canlicapital-com Research API
  slug: canlicapital-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-research-api-openapi.yml
- filename: canlicapital-com-sleeves-api-openapi.yml
  format: yaml
  label: canlicapital-com Sleeves API
  slug: canlicapital-com-sleeves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-sleeves-api-openapi.yml
- filename: canlicapital-com-status-api-openapi.yml
  format: yaml
  label: canlicapital-com Status API
  slug: canlicapital-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-status-api-openapi.yml
- filename: canlicapital-com-trials-api-openapi.yml
  format: yaml
  label: canlicapital-com Trials API
  slug: canlicapital-com-trials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-trials-api-openapi.yml
- filename: canlicapital-com-validate-api-openapi.yml
  format: yaml
  label: canlicapital-com Validate API
  slug: canlicapital-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canlicapital-com/openapi/canlicapital-com-validate-api-openapi.yml
consequence_counts:
  read: 18
  safety-critical: 4
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Canlicapital Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/keys/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/keys/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/validate/luck-trials
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/validate/luck-trials
operation_count: 40
overview: 'canlicapital-com exposes 40 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 18 write, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: canlicapital-com
provider_slug: canlicapital-com
slug: canlicapital-com-agentic-access
source_filename: canlicapital-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/canlicapital-com-openapi-site.json, openapi/canlicapital-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 40\n  by_action_class:\n    connected: 18\n    acting: 22\n  by_consequence:\n    read: 18\n    safety-critical: 4\n    write: 18\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/chain/head\n  method: get\n  operationId: chain_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/record\n  method: get\n  operationId: record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/research\n  method: get\n  operationId: research\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sleeves\n  method: get\n  operationId: sleeves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trials/summary\n  method: get\n  operationId: trials_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/revoke\n  method: post\n  operationId: keys_revoke\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/keys\n  method: post\n  operationId: keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/deflated-sharpe\n  method: post\n  operationId: validate_deflated_sharpe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/overfitting\n\
  \  method: post\n  operationId: validate_overfitting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/paper-evidence\n  method: post\n  operationId: validate_paper_evidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/breadth\n  method: post\n  operationId: validate_breadth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/track-record\n  method: post\n  operationId: validate_track_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/backtest-length\n  method: post\n  operationId: validate_backtest_length\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/haircut-sharpe\n  method: post\n  operationId: validate_haircut_sharpe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/luck-trials\n  method: post\n  operationId: validate_luck_trials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/validate/reality-check\n  method: post\n  operationId: validate_reality_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/status\n  method:\
  \ get\n  operationId: validate_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{id}\n  method: get\n  operationId: receipts_id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{id}/badge.svg\n  method: get\n  operationId: receipts_id_badge_svg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/chain/head\n  method: get\n  operationId: chain_head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/record\n  method: get\n  operationId: record\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/research\n  method: get\n  operationId: research\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sleeves\n  method: get\n  operationId: sleeves\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trials/summary\n  method: get\n  operationId: trials_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/revoke\n  method: post\n  operationId: keys_revoke\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/keys\n  method: post\n  operationId: keys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/deflated-sharpe\n  method: post\n  operationId: validate_deflated_sharpe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/validate/overfitting\n  method: post\n  operationId: validate_overfitting\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/paper-evidence\n  method: post\n  operationId: validate_paper_evidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/breadth\n  method: post\n  operationId: validate_breadth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/track-record\n  method: post\n  operationId: validate_track_record\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/backtest-length\n  method: post\n  operationId: validate_backtest_length\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/haircut-sharpe\n  method: post\n  operationId: validate_haircut_sharpe\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/validate/luck-trials\n  method: post\n  operationId: validate_luck_trials\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/validate/reality-check\n  method: post\n  operationId: validate_reality_check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/v1/validate/status\n  method: get\n  operationId: validate_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{id}\n  method: get\n  operationId: receipts_id_\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/receipts/{id}/badge.svg\n  method: get\n  operationId: receipts_id_badge_svg\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/canlicapital-com/agentic-access/canlicapital-com-agentic-access.yml
summary_line: 40 operations · 22 acting · 4 human-in-the-loop
tags:
- Finance
- Data
- Artificial Intelligence
- QuantitativeTools
- Developer API
---
