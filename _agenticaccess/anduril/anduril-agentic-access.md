---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 11
api_specs:
- filename: anduril-entities-api-openapi.yml
  format: yaml
  label: Anduril Industries Entities API
  slug: anduril-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-entities-api-openapi.yml
- filename: anduril-objects-api-openapi.yml
  format: yaml
  label: Anduril Industries Objects API
  slug: anduril-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-objects-api-openapi.yml
- filename: anduril-tasks-api-openapi.yml
  format: yaml
  label: Anduril Industries Tasks API
  slug: anduril-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-tasks-api-openapi.yml
- filename: anduril-oauth-api-openapi.yml
  format: yaml
  label: Anduril Industries O Auth API
  slug: anduril-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-oauth-api-openapi.yml
consequence_counts:
  read: 11
  safety-critical: 2
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Anduril Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /entities/{entity_id}/override
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /entities/{entity_id}/override/{field_path}
operation_count: 22
overview: 'Anduril Industries exposes 22 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 9 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anduril Industries
provider_slug: anduril
slug: anduril-agentic-access
source_filename: anduril-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/anduril-entities-api-openapi.yml, openapi/anduril-oauth-api-openapi.yml, openapi/anduril-objects-api-openapi.yml,\n  openapi/anduril-tasks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 22\n  by_action_class:\n    acting: 11\n    connected: 11\n  by_consequence:\n    write: 9\n    read: 11\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /entities\n  method: post\n  operationId: postEntities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /entities/{entity_id}\n  method: get\n  operationId: getEntitiesByEntityId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /entities/{entity_id}/override\n  method: patch\n  operationId: patchEntitiesByEntityIdOverride\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /entities/{entity_id}/override/{field_path}\n  method: delete\n  operationId: deleteEntitiesByEntityIdOverrideByFieldPath\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /entities/events:longPoll\n  method: post\n  operationId: postEntitiesEvents:longPoll\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /entities:stream\n  method: get\n  operationId: getEntities:stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: postOauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /objects\n  method: get\n  operationId: getObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects:listDeleted\n  method: get\n  operationId: getObjects:listDeleted\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{object_path}\n  method: get\n  operationId: getObjectsByObjectPath\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /objects/{object_path}\n  method: put\n  operationId: putObjectsByObjectPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{object_path}\n  method: delete\n  operationId: deleteObjectsByObjectPath\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /objects/{object_path}:metadata\n  method: get\n  operationId: getObjects{objectPath}:metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks\n  method: post\n  operationId: postTasks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /tasks/{task_id}\n  method: get\n  operationId: getTasksByTaskId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks/{task_id}/status\n  method: patch\n  operationId: patchTasksByTaskIdStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks/{task_id}:cancel\n  method: post\n  operationId: postTasks{taskId}:cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks:query\n\
  \  method: post\n  operationId: postTasks:query\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks:stream\n  method: get\n  operationId: getTasks:stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tasks:listenAsAgent\n  method: post\n  operationId: postTasks:listenAsAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks:streamAsAgent\n  method: get\n  operationId: getTasks:streamAsAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /tasks/{task_id}/manualControlFrames:stream\n  method: get\n  operationId: getTasksByTaskIdManualControlFrames:stream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/agentic-access/anduril-agentic-access.yml
summary_line: 22 operations · 11 acting · 2 human-in-the-loop
tags:
- Defense
- Autonomy
- Lattice
- Command and Control
- C2
- Sensors
- Effectors
- Counter-UAS
- Unmanned Systems
- Mission Software
- Edge AI
- ITAR
---
