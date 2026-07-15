---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Jobs API
  slug: workiz-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Leads API
  slug: workiz-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Team API
  slug: workiz-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Time Off API
  slug: workiz-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Payments API
  slug: workiz-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
- filename: workiz-openapi.yml
  format: yaml
  label: Workiz Webhooks
  slug: workiz-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/openapi/workiz-openapi.yml
consequence_counts:
  physical: 1
  read: 8
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workiz Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /job/addPayment/{UUID}/
operation_count: 15
overview: 'Workiz exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Workiz
provider_slug: workiz
slug: workiz-agentic-access
source_filename: workiz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workiz-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /job/all/\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/get/{UUID}/\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /job/create/\n  method: post\n  operationId:\
  \ createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/update/\n  method: post\n  operationId: updateJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/assign/\n  method: post\n  operationId: assignJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/unassign/\n  method:\
  \ post\n  operationId: unassignJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /job/addPayment/{UUID}/\n  method: post\n  operationId: addJobPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lead/all/\n  method: get\n  operationId: listLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lead/get/{UUID}/\n  method: get\n  operationId: getLead\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lead/create/\n  method: post\n  operationId: createLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lead/update/\n  method: post\n  operationId: updateLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /team/all/\n  method: get\n  operationId: listTeam\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /team/get/{USER_ID}/\n  method: get\n  operationId: getTeamMember\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeoff/get/\n  method: get\n  operationId: listTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /timeoff/get/{USER_NAME}/\n  method: get\n  operationId: getUserTimeOff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workiz/refs/heads/main/agentic-access/workiz-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- Field Service Management
- FSM
- Home Services
- Scheduling
- Dispatch
- CRM
- Jobs
- Invoicing
---
