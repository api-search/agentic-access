---
acting_count: 0
action_class_counts:
  connected: 13
api_specs:
- filename: yale-search-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Search API
  slug: yale-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-search-api-openapi.yml
- filename: yale-documents-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Documents API
  slug: yale-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-documents-api-openapi.yml
- filename: yale-facets-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Facets API
  slug: yale-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-facets-api-openapi.yml
- filename: yale-related-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Related API
  slug: yale-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-related-api-openapi.yml
- filename: yale-configuration-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Configuration API
  slug: yale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-configuration-api-openapi.yml
- filename: yale-federation-api-openapi.yml
  format: yaml
  label: Yale University Federation API
  slug: yale-federation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-federation-api-openapi.yml
- filename: yale-iiif-api-openapi.yml
  format: yaml
  label: Yale University IIIF API
  slug: yale-iiif-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-iiif-api-openapi.yml
- filename: yale-info-api-openapi.yml
  format: yaml
  label: Yale University Info API
  slug: yale-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-info-api-openapi.yml
consequence_counts:
  read: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Yale Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Yale University exposes 13 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yale University
provider_slug: yale
slug: yale-agentic-access
source_filename: yale-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/yale-configuration-api-openapi.yml, openapi/yale-documents-api-openapi.yml,\n  openapi/yale-facets-api-openapi.yml, openapi/yale-federation-api-openapi.yml, openapi/yale-iiif-api-openapi.yml,\n  openapi/yale-info-api-openapi.yml, openapi/yale-related-api-openapi.yml, openapi/yale-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 13\n  by_consequence:\n    read: 13\n  human_in_the_loop_required: 0\noperations:\n- path: /api/advanced-search-config\n  method: get\n  operationId: advancedSearchConfig\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /data/{type}/{id}\n  method: get\n  operationId: getDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/facets/{scope}\n  method: get\n  operationId: facets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /idp/shibboleth\n  method: get\n  operationId: getIdpMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifests/{oid}\n  method: get\n  operationId: getManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/info/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/info/server\n  method: get\n  operationId: getServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/info/metrics/datasets\n  method: get\n  operationId: getDatasetMetrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/metadatablocks/{name}\n  method: get\n  operationId: getMetadataBlock\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/related-list/{scope}\n  method: get\n  operationId: relatedList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /api/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search/{scope}\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/search-estimate/{scope}\n  method: get\n  operationId: searchEstimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/agentic-access/yale-agentic-access.yml
summary_line: 13 operations
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Research
- Research Data
- Research Repository
- Identity Federation
- Library
- Cultural Heritage
- Linked Data
- IIIF
- Course Catalog
---
