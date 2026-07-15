---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 12
api_specs:
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Events & Tracking API
  slug: leanplum-events-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum User & Device Attributes API
  slug: leanplum-user-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Messaging API
  slug: leanplum-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum A/B Tests API
  slug: leanplum-ab-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Content & Variables API
  slug: leanplum-content-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Data Export API
  slug: leanplum-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
- filename: leanplum-openapi.yml
  format: yaml
  label: Leanplum Postbacks & Batch API
  slug: leanplum-postbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/openapi/leanplum-openapi.yml
consequence_counts:
  physical: 1
  read: 12
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Leanplum Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api?action=stop
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api?action=sendMessage
operation_count: 27
overview: 'Leanplum exposes 27 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 13 write, 1 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Leanplum
provider_slug: leanplum
slug: leanplum-agentic-access
source_filename: leanplum-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/leanplum-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    acting: 15\n    connected: 12\n  by_consequence:\n    write: 13\n    safety-critical: 1\n    physical: 1\n    read: 12\n  human_in_the_loop_required: 1\noperations:\n- path: /api?action=start\n  method: post\n  operationId: start\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=pauseSession\n  method: post\n  operationId: pauseSession\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=resumeSession\n  method: post\n  operationId: resumeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=heartbeat\n  method: post\n  operationId: heartbeat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=stop\n  method:\
  \ post\n  operationId: stop\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api?action=track\n  method: post\n  operationId: track\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=advance\n  method: post\n  operationId: advance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api?action=setUserAttributes\n  method: post\n  operationId: setUserAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=setDeviceAttributes\n  method: post\n  operationId: setDeviceAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=setTrafficSourceInfo\n  method: post\n  operationId: setTrafficSourceInfo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=deleteUser\n  method: post\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=sendMessage\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=getMessages\n  method: get\n  operationId: getMessages\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getMessage\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getAbTests\n  method: get\n  operationId: getAbTests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getAbTest\n  method: get\n  operationId: getAbTest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getVariant\n  method: get\n  operationId: getVariant\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getVars\n\
  \  method: get\n  operationId: getVars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=setVars\n  method: post\n  operationId: setVars\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=downloadFile\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=exportData\n  method: get\n  operationId: exportData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=exportUsers\n\
  \  method: get\n  operationId: exportUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=exportUser\n  method: get\n  operationId: exportUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=exportReport\n  method: get\n  operationId: exportReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=getMultiResults\n  method: get\n  operationId: getMultiResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api?action=addPostback\n  method: post\n  operationId: addPostback\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api?action=multi\n  method: post\n  operationId: multi\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanplum/refs/heads/main/agentic-access/leanplum-agentic-access.yml
summary_line: 27 operations · 15 acting · 1 human-in-the-loop
tags:
- Mobile Marketing
- Customer Engagement
- Push Notifications
- Messaging
- A/B Testing
- Analytics
- CleverTap
---
