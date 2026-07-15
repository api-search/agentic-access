---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 9
api_specs:
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks SMS API
  slug: 46elks-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks MMS API
  slug: 46elks-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Voice Calls API
  slug: 46elks-voice-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Phone Numbers API
  slug: 46elks-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Media API
  slug: 46elks-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Verification API
  slug: 46elks-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
consequence_counts:
  physical: 2
  read: 9
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 46Elks Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms
operation_count: 15
overview: '46elks exposes 15 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 4 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 46elks
provider_slug: 46elks
slug: 46elks-agentic-access
source_filename: 46elks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/46elks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    acting: 6\n    connected: 9\n  by_consequence:\n    physical: 2\n    read: 9\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /sms\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms\n  method: get\n  operationId: listSms\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/{id}\n  method: get\n  operationId: getSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms\n  method: post\n  operationId: sendMms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms\n  method: get\n  operationId: listMms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/{id}\n  method: get\n  operationId: getMms\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: post\n  operationId: makeCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls\n  method: get\n  operationId: listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{id}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers\n  method: post\n  operationId: allocateNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers\n  method: get\n  operationId: listNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /numbers/{id}\n  method: post\n  operationId: updateNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /numbers/{id}\n  method: delete\n  operationId: deallocateNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recordings\n  method: get\n  operationId: listRecordings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /images\n  method: get\n  operationId: listImages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/agentic-access/46elks-agentic-access.yml
summary_line: 15 operations · 6 acting
tags:
- CPaaS
- SMS
- MMS
- Voice
- Messaging
- Phone Numbers
- Communications
---
