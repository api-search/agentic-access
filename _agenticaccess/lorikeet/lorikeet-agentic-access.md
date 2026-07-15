---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 6
api_specs:
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Conversations API
  slug: lorikeet-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Messages API
  slug: lorikeet-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Webhooks & Events API
  slug: lorikeet-webhooks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Actions & Tools API
  slug: lorikeet-actions-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
- filename: lorikeet-openapi.yml
  format: yaml
  label: Lorikeet Knowledge Ingestion API
  slug: lorikeet-knowledge-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/openapi/lorikeet-openapi.yml
consequence_counts:
  read: 6
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lorikeet Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Lorikeet exposes 13 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lorikeet
provider_slug: lorikeet
slug: lorikeet-agentic-access
source_filename: lorikeet-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lorikeet-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 7\n    connected: 6\n  by_consequence:\n    write: 7\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /conversations\n  method: post\n  operationId: createConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations\n  method: get\n  operationId: listConversations\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}\n  method: get\n  operationId: getConversation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}\n  method: post\n  operationId: continueConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversation_id}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversation_id}/messages\n  method:\
  \ post\n  operationId: createMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge/sources\n  method: get\n  operationId: listKnowledgeSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /knowledge/sources\n  method: post\n  operationId: ingestKnowledgeSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /knowledge/sources/{source_id}\n  method: get\n  operationId: getKnowledgeSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /knowledge/sources/{source_id}\n  method: delete\n  operationId: deleteKnowledgeSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorikeet/refs/heads/main/agentic-access/lorikeet-agentic-access.yml
summary_line: 13 operations · 7 acting
tags:
- AI
- Customer Support
- AI Agent
- Support Automation
- Workflows
- Helpdesk
---
