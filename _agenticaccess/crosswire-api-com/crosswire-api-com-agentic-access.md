---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: crosswire-api-com-adoption-api-openapi.yml
  format: yaml
  label: Crosswire Adoption API
  slug: crosswire-api-com-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-adoption-api-openapi.yml
- filename: crosswire-api-com-audit-api-openapi.yml
  format: yaml
  label: Crosswire Audit API
  slug: crosswire-api-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-audit-api-openapi.yml
- filename: crosswire-api-com-events-api-openapi.yml
  format: yaml
  label: Crosswire Events API
  slug: crosswire-api-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-events-api-openapi.yml
- filename: crosswire-api-com-health-api-openapi.yml
  format: yaml
  label: Crosswire Health API
  slug: crosswire-api-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-health-api-openapi.yml
- filename: crosswire-api-com-live-api-openapi.yml
  format: yaml
  label: Crosswire Live API
  slug: crosswire-api-com-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswire-api-com/openapi/crosswire-api-com-live-api-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crosswire Api Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Crosswire exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crosswire
provider_slug: crosswire-api-com
slug: crosswire-api-com-agentic-access
source_filename: crosswire-api-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crosswire-api-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/health\n  method: get\n  operationId: health_v1_health_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/live\n  method: get\n  operationId: live_v1_live_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/events\n  method: get\n\
  \  operationId: events_v1_events_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/adoption\n  method: get\n  operationId: adoption_v1_adoption_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/audit\n  method: post\n  operationId: audit_pair_v1_audit_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/crosswire-api-com/agentic-access/crosswire-api-com-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Finance
- Trading
- Cryptocurrency
- Risk Management
---
