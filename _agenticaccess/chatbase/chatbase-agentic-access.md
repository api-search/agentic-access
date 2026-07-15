---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 6
api_specs:
- filename: chatbase-openapi.yml
  format: yaml
  label: Chatbase Chat API
  slug: chatbase-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-openapi.yml
- filename: chatbase-openapi.yml
  format: yaml
  label: Chatbase Chatbots and Agents API
  slug: chatbase-chatbots-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-openapi.yml
- filename: chatbase-openapi.yml
  format: yaml
  label: Chatbase Conversations API
  slug: chatbase-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-openapi.yml
- filename: chatbase-openapi.yml
  format: yaml
  label: Chatbase Sources and Data API
  slug: chatbase-sources-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-openapi.yml
- filename: chatbase-openapi.yml
  format: yaml
  label: Chatbase Leads API
  slug: chatbase-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/openapi/chatbase-openapi.yml
consequence_counts:
  read: 6
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chatbase Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Chatbase exposes 16 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chatbase
provider_slug: chatbase
slug: chatbase-agentic-access
source_filename: chatbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/chatbase-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    acting: 10\n    connected: 6\n  by_consequence:\n    write: 10\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /chat\n  method: post\n  operationId: chat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /create-chatbot\n  method: post\n  operationId: createChatbot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update-chatbot-data\n  method: post\n  operationId: updateChatbotData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update-chatbot-settings\n  method: post\n  operationId: updateChatbotSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-chatbots\n  method: get\n  operationId: getChatbots\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /delete-chatbot\n  method: delete\n  operationId: deleteChatbot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-conversations\n  method: get\n  operationId: getConversations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /get-leads\n  method: get\n  operationId: getLeads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatbots/{chatbotId}/contacts\n  method: post\n  operationId: createContacts\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbots/{chatbotId}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatbots/{chatbotId}/contacts/{contactId}\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatbots/{chatbotId}/contacts/{contactId}\n  method: patch\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbots/{chatbotId}/contacts/{contactId}\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbots/{chatbotId}/custom-attributes\n  method: post\n  operationId: createCustomAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chatbots/{chatbotId}/custom-attributes\n  method: get\n  operationId: getCustomAttributes\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /chatbots/{chatbotId}/custom-attributes/{name}\n  method: put\n  operationId: updateCustomAttribute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatbase/refs/heads/main/agentic-access/chatbase-agentic-access.yml
summary_line: 16 operations · 10 acting
tags:
- AI
- Chatbot
- AI Agent
- Customer Support
- Conversational AI
---
