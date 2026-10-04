---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 4
api_specs:
- filename: trainerize-client-data-api-openapi.yml
  format: yaml
  label: ABC Trainerize Client Data API
  slug: trainerize-client-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-client-data-api-openapi.yml
- filename: trainerize-clients-api-openapi.yml
  format: yaml
  label: ABC Trainerize Clients API
  slug: trainerize-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-clients-api-openapi.yml
- filename: trainerize-messaging-api-openapi.yml
  format: yaml
  label: ABC Trainerize Messaging API
  slug: trainerize-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-messaging-api-openapi.yml
- filename: trainerize-training-api-openapi.yml
  format: yaml
  label: ABC Trainerize Training API
  slug: trainerize-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-training-api-openapi.yml
- filename: trainerize-webhooks-api-openapi.yml
  format: yaml
  label: ABC Trainerize Webhooks API
  slug: trainerize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/openapi/trainerize-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Trainerize Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /message/send
operation_count: 19
overview: 'ABC Trainerize exposes 19 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 14 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ABC Trainerize
provider_slug: trainerize
slug: trainerize-agentic-access
source_filename: trainerize-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/trainerize-client-data-api-openapi.yml, openapi/trainerize-clients-api-openapi.yml,\n  openapi/trainerize-messaging-api-openapi.yml, openapi/trainerize-training-api-openapi.yml,\n  openapi/trainerize-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    connected: 4\n    acting: 15\n  by_consequence:\n    read: 4\n    write: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /clientData/get\n  method: post\n  operationId: getClientData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clientData/set\n  method:\
  \ post\n  operationId: setClientData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/find\n  method: post\n  operationId: findClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/addOrUpdate\n  method: post\n  operationId: addOrUpdateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/deactivate\n  method: post\n  operationId: deactivateClient\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/reactivate\n  method: post\n  operationId: reactivateClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/assignTrainer\n  method: post\n  operationId: assignTrainer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/tag\n  method: post\n  operationId: modifyClientTag\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/group\n  method: post\n  operationId: modifyClientGroup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /attachment/upload\n  method: post\n  operationId: uploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/copyMaster\n  method: post\n  operationId: copyMasterProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/subscribe\n  method: post\n  operationId: subscribeProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/unsubscribe\n  method: post\n  operationId: unsubscribeProgram\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /program/addTrainingPhase\n  method: post\n  operationId: addTrainingPhase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workout/getList\n  method: post\n  operationId: getWorkoutList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /webhook/register\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/list\n  method: post\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/delete\n  method: post\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainerize/refs/heads/main/agentic-access/trainerize-agentic-access.yml
summary_line: 19 operations · 15 acting
tags:
- Fitness
- Personal Training
- Coaching
- Fitness Software
- Client Management
- Software-as-a-Service
---
