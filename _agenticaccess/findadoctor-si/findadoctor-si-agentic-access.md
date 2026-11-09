---
acting_count: 0
action_class_counts:
  connected: 20
api_specs:
- filename: findadoctor-si-about-api-openapi.yml
  format: yaml
  label: findadoctor-si About API
  slug: findadoctor-si-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-about-api-openapi.yml
- filename: findadoctor-si-doctors-api-openapi.yml
  format: yaml
  label: findadoctor-si Doctors API
  slug: findadoctor-si-doctors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-doctors-api-openapi.yml
- filename: findadoctor-si-gp-practices-api-openapi.yml
  format: yaml
  label: findadoctor-si Gp Practices API
  slug: findadoctor-si-gp-practices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-gp-practices-api-openapi.yml
- filename: findadoctor-si-procedure-volumes-api-openapi.yml
  format: yaml
  label: findadoctor-si Procedure Volumes API
  slug: findadoctor-si-procedure-volumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-procedure-volumes-api-openapi.yml
- filename: findadoctor-si-procedures-api-openapi.yml
  format: yaml
  label: findadoctor-si Procedures API
  slug: findadoctor-si-procedures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-procedures-api-openapi.yml
- filename: findadoctor-si-search-api-openapi.yml
  format: yaml
  label: findadoctor-si Search API
  slug: findadoctor-si-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-search-api-openapi.yml
- filename: findadoctor-si-specialties-api-openapi.yml
  format: yaml
  label: findadoctor-si Specialties API
  slug: findadoctor-si-specialties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-specialties-api-openapi.yml
- filename: findadoctor-si-terms-api-openapi.yml
  format: yaml
  label: findadoctor-si Terms API
  slug: findadoctor-si-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-terms-api-openapi.yml
- filename: findadoctor-si-waitlist-api-openapi.yml
  format: yaml
  label: findadoctor-si Waitlist API
  slug: findadoctor-si-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-waitlist-api-openapi.yml
consequence_counts:
  read: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Findadoctor Si Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'findadoctor-si exposes 20 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: findadoctor-si
provider_slug: findadoctor-si
slug: findadoctor-si-agentic-access
source_filename: findadoctor-si-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/findadoctor-si-fr-openapi.json, openapi/findadoctor-si-nz-openapi.json, openapi/findadoctor-si-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 20\n  by_consequence:\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/search\n  method: get\n  operationId: searchDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/doctors/{doctor_id}\n  method: get\n  operationId: getDoctor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/doctors\n  method: get\n  operationId: getDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/procedure-volumes\n  method: get\n  operationId: hospitalProcedureVolumes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/specialties\n  method: get\n  operationId: listSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/about\n  method: get\n  operationId: aboutDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchDoctors\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/doctors/{doctor_id}\n  method: get\n  operationId: getDoctor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/doctors\n  method: get\n  operationId: getDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/gp-practices\n  method: get\n  operationId: searchGpPractices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/specialties\n  method: get\n  operationId: listSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/waitlist\n  method: get\n  operationId: publicWaitlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/about\n  method: get\n  operationId: aboutDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  operationId: searchDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/doctors/{doctor_id}\n  method: get\n  operationId: getDoctor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/doctors\n  method: get\n  operationId: getDoctors\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/terms\n  method: get\n  operationId: lookupTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/procedures\n  method: get\n  operationId: listProcedures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/specialties\n  method: get\n  operationId: listSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/about\n  method: get\n  operationId: aboutDatabase\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/findadoctor-si/agentic-access/findadoctor-si-agentic-access.yml
summary_line: 20 operations
tags:
- Company
- Healthcare
- Data
- Artificial Intelligence
- Doctor
- International
---
