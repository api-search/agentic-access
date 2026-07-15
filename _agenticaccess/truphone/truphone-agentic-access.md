---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 11
api_specs:
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) SIMs / eSIMs API
  slug: truphone-sims-esims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Connectivity / Usage API
  slug: truphone-connectivity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Plans API
  slug: truphone-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
- filename: truphone-openapi.yml
  format: yaml
  label: Truphone (1GLOBAL) Device Management API
  slug: truphone-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/openapi/truphone-openapi.yml
consequence_counts:
  read: 11
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Truphone Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'Truphone (1GLOBAL) exposes 17 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Truphone (1GLOBAL)
provider_slug: truphone
slug: truphone-agentic-access
source_filename: truphone-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/truphone-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 11\n    acting: 6\n  by_consequence:\n    read: 11\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v2.2/sims\n  method: get\n  operationId: listSims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.2/sims/{iccid}\n  method: get\n  operationId: getSim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.2/sims/{iccid}\n  method: patch\n  operationId:\
  \ updateSim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.2/sims/{iccid}/status\n  method: get\n  operationId: getSimStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/sims/change_status\n  method: post\n  operationId: changeSimStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/sims/change_data_status\n  method: post\n  operationId: changeDataStatus\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/sims/ongoing_sessions\n  method: get\n  operationId: listOngoingSessions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/sims/{iccid}/cdr\n  method: get\n  operationId: listCdrs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/rate_plans\n  method: get\n  operationId: listRatePlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/rate_plans/{id}\n  method: get\n  operationId: getRatePlan\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/sims/{iccid}/subscription\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/sims/{iccid}/subscription\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.2/devices\n  method: get\n  operationId: listDevices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.2/devices/{id}\n  method: get\n  operationId:\
  \ getDevice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.2/devices/{id}\n  method: patch\n  operationId: updateDevice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2.0/tags\n  method: get\n  operationId: listTags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2.0/tags\n  method: post\n  operationId: createTag\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truphone/refs/heads/main/agentic-access/truphone-agentic-access.yml
summary_line: 17 operations · 6 acting
tags:
- eSIM
- IoT
- Connectivity
- SIM Management
- Telecom
- Mobile Network
---
