---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 8
api_specs:
- filename: anyhook-net-anyhook-api-api-openapi.yml
  format: yaml
  label: AnyHook AnyHook API
  slug: anyhook-net-anyhook-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-anyhook-api-api-openapi.yml
- filename: anyhook-net-api-keys-api-openapi.yml
  format: yaml
  label: AnyHook Api Keys API
  slug: anyhook-net-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-api-keys-api-openapi.yml
- filename: anyhook-net-apps-api-openapi.yml
  format: yaml
  label: AnyHook Apps API
  slug: anyhook-net-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-apps-api-openapi.yml
- filename: anyhook-net-claim-api-openapi.yml
  format: yaml
  label: AnyHook Claim API
  slug: anyhook-net-claim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-claim-api-openapi.yml
- filename: anyhook-net-connect-api-openapi.yml
  format: yaml
  label: AnyHook Connect API
  slug: anyhook-net-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-connect-api-openapi.yml
- filename: anyhook-net-events-api-openapi.yml
  format: yaml
  label: AnyHook Events API
  slug: anyhook-net-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-events-api-openapi.yml
- filename: anyhook-net-quickstart-api-openapi.yml
  format: yaml
  label: AnyHook Quickstart API
  slug: anyhook-net-quickstart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-quickstart-api-openapi.yml
- filename: anyhook-net-usage-api-openapi.yml
  format: yaml
  label: AnyHook Usage API
  slug: anyhook-net-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anyhook-net/openapi/anyhook-net-usage-api-openapi.yml
consequence_counts:
  read: 8
  safety-critical: 1
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Anyhook Net Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1/api-keys/{id}/revoke
operation_count: 25
overview: 'AnyHook exposes 25 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 16 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AnyHook
provider_slug: anyhook-net
slug: anyhook-net-agentic-access
source_filename: anyhook-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anyhook-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 8\n    acting: 17\n  by_consequence:\n    read: 8\n    write: 16\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/api-keys/{id}/revoke\n  method: patch\n  operationId: revokeApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps\n  method: post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}\n  method: patch\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}\n  method: delete\n  operationId: deleteApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/destinations/{index}/rotate-secret\n  method: post\n  operationId: rotateDestinationSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/events/undelivered\n  method: get\n  operationId: listUndeliveredEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{slug}/replay-failed\n  method: post\n  operationId: replayFailedEvents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/events/{id}/replay\n\
  \  method: post\n  operationId: replayEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{user-slug}/{app-slug}\n  method: post\n  operationId: receiveWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/connect\n  method: post\n  operationId: connectProvider\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/quickstart\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/claim\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{slug}/code\n  method: get\n  operationId: getCodeHandler\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{slug}/code\n  method: put\n  operationId: putCodeHandler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/code\n  method: delete\n  operationId: deleteCodeHandler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/code/test\n  method: post\n  operationId: testCodeHandler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/store\n  method: get\n  operationId: listCodeStore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/apps/{slug}/store\n  method: post\n  operationId: importCodeStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/apps/{slug}/store\n  method: delete\n  operationId: clearCodeStore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anyhook-net/agentic-access/anyhook-net-agentic-access.yml
summary_line: 25 operations · 17 acting · 1 human-in-the-loop
tags:
- Webhook
- Integration
- Reliability
- Developer Tools
- event-replay
---
