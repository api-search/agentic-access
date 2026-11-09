---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 15
api_specs:
- filename: ticexplorer-com-admin-api-openapi.yml
  format: yaml
  label: ticexplorer-com Admin API
  slug: ticexplorer-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-admin-api-openapi.yml
- filename: ticexplorer-com-analytics-api-openapi.yml
  format: yaml
  label: ticexplorer-com Analytics API
  slug: ticexplorer-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-analytics-api-openapi.yml
- filename: ticexplorer-com-claims-api-openapi.yml
  format: yaml
  label: ticexplorer-com Claims API
  slug: ticexplorer-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-claims-api-openapi.yml
- filename: ticexplorer-com-codes-api-openapi.yml
  format: yaml
  label: ticexplorer-com Codes API
  slug: ticexplorer-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-codes-api-openapi.yml
- filename: ticexplorer-com-guide-api-openapi.yml
  format: yaml
  label: ticexplorer-com Guide API
  slug: ticexplorer-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-guide-api-openapi.yml
- filename: ticexplorer-com-plans-api-openapi.yml
  format: yaml
  label: ticexplorer-com Plans API
  slug: ticexplorer-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-plans-api-openapi.yml
- filename: ticexplorer-com-providers-api-openapi.yml
  format: yaml
  label: ticexplorer-com Providers API
  slug: ticexplorer-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-providers-api-openapi.yml
- filename: ticexplorer-com-rates-api-openapi.yml
  format: yaml
  label: ticexplorer-com Rates API
  slug: ticexplorer-com-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-rates-api-openapi.yml
consequence_counts:
  read: 15
  safety-critical: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Ticexplorer Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/admin/keys/{key_id}
operation_count: 21
overview: 'ticexplorer-com exposes 21 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read, 5 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ticexplorer-com
provider_slug: ticexplorer-com
slug: ticexplorer-com-agentic-access
source_filename: ticexplorer-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/ticexplorer-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 15\n    acting: 6\n  by_consequence:\n    read: 15\n    write: 5\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/plans\n  method: get\n  operationId: find_plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/plans/{plan_id}\n  method: get\n  operationId: get_plan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/providers\n\
  \  method: get\n  operationId: find_providers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/codes\n  method: get\n  operationId: find_codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rates\n  method: post\n  operationId: get_rates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rates/batch\n  method: post\n  operationId: get_rates_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claims/price\n  method: post\n  operationId: price_claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/estimate\n  method: post\n  operationId: estimate_market_analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/jobs\n  method: post\n  operationId: start_market_analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/jobs\n  method: get\n  operationId: list_market_analyses\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/jobs/{job_id}\n  method: get\n  operationId: get_market_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/analytics/jobs/{job_id}\n  method: delete\n  operationId: cancel_market_analysis\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/analytics/jobs/{job_id}/export\n  method: get\n  operationId: export_market_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/guide\n  method:\
  \ get\n  operationId: guide_index\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/guide/{topic}\n  method: get\n  operationId: guide_topic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows\n  method: get\n  operationId: list_workflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workflows/{workflow_id}\n  method: get\n  operationId: get_workflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: whoami\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/admin/keys\n  method: get\n  operationId: list_api_keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/admin/keys\n  method: post\n  operationId: create_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/admin/keys/{key_id}\n  method: delete\n  operationId: revoke_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/ticexplorer-com/agentic-access/ticexplorer-com-agentic-access.yml
summary_line: 21 operations · 6 acting · 1 human-in-the-loop
tags:
- Health
- Finance
- Transparency
- Healthcare
---
