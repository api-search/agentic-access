---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 7
api_specs:
- filename: layercall-com-ai-agents-api-openapi.yml
  format: yaml
  label: layercall-com AI agents API
  slug: layercall-com-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-ai-agents-api-openapi.yml
- filename: layercall-com-batch-api-openapi.yml
  format: yaml
  label: layercall-com Batch API
  slug: layercall-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-batch-api-openapi.yml
- filename: layercall-com-device-api-openapi.yml
  format: yaml
  label: layercall-com Device API
  slug: layercall-com-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-device-api-openapi.yml
- filename: layercall-com-reputation-api-openapi.yml
  format: yaml
  label: layercall-com Reputation API
  slug: layercall-com-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-reputation-api-openapi.yml
- filename: layercall-com-rules-api-openapi.yml
  format: yaml
  label: layercall-com Rules API
  slug: layercall-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-rules-api-openapi.yml
- filename: layercall-com-scoring-api-openapi.yml
  format: yaml
  label: layercall-com Scoring API
  slug: layercall-com-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-scoring-api-openapi.yml
- filename: layercall-com-unified-api-openapi.yml
  format: yaml
  label: layercall-com Unified API
  slug: layercall-com-unified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-unified-api-openapi.yml
consequence_counts:
  read: 7
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Layercall Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'layercall-com exposes 19 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 12 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: layercall-com
provider_slug: layercall-com
slug: layercall-com-agentic-access
source_filename: layercall-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/layercall-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 7\n    acting: 12\n  by_consequence:\n    read: 7\n    write: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/score/ip\n  method: get\n  operationId: scoreIp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify/email\n  method: get\n  operationId: verifyEmail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lookup/phone\n  method: get\n \
  \ operationId: lookupPhone\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/score/domain\n  method: get\n  operationId: scoreDomain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/score/user\n  method: post\n  operationId: scoreUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/score/user\n  method: get\n  operationId: scoreUserGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/score/device\n  method: post\n  operationId:\
  \ scoreDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/report\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/outcome\n  method: post\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/verify/agent\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/authorize\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/agent/policy\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent/policy\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rules\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/rules/import\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/layercall-com/agentic-access/layercall-com-agentic-access.yml
summary_line: 19 operations · 12 acting
tags:
- Company
- Fraud Prevention
- TrustIntelligence
- Security
---
