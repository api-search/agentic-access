---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: osmaura-prospect-openapi.yml
  format: yaml
  label: Osmaura Prospect API
  slug: osmaura-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/openapi/osmaura-prospect-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Osmaura Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Osmaura exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Osmaura
provider_slug: osmaura
slug: osmaura-agentic-access
source_filename: osmaura-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/osmaura-prospect-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/prospects\n  method: get\n  operationId: getProspects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/prospect-editions\n  method: get\n  operationId: listProspectEditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signals\n  method: get\n  operationId: getLegacySignals\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/signal-editions\n  method: get\n  operationId: listLegacySignalEditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osmaura/refs/heads/main/agentic-access/osmaura-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Legal
- LegalTech
- Artificial Intelligence
- Sales Enablement
- Business Development
- Y Combinator
- Market Intelligence
- Data
- Government Data
- Prospecting
---
