---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 1
api_specs:
- filename: openapi.json
  format: json
  label: Microsoft Copilot API
  slug: microsoft-copilot-api
  spec_type: OpenAPI
  url: https://api.copilot.microsoft.com/openapi.json
- filename: openapi.json
  format: json
  label: Microsoft Graph API (Copilot Integration)
  slug: microsoft-graph-api-copilot-integration
  spec_type: OpenAPI
  url: https://graph.microsoft.com/openapi.json
- filename: microsoft-copilot-openapi.yml
  format: yaml
  label: Microsoft 365 Copilot APIs
  slug: microsoft-365-copilot-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/openapi/microsoft-copilot-openapi.yml
consequence_counts:
  read: 1
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Microsoft Copilot Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Microsoft Copilot exposes 6 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
slug: microsoft-copilot-agentic-access
source_filename: microsoft-copilot-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/microsoft-copilot-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 5\n    connected: 1\n  by_consequence:\n    write: 5\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /copilot/retrieval\n  method: post\n  operationId: copilot.retrieval\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Files.Read.All\n    - Sites.Read.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/search\n  method: post\n  operationId:\
  \ copilot.search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Files.Read.All\n    - Sites.Read.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/chat/conversations\n  method: post\n  operationId: copilot.chat.startConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Chat.Read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/chat/conversations/{conversationId}/messages\n  method: post\n  operationId: copilot.chat.continueConversation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - Chat.Read\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /copilot/interactionHistory/getAllEnterpriseInteractions\n  method: get\n  operationId: copilot.interactionHistory.getAllEnterpriseInteractions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIInteraction.Read.All\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subscriptions\n  method: post\n  operationId: copilot.changeNotifications.createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - AIInteraction.Read.All\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/agentic-access/microsoft-copilot-agentic-access.yml
summary_line: 6 operations · 5 acting
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
---
