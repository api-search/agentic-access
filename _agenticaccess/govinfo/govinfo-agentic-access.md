---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: govinfo-collections-api-openapi.yml
  format: yaml
  label: GovInfo Collections API
  slug: govinfo-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-collections-api-openapi.yml
- filename: govinfo-packages-api-openapi.yml
  format: yaml
  label: GovInfo Packages API
  slug: govinfo-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-packages-api-openapi.yml
- filename: govinfo-published-api-openapi.yml
  format: yaml
  label: GovInfo Published API
  slug: govinfo-published-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-published-api-openapi.yml
- filename: govinfo-related-api-openapi.yml
  format: yaml
  label: GovInfo Related API
  slug: govinfo-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-related-api-openapi.yml
- filename: govinfo-search-api-openapi.yml
  format: yaml
  label: GovInfo Search API
  slug: govinfo-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/openapi/govinfo-search-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Govinfo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'GovInfo exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: GovInfo
provider_slug: govinfo
slug: govinfo-agentic-access
source_filename: govinfo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/govinfo-collections-api-openapi.yml, openapi/govinfo-packages-api-openapi.yml,\n  openapi/govinfo-published-api-openapi.yml, openapi/govinfo-related-api-openapi.yml, openapi/govinfo-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /collections\n  method: get\n  operationId: getCollectionSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/{lastModifiedStartDate}\n  method: get\n  operationId: getModifiedCollections\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collections/{collection}/{lastModifiedStartDate}/{lastModifiedEndDate}\n  method: get\n  operationId: getModifiedCollections_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{packageId}/summary\n  method: get\n  operationId: packageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{packageId}/granules\n  method: get\n  operationId: getGranulesForPackage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /packages/{packageId}/granules/{granuleId}/summary\n  method: get\n  operationId: getGranuleContentDetail\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /published/{dateIssuedStartDate}\n  method: get\n  operationId: getPackagesByDateIssued\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /published/{dateIssuedStartDate}/{dateIssuedEndDate}\n  method: get\n  operationId: getPackagesByDateIssued_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related/{accessId}\n  method: get\n  operationId: relatedPackageDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /related/{accessId}/{collection}\n  method: get\n  operationId: relatedVersionsDetails\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govinfo/refs/heads/main/agentic-access/govinfo-agentic-access.yml
summary_line: 11 operations
tags:
- Federal Government
- Government Publishing
- Documents
- Open Data
---
