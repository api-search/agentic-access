---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 7
api_specs:
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage SMS API
  slug: vonage-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Voice API
  slug: vonage-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Messages API
  slug: vonage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Verify API
  slug: vonage-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Numbers API
  slug: vonage-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
- filename: vonage-openapi.yml
  format: yaml
  label: Vonage Application API
  slug: vonage-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/openapi/vonage-openapi.yml
consequence_counts:
  physical: 2
  read: 7
  safety-critical: 3
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Vonage Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/calls/{uuid}/stream
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/calls/{uuid}/talk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /verify/control/{format}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/json
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/messages
operation_count: 25
overview: 'Vonage exposes 25 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 13 write, 2 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vonage
provider_slug: vonage
slug: vonage-agentic-access
source_filename: vonage-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vonage-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    acting: 18\n    connected: 7\n  by_consequence:\n    physical: 2\n    read: 7\n    write: 13\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /sms/json\n  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls\n  method: get\n  operationId:\
  \ listCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls\n  method: post\n  operationId: createCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{uuid}\n  method: get\n  operationId: getCall\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calls/{uuid}\n  method: put\n  operationId: updateCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{uuid}/stream\n  method: put\n  operationId: playAudioStream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{uuid}/stream\n  method: delete\n  operationId: stopAudioStream\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/calls/{uuid}/talk\n  method: put\n  operationId: playTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/calls/{uuid}/talk\n  method: delete\n  operationId: stopTextToSpeech\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/messages/{message_uuid}\n  method:\
  \ patch\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/{format}\n  method: post\n  operationId: requestVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verify/check/{format}\n  method: post\n  operationId: checkVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /verify/search/{format}\n  method: get\n  operationId: searchVerification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verify/control/{format}\n  method: post\n  operationId: controlVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /account/numbers\n  method: get\n  operationId: listOwnedNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /number/search\n  method: get\n  operationId: searchAvailableNumbers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /number/buy\n  method: post\n  operationId: buyNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number/cancel\n  method: post\n  operationId: cancelNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /number/update\n  method: post\n  operationId: updateNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications\n  method: get\n  operationId: listApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/applications\n  method: post\n  operationId: createApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications/{id}\n  method: get\n  operationId: getApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/applications/{id}\n  method: put\n  operationId: updateApplication\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/applications/{id}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vonage/refs/heads/main/agentic-access/vonage-agentic-access.yml
summary_line: 25 operations · 18 acting · 3 human-in-the-loop
tags:
- Communication
- Messaging
- Telecommunications
- Video Conferencing
- Voice
- SMS
- Verification
---
