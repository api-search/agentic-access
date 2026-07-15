---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 1
api_specs:
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Conversations API
  slug: gradient-labs-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Messages API
  slug: gradient-labs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Hand-off & Assignment API
  slug: gradient-labs-hand-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Actions & Tools API
  slug: gradient-labs-actions-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Knowledge API
  slug: gradient-labs-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
- filename: gradient-labs-openapi.yml
  format: yaml
  label: Gradient Labs Webhooks API
  slug: gradient-labs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/openapi/gradient-labs-openapi.yml
consequence_counts:
  read: 1
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gradient Labs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Gradient Labs exposes 11 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gradient Labs
provider_slug: gradient-labs
slug: gradient-labs-agentic-access
source_filename: gradient-labs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gradient-labs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 10\n    connected: 1\n  by_consequence:\n    write: 10\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /conversations\n  method: post\n  operationId: startConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/read\n  method: get\n  operationId: readConversation\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /conversations/{conversationID}/messages\n  method: post\n  operationId: addMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/assignee\n  method: put\n  operationId: assignConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/finish\n  method: put\n  operationId: finishConversation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/cancel\n  method: put\n  operationId: cancelConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/resume\n  method: put\n  operationId: resumeConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /conversations/{conversationID}/rate\n\
  \  method: put\n  operationId: rateConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools\n  method: post\n  operationId: createTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/{id}/execute\n  method: post\n  operationId: executeTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /articles\n  method: post\n  operationId: upsertArticle\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gradient-labs/refs/heads/main/agentic-access/gradient-labs-agentic-access.yml
summary_line: 11 operations · 10 acting
tags:
- AI
- Customer Support
- AI Agent
- Conversations
- Financial Services
- Regulated
---
