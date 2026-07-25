---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 9
api_specs:
- filename: ironclad-clickwrap-activity-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Activity API
  slug: ironclad-clickwrap-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-activity-api-openapi.yml
- filename: ironclad-clickwrap-contracts-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Contracts API
  slug: ironclad-clickwrap-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-contracts-api-openapi.yml
- filename: ironclad-clickwrap-groups-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Groups API
  slug: ironclad-clickwrap-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-groups-api-openapi.yml
- filename: ironclad-clickwrap-signers-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Signers API
  slug: ironclad-clickwrap-signers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-signers-api-openapi.yml
- filename: ironclad-clickwrap-sites-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Sites API
  slug: ironclad-clickwrap-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-sites-api-openapi.yml
consequence_counts:
  physical: 3
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ironclad Clickwrap Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/agreed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/displayed
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send/visited
operation_count: 12
overview: 'Ironclad Clickwrap exposes 12 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Ironclad Clickwrap
provider_slug: ironclad-clickwrap
slug: ironclad-clickwrap-agentic-access
source_filename: ironclad-clickwrap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ironclad-clickwrap-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 9\n    acting: 3\n  by_consequence:\n    read: 9\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /sites\n  method: get\n  operationId: listSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sites/{siteId}\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId:\
  \ listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}\n  method: get\n  operationId: getGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts\n  method: get\n  operationId: listContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /signers\n  method: get\n  operationId: listSigners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /signers/{signerId}\n  method: get\n  operationId: getSigner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /send/agreed\n  method: post\n  operationId: sendAgreed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send/displayed\n  method: post\n  operationId: sendDisplayed\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /send/visited\n  method: post\n  operationId: sendVisited\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /retrieve/latest\n  method: get\n  operationId: retrieveLatest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/agentic-access/ironclad-clickwrap-agentic-access.yml
summary_line: 12 operations · 3 acting
tags:
- Agreements
- Compliance
- Contracts
- Legal
---
