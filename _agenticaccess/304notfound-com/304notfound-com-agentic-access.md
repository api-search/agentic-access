---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 7
api_specs:
- filename: 304notfound-com-answer-api-openapi.yml
  format: yaml
  label: 304NotModified Answer API
  slug: 304notfound-com-answer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-answer-api-openapi.yml
- filename: 304notfound-com-ask-api-openapi.yml
  format: yaml
  label: 304NotModified Ask API
  slug: 304notfound-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-ask-api-openapi.yml
- filename: 304notfound-com-calculs-sur-vos-donn-es-api-openapi.yml
  format: yaml
  label: 304NotModified Calculs sur vos données API
  slug: 304notfound-com-calculs-sur-vos-donn-es-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-calculs-sur-vos-donn-es-api-openapi.yml
- filename: 304notfound-com-comment-api-openapi.yml
  format: yaml
  label: 304NotModified Comment API
  slug: 304notfound-com-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-comment-api-openapi.yml
- filename: 304notfound-com-domains-api-openapi.yml
  format: yaml
  label: 304NotModified Domains API
  slug: 304notfound-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-domains-api-openapi.yml
- filename: 304notfound-com-feedback-api-openapi.yml
  format: yaml
  label: 304NotModified Feedback API
  slug: 304notfound-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-feedback-api-openapi.yml
- filename: 304notfound-com-health-api-openapi.yml
  format: yaml
  label: 304NotModified Health API
  slug: 304notfound-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-health-api-openapi.yml
- filename: 304notfound-com-keys-api-openapi.yml
  format: yaml
  label: 304NotModified Keys API
  slug: 304notfound-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-keys-api-openapi.yml
- filename: 304notfound-com-llms-txt-api-openapi.yml
  format: yaml
  label: 304NotModified Llms.txt API
  slug: 304notfound-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-llms-txt-api-openapi.yml
- filename: 304notfound-com-services-api-openapi.yml
  format: yaml
  label: 304NotModified Services API
  slug: 304notfound-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/304notfound-com/openapi/304notfound-com-services-api-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 1
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: 304Notfound Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/calc/position-size
operation_count: 16
overview: '304NotModified exposes 16 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 8 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 304NotModified
provider_slug: 304notfound-com
slug: 304notfound-com-agentic-access
source_filename: 304notfound-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/304notfound-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 7\n    acting: 9\n  by_consequence:\n    read: 7\n    write: 8\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /health\n  method: get\n  operationId: health_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms_txt_llms_txt_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains\n\
  \  method: get\n  operationId: public_domains_v1_domains_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: self_service_key_v1_keys_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/answer\n  method: post\n  operationId: answer_v1_answer_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ask\n  method: get\n  operationId: ask_v1_ask_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calc/ichimoku-rvol\n  method: post\n  operationId: calc_ichimoku_v1_calc_ichimoku_rvol_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calc/regime\n  method: post\n  operationId: calc_regime_v1_calc_regime_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calc/position-size\n  method: post\n  operationId: calc_position_v1_calc_position_size_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/services\n  method: get\n  operationId: list_services_v1_services_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{service_id}\n  method: get\n  operationId: get_service_v1_services__service_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/{service_id}/quote\n  method: post\n  operationId: quote_v1_services__service_id__quote_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/services/{service_id}/run\n  method: post\n  operationId: run_v1_services__service_id__run_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/runs/{run_id}\n  method: get\n  operationId: get_run_v1_runs__run_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/feedback\n  method: post\n  operationId: feedback_v1_feedback_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/comment\n  method: post\n  operationId: comment_v1_comment_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/304notfound-com/agentic-access/304notfound-com-agentic-access.yml
summary_line: 16 operations · 9 acting · 1 human-in-the-loop
tags:
- Artificial Intelligence
- Knowledge Base
- French
- Fact Checking
---
