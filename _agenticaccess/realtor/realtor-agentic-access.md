---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: realtor-connections-plus-asyncapi.yml
  format: yaml
  label: Realtor.com Connections Plus API
  slug: connections-plus-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-connections-plus-asyncapi.yml
- filename: realtor-lead-delivery-asyncapi.yml
  format: yaml
  label: Realtor.com Lead Delivery API
  slug: lead-delivery-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-lead-delivery-asyncapi.yml
- filename: realtor-property-data-openapi.yml
  format: yaml
  label: Realtor.com Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/openapi/realtor-property-data-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Realtor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'realtor exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: realtor
provider_slug: realtor
slug: realtor-agentic-access
source_filename: realtor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/realtor-property-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /locations/v2/auto-complete\n  method: get\n  operationId: autoCompleteLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/v3/list\n  method: post\n  operationId: listProperties\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /properties/v2/detail\n  method: get\n  operationId: getPropertyDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/v2/list-by-mls\n  method: get\n  operationId: listPropertiesByMls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/v2/list-similar-homes\n  method: get\n  operationId: listSimilarHomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /properties/v2/list-similar-rental-homes\n  method: get\n  operationId: listSimilarRentalHomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents/list\n  method: get\n  operationId: listAgents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance/rates\n  method: get\n  operationId: getMortgageRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/agentic-access/realtor-agentic-access.yml
summary_line: 8 operations · 1 acting
tags: []
---
