---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: clearhouse-sh-evidence-api-openapi.yml
  format: yaml
  label: Clearhouse Evidence API
  slug: clearhouse-sh-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-evidence-api-openapi.yml
- filename: clearhouse-sh-index-api-openapi.yml
  format: yaml
  label: Clearhouse Index API
  slug: clearhouse-sh-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-index-api-openapi.yml
- filename: clearhouse-sh-receipts-api-openapi.yml
  format: yaml
  label: Clearhouse Receipts API
  slug: clearhouse-sh-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-receipts-api-openapi.yml
- filename: clearhouse-sh-service-api-openapi.yml
  format: yaml
  label: Clearhouse Service API
  slug: clearhouse-sh-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearhouse-sh/openapi/clearhouse-sh-service-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clearhouse Sh Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Clearhouse exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clearhouse
provider_slug: clearhouse-sh
slug: clearhouse-sh-agentic-access
source_filename: clearhouse-sh-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/clearhouse-sh-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /healthz\n  method: get\n  operationId: healthz_healthz_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/stats\n  method: get\n  operationId: stats_v0_stats_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/search\n  method: get\n  operationId: search_v0_search_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/listing/{listing_id}\n  method: get\n  operationId: listing_v0_listing__listing_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/evidence/{listing_id}\n  method: get\n  operationId: evidence_v0_evidence__listing_id__get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v0/methodology\n  method: get\n  operationId: methodology_v0_methodology_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/clearhouse-keys.json\n  method: get\n  operationId: wellknown_keys__well_known_clearhouse_keys_json_get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/clearhouse-sh/agentic-access/clearhouse-sh-agentic-access.yml
summary_line: 7 operations
tags:
- Agent Registry
- Call Routing
- Signed Receipts
- Pay-per-call
- MCP
- A2A
---
