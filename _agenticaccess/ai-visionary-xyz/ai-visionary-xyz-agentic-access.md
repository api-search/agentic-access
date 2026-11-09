---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: ai-visionary-xyz-entity-api-openapi.yml
  format: yaml
  label: AI Visionary Entity API
  slug: ai-visionary-xyz-entity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-visionary-xyz/openapi/ai-visionary-xyz-entity-api-openapi.yml
- filename: ai-visionary-xyz-live-api-openapi.yml
  format: yaml
  label: AI Visionary Live API
  slug: ai-visionary-xyz-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-visionary-xyz/openapi/ai-visionary-xyz-live-api-openapi.yml
- filename: ai-visionary-xyz-llm-api-openapi.yml
  format: yaml
  label: AI Visionary Llm API
  slug: ai-visionary-xyz-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-visionary-xyz/openapi/ai-visionary-xyz-llm-api-openapi.yml
- filename: ai-visionary-xyz-search-api-openapi.yml
  format: yaml
  label: AI Visionary Search API
  slug: ai-visionary-xyz-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-visionary-xyz/openapi/ai-visionary-xyz-search-api-openapi.yml
- filename: ai-visionary-xyz-stats-api-openapi.yml
  format: yaml
  label: AI Visionary Stats API
  slug: ai-visionary-xyz-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-visionary-xyz/openapi/ai-visionary-xyz-stats-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ai Visionary Xyz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'AI Visionary exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI Visionary
provider_slug: ai-visionary-xyz
slug: ai-visionary-xyz-agentic-access
source_filename: ai-visionary-xyz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ai-visionary-xyz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /llm/{domain}\n  method: get\n  operationId: getLlmSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: searchEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entity/{domain}\n  method: get\n  operationId: getEntity\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stats\n  method: get\n  operationId: getStats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /live\n  method: get\n  operationId: getLiveRegistry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ai-visionary-xyz/agentic-access/ai-visionary-xyz-agentic-access.yml
summary_line: 5 operations
tags:
- Artificial Intelligence
- Data-Structuring
- AI-Readiness
- Knowledge-Representation
- Services
---
