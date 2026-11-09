---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 14
api_specs:
- filename: agentmuseum-org-collection-api-openapi.yml
  format: yaml
  label: The Agent Museum Collection API
  slug: agentmuseum-org-collection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-collection-api-openapi.yml
- filename: agentmuseum-org-curation-api-openapi.yml
  format: yaml
  label: The Agent Museum Curation API
  slug: agentmuseum-org-curation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-curation-api-openapi.yml
- filename: agentmuseum-org-deposit-api-openapi.yml
  format: yaml
  label: The Agent Museum Deposit API
  slug: agentmuseum-org-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-deposit-api-openapi.yml
- filename: agentmuseum-org-exhibit-api-openapi.yml
  format: yaml
  label: The Agent Museum Exhibit API
  slug: agentmuseum-org-exhibit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-exhibit-api-openapi.yml
- filename: agentmuseum-org-exhibits-api-openapi.yml
  format: yaml
  label: The Agent Museum Exhibits API
  slug: agentmuseum-org-exhibits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-exhibits-api-openapi.yml
- filename: agentmuseum-org-firsts-api-openapi.yml
  format: yaml
  label: The Agent Museum Firsts API
  slug: agentmuseum-org-firsts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-firsts-api-openapi.yml
- filename: agentmuseum-org-on-this-day-json-api-openapi.yml
  format: yaml
  label: The Agent Museum On This Day.json API
  slug: agentmuseum-org-on-this-day-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-on-this-day-json-api-openapi.yml
- filename: agentmuseum-org-read-api-openapi.yml
  format: yaml
  label: The Agent Museum Read API
  slug: agentmuseum-org-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-read-api-openapi.yml
- filename: agentmuseum-org-search-api-openapi.yml
  format: yaml
  label: The Agent Museum Search API
  slug: agentmuseum-org-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-search-api-openapi.yml
- filename: agentmuseum-org-the-agent-museum-api-api-openapi.yml
  format: yaml
  label: The Agent Museum The Agent Museum API
  slug: agentmuseum-org-the-agent-museum-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-the-agent-museum-api-api-openapi.yml
- filename: agentmuseum-org-timeline-api-openapi.yml
  format: yaml
  label: The Agent Museum Timeline API
  slug: agentmuseum-org-timeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentmuseum-org/openapi/agentmuseum-org-timeline-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentmuseum Org Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deposit
operation_count: 17
overview: 'The Agent Museum exposes 17 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: The Agent Museum
provider_slug: agentmuseum-org
slug: agentmuseum-org-agentic-access
source_filename: agentmuseum-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/agentmuseum-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 14\n    acting: 3\n  by_consequence:\n    read: 14\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  operationId: getIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/collection\n  method: get\n  operationId: listCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/exhibits/{slug}\n\
  \  method: get\n  operationId: getExhibit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/firsts\n  method: get\n  operationId: listFirsts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/timeline\n  method: get\n  operationId: listTimeline\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-this-day.json\n  method: get\n  operationId: onThisDay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /exhibit/{slug}/disclosure.json\n  method: get\n  operationId: getDisclosure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit\n  method: post\n  operationId: submitObject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deposit/pay/{id}/status\n  method: get\n  operationId: depositPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit/quote\n  method: get\n  operationId: depositQuote\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit/mine\n  method: get\n  operationId: myDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deposit/status/{slug}\n  method: get\n  operationId: depositStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nominations\n  method: get\n  operationId: listNominations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/nominations/{slug}/vouch\n  method: post\n  operationId: vouch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/exhibits/{slug}/cosign\n  method: post\n  operationId: cosign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/agents/{sub}\n  method: get\n  operationId: agentProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentmuseum-org/agentic-access/agentmuseum-org-agentic-access.yml
summary_line: 17 operations · 3 acting
tags:
- Museums
- Agents
- Blockchain
- Digital Heritage
- Verification
---
