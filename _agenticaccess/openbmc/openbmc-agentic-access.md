---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: openbmc-openapi.yml
  format: yaml
  label: OpenBMC API
  slug: openbmc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/openapi/openbmc-openapi.yml
consequence_counts:
  read: 7
  safety-critical: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Openbmc Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Managers/bmc/Actions/Manager.Reset
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Managers/bmc/Actions/Manager.ResetToDefaults
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /Systems/system/Actions/ComputerSystem.Reset
operation_count: 13
overview: 'OpenBMC exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 3 write, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenBMC
provider_slug: openbmc
slug: openbmc-agentic-access
source_filename: openbmc-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openbmc-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 3\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /\n  method: get\n  operationId: getServiceRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /SessionService/Sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Chassis\n  method: get\n  operationId: listChassis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Managers\n  method: get\n  operationId: listManagers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Systems\n  method: get\n  operationId: listSystems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Systems/system/Actions/ComputerSystem.Reset\n  method: post\n  operationId: resetComputerSystem\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n  \
  \    exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /Managers/bmc/Actions/Manager.Reset\n  method: post\n  operationId: resetBmc\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /Managers/bmc/Actions/Manager.ResetToDefaults\n  method: post\n  operationId: resetBmcToDefaults\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /Systems/system/LogServices/EventLog/Entries\n\
  \  method: get\n  operationId: getEventLogEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /UpdateService\n  method: get\n  operationId: getUpdateService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /AccountService/Accounts/root\n  method: patch\n  operationId: patchRootAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /EventService/Subscriptions\n  method: get\n  operationId: listEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /EventService/Subscriptions\n  method: post\n  operationId: createEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openbmc/refs/heads/main/agentic-access/openbmc-agentic-access.yml
summary_line: 13 operations · 6 acting · 3 human-in-the-loop
tags:
- Firmware
- Hardware
- Linux Foundation
- Server
---
