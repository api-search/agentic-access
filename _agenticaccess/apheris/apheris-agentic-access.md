---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: apheris-apheris-api-api-openapi.yml
  format: yaml
  label: Apheris Apheris API
  slug: apheris-apheris-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-apheris-api-api-openapi.yml
- filename: apheris-health-api-openapi.yml
  format: yaml
  label: Apheris Health API
  slug: apheris-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-health-api-openapi.yml
- filename: apheris-predict-async-api-openapi.yml
  format: yaml
  label: Apheris Predict Async API
  slug: apheris-predict-async-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-predict-async-api-openapi.yml
- filename: apheris-results-api-openapi.yml
  format: yaml
  label: Apheris Results API
  slug: apheris-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-results-api-openapi.yml
- filename: apheris-schema-api-openapi.yml
  format: yaml
  label: Apheris Schema API
  slug: apheris-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-schema-api-openapi.yml
- filename: apheris-ticket-api-openapi.yml
  format: yaml
  label: Apheris Ticket API
  slug: apheris-ticket-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-ticket-api-openapi.yml
- filename: apheris-weights-api-openapi.yml
  format: yaml
  label: Apheris Weights API
  slug: apheris-weights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apheris/openapi/apheris-weights-api-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apheris Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Apheris exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apheris
provider_slug: apheris
slug: apheris-agentic-access
source_filename: apheris-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/apheris-apheris-api-api-openapi.yml, openapi/apheris-health-api-openapi.yml,\n  openapi/apheris-predict-async-api-openapi.yml, openapi/apheris-results-api-openapi.yml, openapi/apheris-schema-api-openapi.yml,\n  openapi/apheris-ticket-api-openapi.yml, openapi/apheris-weights-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 7\n    acting: 2\n  by_consequence:\n    read: 7\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health/ready\n\
  \  method: get\n  operationId: get_v1_health_ready\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/predict-async\n  method: post\n  operationId: post_api_v1_predict_async\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/predict-async/{jobid}/{id}\n  method: get\n  operationId: get_api_v1_predict_async_jobid_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /results/{uuid}\n  method: get\n  operationId: get_results_uuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /schema\n  method: get\n  operationId: get_schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ticket\n  method: post\n  operationId: post_ticket\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ticket/{uuid}\n  method: get\n  operationId: get_ticket_uuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /weights\n  method: get\n  operationId: get_weights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://artifacts.apis.io/apheris/agentic-access/apheris-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Company
- Artificial Intelligence
- Drug Discovery
- Federated Learning
- Biotechnology
---
