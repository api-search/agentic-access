---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: als-global-preference-api-openapi.yml
  format: yaml
  label: ALS Preference API
  slug: als-global-preference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-preference-api-openapi.yml
- filename: als-global-sample-api-openapi.yml
  format: yaml
  label: ALS Sample API
  slug: als-global-sample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-sample-api-openapi.yml
- filename: als-global-search-api-openapi.yml
  format: yaml
  label: ALS Search API
  slug: als-global-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/openapi/als-global-search-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Als Global Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'ALS exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ALS
provider_slug: als-global
slug: als-global-agentic-access
source_filename: als-global-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: generated\nsource: openapi/als-global-webtrieve-export-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 5\n    acting: 1\n  by_consequence:\n    read: 5\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /Preference/Version\n  method: get\n  operationId: Preference_Version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SampleSubmission/SampleSubmission\n  method: post\n  operationId: Sample_SampleSubmissionImport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /SampleSubmission/GetSubmissionsDetails\n  method: post\n  operationId: Sample_SampleSubmissionGetDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SampleSubmission/GetPrintLabels\n  method: post\n  operationId: Sample_SampleSubmissionGetPrintLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SampleResultsExport/SampleResults\n  method: post\n  operationId: Search_GetSampleExportResultsExposed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SampleResultsExport/GetSyncTime\n  method: get\n  operationId:\
  \ Search_GetSampleSyncTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/als-global/refs/heads/main/agentic-access/als-global-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Company
- Laboratory Testing
- Environmental Testing
- Inspection
- Certification
- Geochemistry
- Food Testing
- LIMS Integration
---
