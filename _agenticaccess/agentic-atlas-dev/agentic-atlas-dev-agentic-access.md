---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 14
api_specs:
- filename: agentic-atlas-dev-agent-api-openapi.yml
  format: yaml
  label: Agentic Atlas Agent API
  slug: agentic-atlas-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-agent-api-openapi.yml
- filename: agentic-atlas-dev-cards-api-openapi.yml
  format: yaml
  label: Agentic Atlas Cards API
  slug: agentic-atlas-dev-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-cards-api-openapi.yml
- filename: agentic-atlas-dev-compare-api-openapi.yml
  format: yaml
  label: Agentic Atlas Compare API
  slug: agentic-atlas-dev-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-compare-api-openapi.yml
- filename: agentic-atlas-dev-decisions-api-openapi.yml
  format: yaml
  label: Agentic Atlas Decisions API
  slug: agentic-atlas-dev-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-decisions-api-openapi.yml
- filename: agentic-atlas-dev-glossary-api-openapi.yml
  format: yaml
  label: Agentic Atlas Glossary API
  slug: agentic-atlas-dev-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-glossary-api-openapi.yml
- filename: agentic-atlas-dev-links-api-openapi.yml
  format: yaml
  label: Agentic Atlas Links API
  slug: agentic-atlas-dev-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-links-api-openapi.yml
- filename: agentic-atlas-dev-nodes-api-openapi.yml
  format: yaml
  label: Agentic Atlas Nodes API
  slug: agentic-atlas-dev-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-nodes-api-openapi.yml
- filename: agentic-atlas-dev-orient-api-openapi.yml
  format: yaml
  label: Agentic Atlas Orient API
  slug: agentic-atlas-dev-orient-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-orient-api-openapi.yml
- filename: agentic-atlas-dev-resolve-api-openapi.yml
  format: yaml
  label: Agentic Atlas Resolve API
  slug: agentic-atlas-dev-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-resolve-api-openapi.yml
- filename: agentic-atlas-dev-search-api-openapi.yml
  format: yaml
  label: Agentic Atlas Search API
  slug: agentic-atlas-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-search-api-openapi.yml
- filename: agentic-atlas-dev-tour-api-openapi.yml
  format: yaml
  label: Agentic Atlas Tour API
  slug: agentic-atlas-dev-tour-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-tour-api-openapi.yml
- filename: agentic-atlas-dev-tree-api-openapi.yml
  format: yaml
  label: Agentic Atlas Tree API
  slug: agentic-atlas-dev-tree-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentic-atlas-dev/openapi/agentic-atlas-dev-tree-api-openapi.yml
consequence_counts:
  read: 14
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentic Atlas Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 19
overview: 'Agentic Atlas exposes 19 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Agentic Atlas
provider_slug: agentic-atlas-dev
slug: agentic-atlas-dev-agentic-access
source_filename: agentic-atlas-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/agentic-atlas-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 14\n    acting: 5\n  by_consequence:\n    read: 14\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/orient\n  method: get\n  operationId: orient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tour\n  method: get\n  operationId: readTour\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cards\n  method: get\n  operationId: readCards\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/agent/orient\n  method: post\n  operationId: agent_orient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/cards\n  method: post\n  operationId: agent_cards\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /api/agent/read\n  method: post\n  operationId: agent_read\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/links\n  method: post\n  operationId: agent_links\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/agent/navigate\n  method: post\n  operationId: agent_navigate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/compare\n  method: get\n  operationId: compare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/glossary\n  method: get\n  operationId: listGlossary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/glossary/{term_key}/usages\n  method: get\n  operationId: readTermUsages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/glossary/{term}\n  method: get\n  operationId: defineTerm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decisions\n  method: get\n  operationId:\
  \ listDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/decisions/{canonical_id}\n  method: get\n  operationId: readDecision\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/links/{canonical_id}\n  method: get\n  operationId: readLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nodes/{canonical_id}\n  method: get\n  operationId: readNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tree\n  method: get\n  operationId: readTree\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/resolve\n  method: get\n  operationId: resolveName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentic-atlas-dev/agentic-access/agentic-atlas-dev-agentic-access.yml
summary_line: 19 operations · 5 acting
tags:
- Agentic Systems
- AI Patterns
- MCP
- OpenAPI
---
