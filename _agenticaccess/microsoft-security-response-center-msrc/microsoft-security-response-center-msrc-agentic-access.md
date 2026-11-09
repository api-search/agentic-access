---
acting_count: 0
action_class_counts:
  connected: 52
api_specs:
- filename: microsoft-security-response-center-msrc-acknowledgement-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Acknowledgement API
  slug: microsoft-security-response-center-msrc-acknowledgement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-acknowledgement-api-openapi.yml
- filename: microsoft-security-response-center-msrc-advisory-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Advisory API
  slug: microsoft-security-response-center-msrc-advisory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-advisory-api-openapi.yml
- filename: microsoft-security-response-center-msrc-affectedproduct-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Affected Product API
  slug: microsoft-security-response-center-msrc-affectedproduct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-affectedproduct-api-openapi.yml
- filename: microsoft-security-response-center-msrc-csaf-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Csaf API
  slug: microsoft-security-response-center-msrc-csaf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-csaf-api-openapi.yml
- filename: microsoft-security-response-center-msrc-cvrf-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Cvrf API
  slug: microsoft-security-response-center-msrc-cvrf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-cvrf-api-openapi.yml
- filename: microsoft-security-response-center-msrc-deployment-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Deployment API
  slug: microsoft-security-response-center-msrc-deployment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-deployment-api-openapi.yml
- filename: microsoft-security-response-center-msrc-headercontent-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Header Content API
  slug: microsoft-security-response-center-msrc-headercontent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-headercontent-api-openapi.yml
- filename: microsoft-security-response-center-msrc-metadata-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Metadata API
  slug: microsoft-security-response-center-msrc-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-metadata-api-openapi.yml
- filename: microsoft-security-response-center-msrc-releasenote-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Release Note API
  slug: microsoft-security-response-center-msrc-releasenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-releasenote-api-openapi.yml
- filename: microsoft-security-response-center-msrc-revisionnote-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Revision Note API
  slug: microsoft-security-response-center-msrc-revisionnote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-revisionnote-api-openapi.yml
- filename: microsoft-security-response-center-msrc-updates-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Updates API
  slug: microsoft-security-response-center-msrc-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-updates-api-openapi.yml
- filename: microsoft-security-response-center-msrc-vulnerability-api-openapi.yml
  format: yaml
  label: Microsoft Security Response Center (MSRC) Vulnerability API
  slug: microsoft-security-response-center-msrc-vulnerability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-security-response-center-msrc/openapi/microsoft-security-response-center-msrc-vulnerability-api-openapi.yml
consequence_counts:
  read: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Security Response Center Msrc Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 52
overview: 'Microsoft Security Response Center (MSRC) exposes 52 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 52 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Security Response Center (MSRC)
provider_slug: microsoft-security-response-center-msrc
slug: microsoft-security-response-center-msrc-agentic-access
source_filename: microsoft-security-response-center-msrc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/microsoft-security-response-center-msrc-cvrf-openapi.yml, openapi/microsoft-security-response-center-msrc-sug-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 52\n  by_consequence:\n    read: 52\n  human_in_the_loop_required: 0\noperations:\n- path: /csaf/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cvrf({id})\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /./$metadata\n  method: get\n  operationId: ./$metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /$metadata\n  method: get\n  operationId: $metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.\n  method: get\n  operationId: ./\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updates\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Updates\n  method: get\n  operationId: Updates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Updates/$count\n  method: get\n  operationId: Updates/$count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updates({key})\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updates/{key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Updates({key})\n  method: get\n  operationId: Updates({key})\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Updates/{key}\n  method: get\n  operationId: Updates/{key}\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/acknowledgement({key})\n  method: get\n  operationId: '{culture}/acknowledgement({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/acknowledgement/{key}\n  method: get\n  operationId: '{culture}/acknowledgement/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/acknowledgement\n  method: get\n  operationId: '{culture}/acknowledgement'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/acknowledgement/$count\n  method: get\n  operationId: '{culture}/acknowledgement/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/advisory({key})\n  method: get\n  operationId: '{culture}/advisory({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/advisory/{key}\n  method: get\n  operationId: '{culture}/advisory/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/advisory\n  method: get\n  operationId: '{culture}/advisory'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /{culture}/advisory/$count\n  method: get\n  operationId: '{culture}/advisory/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/affectedProduct({key})\n  method: get\n  operationId: '{culture}/affectedProduct({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/affectedProduct/{key}\n  method: get\n  operationId: '{culture}/affectedProduct/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/affectedProduct\n  method: get\n  operationId: '{culture}/affectedProduct'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{culture}/affectedProduct/$count\n  method: get\n  operationId: '{culture}/affectedProduct/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/deployment({key})\n  method: get\n  operationId: '{culture}/deployment({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/deployment/{key}\n  method: get\n  operationId: '{culture}/deployment/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/deployment\n  method: get\n  operationId: '{culture}/deployment'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /{culture}/deployment/$count\n  method: get\n  operationId: '{culture}/deployment/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/headerContent({key})\n  method: get\n  operationId: '{culture}/headerContent({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/headerContent/{key}\n  method: get\n  operationId: '{culture}/headerContent/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/headerContent\n  method: get\n  operationId: '{culture}/headerContent'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/headerContent/$count\n\
  \  method: get\n  operationId: '{culture}/headerContent/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/metadata({key})\n  method: get\n  operationId: '{culture}/metadata({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/metadata/{key}\n  method: get\n  operationId: '{culture}/metadata/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/metadata\n  method: get\n  operationId: '{culture}/metadata'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/metadata/$count\n  method: get\n  operationId: '{culture}/metadata/$count'\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/$metadata\n  method: get\n  operationId: '{culture}/$metadata'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}\n  method: get\n  operationId: '{culture}/'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/releaseNote({key})\n  method: get\n  operationId: '{culture}/releaseNote({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/releaseNote/{key}\n  method: get\n  operationId: '{culture}/releaseNote/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/releaseNote\n  method: get\n  operationId: '{culture}/releaseNote'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/releaseNote/$count\n  method: get\n  operationId: '{culture}/releaseNote/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/revisionNote({key})\n  method: get\n  operationId: '{culture}/revisionNote({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/revisionNote/{key}\n  method: get\n  operationId: '{culture}/revisionNote/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/revisionNote\n  method: get\n  operationId: '{culture}/revisionNote'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/revisionNote/$count\n  method: get\n  operationId: '{culture}/revisionNote/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/vulnerability({key})\n  method: get\n  operationId: '{culture}/vulnerability({key})'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/vulnerability/{key}\n  method: get\n  operationId: '{culture}/vulnerability/{key}'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /{culture}/vulnerability\n  method: get\n  operationId: '{culture}/vulnerability'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{culture}/vulnerability/$count\n  method: get\n  operationId: '{culture}/vulnerability/$count'\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/microsoft-security-response-center-msrc/agentic-access/microsoft-security-response-center-msrc-agentic-access.yml
summary_line: 52 operations
tags:
- CSAF
- CVRF
- OData
- Public APIs
- Security
- Security Updates
- Vulnerabilities
---
