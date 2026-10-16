---
acting_count: 13
action_class_counts:
  acting: 13
  connected: 6
api_specs:
- filename: jitterbit-login-api-openapi.yml
  format: yaml
  label: Jitterbit Login API
  slug: jitterbit-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-login-api-openapi.yml
- filename: jitterbit-operations-api-openapi.yml
  format: yaml
  label: Jitterbit Operations API
  slug: jitterbit-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-operations-api-openapi.yml
- filename: jitterbit-projects-api-openapi.yml
  format: yaml
  label: Jitterbit Projects API
  slug: jitterbit-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-projects-api-openapi.yml
- filename: jitterbit-schedules-api-openapi.yml
  format: yaml
  label: Jitterbit Schedules API
  slug: jitterbit-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/openapi/jitterbit-schedules-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  safety-critical: 1
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Jitterbit Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /schedules-toggle
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /project
operation_count: 19
overview: 'Jitterbit exposes 19 API operations that an AI agent could call, of which 13 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 11 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Jitterbit
provider_slug: jitterbit
slug: jitterbit-agentic-access
source_filename: jitterbit-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: generated\nsource: openapi/jitterbit-login-api-openapi.yml, openapi/jitterbit-operations-api-openapi.yml,\n  openapi/jitterbit-projects-api-openapi.yml, openapi/jitterbit-schedules-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 13\n    connected: 6\n  by_consequence:\n    write: 11\n    read: 6\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /login\n  method: post\n  operationId: authenticate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /login\n  method: get\n  operationId: convertAuthtokenToJwt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation-logs\n  method: get\n  operationId: getOperationLogDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operation-logs\n  method: put\n  operationId: getOperationLogs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project\n  method: get\n  operationId: getProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /project\n  method: put\n  operationId: deployProject\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project\n  method: post\n  operationId: createProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project\n  method: delete\n  operationId: deleteProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-variables\n  method: get\n  operationId: projectVariablesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-variables\n  method: put\n  operationId: projectVariablesSet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /project-import-export\n  method: get\n  operationId: exportProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /project-import-export\n  method: post\n  operationId: importProject\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /migration\n  method: put\n  operationId: migrateProjectUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /migration\n  method: post\n  operationId: migrateProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedules\n  method:\
  \ get\n  operationId: getSchedules\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedules\n  method: put\n  operationId: updateSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedules\n  method: post\n  operationId: createSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedules\n  method: delete\n  operationId: deleteSchedules\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedules-toggle\n  method: put\n  operationId: enableDisableSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitterbit/refs/heads/main/agentic-access/jitterbit-agentic-access.yml
summary_line: 19 operations · 13 acting · 1 human-in-the-loop
tags:
- API Management
- Automation
- Integration
- iPaaS
- EDI
- Low-Code
- Enterprise
- API Gateway
- Workflow Automation
- Connectors
---
