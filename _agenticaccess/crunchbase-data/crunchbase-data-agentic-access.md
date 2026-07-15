---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Entity Lookup API
  slug: crunchbase-data-entity-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Search API
  slug: crunchbase-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Autocomplete API
  slug: crunchbase-data-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Deleted Entities API
  slug: crunchbase-data-deleted-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crunchbase Data Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Crunchbase exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crunchbase
provider_slug: crunchbase-data
slug: crunchbase-data-agentic-access
source_filename: crunchbase-data-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/crunchbase-data-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /entities/{collection}/{entity_id}\n  method: get\n  operationId: getEntity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{collection}/{entity_id}/cards/{card_id}\n  method: get\n  operationId: getEntityCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /searches/{collection}\n  method: post\n  operationId: searchCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autocompletes\n  method: get\n  operationId: autocomplete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deleted_entities\n  method: get\n  operationId: listDeletedEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /deleted_entities/{collection_id}\n  method: get\n  operationId: listDeletedEntitiesForCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/agentic-access/crunchbase-data-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Company Data
- Web Intelligence
- Funding Data
- Firmographics
- B2B Data
- Investor Data
- Reference Data
- Fortune 1000
---
