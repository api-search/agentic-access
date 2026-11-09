---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: finddoc-ca-clinics-api-openapi.yml
  format: yaml
  label: FindDoc Clinics API
  slug: finddoc-ca-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-clinics-api-openapi.yml
- filename: finddoc-ca-doctors-api-openapi.yml
  format: yaml
  label: FindDoc Doctors API
  slug: finddoc-ca-doctors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-doctors-api-openapi.yml
- filename: finddoc-ca-health-api-openapi.yml
  format: yaml
  label: FindDoc Health API
  slug: finddoc-ca-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-health-api-openapi.yml
- filename: finddoc-ca-metadata-api-openapi.yml
  format: yaml
  label: FindDoc Metadata API
  slug: finddoc-ca-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-metadata-api-openapi.yml
- filename: finddoc-ca-specialists-api-openapi.yml
  format: yaml
  label: FindDoc Specialists API
  slug: finddoc-ca-specialists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-specialists-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finddoc Ca Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'FindDoc exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FindDoc
provider_slug: finddoc-ca
slug: finddoc-ca-agentic-access
source_filename: finddoc-ca-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/finddoc-ca-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiReadiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ping\n  method: get\n  operationId: getApiLiveness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doctors\n  method: get\n  operationId: listDoctors\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doctors/search\n  method: get\n  operationId: searchDoctors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doctors/summary\n  method: get\n  operationId: getDoctorSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doctors/{cpso}\n  method: get\n  operationId: getDoctor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /doctors/{cpso}/reviews\n  method: get\n  operationId: listDoctorReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /doctors/{cpso}/signals\n  method: get\n  operationId: getDoctorSignals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinics\n  method: get\n  operationId: listClinics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinics/{id}\n  method: get\n  operationId: getClinic\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinics/{id}/reviews\n  method: get\n  operationId: listClinicReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clinics/{id}/signals\n  method: get\n  operationId: getClinicSignals\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /specialists\n  method: get\n  operationId: listSpecialists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/specialties\n  method: get\n  operationId: listSpecialties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/finddoc-ca/agentic-access/finddoc-ca-agentic-access.yml
summary_line: 15 operations
tags:
- Healthcare
- API
- Doctors
- Clinics
- Canada
---
