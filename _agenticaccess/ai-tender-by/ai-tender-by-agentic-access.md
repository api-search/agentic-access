---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: ai-tender-by-counterparty-check-php-api-openapi.yml
  format: yaml
  label: AI-TENDER Counterparty Check.php API
  slug: ai-tender-by-counterparty-check-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-tender-by/openapi/ai-tender-by-counterparty-check-php-api-openapi.yml
- filename: ai-tender-by-public-api-openapi.yml
  format: yaml
  label: AI-TENDER Public API
  slug: ai-tender-by-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-tender-by/openapi/ai-tender-by-public-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ai Tender By Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'AI-TENDER exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI-TENDER
provider_slug: ai-tender-by
slug: ai-tender-by-agentic-access
source_filename: ai-tender-by-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ai-tender-by-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/tenders.php\n  method: get\n  operationId: listOpenTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/tender.php\n  method: get\n  operationId: getOpenTender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/counterparty_check.php\n  method: get\n\
  \  operationId: checkCounterparty\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/search.php\n  method: get\n  operationId: searchOpenTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ai-tender-by/agentic-access/ai-tender-by-agentic-access.yml
summary_line: 4 operations
tags:
- Artificial Intelligence
- Tender
- Government Procurement
- Belarus
- Invitation-only
---
