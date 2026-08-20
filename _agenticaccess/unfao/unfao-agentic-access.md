---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: unfao-catalog-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Catalog API
  slug: unfao-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-catalog-api-openapi.yml
- filename: unfao-data-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Data API
  slug: unfao-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-data-api-openapi.yml
- filename: unfao-dimensions-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Dimensions API
  slug: unfao-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-dimensions-api-openapi.yml
- filename: unfao-domains-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Domains API
  slug: unfao-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-domains-api-openapi.yml
- filename: unfao-downloads-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Downloads API
  slug: unfao-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-downloads-api-openapi.yml
- filename: unfao-metadata-api-openapi.yml
  format: yaml
  label: FAO FAOSTAT Metadata API
  slug: unfao-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/openapi/unfao-metadata-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unfao Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'FAO FAOSTAT exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FAO FAOSTAT
provider_slug: unfao
slug: unfao-agentic-access
source_filename: unfao-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/faostat-bulk-api.json, openapi/faostat-data-api.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog.json\n  method: get\n  operationId: getCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{filename}\n  method: get\n  operationId: downloadDataset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/groupsanddomains\n  method:\
  \ get\n  operationId: getGroupsAndDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/definitions/types/domain\n  method: get\n  operationId: getDomainList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/dimensions/{domain}\n  method: get\n  operationId: getDomainDimensions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/dimensions/{domain}/{dimension}\n  method: get\n  operationId: getDimensionMembers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/data/{domain}\n  method: get\n  operationId: getDomainData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/definitions/types/flag\n  method: get\n  operationId: getFlags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/definitions/types/area\n  method: get\n  operationId: getAreaList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/definitions/types/area/{area_code}\n  method: get\n  operationId: getAreaDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{lang}/metadata/{domain}\n  method: get\n  operationId: getDomainMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unfao/refs/heads/main/agentic-access/unfao-agentic-access.yml
summary_line: 11 operations
tags:
- Agriculture
- food security
- Statistics
- Trade
- Land Use
- Environment
- UN
- Open Data
---
