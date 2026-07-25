---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: opencitations-authors-api-openapi.yml
  format: yaml
  label: OpenCitations Authors API
  slug: opencitations-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-authors-api-openapi.yml
- filename: opencitations-citations-api-openapi.yml
  format: yaml
  label: OpenCitations Citations API
  slug: opencitations-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-citations-api-openapi.yml
- filename: opencitations-editors-api-openapi.yml
  format: yaml
  label: OpenCitations Editors API
  slug: opencitations-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-editors-api-openapi.yml
- filename: opencitations-metadata-api-openapi.yml
  format: yaml
  label: OpenCitations Metadata API
  slug: opencitations-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-metadata-api-openapi.yml
- filename: opencitations-references-api-openapi.yml
  format: yaml
  label: OpenCitations References API
  slug: opencitations-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-references-api-openapi.yml
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Opencitations Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'OpenCitations exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenCitations
provider_slug: opencitations
slug: opencitations-agentic-access
source_filename: opencitations-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/index-api.yml, openapi/meta-api.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /citation/{oci}\n  method: get\n  operationId: getCitationByOCI\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /citation-count/{id}\n  method: get\n  operationId: getCitationCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /venue-citation-count/{id}\n  method:\
  \ get\n  operationId: getVenueCitationCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference-count/{id}\n  method: get\n  operationId: getReferenceCount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /citations/{id}\n  method: get\n  operationId: getCitations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /references/{id}\n  method: get\n  operationId: getReferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metadata/{ids}\n  method: get\n  operationId: getMetadataByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /author/{id}\n  method: get\n  operationId: getWorksByAuthor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /editor/{id}\n  method: get\n  operationId: getWorksByEditor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/agentic-access/opencitations-agentic-access.yml
summary_line: 9 operations
tags:
- Citations
- Scholarly
- Research
- Open Science
- Bibliometrics
- DOI
- Academic
---
