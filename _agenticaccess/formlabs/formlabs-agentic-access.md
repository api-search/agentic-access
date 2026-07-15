---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Printers
  slug: formlabs-web-api-printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Prints
  slug: formlabs-web-api-prints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Consumables
  slug: formlabs-web-api-consumables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Events
  slug: formlabs-web-api-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Groups
  slug: formlabs-web-api-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
consequence_counts:
  physical: 1
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Formlabs Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /groups/{group_id}/members/
operation_count: 16
overview: 'Formlabs exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 6 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Formlabs
provider_slug: formlabs
slug: formlabs-agentic-access
source_filename: formlabs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/formlabs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 6\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /printers/\n  method: get\n  operationId: listPrinters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /printers/{printer_serial}/\n  method: get\n  operationId: getPrinter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /printers/{printer_serial}/prints/\n\
  \  method: get\n  operationId: listPrinterPrints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /prints/\n  method: get\n  operationId: listPrints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tanks/\n  method: get\n  operationId: listTanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cartridges/\n  method: get\n  operationId: listCartridges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /groups/\n  method: get\n  operationId: listGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/\n  method: post\n  operationId: createGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/\n  method: patch\n  operationId: updateGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/\n  method: delete\n  operationId: deleteGroup\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/bulk-add-printers/\n  method: post\n  operationId: bulkAddPrintersToGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/members/\n  method: post\n  operationId: inviteGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/members/\n\
  \  method: put\n  operationId: updateGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/members/\n  method: delete\n  operationId: removeGroupMember\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group_id}/queue/\n  method: get\n  operationId: listGroupQueue\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/agentic-access/formlabs-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- 3D Printing
- Additive Manufacturing
- SLA
- SLS
- Hardware
- Dashboard
---
