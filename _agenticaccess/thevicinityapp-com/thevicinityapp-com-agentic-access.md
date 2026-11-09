---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 10
api_specs:
- filename: thevicinityapp-com-account-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Account API
  slug: thevicinityapp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-account-api-openapi.yml
- filename: thevicinityapp-com-cities-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Cities API
  slug: thevicinityapp-com-cities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-cities-api-openapi.yml
- filename: thevicinityapp-com-discovery-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Discovery API
  slug: thevicinityapp-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-discovery-api-openapi.yml
- filename: thevicinityapp-com-events-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Events API
  slug: thevicinityapp-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-events-api-openapi.yml
- filename: thevicinityapp-com-intents-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Intents API
  slug: thevicinityapp-com-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-intents-api-openapi.yml
- filename: thevicinityapp-com-places-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Places API
  slug: thevicinityapp-com-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-places-api-openapi.yml
- filename: thevicinityapp-com-reference-api-openapi.yml
  format: yaml
  label: thevicinityapp-com Reference API
  slug: thevicinityapp-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thevicinityapp-com/openapi/thevicinityapp-com-reference-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thevicinityapp Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /account/claim
operation_count: 16
overview: 'thevicinityapp-com exposes 16 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 4 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: thevicinityapp-com
provider_slug: thevicinityapp-com
slug: thevicinityapp-com-agentic-access
source_filename: thevicinityapp-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/thevicinityapp-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 10\n    acting: 6\n  by_consequence:\n    read: 10\n    write: 4\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /coverage\n  method: get\n  operationId: getCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sections\n  method: get\n  operationId: listSections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities\n  method:\
  \ get\n  operationId: listCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cities/{slug}\n  method: get\n  operationId: getCity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places\n  method: get\n  operationId: listPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /places/{slug}\n  method: get\n  operationId: getPlace\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiDoc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intents\n  method: get\n  operationId: listIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intents\n  method: post\n  operationId: publishIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intents/{intentId}/reciprocate\n  method: post\n  operationId: reciprocateIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /intents/{intentId}/report\n  method: post\n  operationId: reportIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/topup\n  method: post\n  operationId: topup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /account/checkout\n  method: post\n  operationId: checkout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account/claim\n  method: post\n  operationId: claimPurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/thevicinityapp-com/agentic-access/thevicinityapp-com-agentic-access.yml
summary_line: 16 operations · 6 acting
tags:
- Company
- Social
- Chat
- Location-based
- Community
- Mobile
---
