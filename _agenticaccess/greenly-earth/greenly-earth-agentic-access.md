---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 9
api_specs:
- filename: greenly-carbon-analytics-api-openapi.yml
  format: yaml
  label: Greenly Carbon Analytics API
  slug: greenly-carbon-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/openapi/greenly-carbon-analytics-api-openapi.yml
consequence_counts:
  read: 9
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Greenly Earth Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Greenly exposes 14 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Greenly
provider_slug: greenly-earth
slug: greenly-earth-agentic-access
source_filename: greenly-earth-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/greenly-carbon-analytics-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 9\n    acting: 5\n  by_consequence:\n    read: 9\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /alternatives\n  method: get\n  operationId: GetAlternatives\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /alternatives/{id}\n  method: get\n  operationId: GetAlternative\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offsetProjects\n\
  \  method: get\n  operationId: GetOffsetProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offsetProjects/{offsetProjectId}\n  method: get\n  operationId: GetOffsetProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /offsetProjects/bookOffsetQuantity\n  method: post\n  operationId: BookOffsetQuantity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /live\n  method: get\n  operationId: IsLive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /ready\n  method: get\n  operationId: IsReady\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseCategories\n  method: get\n  operationId: GetPurchaseCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /purchaseCategories/{purchaseCategoryId}\n  method: get\n  operationId: GetPurchaseCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/calculateCarbonFootprints\n  method: post\n  operationId: CalculateCarbonFootprints\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /users/createUser\n  method: post\n  operationId: CreateUserAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: put\n  operationId: UpdateUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}\n  method: get\n  operationId: GetUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: delete\n\
  \  operationId: DeleteUserAPI\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenly-earth/refs/heads/main/agentic-access/greenly-earth-agentic-access.yml
summary_line: 14 operations · 5 acting
tags:
- Carbon Accounting
- Carbon Footprint
- Carbon Analytics
- Greenhouse Gas
- GHG Protocol
- Scope 1
- Scope 2
- Scope 3
- Sustainability
- ESG
- Climate
- CSRD
- CBAM
- EUDR
- SBTi
- TCFD
- EcoVadis
- Bilan Carbone
- Life Cycle Assessment
- Carbon Offsets
- SMB
- Fintech
- Transaction Enrichment
---
