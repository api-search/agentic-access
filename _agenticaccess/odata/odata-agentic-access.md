---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: odata-batch-api-openapi.yml
  format: yaml
  label: OData $Batch API
  slug: odata-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-batch-api-openapi.yml
- filename: odata-metadata-api-openapi.yml
  format: yaml
  label: OData $Metadata API
  slug: odata-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-metadata-api-openapi.yml
- filename: odata-odata-service-api-api-openapi.yml
  format: yaml
  label: OData Service API
  slug: odata-odata-service-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odata/openapi/odata-odata-service-api-api-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Odata Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'OData exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OData
provider_slug: odata
slug: odata-agentic-access
source_filename: odata-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/odata-batch-api-openapi.yml, openapi/odata-metadata-api-openapi.yml, openapi/odata-odata-service-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 4\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /$batch\n  method: post\n  operationId: executeBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /$metadata\n  method: get\n  operationId:\
  \ getMetadataDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getServiceDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entitySet}\n  method: get\n  operationId: getEntityCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entitySet}\n  method: post\n  operationId: createEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{entitySet}({key})\n  method: get\n  operationId: getEntity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{entitySet}({key})\n  method: patch\n  operationId: updateEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{entitySet}({key})\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/odata/agentic-access/odata-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- OASIS Standard
- OData
- Open Data Protocol
- Query Language
- RESTful APIs
---
