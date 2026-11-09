---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 11
api_specs:
- filename: vigotime-com-account-api-openapi.yml
  format: yaml
  label: vigotime-com Account API
  slug: vigotime-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vigotime-com/openapi/vigotime-com-account-api-openapi.yml
- filename: vigotime-com-api-tokens-api-openapi.yml
  format: yaml
  label: vigotime-com API Tokens API
  slug: vigotime-com-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vigotime-com/openapi/vigotime-com-api-tokens-api-openapi.yml
- filename: vigotime-com-health-api-openapi.yml
  format: yaml
  label: vigotime-com Health API
  slug: vigotime-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vigotime-com/openapi/vigotime-com-health-api-openapi.yml
- filename: vigotime-com-signup-api-openapi.yml
  format: yaml
  label: vigotime-com Signup API
  slug: vigotime-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vigotime-com/openapi/vigotime-com-signup-api-openapi.yml
- filename: vigotime-com-stateless-solve-api-openapi.yml
  format: yaml
  label: vigotime-com Stateless Solve API
  slug: vigotime-com-stateless-solve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vigotime-com/openapi/vigotime-com-stateless-solve-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 1
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Vigotime Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/v1/tokens/{token_id}
operation_count: 16
overview: 'vigotime-com exposes 16 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 4 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: vigotime-com
provider_slug: vigotime-com
slug: vigotime-com-agentic-access
source_filename: vigotime-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/vigotime-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 11\n    acting: 5\n  by_consequence:\n    read: 11\n    write: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/account/balance\n  method: get\n  operationId: get_balance_api_v1_account_balance_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/packages\n  method: get\n  operationId: get_packages_api_v1_account_packages_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account/usage\n  method: get\n  operationId: get_usage_api_v1_account_usage_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/signup\n  method: post\n  operationId: request_signup_api_v1_signup_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/signup/verify\n  method: post\n  operationId: verify_signup_api_v1_signup_verify_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/v1/solve\n  method: get\n  operationId: list_solve_jobs_api_v1_solve_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/solve\n  method: post\n  operationId: submit_solve_api_v1_solve_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/solve/stats\n  method: get\n  operationId: get_solve_stats_api_v1_solve_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/solve/{job_id}\n  method: get\n  operationId: get_solve_status_api_v1_solve__job_id__get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/solve/{job_id}/result\n  method: get\n  operationId: get_solve_result_api_v1_solve__job_id__result_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tokens\n  method: get\n  operationId: list_tokens_api_v1_tokens_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/tokens\n  method: post\n  operationId: issue_token_api_v1_tokens_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/tokens/{token_id}\n\
  \  method: delete\n  operationId: revoke_token_api_v1_tokens__token_id__delete\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /health\n  method: get\n  operationId: health_check_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: liveness_check_live_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ready\n  method: get\n  operationId: readiness_check_ready_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/vigotime-com/agentic-access/vigotime-com-agentic-access.yml
summary_line: 16 operations · 5 acting · 1 human-in-the-loop
tags:
- Company
- Scheduling
- Time Tracking
- Workforce Management
- Automation
---
