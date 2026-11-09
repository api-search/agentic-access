---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 7
api_specs:
- filename: agenticfabricationnetwork-ai-agents-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Agents API
  slug: agenticfabricationnetwork-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-agents-api-openapi.yml
- filename: agenticfabricationnetwork-ai-attestations-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Attestations API
  slug: agenticfabricationnetwork-ai-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-attestations-api-openapi.yml
- filename: agenticfabricationnetwork-ai-capabilities-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Capabilities API
  slug: agenticfabricationnetwork-ai-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-capabilities-api-openapi.yml
- filename: agenticfabricationnetwork-ai-checkout-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Checkout API
  slug: agenticfabricationnetwork-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-checkout-api-openapi.yml
- filename: agenticfabricationnetwork-ai-files-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Files API
  slug: agenticfabricationnetwork-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-files-api-openapi.yml
- filename: agenticfabricationnetwork-ai-orders-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Orders API
  slug: agenticfabricationnetwork-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-orders-api-openapi.yml
- filename: agenticfabricationnetwork-ai-parts-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Parts API
  slug: agenticfabricationnetwork-ai-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-parts-api-openapi.yml
- filename: agenticfabricationnetwork-ai-quotes-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Quotes API
  slug: agenticfabricationnetwork-ai-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-quotes-api-openapi.yml
- filename: agenticfabricationnetwork-ai-ufp-api-openapi.yml
  format: yaml
  label: Agentic Fabrication Network Ufp API
  slug: agenticfabricationnetwork-ai-ufp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticfabricationnetwork-ai/openapi/agenticfabricationnetwork-ai-ufp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agenticfabricationnetwork Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/orders/{id}/review
operation_count: 14
overview: 'Agentic Fabrication Network exposes 14 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic Fabrication Network
provider_slug: agenticfabricationnetwork-ai
slug: agenticfabricationnetwork-ai-agentic-access
source_filename: agenticfabricationnetwork-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agenticfabricationnetwork-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    acting: 7\n    connected: 7\n  by_consequence:\n    write: 5\n    read: 7\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/agents\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/capabilities\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ufp/spec.schema.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/files\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quotes/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/quotes/{id}/refine\n  method: post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quotes/{id}/preview\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/orders\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/orders/{id}/review\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/parts/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/attestations\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/agenticfabricationnetwork-ai/agentic-access/agenticfabricationnetwork-ai-agentic-access.yml
summary_line: 14 operations · 7 acting
tags:
- Artificial Intelligence
- Manufacturing
- Fabrication
- Marketplace
- Procurement
---
