---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 31
api_specs:
- filename: moveworks-events-api-openapi.yaml
  format: yaml
  label: Moveworks Events API
  slug: moveworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-events-api-openapi.yaml
- filename: moveworks-conversations-api-openapi.yaml
  format: yaml
  label: Moveworks Conversations API
  slug: moveworks-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-conversations-api-openapi.yaml
- filename: moveworks-beta-conversations-api-openapi.yaml
  format: yaml
  label: Moveworks Conversations API (Beta)
  slug: moveworks-conversations-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-beta-conversations-api-openapi.yaml
- filename: moveworks-data-api-openapi.yaml
  format: yaml
  label: Moveworks Data API
  slug: moveworks-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-data-api-openapi.yaml
- filename: moveworks-webhook-listeners-openapi.yaml
  format: yaml
  label: Moveworks Webhook Listeners
  slug: moveworks-webhook-listeners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-webhook-listeners-openapi.yaml
consequence_counts:
  physical: 3
  read: 31
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Moveworks Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v1/events/{event_id}/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /rest/v1/messages/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/v1/listeners/{listener_id}/notify
operation_count: 46
overview: 'Moveworks exposes 46 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 31 read, 12 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Moveworks
provider_slug: moveworks
slug: moveworks-agentic-access
source_filename: moveworks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: generated\nsource: openapi/moveworks-beta-conversations-api-openapi.yaml, openapi/moveworks-content-gateway-openapi.yaml,\n  openapi/moveworks-conversations-api-openapi.yaml, openapi/moveworks-data-api-openapi.yaml,\n  openapi/moveworks-events-api-openapi.yaml, openapi/moveworks-forms-gateway-openapi.yaml, openapi/moveworks-identity-gateway-openapi.yaml,\n  openapi/moveworks-knowledge-gateway-openapi.yaml, openapi/moveworks-webhook-listeners-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 31\n    acting: 15\n  by_consequence:\n    read: 31\n    write: 12\n    physical: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /conversations\n  method: get\n \
  \ operationId: list-conversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations\n  method: post\n  operationId: create-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}\n  method: get\n  operationId: get-conversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}\n  method: patch\n  operationId: update-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses\n  method: post\n  operationId: create-response\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/responses/stream\n  method: post\n  operationId: create-response-stream\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/responses/{response_id}\n  method: get\n  operationId: get-response\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/messages\n  method: get\n  operationId: list-conversation-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses/{response_id}/messages\n  method: get\n  operationId: list-response-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses/{response_id}/messages/{message_id}/feedback\n\
  \  method: post\n  operationId: submit-feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: list-files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}\n  method: get\n  operationId: get-file-metadata-and-html-content-body\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/download\n  method: get\n  operationId: download-file\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n\
  \  method: get\n  operationId: list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups\n  method: get\n  operationId: list-groups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /groups/{groupId}/members\n  method: get\n  operationId: list-group-members\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/permissions/metadata\n  method: get\n  operationId: get-permission-model-metadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{id}/permissions\n  method: get\n  operationId: get-content-permissions\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations\n  method: get\n  operationId: list-conversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations\n  method: post\n  operationId: create-conversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}\n  method: get\n  operationId: get-conversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}\n  method: patch\n  operationId: update-conversation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/events\n  method: get\n  operationId: list-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses\n  method: post\n  operationId: create-response\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/responses/stream\n  method: post\n  operationId: create-response-stream\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/responses/{response_id}\n  method: get\n  operationId: get-response\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/messages\n  method: get\n  operationId: list-conversation-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses/{response_id}/messages\n  method: get\n  operationId: list-response-messages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/responses/{response_id}/messages/{message_id}/feedback\n  method: post\n  operationId: submit-feedback\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: get\n  operationId: list-conversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /interactions\n  method: get\n  operationId: list-interactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugin-calls\n  method: get\n  operationId: list-plugins-calls\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /plugin-resources\n  method: get\n  operationId: list-plugin-resources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/events/{event_id}/messages/send\n  method: post\n  operationId: send-message-for-event\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /oauth/v1/token\n  method: post\n  operationId: create-o-auth-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rest/v1/auth/test\n  method: get\n  operationId: test-auth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rest/v1/messages/send\n  method: post\n  operationId: send-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /forms\n  method: get\n\
  \  operationId: list-forms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{formId}\n  method: get\n  operationId: get-form-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /forms/{formId}/submit\n  method: post\n  operationId: submit-form\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users\n  method: get\n  operationId: list-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}\n  method: get\n  operationId:\
  \ get-user-by-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /articles\n  method: get\n  operationId: list-articles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/v1/listeners/{listener_id}/notify\n  method: post\n  operationId: send-a-webhook-to-a-webhook-listener\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/agentic-access/moveworks-agentic-access.yml
summary_line: 46 operations · 15 acting
tags:
- Company
- Artificial Intelligence
- Agentic AI
- AI Assistant
- Enterprise Automation
- Conversational AI
- Employee Experience
- IT Service Management
- Enterprise Search
---
