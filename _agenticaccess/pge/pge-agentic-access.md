---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: pge-applicationinformation-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Application Information API
  slug: pge-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-applicationinformation-api-openapi.yml
- filename: pge-authorization-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Authorization API
  slug: pge-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-authorization-api-openapi.yml
- filename: pge-batch-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Batch API
  slug: pge-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-batch-api-openapi.yml
- filename: pge-usagepoint-api-openapi.yml
  format: yaml
  label: Pacific Gas and Electric Usage Point API
  slug: pge-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/openapi/pge-usagepoint-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pge Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Pacific Gas and Electric exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Pacific Gas and Electric
provider_slug: pge
slug: pge-agentic-access
source_filename: pge-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/green-button-alliance-espi-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /espi/1_1/resource/ApplicationInformation\n  method: get\n  operationId: findApplicationInformations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/ApplicationInformation/{applicationInformationId}\n  method: get\n  operationId: getApplicationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Authorization\n  method: get\n  operationId: findAuthorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Authorization/{authorizationId}\n  method: get\n  operationId: getAuthorization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/Batch/Bulk/{bulkId}\n  method: get\n  operationId: downloadBulkData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /espi/1_1/resource/UsagePoint\n  method: get\n  operationId: findUsagePoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /espi/1_1/resource/UsagePoint/{usagePointId}\n  method: get\n  operationId: getUsagePoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pge/refs/heads/main/agentic-access/pge-agentic-access.yml
summary_line: 7 operations
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- California
- Smart Metering
- Green Button
- ESPI
- Energy Data
- Grid
- Demand Response
- Investor-Owned Utility
---
