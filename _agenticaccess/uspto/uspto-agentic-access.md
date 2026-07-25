---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: uspto-assignments-api-openapi.yml
  format: yaml
  label: USPTO Assignments API
  slug: uspto-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-assignments-api-openapi.yml
- filename: uspto-patents-api-openapi.yml
  format: yaml
  label: USPTO Patents API
  slug: uspto-patents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-patents-api-openapi.yml
- filename: uspto-ptab-api-openapi.yml
  format: yaml
  label: USPTO PTAB API
  slug: uspto-ptab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-ptab-api-openapi.yml
- filename: uspto-trademarks-api-openapi.yml
  format: yaml
  label: USPTO Trademarks API
  slug: uspto-trademarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/openapi/uspto-trademarks-api-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uspto Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'USPTO exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: USPTO
provider_slug: uspto
slug: uspto-agentic-access
source_filename: uspto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uspto-patent-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /patent/applications/search\n  method: get\n  operationId: searchPatentApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patent/applications/{applicationNumber}\n  method: get\n  operationId: getPatentApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /patent/grants/{patentNumber}\n  method: get\n  operationId: getGrantedPatent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ptab/trials\n  method: get\n  operationId: searchPTABTrials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ptab/trials/{trialNumber}\n  method: get\n  operationId: getPTABTrial\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ptab/decisions/search\n  method: get\n  operationId: searchPTABDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trademark/status/{serialNumber}\n  method: get\n  operationId: getTrademarkStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /patent/assignments/search\n  method: get\n  operationId: searchPatentAssignments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uspto/refs/heads/main/agentic-access/uspto-agentic-access.yml
summary_line: 8 operations
tags:
- Government
- Intellectual Property
- Open Data
- Patents
- Regulatory
- Trademarks
- USPTO
---
