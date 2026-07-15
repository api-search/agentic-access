---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: cfpb-ccdb-openapi.yml
  format: yaml
  label: Consumer Complaint Database API
  slug: ccdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/cfpb-ccdb-openapi.yml
- filename: cfpb-hmda-data-browser-openapi.yml
  format: yaml
  label: HMDA Data Browser API
  slug: hmda-data-browser
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/cfpb-hmda-data-browser-openapi.yml
- filename: cfpb-hmda-institutions-openapi.yml
  format: yaml
  label: HMDA Institutions API
  slug: hmda-institutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/openapi/cfpb-hmda-institutions-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Consumer Financial Protection Bureau Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Consumer Financial Protection Bureau exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Consumer Financial Protection Bureau
provider_slug: consumer-financial-protection-bureau
slug: consumer-financial-protection-bureau-agentic-access
source_filename: consumer-financial-protection-bureau-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cfpb-ccdb-openapi.yml, openapi/cfpb-hmda-data-browser-openapi.yml, openapi/cfpb-hmda-institutions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: searchComplaints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{complaintId}/\n  method: get\n  operationId: getComplaint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /trends/\n  method: get\n  operationId: getTrends\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/states/\n  method: get\n  operationId: getGeoStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suggest/\n  method: get\n  operationId: getSuggestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/nationwide/aggregations\n  method: get\n  operationId: getNationwideAggregations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/aggregations\n  method: get\n  operationId: getAggregations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/nationwide/csv\n  method: get\n  operationId: getNationwideCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/csv\n  method: get\n  operationId: getCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /view/filers\n  method: get\n  operationId: listFilers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/filers/{year}\n  method: get\n  operationId: listInstitutionsByYear\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /public/institutions/{year}/{lei}\n\
  \  method: get\n  operationId: getInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/agentic-access/consumer-financial-protection-bureau-agentic-access.yml
summary_line: 12 operations
tags:
- Banking
- Complaints
- Consumer Protection
- Federal Government
- Financial Services
- HMDA
- Mortgages
- Open Data
---
