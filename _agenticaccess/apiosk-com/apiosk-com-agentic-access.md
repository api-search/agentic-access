---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: apiosk-com-ask-api-openapi.yml
  format: yaml
  label: Apiosk Ask API
  slug: apiosk-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-ask-api-openapi.yml
- filename: apiosk-com-asks-api-openapi.yml
  format: yaml
  label: Apiosk Asks API
  slug: apiosk-com-asks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-asks-api-openapi.yml
- filename: apiosk-com-balance-api-openapi.yml
  format: yaml
  label: Apiosk Balance API
  slug: apiosk-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-balance-api-openapi.yml
- filename: apiosk-com-capabilities-api-openapi.yml
  format: yaml
  label: Apiosk Capabilities API
  slug: apiosk-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-capabilities-api-openapi.yml
- filename: apiosk-com-execute-api-openapi.yml
  format: yaml
  label: Apiosk Execute API
  slug: apiosk-com-execute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-execute-api-openapi.yml
- filename: apiosk-com-health-api-openapi.yml
  format: yaml
  label: Apiosk Health API
  slug: apiosk-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-health-api-openapi.yml
- filename: apiosk-com-runs-api-openapi.yml
  format: yaml
  label: Apiosk Runs API
  slug: apiosk-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-runs-api-openapi.yml
- filename: apiosk-com-source-readiness-api-openapi.yml
  format: yaml
  label: Apiosk Source Readiness API
  slug: apiosk-com-source-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-source-readiness-api-openapi.yml
- filename: apiosk-com-sources-api-openapi.yml
  format: yaml
  label: Apiosk Sources API
  slug: apiosk-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-sources-api-openapi.yml
- filename: apiosk-com-usage-api-openapi.yml
  format: yaml
  label: Apiosk Usage API
  slug: apiosk-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiosk-com/openapi/apiosk-com-usage-api-openapi.yml
consequence_counts:
  read: 11
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Apiosk Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Apiosk exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Apiosk
provider_slug: apiosk-com
slug: apiosk-com-agentic-access
source_filename: apiosk-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/apiosk-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 11\n    acting: 9\n  by_consequence:\n    read: 11\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/sources\n  method: get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sources/{source_id}\n  method: get\n  operationId: getSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/execute/{source}/{operation}\n\
  \  method: post\n  operationId: executeSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sources/{source_id}/run\n  method: post\n  operationId: runSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ask/plan\n  method: post\n  operationId: planAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /v2/ask\n  method: post\n  operationId: ask\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/asks/{id}/run\n  method: post\n  operationId: runAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/asks/{id}/continue\n  method: post\n  operationId: continueAsk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/runs/{id}\n  method: get\n  operationId: getRun\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/execute/{source}/{operation}\n  method: post\n  operationId: executeSourceV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/asks/{id}\n  method: get\n  operationId: readAsk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/source-readiness\n  method: get\n  operationId: sourceReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: gatewayHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/sources/{source_id}/endpoints\n  method: get\n  operationId: listSourceEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ask/workflows\n  method: get\n  operationId: listAskWorkflows\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/capabilities/resolve\n  method: post\n  operationId: resolveEuropeanCapability\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/capabilities/plan\n  method: post\n  operationId: planEuropeanCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/execute\n  method: post\n  operationId: executeSelectedApi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/apiosk-com/agentic-access/apiosk-com-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- Artificial Intelligence
- Compliance
- Verification
- Sanctions
- Monitoring
- Company
---
