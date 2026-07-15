---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat API
  slug: ecobee-thermostat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Thermostat Update and Functions API
  slug: ecobee-thermostat-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Runtime Report API
  slug: ecobee-runtime-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Group API
  slug: ecobee-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Demand Response API
  slug: ecobee-demand-response-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Hierarchy API
  slug: ecobee-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Meter Report API
  slug: ecobee-meter-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
- filename: ecobee-openapi.yml
  format: yaml
  label: ecobee Authorization API
  slug: ecobee-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/openapi/ecobee-openapi.yml
consequence_counts:
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ecobee Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'ecobee exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ecobee
provider_slug: ecobee
slug: ecobee-agentic-access
source_filename: ecobee-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ecobee-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /thermostat\n  method: get\n  operationId: getThermostats\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /thermostat\n  method: post\n  operationId: updateThermostats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /thermostatSummary\n  method: get\n  operationId: getThermostatSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /runtimeReport\n  method: get\n  operationId: getRuntimeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /meterReport\n  method: get\n  operationId: getMeterReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group\n  method: get\n  operationId: getGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /group\n  method: post\n  operationId: updateGroups\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /demandResponse\n  method: get\n  operationId: listDemandResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demandResponse\n  method: post\n  operationId: issueDemandResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy/thermostat\n  method: post\n  operationId: hierarchyThermostat\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy/set\n  method: get\n  operationId: listHierarchySets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hierarchy/set\n  method: post\n  operationId: manageHierarchySet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hierarchy/user\n  method: get\n  operationId: listHierarchyUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /hierarchy/user\n  method: post\n  operationId: manageHierarchyUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecobee/refs/heads/main/agentic-access/ecobee-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- Smart Home
- Thermostat
- IoT
- HVAC
- Energy
- Home Automation
- Demand Response
---
