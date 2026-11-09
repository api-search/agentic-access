---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: startup-jobs-companies-api-openapi.yml
  format: yaml
  label: startup-jobs Companies API
  slug: startup-jobs-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-companies-api-openapi.yml
- filename: startup-jobs-jobs-api-openapi.yml
  format: yaml
  label: startup-jobs Jobs API
  slug: startup-jobs-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-jobs-api-openapi.yml
- filename: startup-jobs-locations-api-openapi.yml
  format: yaml
  label: startup-jobs Locations API
  slug: startup-jobs-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-locations-api-openapi.yml
- filename: startup-jobs-openapi-json-api-openapi.yml
  format: yaml
  label: startup-jobs Openapi.json API
  slug: startup-jobs-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-openapi-json-api-openapi.yml
- filename: startup-jobs-roles-api-openapi.yml
  format: yaml
  label: startup-jobs Roles API
  slug: startup-jobs-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/startup-jobs/openapi/startup-jobs-roles-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Startup Jobs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'startup-jobs exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: startup-jobs
provider_slug: startup-jobs
slug: startup-jobs-agentic-access
source_filename: startup-jobs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/startup-jobs-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{slug}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/{slug}/jobs\n  method: get\n  operationId: listCompanyJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/roles\n  method: get\n  operationId: listRoles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  operationId: getOpenApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/startup-jobs/agentic-access/startup-jobs-agentic-access.yml
summary_line: 7 operations
tags:
- Company
---
