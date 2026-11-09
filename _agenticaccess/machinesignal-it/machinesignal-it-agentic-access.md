---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: machinesignal-it-health-api-openapi.yml
  format: yaml
  label: machinesignal-it Health API
  slug: machinesignal-it-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machinesignal-it/openapi/machinesignal-it-health-api-openapi.yml
- filename: machinesignal-it-lead-opportunity-score-api-openapi.yml
  format: yaml
  label: machinesignal-it Lead Opportunity Score API
  slug: machinesignal-it-lead-opportunity-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machinesignal-it/openapi/machinesignal-it-lead-opportunity-score-api-openapi.yml
- filename: machinesignal-it-order-intents-api-openapi.yml
  format: yaml
  label: machinesignal-it Order Intents API
  slug: machinesignal-it-order-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machinesignal-it/openapi/machinesignal-it-order-intents-api-openapi.yml
- filename: machinesignal-it-previews-api-openapi.yml
  format: yaml
  label: machinesignal-it Previews API
  slug: machinesignal-it-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machinesignal-it/openapi/machinesignal-it-previews-api-openapi.yml
- filename: machinesignal-it-usage-api-openapi.yml
  format: yaml
  label: machinesignal-it Usage API
  slug: machinesignal-it-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machinesignal-it/openapi/machinesignal-it-usage-api-openapi.yml
consequence_counts:
  physical: 2
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Machinesignal It Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order-intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order-intents/{order_intent_id}/inputs
operation_count: 8
overview: 'machinesignal-it exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: machinesignal-it
provider_slug: machinesignal-it
slug: machinesignal-it-agentic-access
source_filename: machinesignal-it-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/api.machinesignal.it-openapi.json, openapi/machinesignal-it-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 2\n    physical: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/previews/public-readiness\n  method: post\n  operationId: createMachineSignalMiniDecPreview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order-intents\n\
  \  method: post\n  operationId: createMachineSignalOrderIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order-intents/{order_intent_id}\n  method: get\n  operationId: getMachineSignalOrderIntentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order-intents/{order_intent_id}/inputs\n  method: post\n  operationId: submitMachineSignalPaidOrderInputs\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order-intents/{order_intent_id}/artifact\n  method: get\n  operationId: getMachineSignalPaidOrderArtifact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/lead-opportunity-score\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/machinesignal-it/agentic-access/machinesignal-it-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Company
- B2B
- Automation
- Data
- Italy
---
