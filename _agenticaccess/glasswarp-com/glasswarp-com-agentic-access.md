---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 12
api_specs:
- filename: glasswarp-com-agent-api-openapi.yml
  format: yaml
  label: glasswarp-com Agent API
  slug: glasswarp-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-agent-api-openapi.yml
- filename: glasswarp-com-api-keys-api-openapi.yml
  format: yaml
  label: glasswarp-com API Keys API
  slug: glasswarp-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-api-keys-api-openapi.yml
- filename: glasswarp-com-apps-api-openapi.yml
  format: yaml
  label: glasswarp-com Apps API
  slug: glasswarp-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-apps-api-openapi.yml
- filename: glasswarp-com-grounding-api-openapi.yml
  format: yaml
  label: glasswarp-com Grounding API
  slug: glasswarp-com-grounding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-grounding-api-openapi.yml
- filename: glasswarp-com-input-api-openapi.yml
  format: yaml
  label: glasswarp-com Input API
  slug: glasswarp-com-input-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-input-api-openapi.yml
- filename: glasswarp-com-rigs-api-openapi.yml
  format: yaml
  label: glasswarp-com Rigs API
  slug: glasswarp-com-rigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-rigs-api-openapi.yml
- filename: glasswarp-com-screenshots-api-openapi.yml
  format: yaml
  label: glasswarp-com Screenshots API
  slug: glasswarp-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-screenshots-api-openapi.yml
- filename: glasswarp-com-sessions-api-openapi.yml
  format: yaml
  label: glasswarp-com Sessions API
  slug: glasswarp-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-sessions-api-openapi.yml
- filename: glasswarp-com-streaming-api-openapi.yml
  format: yaml
  label: glasswarp-com Streaming API
  slug: glasswarp-com-streaming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-streaming-api-openapi.yml
- filename: glasswarp-com-webhooks-api-openapi.yml
  format: yaml
  label: glasswarp-com Webhooks API
  slug: glasswarp-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  safety-critical: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Glasswarp Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/sessions/{sessionId}/app/kill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sessions/{sessionId}/input
operation_count: 21
overview: 'glasswarp-com exposes 21 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 6 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: glasswarp-com
provider_slug: glasswarp-com
slug: glasswarp-com-agentic-access
source_filename: glasswarp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/glasswarp-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 21\n  by_action_class:\n    connected: 12\n    acting: 9\n  by_consequence:\n    read: 12\n    write: 6\n    safety-critical: 2\n    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /v1/agent/latest\n  method: get\n  operationId: getAgentLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/rigs\n  method: get\n  operationId: listRigs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /v1/rigs/{rigId}\n  method: get\n  operationId: getRig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions\n  method: get\n  operationId: listSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}\n  method: get\n  operationId: getSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}\n\
  \  method: delete\n  operationId: endSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{sessionId}/screenshot\n  method: get\n  operationId: takeScreenshot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/dirty\n  method: get\n  operationId: getDirtyRects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/observe\n  method: get\n  operationId: observeSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/targets\n  method: get\n  operationId: listTargets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/stream\n  method: get\n  operationId: getStreamConnection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sessions/{sessionId}/app/launch\n  method: post\n  operationId: launchApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sessions/{sessionId}/app/kill\n  method: post\n  operationId: killApp\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/sessions/{sessionId}/input\n  method: post\n  operationId: sendInput\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys\n  method: get\n  operationId: listKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys\n  method: post\n  operationId: createKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/{keyId}\n  method: delete\n  operationId: revokeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/glasswarp-com/agentic-access/glasswarp-com-agentic-access.yml
summary_line: 21 operations · 9 acting · 2 human-in-the-loop
tags:
- Company
- Automation
- Windows
- RPA
---
