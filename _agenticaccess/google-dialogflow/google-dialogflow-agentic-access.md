---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 5
api_specs:
- filename: rest
  format: yaml
  label: Dialogflow API
  slug: dialogflow-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v2
- filename: rest
  format: yaml
  label: Dialogflow CX API
  slug: dialogflow-cx-api
  spec_type: OpenAPI
  url: https://dialogflow.googleapis.com/$discovery/rest?version=v3
consequence_counts:
  read: 5
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Google Dialogflow Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'Google Dialogflow exposes 14 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Google Dialogflow
provider_slug: google-dialogflow
slug: google-dialogflow-agentic-access
source_filename: google-dialogflow-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/google-dialogflow-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 5\n    acting: 9\n  by_consequence:\n    read: 5\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/projects/{project}/agent\n  method: get\n  operationId: getAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}:setAgent\n  method: post\n  operationId: setAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}:deleteAgent\n  method: delete\n  operationId: deleteAgent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/intents\n  method: get\n  operationId: listIntents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/intents\n  method: post\n  operationId:\
  \ createIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/intents/{intent}\n  method: get\n  operationId: getIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/intents/{intent}\n  method: patch\n  operationId: updateIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/intents/{intent}\n  method: delete\n  operationId: deleteIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/sessions/{session}:detectIntent\n  method: post\n  operationId: detectIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/sessions/{session}/contexts\n\
  \  method: delete\n  operationId: deleteAllContexts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/entityTypes\n  method: get\n  operationId: listEntityTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/agent/entityTypes\n  method: post\n  operationId: createEntityType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/knowledgeBases\n  method: get\n  operationId: listKnowledgeBases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - cloud-platform\n    - dialogflow\n- path: /v2/projects/{project}/knowledgeBases\n  method: post\n  operationId: createKnowledgeBase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - cloud-platform\n    - dialogflow\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-dialogflow/refs/heads/main/agentic-access/google-dialogflow-agentic-access.yml
summary_line: 14 operations · 9 acting
tags:
- Artificial Intelligence
- Chatbots
- Conversational AI
- Machine Learning
- Natural Language Processing
- Voice Assistants
---
