---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 10
api_specs:
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Data Service API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless User Service API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless File Service API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Messaging and Push API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Geo Service API
  slug: geo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cache and Atomic Counters API
  slug: cache-counters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cloud Code API
  slug: cloud-code
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Backendless Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /counters/{counter-name}/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messaging/email
operation_count: 26
overview: 'Backendless exposes 26 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 14 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Backendless
provider_slug: backendless
slug: backendless-agentic-access
source_filename: backendless-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/backendless-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 16\n    connected: 10\n  by_consequence:\n    write: 14\n    read: 10\n    physical: 1\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /data/{table-name}\n  method: post\n  operationId: createObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table-name}\n  method: get\n  operationId: findObjects\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{table-name}/{object-id}\n  method: get\n  operationId: getObjectById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/{table-name}/{object-id}\n  method: put\n  operationId: updateObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table-name}/{object-id}\n  method: delete\n  operationId: deleteObject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/{table-name}/count\n  method: get\n  operationId: countObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/register\n  method: post\n  operationId: registerUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/login\n  method: post\n  operationId: loginUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/logout\n\
  \  method: get\n  operationId: logoutUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/restorepassword/{identity}\n  method: get\n  operationId: restorePassword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{path}\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files/{path}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/{channel-name}\n  method: post\n  operationId: publishMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messaging/{channel-name}/{subscription-id}\n  method: get\n  operationId: pollMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messaging/email\n  method: post\n  operationId: sendEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/points\n  method: get\n  operationId: findGeoPoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geo/points\n  method: post\n  operationId: saveGeoPoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cache/{key}\n  method: put\n  operationId: cachePut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /cache/{key}\n  method: get\n  operationId: cacheGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cache/{key}\n  method: delete\n  operationId: cacheDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cache/{key}/check\n  method: get\n  operationId: cacheContains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counters/{counter-name}/increment/get\n  method: put\n  operationId: incrementAndGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counters/{counter-name}/incrementby/get\n  method: put\n  operationId: incrementByAndGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /counters/{counter-name}/get\n  method: get\n  operationId: getCounter\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /counters/{counter-name}/reset\n  method: put\n  operationId: resetCounter\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n\
  \      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /services/{service-name}/{method-name}\n  method: post\n  operationId: invokeCloudCodeService\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/agentic-access/backendless-agentic-access.yml
summary_line: 26 operations · 16 acting · 1 human-in-the-loop
tags:
- BaaS
- Backend as a Service
- Visual Development
- Low Code
- Database
- Realtime
---
