---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: federal-motor-carrier-safety-administration-openapi.yml
  format: yaml
  label: Federal Motor Carrier Safety Administration QCMobile API
  slug: federal-motor-carrier-safety-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/openapi/federal-motor-carrier-safety-administration-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Federal Motor Carrier Safety Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Federal Motor Carrier Safety Administration exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Federal Motor Carrier Safety Administration
provider_slug: federal-motor-carrier-safety-administration
slug: federal-motor-carrier-safety-administration-agentic-access
source_filename: federal-motor-carrier-safety-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/federal-motor-carrier-safety-administration-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /carriers/{dotNumber}\n  method: get\n  operationId: getCarrierByDotNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/name/{name}\n  method: get\n  operationId: searchCarriersByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/cargo-carried\n\
  \  method: get\n  operationId: getCarrierCargoCarried\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/operation-classification\n  method: get\n  operationId: getCarrierOperationClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/oos\n  method: get\n  operationId: getCarrierOos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/docket-numbers\n  method: get\n  operationId: getCarrierDocketNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /carriers/{dotNumber}/authority\n  method: get\n  operationId:\
  \ getCarrierAuthority\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/agentic-access/federal-motor-carrier-safety-administration-agentic-access.yml
summary_line: 7 operations
tags:
- Federal Government
- Safety
- Transportation
---
